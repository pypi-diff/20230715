# Comparing `tmp/maco-1.0.6.tar.gz` & `tmp/maco-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maco-1.0.6.tar", last modified: Fri Feb  3 16:29:53 2023, max compression
+gzip compressed data, was "maco-1.0.7.tar", last modified: Sat Jul 15 05:49:35 2023, max compression
```

## Comparing `maco-1.0.6.tar` & `maco-1.0.7.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-03 16:29:53.655220 maco-1.0.6/
--rw-r--r--   0 vsts      (1001) docker     (122)     3095 2023-02-03 16:29:37.000000 maco-1.0.6/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (122)     1478 2023-02-03 16:29:37.000000 maco-1.0.6/LICENSE.md
--rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-02-03 16:29:53.655220 maco-1.0.6/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     8055 2023-02-03 16:29:37.000000 maco-1.0.6/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-03 16:29:53.647220 maco-1.0.6/demo_extractors/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-03 16:29:53.647220 maco-1.0.6/demo_extractors/complex/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-03 16:29:37.000000 maco-1.0.6/demo_extractors/complex/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2290 2023-02-03 16:29:37.000000 maco-1.0.6/demo_extractors/complex/complex.py
--rw-r--r--   0 vsts      (1001) docker     (122)      123 2023-02-03 16:29:37.000000 maco-1.0.6/demo_extractors/complex/complex_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)      792 2023-02-03 16:29:37.000000 maco-1.0.6/demo_extractors/elfy.py
--rw-r--r--   0 vsts      (1001) docker     (122)      951 2023-02-03 16:29:37.000000 maco-1.0.6/demo_extractors/limit_other.py
--rw-r--r--   0 vsts      (1001) docker     (122)      628 2023-02-03 16:29:37.000000 maco-1.0.6/demo_extractors/nothing.py
--rw-r--r--   0 vsts      (1001) docker     (122)      266 2023-02-03 16:29:37.000000 maco-1.0.6/demo_extractors/shared.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-03 16:29:53.651220 maco-1.0.6/maco/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-02-03 16:29:37.000000 maco-1.0.6/maco/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2555 2023-02-03 16:29:37.000000 maco-1.0.6/maco/base_test.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7539 2023-02-03 16:29:37.000000 maco-1.0.6/maco/cli.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5598 2023-02-03 16:29:37.000000 maco-1.0.6/maco/collector.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2973 2023-02-03 16:29:37.000000 maco-1.0.6/maco/extractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18082 2023-02-03 16:29:37.000000 maco-1.0.6/maco/model.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-03 16:29:53.651220 maco-1.0.6/maco.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-02-03 16:29:53.000000 maco-1.0.6/maco.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      783 2023-02-03 16:29:53.000000 maco-1.0.6/maco.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-02-03 16:29:53.000000 maco-1.0.6/maco.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       39 2023-02-03 16:29:53.000000 maco-1.0.6/maco.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       26 2023-02-03 16:29:53.000000 maco-1.0.6/maco.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-02-03 16:29:53.000000 maco-1.0.6/maco.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-03 16:29:53.651220 maco-1.0.6/pipelines/
--rw-r--r--   0 vsts      (1001) docker     (122)     1534 2023-02-03 16:29:37.000000 maco-1.0.6/pipelines/publish.yaml
--rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-02-03 16:29:37.000000 maco-1.0.6/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-02-03 16:29:53.655220 maco-1.0.6/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      604 2023-02-03 16:29:37.000000 maco-1.0.6/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-03 16:29:53.651220 maco-1.0.6/tests/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-03 16:29:53.651220 maco-1.0.6/tests/data/
--rw-r--r--   0 vsts      (1001) docker     (122)      289 2023-02-03 16:29:37.000000 maco-1.0.6/tests/data/example.txt.cart
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-02-03 16:29:53.655220 maco-1.0.6/tests/extractors/
--rw-r--r--   0 vsts      (1001) docker     (122)      849 2023-02-03 16:29:37.000000 maco-1.0.6/tests/extractors/basic.py
--rw-r--r--   0 vsts      (1001) docker     (122)      881 2023-02-03 16:29:37.000000 maco-1.0.6/tests/extractors/basic_longer.py
--rw-r--r--   0 vsts      (1001) docker     (122)      697 2023-02-03 16:29:37.000000 maco-1.0.6/tests/extractors/test_basic.py
--rw-r--r--   0 vsts      (1001) docker     (122)      456 2023-02-03 16:29:37.000000 maco-1.0.6/tests/test_base_test.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1403 2023-02-03 16:29:37.000000 maco-1.0.6/tests/test_extractor.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2471 2023-02-03 16:29:37.000000 maco-1.0.6/tests/test_helpers.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4297 2023-02-03 16:29:37.000000 maco-1.0.6/tests/test_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)      148 2023-02-03 16:29:37.000000 maco-1.0.6/tox.ini
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.402708 maco-1.0.7/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3095 2023-07-15 05:49:21.000000 maco-1.0.7/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (122)     1478 2023-07-15 05:49:21.000000 maco-1.0.7/LICENSE.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-07-15 05:49:35.402708 maco-1.0.7/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     8055 2023-07-15 05:49:21.000000 maco-1.0.7/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.394708 maco-1.0.7/demo_extractors/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.394708 maco-1.0.7/demo_extractors/complex/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:21.000000 maco-1.0.7/demo_extractors/complex/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2290 2023-07-15 05:49:21.000000 maco-1.0.7/demo_extractors/complex/complex.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      123 2023-07-15 05:49:21.000000 maco-1.0.7/demo_extractors/complex/complex_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      792 2023-07-15 05:49:21.000000 maco-1.0.7/demo_extractors/elfy.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      951 2023-07-15 05:49:21.000000 maco-1.0.7/demo_extractors/limit_other.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      628 2023-07-15 05:49:21.000000 maco-1.0.7/demo_extractors/nothing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      266 2023-07-15 05:49:21.000000 maco-1.0.7/demo_extractors/shared.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.394708 maco-1.0.7/maco/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:21.000000 maco-1.0.7/maco/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2555 2023-07-15 05:49:21.000000 maco-1.0.7/maco/base_test.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7539 2023-07-15 05:49:21.000000 maco-1.0.7/maco/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5598 2023-07-15 05:49:21.000000 maco-1.0.7/maco/collector.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2973 2023-07-15 05:49:21.000000 maco-1.0.7/maco/extractor.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.398708 maco-1.0.7/maco/model/
+-rw-r--r--   0 vsts      (1001) docker     (122)       31 2023-07-15 05:49:21.000000 maco-1.0.7/maco/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18082 2023-07-15 05:49:21.000000 maco-1.0.7/maco/model/model.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.398708 maco-1.0.7/maco.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)      120 2023-07-15 05:49:35.000000 maco-1.0.7/maco.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      832 2023-07-15 05:49:35.000000 maco-1.0.7/maco.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-15 05:49:35.000000 maco-1.0.7/maco.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       39 2023-07-15 05:49:35.000000 maco-1.0.7/maco.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       34 2023-07-15 05:49:35.000000 maco-1.0.7/maco.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-07-15 05:49:35.000000 maco-1.0.7/maco.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.398708 maco-1.0.7/pipelines/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2624 2023-07-15 05:49:21.000000 maco-1.0.7/pipelines/publish.yaml
+-rw-r--r--   0 vsts      (1001) docker     (122)       34 2023-07-15 05:49:21.000000 maco-1.0.7/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-07-15 05:49:35.402708 maco-1.0.7/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      604 2023-07-15 05:49:21.000000 maco-1.0.7/setup.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      454 2023-07-15 05:49:21.000000 maco-1.0.7/setup_model_only.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.402708 maco-1.0.7/tests/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.402708 maco-1.0.7/tests/data/
+-rw-r--r--   0 vsts      (1001) docker     (122)      289 2023-07-15 05:49:21.000000 maco-1.0.7/tests/data/example.txt.cart
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 05:49:35.402708 maco-1.0.7/tests/extractors/
+-rw-r--r--   0 vsts      (1001) docker     (122)      849 2023-07-15 05:49:21.000000 maco-1.0.7/tests/extractors/basic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      881 2023-07-15 05:49:21.000000 maco-1.0.7/tests/extractors/basic_longer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      697 2023-07-15 05:49:21.000000 maco-1.0.7/tests/extractors/test_basic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      456 2023-07-15 05:49:21.000000 maco-1.0.7/tests/test_base_test.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1403 2023-07-15 05:49:21.000000 maco-1.0.7/tests/test_extractor.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2471 2023-07-15 05:49:21.000000 maco-1.0.7/tests/test_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4297 2023-07-15 05:49:21.000000 maco-1.0.7/tests/test_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      148 2023-07-15 05:49:21.000000 maco-1.0.7/tox.ini
```

### Comparing `maco-1.0.6/.gitignore` & `maco-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `maco-1.0.6/LICENSE.md` & `maco-1.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `maco-1.0.6/README.md` & `maco-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `maco-1.0.6/demo_extractors/complex/complex.py` & `maco-1.0.7/demo_extractors/complex/complex.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.6/demo_extractors/elfy.py` & `maco-1.0.7/demo_extractors/elfy.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.6/demo_extractors/limit_other.py` & `maco-1.0.7/demo_extractors/limit_other.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.6/demo_extractors/nothing.py` & `maco-1.0.7/demo_extractors/nothing.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.6/maco/base_test.py` & `maco-1.0.7/maco/base_test.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.6/maco/cli.py` & `maco-1.0.7/maco/cli.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.6/maco/collector.py` & `maco-1.0.7/maco/collector.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.6/maco/extractor.py` & `maco-1.0.7/maco/extractor.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.6/maco/model.py` & `maco-1.0.7/maco/model/model.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.6/maco.egg-info/SOURCES.txt` & `maco-1.0.7/maco.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 .gitignore
 LICENSE.md
 README.md
 requirements.txt
 setup.py
+setup_model_only.py
 tox.ini
 demo_extractors/elfy.py
 demo_extractors/limit_other.py
 demo_extractors/nothing.py
 demo_extractors/shared.py
 demo_extractors/complex/__init__.py
 demo_extractors/complex/complex.py
 demo_extractors/complex/complex_utils.py
 maco/__init__.py
 maco/base_test.py
 maco/cli.py
 maco/collector.py
 maco/extractor.py
-maco/model.py
 maco.egg-info/PKG-INFO
 maco.egg-info/SOURCES.txt
 maco.egg-info/dependency_links.txt
 maco.egg-info/entry_points.txt
 maco.egg-info/requires.txt
 maco.egg-info/top_level.txt
+maco/model/__init__.py
+maco/model/model.py
 pipelines/publish.yaml
 tests/test_base_test.py
 tests/test_extractor.py
 tests/test_helpers.py
 tests/test_model.py
 tests/data/example.txt.cart
 tests/extractors/basic.py
```

### Comparing `maco-1.0.6/pipelines/publish.yaml` & `maco-1.0.7/pipelines/publish.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -66,7 +66,48 @@
       sudo env "PATH=$PATH" python -m pip install --no-cache-dir twine
       ls dist
       twine upload --skip-existing dist/*
     displayName: Deploy to PyPI
     env:
       TWINE_USERNAME: $(twineUsername)
       TWINE_PASSWORD: $(twinePassword)
+
+- job: build_and_deploy_model_only
+  dependsOn: test
+  displayName: Build and Deploy
+  variables:
+  - group: deployment-information
+
+  steps:
+  - task: UsePythonVersion@0
+    displayName: 'Use Python 3.9'
+    inputs:
+      versionSpec: '3.9'
+
+  - script: |
+      set -x
+      python -m pip install -U build
+      rm setup.py
+      mv setup_model_only.py setup.py
+      python -m build
+      ls dist
+    displayName: Build
+
+  - script: |
+      set -xv  # Echo commands before they are run
+      sudo env "PATH=$PATH" python -m pip install --no-cache-dir twine
+      ls dist
+      twine upload --skip-existing --repository-url $TEST_REPOSITORY_URL dist/*
+    displayName: Deploy to Test PyPI
+    env:
+      TWINE_USERNAME: $(twineUsername)
+      TWINE_PASSWORD: $(twinePassword)
+
+  - script: |
+      set -xv  # Echo commands before they are run
+      sudo env "PATH=$PATH" python -m pip install --no-cache-dir twine
+      ls dist
+      twine upload --skip-existing dist/*
+    displayName: Deploy to PyPI
+    env:
+      TWINE_USERNAME: $(twineUsername)
+      TWINE_PASSWORD: $(twinePassword)
```

### Comparing `maco-1.0.6/setup.py` & `maco-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.6/tests/extractors/basic.py` & `maco-1.0.7/tests/extractors/basic.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.6/tests/extractors/basic_longer.py` & `maco-1.0.7/tests/extractors/basic_longer.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.6/tests/extractors/test_basic.py` & `maco-1.0.7/tests/extractors/test_basic.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.6/tests/test_extractor.py` & `maco-1.0.7/tests/test_extractor.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.6/tests/test_helpers.py` & `maco-1.0.7/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `maco-1.0.6/tests/test_model.py` & `maco-1.0.7/tests/test_model.py`

 * *Files identical despite different names*

