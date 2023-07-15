# Comparing `tmp/chrono-kit-0.0.2.tar.gz` & `tmp/chrono-kit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrono-kit-0.0.2.tar", last modified: Sat Jul 15 18:09:55 2023, max compression
+gzip compressed data, was "chrono-kit-0.1.0.tar", last modified: Sat Jul 15 18:14:24 2023, max compression
```

## Comparing `chrono-kit-0.0.2.tar` & `chrono-kit-0.1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 18:09:55.824614 chrono-kit-0.0.2/
--rw-rw-rw-   0        0        0     1084 2023-07-11 21:09:11.000000 chrono-kit-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1075 2023-07-15 18:09:55.824614 chrono-kit-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      587 2023-07-15 18:06:14.000000 chrono-kit-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 18:09:55.798608 chrono-kit-0.0.2/chrono_kit.egg-info/
--rw-rw-rw-   0        0        0     1075 2023-07-15 18:09:55.000000 chrono-kit-0.0.2/chrono_kit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1223 2023-07-15 18:09:55.000000 chrono-kit-0.0.2/chrono_kit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 18:09:55.000000 chrono-kit-0.0.2/chrono_kit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-15 18:09:55.000000 chrono-kit-0.0.2/chrono_kit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-15 18:09:55.799608 chrono-kit-0.0.2/chronokit/
--rw-rw-rw-   0        0        0       72 2023-07-15 17:59:54.000000 chrono-kit-0.0.2/chronokit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:09:55.801609 chrono-kit-0.0.2/chronokit/decomposition/
--rw-rw-rw-   0        0        0       31 2023-07-15 17:08:20.000000 chrono-kit-0.0.2/chronokit/decomposition/__init__.py
--rw-rw-rw-   0        0        0     2178 2023-07-15 17:11:01.000000 chrono-kit-0.0.2/chronokit/decomposition/decompositions.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:09:55.806610 chrono-kit-0.0.2/chronokit/exponential_smoothing/
--rw-rw-rw-   0        0        0     2604 2023-07-15 17:11:39.000000 chrono-kit-0.0.2/chronokit/exponential_smoothing/ETS.py
--rw-rw-rw-   0        0        0     2010 2023-07-15 17:11:46.000000 chrono-kit-0.0.2/chronokit/exponential_smoothing/ExponentialSmoothing.py
--rw-rw-rw-   0        0        0      132 2023-07-15 17:17:08.000000 chrono-kit-0.0.2/chronokit/exponential_smoothing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:09:55.810611 chrono-kit-0.0.2/chronokit/exponential_smoothing/initialization/
--rw-rw-rw-   0        0        0      103 2023-07-11 20:57:13.000000 chrono-kit-0.0.2/chronokit/exponential_smoothing/initialization/__init__.py
--rw-rw-rw-   0        0        0    20217 2023-07-11 20:57:13.000000 chrono-kit-0.0.2/chronokit/exponential_smoothing/initialization/ets_methods.py
--rw-rw-rw-   0        0        0     7992 2023-07-15 17:11:16.000000 chrono-kit-0.0.2/chronokit/exponential_smoothing/initialization/initialization_methods.py
--rw-rw-rw-   0        0        0     8335 2023-07-11 20:57:13.000000 chrono-kit-0.0.2/chronokit/exponential_smoothing/initialization/smoothing_methods.py
--rw-rw-rw-   0        0        0    12189 2023-07-15 17:23:12.000000 chrono-kit-0.0.2/chronokit/exponential_smoothing/model.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:09:55.814612 chrono-kit-0.0.2/chronokit/exponential_smoothing/models/
--rw-rw-rw-   0        0        0       51 2023-07-15 17:19:37.000000 chrono-kit-0.0.2/chronokit/exponential_smoothing/models/__init__.py
--rw-rw-rw-   0        0        0    68075 2023-07-15 17:11:26.000000 chrono-kit-0.0.2/chronokit/exponential_smoothing/models/ets_models.py
--rw-rw-rw-   0        0        0    11941 2023-07-15 17:11:30.000000 chrono-kit-0.0.2/chronokit/exponential_smoothing/models/smoothing.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:09:55.817613 chrono-kit-0.0.2/chronokit/preprocessing/
--rw-rw-rw-   0        0        0       57 2023-07-15 17:08:47.000000 chrono-kit-0.0.2/chronokit/preprocessing/__init__.py
--rw-rw-rw-   0        0        0    17999 2023-07-15 17:59:12.000000 chrono-kit-0.0.2/chronokit/preprocessing/data_transforms.py
--rw-rw-rw-   0        0        0     2791 2023-07-11 20:57:13.000000 chrono-kit-0.0.2/chronokit/preprocessing/dataloader.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:09:55.818613 chrono-kit-0.0.2/chronokit/utils/
--rw-rw-rw-   0        0        0       41 2023-07-15 18:03:39.000000 chrono-kit-0.0.2/chronokit/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:09:55.820613 chrono-kit-0.0.2/chronokit/utils/evaluation_utils/
--rw-rw-rw-   0        0        0       23 2023-07-15 18:05:09.000000 chrono-kit-0.0.2/chronokit/utils/evaluation_utils/__init__.py
--rw-rw-rw-   0        0        0     1204 2023-07-15 17:15:32.000000 chrono-kit-0.0.2/chronokit/utils/evaluation_utils/metrics.py
-drwxrwxrwx   0        0        0        0 2023-07-15 18:09:55.823614 chrono-kit-0.0.2/chronokit/utils/vis_utils/
--rw-rw-rw-   0        0        0       55 2023-07-15 18:04:23.000000 chrono-kit-0.0.2/chronokit/utils/vis_utils/__init__.py
--rw-rw-rw-   0        0        0     4556 2023-07-15 18:02:52.000000 chrono-kit-0.0.2/chronokit/utils/vis_utils/data_plots.py
--rw-rw-rw-   0        0        0     5120 2023-07-15 17:14:06.000000 chrono-kit-0.0.2/chronokit/utils/vis_utils/model_plots.py
--rw-rw-rw-   0        0        0      572 2023-07-15 18:08:20.000000 chrono-kit-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-15 18:09:55.825613 chrono-kit-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-15 18:14:24.564932 chrono-kit-0.1.0/
+-rw-rw-rw-   0        0        0     1084 2023-07-11 21:09:11.000000 chrono-kit-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1075 2023-07-15 18:14:24.564932 chrono-kit-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      587 2023-07-15 18:06:14.000000 chrono-kit-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 18:14:24.540206 chrono-kit-0.1.0/chrono_kit.egg-info/
+-rw-rw-rw-   0        0        0     1075 2023-07-15 18:14:24.000000 chrono-kit-0.1.0/chrono_kit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1223 2023-07-15 18:14:24.000000 chrono-kit-0.1.0/chrono_kit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 18:14:24.000000 chrono-kit-0.1.0/chrono_kit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-15 18:14:24.000000 chrono-kit-0.1.0/chrono_kit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 18:14:24.541206 chrono-kit-0.1.0/chronokit/
+-rw-rw-rw-   0        0        0       72 2023-07-15 17:59:54.000000 chrono-kit-0.1.0/chronokit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:14:24.543206 chrono-kit-0.1.0/chronokit/decomposition/
+-rw-rw-rw-   0        0        0       31 2023-07-15 17:08:20.000000 chrono-kit-0.1.0/chronokit/decomposition/__init__.py
+-rw-rw-rw-   0        0        0     2178 2023-07-15 17:11:01.000000 chrono-kit-0.1.0/chronokit/decomposition/decompositions.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:14:24.546928 chrono-kit-0.1.0/chronokit/exponential_smoothing/
+-rw-rw-rw-   0        0        0     2604 2023-07-15 17:11:39.000000 chrono-kit-0.1.0/chronokit/exponential_smoothing/ETS.py
+-rw-rw-rw-   0        0        0     2010 2023-07-15 17:11:46.000000 chrono-kit-0.1.0/chronokit/exponential_smoothing/ExponentialSmoothing.py
+-rw-rw-rw-   0        0        0      132 2023-07-15 17:17:08.000000 chrono-kit-0.1.0/chronokit/exponential_smoothing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:14:24.551929 chrono-kit-0.1.0/chronokit/exponential_smoothing/initialization/
+-rw-rw-rw-   0        0        0      103 2023-07-11 20:57:13.000000 chrono-kit-0.1.0/chronokit/exponential_smoothing/initialization/__init__.py
+-rw-rw-rw-   0        0        0    20217 2023-07-11 20:57:13.000000 chrono-kit-0.1.0/chronokit/exponential_smoothing/initialization/ets_methods.py
+-rw-rw-rw-   0        0        0     7992 2023-07-15 17:11:16.000000 chrono-kit-0.1.0/chronokit/exponential_smoothing/initialization/initialization_methods.py
+-rw-rw-rw-   0        0        0     8335 2023-07-11 20:57:13.000000 chrono-kit-0.1.0/chronokit/exponential_smoothing/initialization/smoothing_methods.py
+-rw-rw-rw-   0        0        0    12189 2023-07-15 17:23:12.000000 chrono-kit-0.1.0/chronokit/exponential_smoothing/model.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:14:24.554931 chrono-kit-0.1.0/chronokit/exponential_smoothing/models/
+-rw-rw-rw-   0        0        0       51 2023-07-15 17:19:37.000000 chrono-kit-0.1.0/chronokit/exponential_smoothing/models/__init__.py
+-rw-rw-rw-   0        0        0    68075 2023-07-15 17:11:26.000000 chrono-kit-0.1.0/chronokit/exponential_smoothing/models/ets_models.py
+-rw-rw-rw-   0        0        0    11941 2023-07-15 17:11:30.000000 chrono-kit-0.1.0/chronokit/exponential_smoothing/models/smoothing.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:14:24.557931 chrono-kit-0.1.0/chronokit/preprocessing/
+-rw-rw-rw-   0        0        0       57 2023-07-15 17:08:47.000000 chrono-kit-0.1.0/chronokit/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0    17999 2023-07-15 17:59:12.000000 chrono-kit-0.1.0/chronokit/preprocessing/data_transforms.py
+-rw-rw-rw-   0        0        0     2791 2023-07-11 20:57:13.000000 chrono-kit-0.1.0/chronokit/preprocessing/dataloader.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:14:24.558931 chrono-kit-0.1.0/chronokit/utils/
+-rw-rw-rw-   0        0        0       41 2023-07-15 18:03:39.000000 chrono-kit-0.1.0/chronokit/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:14:24.560931 chrono-kit-0.1.0/chronokit/utils/evaluation_utils/
+-rw-rw-rw-   0        0        0       23 2023-07-15 18:05:09.000000 chrono-kit-0.1.0/chronokit/utils/evaluation_utils/__init__.py
+-rw-rw-rw-   0        0        0     1204 2023-07-15 17:15:32.000000 chrono-kit-0.1.0/chronokit/utils/evaluation_utils/metrics.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:14:24.563931 chrono-kit-0.1.0/chronokit/utils/vis_utils/
+-rw-rw-rw-   0        0        0       55 2023-07-15 18:04:23.000000 chrono-kit-0.1.0/chronokit/utils/vis_utils/__init__.py
+-rw-rw-rw-   0        0        0     4556 2023-07-15 18:02:52.000000 chrono-kit-0.1.0/chronokit/utils/vis_utils/data_plots.py
+-rw-rw-rw-   0        0        0     5120 2023-07-15 17:14:06.000000 chrono-kit-0.1.0/chronokit/utils/vis_utils/model_plots.py
+-rw-rw-rw-   0        0        0      572 2023-07-15 18:13:55.000000 chrono-kit-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-15 18:14:24.564932 chrono-kit-0.1.0/setup.cfg
```

### Comparing `chrono-kit-0.0.2/LICENSE.txt` & `chrono-kit-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chrono-kit-0.0.2/PKG-INFO` & `chrono-kit-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrono-kit
-Version: 0.0.2
+Version: 0.1.0
 Summary: An open source python library for time series analysis and forecasting.
 Author-email: ODTU YZT <odtuyzt@gmail.com>
 Project-URL: Homepage, https://github.com/odtuyzt/chrono-kit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `chrono-kit-0.0.2/README.md` & `chrono-kit-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `chrono-kit-0.0.2/chrono_kit.egg-info/PKG-INFO` & `chrono-kit-0.1.0/chrono_kit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrono-kit
-Version: 0.0.2
+Version: 0.1.0
 Summary: An open source python library for time series analysis and forecasting.
 Author-email: ODTU YZT <odtuyzt@gmail.com>
 Project-URL: Homepage, https://github.com/odtuyzt/chrono-kit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `chrono-kit-0.0.2/chrono_kit.egg-info/SOURCES.txt` & `chrono-kit-0.1.0/chrono_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chrono-kit-0.0.2/chronokit/decomposition/decompositions.py` & `chrono-kit-0.1.0/chronokit/decomposition/decompositions.py`

 * *Files identical despite different names*

### Comparing `chrono-kit-0.0.2/chronokit/exponential_smoothing/ETS.py` & `chrono-kit-0.1.0/chronokit/exponential_smoothing/ETS.py`

 * *Files identical despite different names*

### Comparing `chrono-kit-0.0.2/chronokit/exponential_smoothing/ExponentialSmoothing.py` & `chrono-kit-0.1.0/chronokit/exponential_smoothing/ExponentialSmoothing.py`

 * *Files identical despite different names*

### Comparing `chrono-kit-0.0.2/chronokit/exponential_smoothing/initialization/ets_methods.py` & `chrono-kit-0.1.0/chronokit/exponential_smoothing/initialization/ets_methods.py`

 * *Files identical despite different names*

### Comparing `chrono-kit-0.0.2/chronokit/exponential_smoothing/initialization/initialization_methods.py` & `chrono-kit-0.1.0/chronokit/exponential_smoothing/initialization/initialization_methods.py`

 * *Files identical despite different names*

### Comparing `chrono-kit-0.0.2/chronokit/exponential_smoothing/initialization/smoothing_methods.py` & `chrono-kit-0.1.0/chronokit/exponential_smoothing/initialization/smoothing_methods.py`

 * *Files identical despite different names*

### Comparing `chrono-kit-0.0.2/chronokit/exponential_smoothing/model.py` & `chrono-kit-0.1.0/chronokit/exponential_smoothing/model.py`

 * *Files identical despite different names*

### Comparing `chrono-kit-0.0.2/chronokit/exponential_smoothing/models/ets_models.py` & `chrono-kit-0.1.0/chronokit/exponential_smoothing/models/ets_models.py`

 * *Files identical despite different names*

### Comparing `chrono-kit-0.0.2/chronokit/exponential_smoothing/models/smoothing.py` & `chrono-kit-0.1.0/chronokit/exponential_smoothing/models/smoothing.py`

 * *Files identical despite different names*

### Comparing `chrono-kit-0.0.2/chronokit/preprocessing/data_transforms.py` & `chrono-kit-0.1.0/chronokit/preprocessing/data_transforms.py`

 * *Files identical despite different names*

### Comparing `chrono-kit-0.0.2/chronokit/preprocessing/dataloader.py` & `chrono-kit-0.1.0/chronokit/preprocessing/dataloader.py`

 * *Files identical despite different names*

### Comparing `chrono-kit-0.0.2/chronokit/utils/evaluation_utils/metrics.py` & `chrono-kit-0.1.0/chronokit/utils/evaluation_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `chrono-kit-0.0.2/chronokit/utils/vis_utils/data_plots.py` & `chrono-kit-0.1.0/chronokit/utils/vis_utils/data_plots.py`

 * *Files identical despite different names*

### Comparing `chrono-kit-0.0.2/chronokit/utils/vis_utils/model_plots.py` & `chrono-kit-0.1.0/chronokit/utils/vis_utils/model_plots.py`

 * *Files identical despite different names*

### Comparing `chrono-kit-0.0.2/pyproject.toml` & `chrono-kit-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chrono-kit"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
   { name="ODTU YZT", email="odtuyzt@gmail.com" },
 ]
 description = "An open source python library for time series analysis and forecasting."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

