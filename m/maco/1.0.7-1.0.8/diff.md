# Comparing `tmp/maco-1.0.7.tar.gz` & `tmp/maco-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maco-1.0.7.tar", last modified: Sat Jul 15 05:49:35 2023, max compression
+gzip compressed data, was "maco-1.0.8.tar", last modified: Sat Jul 15 07:09:21 2023, max compression
```

## Comparing `maco-1.0.7.tar` & `maco-1.0.8.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.402708 maco-1.0.7/
--rw-r--r--   0 vsts      (1001) docker     (122)     3095 2023-07-15 05:49:21.000000 maco-1.0.7/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (122)     1478 2023-07-15 05:49:21.000000 maco-1.0.7/LICENSE.md
--rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-07-15 05:49:35.402708 maco-1.0.7/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     8055 2023-07-15 05:49:21.000000 maco-1.0.7/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.394708 maco-1.0.7/demo_extractors/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.394708 maco-1.0.7/demo_extractors/complex/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:21.000000 maco-1.0.7/demo_extractors/complex/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2290 2023-07-15 05:49:21.000000 maco-1.0.7/demo_extractors/complex/complex.py
--rw-r--r--   0 vsts      (1001) docker     (122)      123 2023-07-15 05:49:21.000000 maco-1.0.7/demo_extractors/complex/complex_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)      792 2023-07-15 05:49:21.000000 maco-1.0.7/demo_extractors/elfy.py
--rw-r--r--   0 vsts      (1001) docker     (122)      951 2023-07-15 05:49:21.000000 maco-1.0.7/demo_extractors/limit_other.py
--rw-r--r--   0 vsts      (1001) docker     (122)      628 2023-07-15 05:49:21.000000 maco-1.0.7/demo_extractors/nothing.py
--rw-r--r--   0 vsts      (1001) docker     (122)      266 2023-07-15 05:49:21.000000 maco-1.0.7/demo_extractors/shared.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.394708 maco-1.0.7/maco/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:21.000000 maco-1.0.7/maco/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2555 2023-07-15 05:49:21.000000 maco-1.0.7/maco/base_test.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7539 2023-07-15 05:49:21.000000 maco-1.0.7/maco/cli.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5598 2023-07-15 05:49:21.000000 maco-1.0.7/maco/collector.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2973 2023-07-15 05:49:21.000000 maco-1.0.7/maco/extractor.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.398708 maco-1.0.7/maco/model/
--rw-r--r--   0 vsts      (1001) docker     (122)       31 2023-07-15 05:49:21.000000 maco-1.0.7/maco/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18082 2023-07-15 05:49:21.000000 maco-1.0.7/maco/model/model.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.398708 maco-1.0.7/maco.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-07-15 05:49:35.000000 maco-1.0.7/maco.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      832 2023-07-15 05:49:35.000000 maco-1.0.7/maco.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-15 05:49:35.000000 maco-1.0.7/maco.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       39 2023-07-15 05:49:35.000000 maco-1.0.7/maco.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       34 2023-07-15 05:49:35.000000 maco-1.0.7/maco.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-07-15 05:49:35.000000 maco-1.0.7/maco.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.398708 maco-1.0.7/pipelines/
--rw-r--r--   0 vsts      (1001) docker     (122)     2624 2023-07-15 05:49:21.000000 maco-1.0.7/pipelines/publish.yaml
--rw-r--r--   0 vsts      (1001) docker     (122)       34 2023-07-15 05:49:21.000000 maco-1.0.7/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-07-15 05:49:35.402708 maco-1.0.7/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      604 2023-07-15 05:49:21.000000 maco-1.0.7/setup.py
--rw-r--r--   0 vsts      (1001) docker     (122)      454 2023-07-15 05:49:21.000000 maco-1.0.7/setup_model_only.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.402708 maco-1.0.7/tests/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.402708 maco-1.0.7/tests/data/
--rw-r--r--   0 vsts      (1001) docker     (122)      289 2023-07-15 05:49:21.000000 maco-1.0.7/tests/data/example.txt.cart
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.402708 maco-1.0.7/tests/extractors/
--rw-r--r--   0 vsts      (1001) docker     (122)      849 2023-07-15 05:49:21.000000 maco-1.0.7/tests/extractors/basic.py
--rw-r--r--   0 vsts      (1001) docker     (122)      881 2023-07-15 05:49:21.000000 maco-1.0.7/tests/extractors/basic_longer.py
--rw-r--r--   0 vsts      (1001) docker     (122)      697 2023-07-15 05:49:21.000000 maco-1.0.7/tests/extractors/test_basic.py
--rw-r--r--   0 vsts      (1001) docker     (122)      456 2023-07-15 05:49:21.000000 maco-1.0.7/tests/test_base_test.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1403 2023-07-15 05:49:21.000000 maco-1.0.7/tests/test_extractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2471 2023-07-15 05:49:21.000000 maco-1.0.7/tests/test_helpers.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4297 2023-07-15 05:49:21.000000 maco-1.0.7/tests/test_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)      148 2023-07-15 05:49:21.000000 maco-1.0.7/tox.ini
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:09:21.097122 maco-1.0.8/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3095 2023-07-15 07:09:09.000000 maco-1.0.8/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (122)     1478 2023-07-15 07:09:09.000000 maco-1.0.8/LICENSE.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-07-15 07:09:21.097122 maco-1.0.8/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     8055 2023-07-15 07:09:09.000000 maco-1.0.8/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:09:21.093122 maco-1.0.8/demo_extractors/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:09:21.093122 maco-1.0.8/demo_extractors/complex/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-15 07:09:09.000000 maco-1.0.8/demo_extractors/complex/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2290 2023-07-15 07:09:09.000000 maco-1.0.8/demo_extractors/complex/complex.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      123 2023-07-15 07:09:09.000000 maco-1.0.8/demo_extractors/complex/complex_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      792 2023-07-15 07:09:09.000000 maco-1.0.8/demo_extractors/elfy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      951 2023-07-15 07:09:09.000000 maco-1.0.8/demo_extractors/limit_other.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      628 2023-07-15 07:09:09.000000 maco-1.0.8/demo_extractors/nothing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      266 2023-07-15 07:09:09.000000 maco-1.0.8/demo_extractors/shared.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:09:21.097122 maco-1.0.8/maco/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-15 07:09:09.000000 maco-1.0.8/maco/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2555 2023-07-15 07:09:09.000000 maco-1.0.8/maco/base_test.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7539 2023-07-15 07:09:09.000000 maco-1.0.8/maco/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5598 2023-07-15 07:09:09.000000 maco-1.0.8/maco/collector.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2973 2023-07-15 07:09:09.000000 maco-1.0.8/maco/extractor.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:09:21.097122 maco-1.0.8/maco/model/
+-rw-r--r--   0 vsts      (1001) docker     (122)       31 2023-07-15 07:09:09.000000 maco-1.0.8/maco/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18082 2023-07-15 07:09:09.000000 maco-1.0.8/maco/model/model.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:09:21.097122 maco-1.0.8/maco.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-07-15 07:09:21.000000 maco-1.0.8/maco.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      850 2023-07-15 07:09:21.000000 maco-1.0.8/maco.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-15 07:09:21.000000 maco-1.0.8/maco.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       39 2023-07-15 07:09:21.000000 maco-1.0.8/maco.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       34 2023-07-15 07:09:21.000000 maco-1.0.8/maco.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-07-15 07:09:21.000000 maco-1.0.8/maco.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:09:21.097122 maco-1.0.8/model_setup/
+-rw-r--r--   0 vsts      (1001) docker     (122)      388 2023-07-15 07:09:09.000000 maco-1.0.8/model_setup/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:09:21.097122 maco-1.0.8/pipelines/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1683 2023-07-15 07:09:09.000000 maco-1.0.8/pipelines/publish.yaml
+-rw-r--r--   0 vsts      (1001) docker     (122)       34 2023-07-15 07:09:09.000000 maco-1.0.8/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-07-15 07:09:21.097122 maco-1.0.8/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      604 2023-07-15 07:09:09.000000 maco-1.0.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:09:21.097122 maco-1.0.8/tests/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:09:21.097122 maco-1.0.8/tests/data/
+-rw-r--r--   0 vsts      (1001) docker     (122)      289 2023-07-15 07:09:09.000000 maco-1.0.8/tests/data/example.txt.cart
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:09:21.097122 maco-1.0.8/tests/extractors/
+-rw-r--r--   0 vsts      (1001) docker     (122)      849 2023-07-15 07:09:09.000000 maco-1.0.8/tests/extractors/basic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      881 2023-07-15 07:09:09.000000 maco-1.0.8/tests/extractors/basic_longer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      697 2023-07-15 07:09:09.000000 maco-1.0.8/tests/extractors/test_basic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      456 2023-07-15 07:09:09.000000 maco-1.0.8/tests/test_base_test.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1403 2023-07-15 07:09:09.000000 maco-1.0.8/tests/test_extractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2471 2023-07-15 07:09:09.000000 maco-1.0.8/tests/test_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4297 2023-07-15 07:09:09.000000 maco-1.0.8/tests/test_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      148 2023-07-15 07:09:09.000000 maco-1.0.8/tox.ini
```

### Comparing `maco-1.0.7/.gitignore` & `maco-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `maco-1.0.7/LICENSE.md` & `maco-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `maco-1.0.7/README.md` & `maco-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `maco-1.0.7/demo_extractors/complex/complex.py` & `maco-1.0.8/demo_extractors/complex/complex.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.7/demo_extractors/elfy.py` & `maco-1.0.8/demo_extractors/elfy.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.7/demo_extractors/limit_other.py` & `maco-1.0.8/demo_extractors/limit_other.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.7/demo_extractors/nothing.py` & `maco-1.0.8/demo_extractors/nothing.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.7/maco/base_test.py` & `maco-1.0.8/maco/base_test.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.7/maco/cli.py` & `maco-1.0.8/maco/cli.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.7/maco/collector.py` & `maco-1.0.8/maco/collector.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.7/maco/extractor.py` & `maco-1.0.8/maco/extractor.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.7/maco/model/model.py` & `maco-1.0.8/maco/model/model.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.7/maco.egg-info/SOURCES.txt` & `maco-1.0.8/maco.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 .gitignore
 LICENSE.md
 README.md
 requirements.txt
 setup.py
-setup_model_only.py
 tox.ini
 demo_extractors/elfy.py
 demo_extractors/limit_other.py
 demo_extractors/nothing.py
 demo_extractors/shared.py
 demo_extractors/complex/__init__.py
 demo_extractors/complex/complex.py
@@ -21,14 +20,16 @@
 maco.egg-info/SOURCES.txt
 maco.egg-info/dependency_links.txt
 maco.egg-info/entry_points.txt
 maco.egg-info/requires.txt
 maco.egg-info/top_level.txt
 maco/model/__init__.py
 maco/model/model.py
+model_setup/maco
+model_setup/setup.py
 pipelines/publish.yaml
 tests/test_base_test.py
 tests/test_extractor.py
 tests/test_helpers.py
 tests/test_model.py
 tests/data/example.txt.cart
 tests/extractors/basic.py
```

### Comparing `maco-1.0.7/pipelines/publish.yaml` & `maco-1.0.8/pipelines/publish.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -45,56 +45,23 @@
       versionSpec: '3.9'
 
   - script: |
       set -x
       python -m pip install -U build
       python -m build
       ls dist
-    displayName: Build
-
-  - script: |
-      set -xv  # Echo commands before they are run
-      sudo env "PATH=$PATH" python -m pip install --no-cache-dir twine
-      ls dist
-      twine upload --skip-existing --repository-url $TEST_REPOSITORY_URL dist/*
-    displayName: Deploy to Test PyPI
-    env:
-      TWINE_USERNAME: $(twineUsername)
-      TWINE_PASSWORD: $(twinePassword)
-
-  - script: |
-      set -xv  # Echo commands before they are run
-      sudo env "PATH=$PATH" python -m pip install --no-cache-dir twine
-      ls dist
-      twine upload --skip-existing dist/*
-    displayName: Deploy to PyPI
-    env:
-      TWINE_USERNAME: $(twineUsername)
-      TWINE_PASSWORD: $(twinePassword)
-
-- job: build_and_deploy_model_only
-  dependsOn: test
-  displayName: Build and Deploy
-  variables:
-  - group: deployment-information
-
-  steps:
-  - task: UsePythonVersion@0
-    displayName: 'Use Python 3.9'
-    inputs:
-      versionSpec: '3.9'
+    displayName: Build (Full)
 
   - script: |
       set -x
-      python -m pip install -U build
-      rm setup.py
-      mv setup_model_only.py setup.py
-      python -m build
-      ls dist
-    displayName: Build
+      cd model_setup
+      python -m build --outdir ../dist
+      ls ../dist
+    displayName: Build (Model Only)
+
 
   - script: |
       set -xv  # Echo commands before they are run
       sudo env "PATH=$PATH" python -m pip install --no-cache-dir twine
       ls dist
       twine upload --skip-existing --repository-url $TEST_REPOSITORY_URL dist/*
     displayName: Deploy to Test PyPI
```

### Comparing `maco-1.0.7/setup.py` & `maco-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.7/tests/extractors/basic.py` & `maco-1.0.8/tests/extractors/basic.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.7/tests/extractors/basic_longer.py` & `maco-1.0.8/tests/extractors/basic_longer.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.7/tests/extractors/test_basic.py` & `maco-1.0.8/tests/extractors/test_basic.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.7/tests/test_extractor.py` & `maco-1.0.8/tests/test_extractor.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.7/tests/test_helpers.py` & `maco-1.0.8/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.7/tests/test_model.py` & `maco-1.0.8/tests/test_model.py`

 * *Files identical despite different names*

