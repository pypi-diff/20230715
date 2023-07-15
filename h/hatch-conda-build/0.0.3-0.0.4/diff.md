# Comparing `tmp/hatch_conda_build-0.0.3.tar.gz` & `tmp/hatch_conda_build-0.0.4.tar.gz`

## Comparing `hatch_conda_build-0.0.3.tar` & `hatch_conda_build-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/.github/workflows/release.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/hatch_conda_build/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/hatch_conda_build/__version__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/hatch_conda_build/config.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/hatch_conda_build/hooks.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/hatch_conda_build/plugin.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/tests/test_hatch.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/.gitignore
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/README.md
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/.github/workflows/release.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/hatch_conda_build/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/hatch_conda_build/__version__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/hatch_conda_build/config.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/hatch_conda_build/hooks.py
+-rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/hatch_conda_build/plugin.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/tests/test_hatch.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/.gitignore
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/README.md
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/PKG-INFO
```

### Comparing `hatch_conda_build-0.0.3/.github/workflows/release.yaml` & `hatch_conda_build-0.0.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `hatch_conda_build-0.0.3/hatch_conda_build/plugin.py` & `hatch_conda_build-0.0.4/hatch_conda_build/plugin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,70 @@
 import json
+import tomllib
 import shutil
 import typing
 import pathlib
 import collections
 import tempfile
 import subprocess
 
 from ruamel.yaml import YAML
 from hatchling.builders.plugin.interface import BuilderInterface
 
 from hatch_conda_build.config import CondaBuilderConfig
 
 
+def normalize_pypi_packages(packages: typing.List[str]):
+    _packages = []
+    for package in packages:
+        if 'hatch-conda-build' in package:
+            continue
+
+        if '@' in package:
+            package = package.split('@')[0]
+
+        _packages.append(package)
+    return _packages
+
+
 def construct_meta_yaml_from_pyproject(metadata):
     py_meta = metadata.core_raw_metadata
     conda_meta = collections.defaultdict(dict)
 
     # package
     conda_meta['package']['name'] = metadata.name
     conda_meta['package']['version'] = metadata.version
 
     # source
-    conda_meta['source']['path'] = str(pathlib.Path(metadata._project_file).parent)
+    pyproject_toml = pathlib.Path(metadata._project_file)
+    conda_meta['source']['path'] = str(pyproject_toml.parent)
+    with pyproject_toml.open('rb') as f:
+        full_metadata = tomllib.load(f)
 
     # build
     conda_meta['build']['number'] = 0
     conda_meta['build']['noarch'] = 'python'
     conda_meta['build']['script'] = 'python -m pip install --no-deps --ignore-installed .'
 
     # requirements
+    if 'requires-python' in py_meta:
+        python_spec = f"python {py_meta['requires-python']}"
+    else:
+        python_spec = "python"
+
     conda_meta['requirements']['build'] = []
+
     conda_meta['requirements']['host'] = [
+        python_spec,
         'pip',
-        'hatchling',
-    ]
-    conda_meta['requirements']['run'] = py_meta['dependencies']
+    ] + normalize_pypi_packages(full_metadata['build-system']['requires'])
+
+    conda_meta['requirements']['run'] = [
+        python_spec,
+    ] + py_meta['dependencies']
 
     # test
     conda_meta['test'] = {}
 
     # about
     conda_meta['about'] = {
 
@@ -50,27 +76,29 @@
 def conda_build(
     meta_config: typing.Dict,
     build_directory: pathlib.Path,
     output_directory: pathlib.Path,
     channels: typing.List[str],
     default_numpy_version: str,
 ):
+    print(meta_config)
+
     conda_meta_filename = build_directory / "meta.yaml"
     with conda_meta_filename.open("w") as f:
         json.dump(meta_config, f)
 
     command = ['conda-build', 'build', str(build_directory), '--output-folder', str(output_directory), '--override-channels', '--numpy', default_numpy_version, '--debug']
     for channel in channels:
         command += ['--channel', channel]
     print(command)
 
     import sys
     subprocess.run(command, check=True, stderr=sys.stderr, stdout=sys.stdout)
 
-    package_name = f"{meta_config['package']['name']}-{meta_config['package']['version']}-{meta_config['build']['number']}.tar.bz2"
+    package_name = f"{meta_config['package']['name']}-{meta_config['package']['version']}-py_{meta_config['build']['number']}.tar.bz2"
     return output_directory / 'noarch' / package_name
 
 
 class CondaBuilder(BuilderInterface):
     PLUGIN_NAME = "conda"
 
     def get_version_api(self) -> typing.Dict:
```

### Comparing `hatch_conda_build-0.0.3/tests/conftest.py` & `hatch_conda_build-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_conda_build-0.0.3/pyproject.toml` & `hatch_conda_build-0.0.4/pyproject.toml`

 * *Files identical despite different names*

