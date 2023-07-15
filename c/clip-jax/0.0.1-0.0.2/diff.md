# Comparing `tmp/clip_jax-0.0.1.tar.gz` & `tmp/clip_jax-0.0.2.tar.gz`

## Comparing `clip_jax-0.0.1.tar` & `clip_jax-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 clip_jax-0.0.1/clip_jax/__init__.py
--rw-r--r--   0        0        0    16816 2020-02-02 00:00:00.000000 clip_jax-0.0.1/clip_jax/configuration_clip.py
--rw-r--r--   0        0        0     9659 2020-02-02 00:00:00.000000 clip_jax-0.0.1/clip_jax/data.py
--rw-r--r--   0        0        0    55532 2020-02-02 00:00:00.000000 clip_jax-0.0.1/clip_jax/modeling.py
--rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 clip_jax-0.0.1/clip_jax/partitions.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 clip_jax-0.0.1/clip_jax/utils.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 clip_jax-0.0.1/.gitignore
--rw-r--r--   0        0        0    11354 2020-02-02 00:00:00.000000 clip_jax-0.0.1/LICENSE.md
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 clip_jax-0.0.1/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 clip_jax-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 clip_jax-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 clip_jax-0.0.2/clip_jax/__init__.py
+-rw-r--r--   0        0        0     9123 2020-02-02 00:00:00.000000 clip_jax-0.0.2/clip_jax/data.py
+-rw-r--r--   0        0        0    45939 2020-02-02 00:00:00.000000 clip_jax-0.0.2/clip_jax/modeling.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 clip_jax-0.0.2/clip_jax/partitions.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 clip_jax-0.0.2/clip_jax/tokenizer.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 clip_jax-0.0.2/clip_jax/utils.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 clip_jax-0.0.2/clip_jax/wandb_utils.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 clip_jax-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11354 2020-02-02 00:00:00.000000 clip_jax-0.0.2/LICENSE.md
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 clip_jax-0.0.2/README.md
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 clip_jax-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 clip_jax-0.0.2/PKG-INFO
```

### Comparing `clip_jax-0.0.1/clip_jax/data.py` & `clip_jax-0.0.2/clip_jax/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,65 +3,51 @@
 from dataclasses import dataclass, field
 from pathlib import Path
 
 import jax
 import numpy as np
 import tensorflow as tf
 import tensorflow_io as tfio
-from einops import rearrange
 
 
 @dataclass
 class Dataset:
     train_folder: str = None
     valid_folder: str = None
     train_batch_size: int = 64
     valid_batch_size: int = 64
-    image_size: int = 0  # no resizing if set to 0, (data should be at right dimensions)
+    image_size: int = 0  # crops image, no cropping if set to 0, (data should be at right dimensions)
     min_original_image_size: int = None
     max_original_aspect_ratio: float = None
     seed_dataset: int = None
     format: str = "rgb"  # rgb or lab
     key_image: str = "webp"  # name of key containing image
     key_caption: str = "caption"  # name of key containing captions
     mean: list[float] = (0.5, 0.5, 0.5)  # rescale between -1 and 1 by default
     std: list[float] = (0.5, 0.5, 0.5)  # rescale between -1 and 1 by default
-    valid_batch_size_per_step: int = None  # used in multi-host
-    node_groups: int = 1  # used in multi-host (number of nodes reading the same data when mp>local_devices)
     _train: tf.data.Dataset = field(init=False)
     _valid: tf.data.Dataset = field(init=False)
     rng: tf.random.Generator = field(init=False)
     multi_hosts: bool = field(init=False)
-    valid_groups: int = field(init=False)  # number of groups for validation set (multi-host)
-    valid_group_number: int = field(init=False)  # group number to use for validation set (multi-host)
+    process_count: int = field(init=False)  # number of groups for validation set (multi-host)
+    process_index: int = field(init=False)  # group number to use for validation set (multi-host)
 
     def __post_init__(self):
         # verify valid args
         assert self.format in ["rgb", "lab"], f"Invalid format: {self.format}"
 
         # define rng
         if self.seed_dataset is None:
             self.seed_dataset = random.randint(0, 2**32 - 1)
         self.rng = tf.random.Generator.from_seed(self.seed_dataset, alg="philox")
 
         # check if we are on multi-hosts
         self.multi_hosts = jax.process_count() > 1
-
-        # define valid groups (useful in multi-hosts)
-        if self.multi_hosts:
-            assert self.valid_batch_size_per_step % self.valid_batch_size == 0, (
-                f"valid_batch_size_per_step ({self.valid_batch_size_per_step}) "
-                f"should be a multiple of valid_batch_size ({self.valid_batch_size})"
-            )
-            self.valid_groups = self.valid_batch_size_per_step // self.valid_batch_size
-            self.valid_group_number = jax.process_index() // self.node_groups
-            assert self.valid_groups == jax.process_count() // self.node_groups, (
-                f"valid_groups ({self.valid_groups}) should be equal to "
-                f"jax.process_count() // self.node_groups ({jax.process_count() // self.node_groups})"
-            )
+        self.process_index = jax.process_index()
+        self.process_count = jax.process_count()
 
         # define parsing function
         features = {
             self.key_image: tf.io.FixedLenFeature([], tf.string),
             "original_width": tf.io.FixedLenFeature([], tf.int64),
             "original_height": tf.io.FixedLenFeature([], tf.int64),
             self.key_caption: tf.io.FixedLenFeature([], tf.string, default_value=""),
@@ -141,37 +127,36 @@
                 else:
                     files = [f"{Path(f)}" for f in Path(folder).glob("*.tfrecord")]
                 assert len(files) > 0, f"No files found at folder: {folder}"
 
                 # sort files
                 files = sorted(files)
 
-                # keep only a subset of files
-                if self.multi_hosts and augment:
-                    files = files[self.valid_group_number :: self.valid_groups]
-
-                # shuffle files
+                # shuffle files and select subset
                 if augment:
+                    files = files[self.process_index :: self.process_count]
                     random.shuffle(files)
 
                 # load dataset
                 ds = tf.data.TFRecordDataset(
                     files,
                     num_parallel_reads=tf.data.experimental.AUTOTUNE,
                 )
 
                 # non deterministic read (faster)
                 if augment:
                     ignore_order = tf.data.Options()
                     ignore_order.deterministic = False
                     ds = ds.with_options(ignore_order)
 
-                if self.multi_hosts and augment:
-                    # repeat indefinitely
-                    ds = ds.repeat()
+                    if self.multi_hosts:
+                        # repeat indefinitely
+                        ds = ds.repeat()
+                        # shuffle files
+                        ds = ds.shuffle(len(files))
 
                 # parse dataset
                 if self.min_original_image_size is None and self.max_original_aspect_ratio is None:
                     ds = ds.map(
                         _parse_no_filter,
                         num_parallel_calls=tf.data.experimental.AUTOTUNE,
                     )
@@ -210,23 +195,32 @@
     @property
     def valid(self):
         if not self.multi_hosts:
             yield from self._valid.as_numpy_iterator()
         else:
             # we need to return only a subset of the validation set
             for i, batch in enumerate(self._valid.as_numpy_iterator()):
-                if i % self.valid_groups == self.valid_group_number:
+                if i % self.process_count == self.process_index:
                     # this is the batch to yield for this host
                     batch_group = batch
-                if i % self.valid_groups == (self.valid_groups - 1):
+                if i % self.process_count == (self.process_count - 1):
                     # all nodes have a batch
                     yield batch_group
 
 
-def logits_to_image(logits, mean=(0.0, 0.0, 0.0), std=(1.0, 1.0, 1.0), format="rgb"):
-    logits = np.asarray(logits, dtype=np.float32)
+def logits_to_image(logits, mean=(0.5, 0.5, 0.5), std=(0.5, 0.5, 0.5), format="rgb"):
     if format == "rgb":
         logits = (logits * np.asarray(std, dtype=np.float32)) + np.asarray(mean, dtype=np.float32)
-        logits = logits.clip(0.0, 1.0)
+        logits = np.asarray(logits * 255.0, dtype=np.uint8)
+        logits = logits.clip(0, 255)
     else:
         raise NotImplementedError("LAB not implemented")
     return logits
+
+
+def image_to_logits(image, mean=(0.5, 0.5, 0.5), std=(0.5, 0.5, 0.5), format="rgb"):
+    image = np.asarray(image)
+    if format == "rgb":
+        image = (image / 255.0 - np.asarray(mean, dtype=np.float32)) / np.asarray(std, dtype=np.float32)
+    else:
+        raise NotImplementedError("LAB not implemented")
+    return image
```

### Comparing `clip_jax-0.0.1/clip_jax/utils.py` & `clip_jax-0.0.2/clip_jax/wandb_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,54 @@
 import os
 import tempfile
+from contextlib import contextmanager
 
 import wandb
 
 
-class PretrainedFromWandbMixin:
+class WandbMixin:
     @classmethod
     def from_pretrained(cls, pretrained_model_name_or_path, *model_args, **kwargs):
         """
         Initializes from a wandb artifact or delegates loading to the superclass.
         """
         with tempfile.TemporaryDirectory() as tmp_dir:  # avoid multiple artifact copies
-            if ":" in pretrained_model_name_or_path and not os.path.isdir(pretrained_model_name_or_path):
-                # wandb artifact
-                if wandb.run is not None:
-                    artifact = wandb.run.use_artifact(pretrained_model_name_or_path)
-                else:
-                    artifact = wandb.Api().artifact(pretrained_model_name_or_path)
-                pretrained_model_name_or_path = artifact.download(tmp_dir)
+            pretrained_model_name_or_path = maybe_get_artifact(pretrained_model_name_or_path, tmp_dir)
 
-            return super(PretrainedFromWandbMixin, cls).from_pretrained(
-                pretrained_model_name_or_path, *model_args, **kwargs
-            )
+            return super(WandbMixin, cls).from_pretrained(pretrained_model_name_or_path, *model_args, **kwargs)
 
-    @classmethod
-    def get_config_dict(cls, pretrained_model_name_or_path, *model_args, **kwargs):
-        with tempfile.TemporaryDirectory() as tmp_dir:  # avoid multiple artifact copies
-            if ":" in pretrained_model_name_or_path and not os.path.isdir(pretrained_model_name_or_path):
-                # wandb artifact
-                if wandb.run is not None:
-                    artifact = wandb.run.use_artifact(pretrained_model_name_or_path)
-                else:
-                    artifact = wandb.Api().artifact(pretrained_model_name_or_path)
-                pretrained_model_name_or_path = artifact.download(tmp_dir)
 
-            return super(PretrainedFromWandbMixin, cls).get_config_dict(
-                pretrained_model_name_or_path, *model_args, **kwargs
-            )
+def maybe_get_artifact(pretrained_model_name_or_path, tmp_dir):
+    if (
+        ":" in pretrained_model_name_or_path
+        and "gs:/" not in pretrained_model_name_or_path
+        and not os.path.isdir(pretrained_model_name_or_path)
+    ):
+        # wandb artifact
+        if wandb.run is not None:
+            artifact = wandb.run.use_artifact(pretrained_model_name_or_path)
+        else:
+            artifact = wandb.Api().artifact(pretrained_model_name_or_path)
+        return artifact.download(tmp_dir)
+    else:
+        return pretrained_model_name_or_path
+
+
+@contextmanager
+def maybe_use_artifact(file_path, artifact_file_name=None):
+    try:
+        if ":" in file_path and "gs:/" not in file_path:
+            # wandb artifact
+            if wandb.run is not None:
+                artifact = wandb.run.use_artifact(file_path)
+            else:
+                artifact = wandb.Api().artifact(file_path)
+            with tempfile.TemporaryDirectory() as tmp_dir:
+                artifact_folder = artifact.download(tmp_dir)
+                if artifact_file_name is not None:
+                    yield os.path.join(artifact_folder, artifact_file_name)
+                else:
+                    yield artifact_folder
+        else:
+            yield file_path
+    finally:
+        pass
```

### Comparing `clip_jax-0.0.1/.gitignore` & `clip_jax-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `clip_jax-0.0.1/LICENSE.md` & `clip_jax-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `clip_jax-0.0.1/pyproject.toml` & `clip_jax-0.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 [project]
 name = "clip-jax"
 dynamic = ["version"]
 description = "Training of CLIP in JAX"
 readme = "README.md"
 license = "Apache-2.0"
 dependencies = [
-    "einops",
     "flax",
-    "jax>=0.2.6",
-    "jaxlib",
+    "jax",
     "numpy",
+    "orbax-checkpoint",
     "tensorflow-io[tensorflow-cpu]",
     "transformers",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black[jupyter]",
     "isort",
     "optax",
+    "precondition-opt",
     "tqdm",
+    "wandb",
 ]
 
 [tool.hatch.version]
 path = "clip_jax/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
```

