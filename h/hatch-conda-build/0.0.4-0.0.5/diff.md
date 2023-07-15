# Comparing `tmp/hatch_conda_build-0.0.4.tar.gz` & `tmp/hatch_conda_build-0.0.5.tar.gz`

## Comparing `hatch_conda_build-0.0.4.tar` & `hatch_conda_build-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/.github/workflows/release.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/hatch_conda_build/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/hatch_conda_build/__version__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/hatch_conda_build/config.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/hatch_conda_build/hooks.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/hatch_conda_build/plugin.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/tests/test_hatch.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/.gitignore
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/README.md
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/.github/workflows/release.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/hatch_conda_build/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/hatch_conda_build/__version__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/hatch_conda_build/config.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/hatch_conda_build/hooks.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/hatch_conda_build/plugin.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/tests/conftest.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/tests/test_hatch.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/.gitignore
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/README.md
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/PKG-INFO
```

### Comparing `hatch_conda_build-0.0.4/.github/workflows/release.yaml` & `hatch_conda_build-0.0.5/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `hatch_conda_build-0.0.4/hatch_conda_build/plugin.py` & `hatch_conda_build-0.0.5/hatch_conda_build/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 ):
     print(meta_config)
 
     conda_meta_filename = build_directory / "meta.yaml"
     with conda_meta_filename.open("w") as f:
         json.dump(meta_config, f)
 
-    command = ['conda-build', 'build', str(build_directory), '--output-folder', str(output_directory), '--override-channels', '--numpy', default_numpy_version, '--debug']
+    command = ['conda-build', 'build', str(build_directory), '--output-folder', str(output_directory), '--override-channels', '--numpy', default_numpy_version]
     for channel in channels:
         command += ['--channel', channel]
     print(command)
 
     import sys
     subprocess.run(command, check=True, stderr=sys.stderr, stdout=sys.stdout)
 
@@ -107,15 +107,15 @@
     def clean(directory: str, versions: typing.List[str]):
         shutil.rmtree(directory)
 
     def build_standard(self, directory: str, **build_data: typing.Dict) -> str:
         directory = pathlib.Path(directory)
 
         conda_meta = construct_meta_yaml_from_pyproject(self.metadata)
-        target_config = self.build_config['targets']['conda']
+        target_config = self.build_config.get('targets', {}).get('conda', {})
 
         with tempfile.TemporaryDirectory() as tmpdir:
             tmpdir = pathlib.Path(tmpdir)
 
             conda_build_filename = conda_build(
                 conda_meta,
                 build_directory=tmpdir,
```

### Comparing `hatch_conda_build-0.0.4/tests/conftest.py` & `hatch_conda_build-0.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hatch_conda_build-0.0.4/pyproject.toml` & `hatch_conda_build-0.0.5/pyproject.toml`

 * *Files identical despite different names*

