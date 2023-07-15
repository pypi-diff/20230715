# Comparing `tmp/AutoCarver-5.0.7.tar.gz` & `tmp/AutoCarver-5.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-5.0.7.tar", last modified: Sat Jul 15 13:13:59 2023, max compression
+gzip compressed data, was "AutoCarver-5.0.8.tar", last modified: Sat Jul 15 18:06:52 2023, max compression
```

## Comparing `AutoCarver-5.0.7.tar` & `AutoCarver-5.0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:13:59.884398 AutoCarver-5.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:13:59.876398 AutoCarver-5.0.7/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/AutoCarver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30164 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/AutoCarver/auto_carver.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/AutoCarver/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:13:59.880398 AutoCarver-5.0.7/AutoCarver/discretizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/AutoCarver/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22819 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/AutoCarver/discretizers/discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:13:59.880398 AutoCarver-5.0.7/AutoCarver/discretizers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/AutoCarver/discretizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32200 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/AutoCarver/discretizers/utils/base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/AutoCarver/discretizers/utils/grouped_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/AutoCarver/discretizers/utils/qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/AutoCarver/discretizers/utils/quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/AutoCarver/discretizers/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/AutoCarver/discretizers/utils/type_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28779 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/AutoCarver/feature_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:13:59.880398 AutoCarver-5.0.7/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19539 2023-07-15 13:13:59.000000 AutoCarver-5.0.7/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-15 13:13:59.000000 AutoCarver-5.0.7/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 13:13:59.000000 AutoCarver-5.0.7/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-15 13:13:59.000000 AutoCarver-5.0.7/AutoCarver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-15 13:13:59.000000 AutoCarver-5.0.7/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19539 2023-07-15 13:13:59.884398 AutoCarver-5.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18795 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-15 13:13:59.884398 AutoCarver-5.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:13:59.884398 AutoCarver-5.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/tests/test_auto_carver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/tests/test_base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/tests/test_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/tests/test_feature_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/tests/test_grouped_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/tests/test_qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/tests/test_quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-15 13:13:48.000000 AutoCarver-5.0.7/tests/test_type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:06:52.704797 AutoCarver-5.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:06:52.704797 AutoCarver-5.0.8/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30155 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/auto_carver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:06:52.704797 AutoCarver-5.0.8/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22819 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:06:52.704797 AutoCarver-5.0.8/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32200 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/discretizers/utils/grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/discretizers/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/discretizers/utils/type_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28779 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/AutoCarver/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:06:52.704797 AutoCarver-5.0.8/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-07-15 18:06:52.000000 AutoCarver-5.0.8/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-15 18:06:52.000000 AutoCarver-5.0.8/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 18:06:52.000000 AutoCarver-5.0.8/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-15 18:06:52.000000 AutoCarver-5.0.8/AutoCarver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-15 18:06:52.000000 AutoCarver-5.0.8/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-07-15 18:06:52.704797 AutoCarver-5.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18904 2023-07-15 18:06:36.000000 AutoCarver-5.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-15 18:06:52.704797 AutoCarver-5.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:06:52.704797 AutoCarver-5.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/tests/test_auto_carver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/tests/test_base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/tests/test_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/tests/test_feature_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/tests/test_grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12437 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/tests/test_qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/tests/test_quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-15 18:06:37.000000 AutoCarver-5.0.8/tests/test_type_discretizers.py
```

### Comparing `AutoCarver-5.0.7/AutoCarver/auto_carver.py` & `AutoCarver-5.0.8/AutoCarver/auto_carver.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from .discretizers.discretizers import Discretizer
 from .discretizers.utils.base_discretizers import (
     GroupedListDiscretizer,
     convert_to_labels,
     convert_to_values,
 )
-from .discretizers.utils.grouped_list import GroupedList, is_equal
+from .discretizers.utils.grouped_list import GroupedList
 from .discretizers.utils.serialization import json_deserialize_values_orders
 
 
 class AutoCarver(GroupedListDiscretizer):
     """Automatic carving of continuous, categorical and categorical ordinal
     features that maximizes association with a binary target.
 
@@ -123,15 +123,15 @@
         min_carved_freq: float = 0,  # TODO: update this parameter so that it is set according to frequency rather than number of groups
         sort_by: str = "tschuprowt",
         str_nan: str = "__NAN__",
         str_default: str = "__OTHER__",
         output_dtype: str = "float",
         dropna: bool = True,
         copy: bool = False,
-        verbose: bool = True,
+        verbose: bool = False,
         pretty_print: bool = False,
     ) -> None:
         """_summary_
 
         Parameters
         ----------
         quantitative_features : list[str]
```

### Comparing `AutoCarver-5.0.7/AutoCarver/converters.py` & `AutoCarver-5.0.8/AutoCarver/converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.7/AutoCarver/discretizers/discretizers.py` & `AutoCarver-5.0.8/AutoCarver/discretizers/discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.7/AutoCarver/discretizers/utils/base_discretizers.py` & `AutoCarver-5.0.8/AutoCarver/discretizers/utils/base_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.7/AutoCarver/discretizers/utils/grouped_list.py` & `AutoCarver-5.0.8/AutoCarver/discretizers/utils/grouped_list.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.7/AutoCarver/discretizers/utils/qualitative_discretizers.py` & `AutoCarver-5.0.8/AutoCarver/discretizers/utils/qualitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.7/AutoCarver/discretizers/utils/quantitative_discretizers.py` & `AutoCarver-5.0.8/AutoCarver/discretizers/utils/quantitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.7/AutoCarver/discretizers/utils/serialization.py` & `AutoCarver-5.0.8/AutoCarver/discretizers/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.7/AutoCarver/discretizers/utils/type_discretizers.py` & `AutoCarver-5.0.8/AutoCarver/discretizers/utils/type_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.7/AutoCarver/feature_selector.py` & `AutoCarver-5.0.8/AutoCarver/feature_selector.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.7/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-5.0.8/AutoCarver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.0.7
+Version: 5.0.8
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
@@ -15,18 +15,19 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 \n</p>
-<p align="center">
+<p align="left">
     <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
     <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver?style=flat-square">
+    <img src='https://readthedocs.org/projects/autocarver/badge/?version=latest' alt='Documentation Status' />
 </p>
 
 This is a work in progress.
 
 # AutoCarver
 
 **AutoCarver** is a powerful set of tools designed for binary classification problems. It offers a range of functionalities to enhance the feature engineering process and improve the performance of binary classification models. It provides:
```

### Comparing `AutoCarver-5.0.7/AutoCarver.egg-info/SOURCES.txt` & `AutoCarver-5.0.8/AutoCarver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.7/LICENSE` & `AutoCarver-5.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.7/PKG-INFO` & `AutoCarver-5.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.0.7
+Version: 5.0.8
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
@@ -15,18 +15,19 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 \n</p>
-<p align="center">
+<p align="left">
     <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
     <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver?style=flat-square">
+    <img src='https://readthedocs.org/projects/autocarver/badge/?version=latest' alt='Documentation Status' />
 </p>
 
 This is a work in progress.
 
 # AutoCarver
 
 **AutoCarver** is a powerful set of tools designed for binary classification problems. It offers a range of functionalities to enhance the feature engineering process and improve the performance of binary classification models. It provides:
```

### Comparing `AutoCarver-5.0.7/README.md` & `AutoCarver-5.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 </p>
-<p align="center">
+<p align="left">
     <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
     <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver?style=flat-square">
+    <img src='https://readthedocs.org/projects/autocarver/badge/?version=latest' alt='Documentation Status' />
 </p>
 
 This is a work in progress.
 
 # AutoCarver
 
 **AutoCarver** is a powerful set of tools designed for binary classification problems. It offers a range of functionalities to enhance the feature engineering process and improve the performance of binary classification models. It provides:
```

### Comparing `AutoCarver-5.0.7/setup.py` & `AutoCarver-5.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="AutoCarver",
-    version="5.0.7",
+    version="5.0.8",
     author="Mario DEFRANCE",
     author_email="defrancemario@gmail.com",
     description="Automatic Bucketizing of Features with Optimal Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mdefrance/AutoCarver",
     project_urls={
```

### Comparing `AutoCarver-5.0.7/tests/test_auto_carver.py` & `AutoCarver-5.0.8/tests/test_auto_carver.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.7/tests/test_base_discretizers.py` & `AutoCarver-5.0.8/tests/test_base_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.7/tests/test_discretizers.py` & `AutoCarver-5.0.8/tests/test_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.7/tests/test_grouped_list.py` & `AutoCarver-5.0.8/tests/test_grouped_list.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.7/tests/test_qualitative_discretizers.py` & `AutoCarver-5.0.8/tests/test_qualitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.7/tests/test_quantitative_discretizers.py` & `AutoCarver-5.0.8/tests/test_quantitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.7/tests/test_type_discretizers.py` & `AutoCarver-5.0.8/tests/test_type_discretizers.py`

 * *Files identical despite different names*

