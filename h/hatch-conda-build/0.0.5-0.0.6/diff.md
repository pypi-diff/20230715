# Comparing `tmp/hatch_conda_build-0.0.5.tar.gz` & `tmp/hatch_conda_build-0.0.6.tar.gz`

## Comparing `hatch_conda_build-0.0.5.tar` & `hatch_conda_build-0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/.github/workflows/release.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/hatch_conda_build/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/hatch_conda_build/__version__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/hatch_conda_build/config.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/hatch_conda_build/hooks.py
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/hatch_conda_build/plugin.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/tests/conftest.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/tests/test_hatch.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/.gitignore
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/README.md
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/.github/workflows/release.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/hatch_conda_build/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/hatch_conda_build/__version__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/hatch_conda_build/config.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/hatch_conda_build/hooks.py
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/hatch_conda_build/plugin.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/tests/conftest.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/tests/test_hatch.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/.gitignore
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/README.md
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 hatch_conda_build-0.0.6/PKG-INFO
```

### Comparing `hatch_conda_build-0.0.5/.github/workflows/release.yaml` & `hatch_conda_build-0.0.6/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `hatch_conda_build-0.0.5/hatch_conda_build/plugin.py` & `hatch_conda_build-0.0.6/hatch_conda_build/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -62,38 +62,39 @@
         python_spec,
     ] + py_meta['dependencies']
 
     # test
     conda_meta['test'] = {}
 
     # about
-    conda_meta['about'] = {
+    if 'homepage' in full_metadata['project'].get('urls', {}):
+        conda_meta['about']['home'] = full_metadata['project']['urls']['homepage']
 
-    }
+    if 'description' in full_metadata['project']:
+        conda_meta['about']['summary'] = full_metadata['project']['description']
 
     return conda_meta
 
 
 def conda_build(
     meta_config: typing.Dict,
     build_directory: pathlib.Path,
     output_directory: pathlib.Path,
     channels: typing.List[str],
     default_numpy_version: str,
 ):
-    print(meta_config)
-
+    print('meta.yaml: ' meta_config)
     conda_meta_filename = build_directory / "meta.yaml"
     with conda_meta_filename.open("w") as f:
         json.dump(meta_config, f)
 
     command = ['conda-build', 'build', str(build_directory), '--output-folder', str(output_directory), '--override-channels', '--numpy', default_numpy_version]
     for channel in channels:
         command += ['--channel', channel]
-    print(command)
+    print('command', command)
 
     import sys
     subprocess.run(command, check=True, stderr=sys.stderr, stdout=sys.stdout)
 
     package_name = f"{meta_config['package']['name']}-{meta_config['package']['version']}-py_{meta_config['build']['number']}.tar.bz2"
     return output_directory / 'noarch' / package_name
```

### Comparing `hatch_conda_build-0.0.5/tests/conftest.py` & `hatch_conda_build-0.0.6/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,16 +32,20 @@
 [build-system]
 requires = ["hatchling", "hatch-conda-build @ {plugin_dir.as_uri()}"]
 build-backend = "hatchling.build"
 
 [project]
 name = "project-a"
 version = "0.1.0"
+description = "A description"
 dependencies = {json.dumps(dependencies)}
 
+[project.urls]
+homepage = "https://example.org"
+
 [tool.hatch.build.targets.conda]
 channels = ["conda-forge"]
     """,
             encoding="utf-8",
         )
 
         package_dir = project_dir / "src" / package_name
```

### Comparing `hatch_conda_build-0.0.5/pyproject.toml` & `hatch_conda_build-0.0.6/pyproject.toml`

 * *Files identical despite different names*

