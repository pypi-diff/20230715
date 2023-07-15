# Comparing `tmp/pz-rail-pzflow-0.0.1.tar.gz` & `tmp/pz-rail-pzflow-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-pzflow-0.0.1.tar", last modified: Tue Jun 13 03:42:00 2023, max compression
+gzip compressed data, was "pz-rail-pzflow-0.0.2.tar", last modified: Fri Jul 14 23:55:45 2023, max compression
```

## Comparing `pz-rail-pzflow-0.0.1.tar` & `pz-rail-pzflow-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:42:00.477010 pz-rail-pzflow-0.0.1/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)      275 2023-06-12 21:28:38.000000 pz-rail-pzflow-0.0.1/.copier-answers.yml
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:42:00.462466 pz-rail-pzflow-0.0.1/.github/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     3329 2023-06-12 21:28:39.000000 pz-rail-pzflow-0.0.1/.github/pull_request_template.md
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:42:00.474115 pz-rail-pzflow-0.0.1/.github/workflows/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)      442 2023-06-12 21:28:38.000000 pz-rail-pzflow-0.0.1/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1016 2023-06-13 01:36:01.000000 pz-rail-pzflow-0.0.1/.github/workflows/linting.yml
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1085 2023-06-12 21:28:38.000000 pz-rail-pzflow-0.0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)      876 2023-06-12 21:51:44.000000 pz-rail-pzflow-0.0.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1144 2023-06-12 21:42:40.000000 pz-rail-pzflow-0.0.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1893 2023-06-12 21:28:38.000000 pz-rail-pzflow-0.0.1/.gitignore
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     3059 2023-06-12 21:28:37.000000 pz-rail-pzflow-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1102 2023-06-12 21:28:35.000000 pz-rail-pzflow-0.0.1/LICENSE
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     3441 2023-06-13 03:42:00.476799 pz-rail-pzflow-0.0.1/PKG-INFO
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1662 2023-06-12 21:28:38.000000 pz-rail-pzflow-0.0.1/README.md
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1776 2023-06-13 03:35:37.000000 pz-rail-pzflow-0.0.1/pyproject.toml
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)       38 2023-06-13 03:42:00.477064 pz-rail-pzflow-0.0.1/setup.cfg
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)       70 2023-06-13 03:35:12.000000 pz-rail-pzflow-0.0.1/setup.py
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:42:00.460621 pz-rail-pzflow-0.0.1/src/
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:42:00.475200 pz-rail-pzflow-0.0.1/src/pz_rail_pzflow.egg-info/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     3441 2023-06-13 03:42:00.000000 pz-rail-pzflow-0.0.1/src/pz_rail_pzflow.egg-info/PKG-INFO
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)      754 2023-06-13 03:42:00.000000 pz-rail-pzflow-0.0.1/src/pz_rail_pzflow.egg-info/SOURCES.txt
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)        1 2023-06-13 03:42:00.000000 pz-rail-pzflow-0.0.1/src/pz_rail_pzflow.egg-info/dependency_links.txt
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)       88 2023-06-13 03:42:00.000000 pz-rail-pzflow-0.0.1/src/pz_rail_pzflow.egg-info/requires.txt
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)        5 2023-06-13 03:42:00.000000 pz-rail-pzflow-0.0.1/src/pz_rail_pzflow.egg-info/top_level.txt
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:42:00.461086 pz-rail-pzflow-0.0.1/src/rail/
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:42:00.460757 pz-rail-pzflow-0.0.1/src/rail/creation/
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:42:00.475373 pz-rail-pzflow-0.0.1/src/rail/creation/engines/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    10994 2023-05-17 20:21:20.000000 pz-rail-pzflow-0.0.1/src/rail/creation/engines/flowEngine.py
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:42:00.460912 pz-rail-pzflow-0.0.1/src/rail/estimation/
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:42:00.475550 pz-rail-pzflow-0.0.1/src/rail/estimation/algos/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)    10827 2023-05-17 20:21:50.000000 pz-rail-pzflow-0.0.1/src/rail/estimation/algos/pzflow.py
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:42:00.475917 pz-rail-pzflow-0.0.1/src/rail/pzflow/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)      162 2023-05-18 17:16:11.000000 pz-rail-pzflow-0.0.1/src/rail/pzflow/__init__.py
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)      160 2023-06-13 03:42:00.000000 pz-rail-pzflow-0.0.1/src/rail/pzflow/_version.py
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:42:00.476088 pz-rail-pzflow-0.0.1/src/rail/tools/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     1926 2023-05-17 20:20:10.000000 pz-rail-pzflow-0.0.1/src/rail/tools/flow_handle.py
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:42:00.461232 pz-rail-pzflow-0.0.1/tests/
-drwxr-xr-x   0 echarles (297109139) SLAC\Domain Users (1704612529)        0 2023-06-13 03:42:00.476534 pz-rail-pzflow-0.0.1/tests/pzflow/
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     2349 2023-05-17 20:23:13.000000 pz-rail-pzflow-0.0.1/tests/pzflow/test_algos.py
--rw-r--r--   0 echarles (297109139) SLAC\Domain Users (1704612529)     6982 2023-05-17 20:13:14.000000 pz-rail-pzflow-0.0.1/tests/pzflow/test_flowEngine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:45.849894 pz-rail-pzflow-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:45.849894 pz-rail-pzflow-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:45.849894 pz-rail-pzflow-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-14 23:55:45.849894 pz-rail-pzflow-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 23:55:45.849894 pz-rail-pzflow-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:45.845893 pz-rail-pzflow-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:45.849894 pz-rail-pzflow-0.0.2/src/pz_rail_pzflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-14 23:55:45.000000 pz-rail-pzflow-0.0.2/src/pz_rail_pzflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-14 23:55:45.000000 pz-rail-pzflow-0.0.2/src/pz_rail_pzflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:55:45.000000 pz-rail-pzflow-0.0.2/src/pz_rail_pzflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-14 23:55:45.000000 pz-rail-pzflow-0.0.2/src/pz_rail_pzflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 23:55:45.000000 pz-rail-pzflow-0.0.2/src/pz_rail_pzflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:45.845893 pz-rail-pzflow-0.0.2/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:45.845893 pz-rail-pzflow-0.0.2/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:45.849894 pz-rail-pzflow-0.0.2/src/rail/creation/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/src/rail/creation/engines/flowEngine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:45.845893 pz-rail-pzflow-0.0.2/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:45.849894 pz-rail-pzflow-0.0.2/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/src/rail/estimation/algos/pzflow_nf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:45.849894 pz-rail-pzflow-0.0.2/src/rail/pzflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/src/rail/pzflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 23:55:45.000000 pz-rail-pzflow-0.0.2/src/rail/pzflow/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:45.849894 pz-rail-pzflow-0.0.2/src/rail/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/src/rail/tools/flow_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:45.845893 pz-rail-pzflow-0.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:45.849894 pz-rail-pzflow-0.0.2/tests/pzflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/tests/pzflow/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-07-14 23:55:33.000000 pz-rail-pzflow-0.0.2/tests/pzflow/test_flowEngine.py
```

### Comparing `pz-rail-pzflow-0.0.1/.github/pull_request_template.md` & `pz-rail-pzflow-0.0.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.1/.github/workflows/linting.yml` & `pz-rail-pzflow-0.0.2/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.1/.github/workflows/publish-to-pypi.yml` & `pz-rail-pzflow-0.0.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.1/.github/workflows/smoke-test.yml` & `pz-rail-pzflow-0.0.2/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.1/.github/workflows/testing-and-coverage.yml` & `pz-rail-pzflow-0.0.2/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.1/.gitignore` & `pz-rail-pzflow-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.1/.pre-commit-config.yaml` & `pz-rail-pzflow-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.1/LICENSE` & `pz-rail-pzflow-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.1/pyproject.toml` & `pz-rail-pzflow-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.1/src/pz_rail_pzflow.egg-info/SOURCES.txt` & `pz-rail-pzflow-0.0.2/src/pz_rail_pzflow.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 .copier-answers.yml
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
+environment.yml
 pyproject.toml
 setup.py
 .github/pull_request_template.md
 .github/workflows/add-issue-to-project-tracker.yml
 .github/workflows/linting.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/smoke-test.yml
 .github/workflows/testing-and-coverage.yml
 src/pz_rail_pzflow.egg-info/PKG-INFO
 src/pz_rail_pzflow.egg-info/SOURCES.txt
 src/pz_rail_pzflow.egg-info/dependency_links.txt
 src/pz_rail_pzflow.egg-info/requires.txt
 src/pz_rail_pzflow.egg-info/top_level.txt
 src/rail/creation/engines/flowEngine.py
-src/rail/estimation/algos/pzflow.py
+src/rail/estimation/algos/pzflow_nf.py
 src/rail/pzflow/__init__.py
 src/rail/pzflow/_version.py
 src/rail/tools/flow_handle.py
 tests/pzflow/test_algos.py
 tests/pzflow/test_flowEngine.py
```

### Comparing `pz-rail-pzflow-0.0.1/src/rail/creation/engines/flowEngine.py` & `pz-rail-pzflow-0.0.2/src/rail/creation/engines/flowEngine.py`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.1/src/rail/estimation/algos/pzflow.py` & `pz-rail-pzflow-0.0.2/src/rail/estimation/algos/pzflow_nf.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                     mag_err_g_lsst="mag_g_lsst_err",
                     mag_err_r_lsst="mag_r_lsst_err",
                     mag_err_i_lsst="mag_i_lsst_err",
                     mag_err_z_lsst="mag_z_lsst_err",
                     mag_err_y_lsst="mag_y_lsst_err")
 
 
-class Inform_PZFlowPDF(CatInformer):
+class PZFlowInformer(CatInformer):
     """ Subclass to train a pzflow-based estimator
     """
     name = 'Inform_PZFlowPdf'
     outputs = [('model', FlowHandle)]
     config_options = CatInformer.config_options.copy()
     config_options.update(zmin=Param(float, 0.0, msg="min z"),
                           zmax=Param(float, 3.0, msg="max_z"),
@@ -147,18 +147,18 @@
         self.model = Flow(flowdf.columns, bijector, seed=self.config.flow_seed)
         _ = self.model.train(flowdf[self.usecols], epochs=self.config.num_training_epochs,
                              verbose=True)
         self.model.save(self.get_output('model'))
 
 
 
-class PZFlowPDF(CatEstimator):
+class PZFlowEstimator(CatEstimator):
     """CatEstimator which uses PZFlow
     """
-    name = 'PZFlowPDF'
+    name = 'PZFlowEstimator'
     inputs = [('model', FlowHandle),
               ('input', TableHandle)]
     config_options = CatEstimator.config_options.copy()
     config_options.update(zmin=Param(float, 0.0, msg="The minimum redshift of the z grid"),
                           zmax=Param(float, 3.0, msg="The maximum redshift of the z grid"),
                           nzbins=Param(int, 301, msg="The number of gridpoints in the z grid"),
                           flow_seed=Param(int, 0, msg="seed for flow"),
```

### Comparing `pz-rail-pzflow-0.0.1/src/rail/tools/flow_handle.py` & `pz-rail-pzflow-0.0.2/src/rail/tools/flow_handle.py`

 * *Files identical despite different names*

### Comparing `pz-rail-pzflow-0.0.1/tests/pzflow/test_algos.py` & `pz-rail-pzflow-0.0.2/tests/pzflow/test_algos.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pytest
 import scipy.special
 
 from rail.core.algo_utils import one_algo
 from rail.core.stage import RailStage
-from rail.estimation.algos import pzflow
+from rail.estimation.algos import pzflow_nf
 
 sci_ver_str = scipy.__version__.split(".")
 
 
 DS = RailStage.data_store
 DS.__class__.allow_overwrite = True
 
@@ -57,16 +57,16 @@
         num_training_epochs=50,
         hdf5_groupname="photometry",
         model="PZflowPDF.pkl",
     )
     estim_config_dict = dict(hdf5_groupname="photometry", model="PZflowPDF.pkl")
 
     # zb_expected = np.array([0.15, 0.14, 0.11, 0.14, 0.12, 0.14, 0.15, 0.16, 0.11, 0.12])
-    train_algo = pzflow.Inform_PZFlowPDF
-    pz_algo = pzflow.PZFlowPDF
+    train_algo = pzflow_nf.PZFlowInformer
+    pz_algo = pzflow_nf.PZFlowEstimator
     results, rerun_results, rerun3_results = one_algo(
         "PZFlow", train_algo, pz_algo, train_config_dict, estim_config_dict
     )
     # temporarily remove comparison to "expected" values, as we are getting
     # slightly different answers for python3.7 vs python3.8 for some reason
     #    assert np.isclose(results.ancil['zmode'], zb_expected, atol=0.05).all()
     assert np.isclose(results.ancil["zmode"], rerun_results.ancil["zmode"], atol=0.05).all()
```

### Comparing `pz-rail-pzflow-0.0.1/tests/pzflow/test_flowEngine.py` & `pz-rail-pzflow-0.0.2/tests/pzflow/test_flowEngine.py`

 * *Files identical despite different names*

