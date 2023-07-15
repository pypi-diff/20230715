# Comparing `tmp/hatch_conda_build-0.0.2.tar.gz` & `tmp/hatch_conda_build-0.0.3.tar.gz`

## Comparing `hatch_conda_build-0.0.2.tar` & `hatch_conda_build-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/.github/workflows/release.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/hatch_conda_build/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/hatch_conda_build/__version__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/hatch_conda_build/config.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/hatch_conda_build/hooks.py
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/hatch_conda_build/plugin.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/tests/test_hatch.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/.gitignore
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/README.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/.github/workflows/release.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/hatch_conda_build/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/hatch_conda_build/__version__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/hatch_conda_build/config.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/hatch_conda_build/hooks.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/hatch_conda_build/plugin.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/tests/test_hatch.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/.gitignore
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/README.md
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/PKG-INFO
```

### Comparing `hatch_conda_build-0.0.2/.github/workflows/release.yaml` & `hatch_conda_build-0.0.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `hatch_conda_build-0.0.2/hatch_conda_build/plugin.py` & `hatch_conda_build-0.0.3/hatch_conda_build/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,74 +2,103 @@
 import shutil
 import typing
 import pathlib
 import collections
 import tempfile
 import subprocess
 
+from ruamel.yaml import YAML
 from hatchling.builders.plugin.interface import BuilderInterface
 
 from hatch_conda_build.config import CondaBuilderConfig
-from grayskull.strategy.py_toml import get_all_toml_info
+
+
+def construct_meta_yaml_from_pyproject(metadata):
+    py_meta = metadata.core_raw_metadata
+    conda_meta = collections.defaultdict(dict)
+
+    # package
+    conda_meta['package']['name'] = metadata.name
+    conda_meta['package']['version'] = metadata.version
+
+    # source
+    conda_meta['source']['path'] = str(pathlib.Path(metadata._project_file).parent)
+
+    # build
+    conda_meta['build']['number'] = 0
+    conda_meta['build']['noarch'] = 'python'
+    conda_meta['build']['script'] = 'python -m pip install --no-deps --ignore-installed .'
+
+    # requirements
+    conda_meta['requirements']['build'] = []
+    conda_meta['requirements']['host'] = [
+        'pip',
+        'hatchling',
+    ]
+    conda_meta['requirements']['run'] = py_meta['dependencies']
+
+    # test
+    conda_meta['test'] = {}
+
+    # about
+    conda_meta['about'] = {
+
+    }
+
+    return conda_meta
+
+
+def conda_build(
+    meta_config: typing.Dict,
+    build_directory: pathlib.Path,
+    output_directory: pathlib.Path,
+    channels: typing.List[str],
+    default_numpy_version: str,
+):
+    conda_meta_filename = build_directory / "meta.yaml"
+    with conda_meta_filename.open("w") as f:
+        json.dump(meta_config, f)
+
+    command = ['conda-build', 'build', str(build_directory), '--output-folder', str(output_directory), '--override-channels', '--numpy', default_numpy_version, '--debug']
+    for channel in channels:
+        command += ['--channel', channel]
+    print(command)
+
+    import sys
+    subprocess.run(command, check=True, stderr=sys.stderr, stdout=sys.stdout)
+
+    package_name = f"{meta_config['package']['name']}-{meta_config['package']['version']}-{meta_config['build']['number']}.tar.bz2"
+    return output_directory / 'noarch' / package_name
 
 
 class CondaBuilder(BuilderInterface):
     PLUGIN_NAME = "conda"
 
     def get_version_api(self) -> typing.Dict:
         return {"standard": self.build_standard}
 
     def clean(directory: str, versions: typing.List[str]):
         shutil.rmtree(directory)
 
     def build_standard(self, directory: str, **build_data: typing.Dict) -> str:
         directory = pathlib.Path(directory)
 
-        py_meta = self.metadata.core_raw_metadata
-        conda_meta = collections.defaultdict(dict)
-
-        # package
-        conda_meta['package']['name'] = self.metadata.name
-        conda_meta['package']['version'] = self.metadata.version
-
-        # source
-        conda_meta['source']['path'] = str(pathlib.Path(self.metadata._project_file).parent)
-
-        # build
-        conda_meta['build']['number'] = 0
-        conda_meta['build']['noarch'] = 'python'
-        conda_meta['build']['script'] = 'python -m pip install --no-deps --ignore-installed .'
-
-        # requirements
-        conda_meta['requirements']['build'] = []
-        conda_meta['requirements']['host'] = [
-            'pip',
-            'hatchling',
-        ]
-        conda_meta['requirements']['run'] = py_meta['dependencies']
-
-        # test
-        conda_meta['test'] = {}
-
-        # about
-        conda_meta['about'] = {
-
-        }
+        conda_meta = construct_meta_yaml_from_pyproject(self.metadata)
+        target_config = self.build_config['targets']['conda']
 
         with tempfile.TemporaryDirectory() as tmpdir:
             tmpdir = pathlib.Path(tmpdir)
-            conda_meta_filename = tmpdir / "meta.yaml"
-            with conda_meta_filename.open("w") as f:
-                json.dump(conda_meta, f)
-
-            subprocess.run(
-                ['conda-build', 'build', str(tmpdir), '--output-folder', str(tmpdir)],
-                check=True)
 
-            conda_build_filename = tmpdir / 'noarch' / f"{conda_meta['package']['name']}-{conda_meta['package']['version']}-{conda_meta['build']['number']}.tar.bz2"
+            conda_build_filename = conda_build(
+                conda_meta,
+                build_directory=tmpdir,
+                output_directory=tmpdir,
+                channels=target_config.get('channels', ['conda-forge']),
+                default_numpy_version=target_config.get('default_numpy_version', '1.22'),
+            )
             shutil.copy2(conda_build_filename, directory / conda_build_filename.name)
 
         return str(directory)
 
     @classmethod
     def get_config_class(cls):
         return CondaBuilderConfig
```

### Comparing `hatch_conda_build-0.0.2/tests/conftest.py` & `hatch_conda_build-0.0.3/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,21 +34,16 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "project-a"
 version = "0.1.0"
 dependencies = {json.dumps(dependencies)}
 
-[project.urls]
-"Homepage" = "https://github.com/pypa/sampleproject"
-"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
-
 [tool.hatch.build.targets.conda]
-a = 1
-b = "2"
+channels = ["conda-forge"]
     """,
             encoding="utf-8",
         )
 
         package_dir = project_dir / "src" / package_name
         package_dir.mkdir(parents=True)
```

### Comparing `hatch_conda_build-0.0.2/pyproject.toml` & `hatch_conda_build-0.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 description = 'conda-build using pyproject.toml'
 dynamic = ["version"]
 requires-python = ">=3.8"
 readme = "README.md"
 dependencies = [
    "grayskull",
    "hatchling",
+   "ruamel.yaml",
 ]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.version]
```

