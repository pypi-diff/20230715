# Comparing `tmp/hatch_conda_build-0.0.6.tar.gz` & `tmp/hatch_conda_build-0.0.7.tar.gz`

## Comparing `hatch_conda_build-0.0.6.tar` & `hatch_conda_build-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/.github/workflows/release.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/hatch_conda_build/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/hatch_conda_build/__version__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/hatch_conda_build/config.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/hatch_conda_build/hooks.py
--rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/hatch_conda_build/plugin.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/tests/conftest.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/tests/test_hatch.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/.gitignore
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/README.md
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.7/.github/workflows/release.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.7/hatch_conda_build/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.7/hatch_conda_build/__version__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.7/hatch_conda_build/config.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.7/hatch_conda_build/hooks.py
+-rw-r--r--   0        0        0     4115 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.7/hatch_conda_build/plugin.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.7/tests/conftest.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.7/tests/test_hatch.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.7/.gitignore
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.7/README.md
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.7/PKG-INFO
```

### Comparing `hatch_conda_build-0.0.6/.github/workflows/release.yaml` & `hatch_conda_build-0.0.7/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `hatch_conda_build-0.0.6/hatch_conda_build/plugin.py` & `hatch_conda_build-0.0.7/hatch_conda_build/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 def conda_build(
     meta_config: typing.Dict,
     build_directory: pathlib.Path,
     output_directory: pathlib.Path,
     channels: typing.List[str],
     default_numpy_version: str,
 ):
-    print('meta.yaml: ' meta_config)
+    print('meta.yaml: ', meta_config)
     conda_meta_filename = build_directory / "meta.yaml"
     with conda_meta_filename.open("w") as f:
         json.dump(meta_config, f)
 
     command = ['conda-build', 'build', str(build_directory), '--output-folder', str(output_directory), '--override-channels', '--numpy', default_numpy_version]
     for channel in channels:
         command += ['--channel', channel]
```

### Comparing `hatch_conda_build-0.0.6/tests/conftest.py` & `hatch_conda_build-0.0.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_conda_build-0.0.6/pyproject.toml` & `hatch_conda_build-0.0.7/pyproject.toml`

 * *Files identical despite different names*

