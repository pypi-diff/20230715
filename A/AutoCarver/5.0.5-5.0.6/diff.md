# Comparing `tmp/AutoCarver-5.0.5.tar.gz` & `tmp/AutoCarver-5.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-5.0.5.tar", last modified: Sat Jul 15 10:32:27 2023, max compression
+gzip compressed data, was "AutoCarver-5.0.6.tar", last modified: Sat Jul 15 10:37:58 2023, max compression
```

## Comparing `AutoCarver-5.0.5.tar` & `AutoCarver-5.0.6.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:32:27.488274 AutoCarver-5.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:32:27.484274 AutoCarver-5.0.5/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31467 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/auto_carver.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:32:27.484274 AutoCarver-5.0.5/AutoCarver/discretizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22819 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/discretizers/discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:32:27.488274 AutoCarver-5.0.5/AutoCarver/discretizers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/discretizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32230 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/discretizers/utils/base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/discretizers/utils/grouped_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/discretizers/utils/qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/discretizers/utils/quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/discretizers/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/discretizers/utils/type_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28779 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/AutoCarver/feature_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:32:27.484274 AutoCarver-5.0.5/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-15 10:32:27.000000 AutoCarver-5.0.5/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-15 10:32:27.000000 AutoCarver-5.0.5/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 10:32:27.000000 AutoCarver-5.0.5/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-15 10:32:27.000000 AutoCarver-5.0.5/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-15 10:32:27.488274 AutoCarver-5.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-15 10:32:27.488274 AutoCarver-5.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:32:27.488274 AutoCarver-5.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/tests/test_auto_carver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/tests/test_base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/tests/test_converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/tests/test_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/tests/test_feature_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/tests/test_grouped_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/tests/test_qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/tests/test_quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-15 10:32:12.000000 AutoCarver-5.0.5/tests/test_type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:58.572585 AutoCarver-5.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:58.568585 AutoCarver-5.0.6/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31467 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/AutoCarver/auto_carver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/AutoCarver/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:58.568585 AutoCarver-5.0.6/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22819 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:58.568585 AutoCarver-5.0.6/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32230 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/AutoCarver/discretizers/utils/grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/AutoCarver/discretizers/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/AutoCarver/discretizers/utils/type_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28779 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/AutoCarver/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:58.568585 AutoCarver-5.0.6/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-15 10:37:58.000000 AutoCarver-5.0.6/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-15 10:37:58.000000 AutoCarver-5.0.6/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 10:37:58.000000 AutoCarver-5.0.6/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-15 10:37:58.000000 AutoCarver-5.0.6/AutoCarver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-15 10:37:58.000000 AutoCarver-5.0.6/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20332 2023-07-15 10:37:58.572585 AutoCarver-5.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-15 10:37:58.572585 AutoCarver-5.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:58.572585 AutoCarver-5.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/tests/test_auto_carver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/tests/test_base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/tests/test_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/tests/test_feature_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/tests/test_grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/tests/test_qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/tests/test_quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-15 10:37:46.000000 AutoCarver-5.0.6/tests/test_type_discretizers.py
```

### Comparing `AutoCarver-5.0.5/AutoCarver/auto_carver.py` & `AutoCarver-5.0.6/AutoCarver/auto_carver.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.5/AutoCarver/converters.py` & `AutoCarver-5.0.6/AutoCarver/converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.5/AutoCarver/discretizers/discretizers.py` & `AutoCarver-5.0.6/AutoCarver/discretizers/discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.5/AutoCarver/discretizers/utils/base_discretizers.py` & `AutoCarver-5.0.6/AutoCarver/discretizers/utils/base_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.5/AutoCarver/discretizers/utils/grouped_list.py` & `AutoCarver-5.0.6/AutoCarver/discretizers/utils/grouped_list.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.5/AutoCarver/discretizers/utils/qualitative_discretizers.py` & `AutoCarver-5.0.6/AutoCarver/discretizers/utils/qualitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.5/AutoCarver/discretizers/utils/quantitative_discretizers.py` & `AutoCarver-5.0.6/AutoCarver/discretizers/utils/quantitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.5/AutoCarver/discretizers/utils/serialization.py` & `AutoCarver-5.0.6/AutoCarver/discretizers/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.5/AutoCarver/discretizers/utils/type_discretizers.py` & `AutoCarver-5.0.6/AutoCarver/discretizers/utils/type_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.5/AutoCarver/feature_selector.py` & `AutoCarver-5.0.6/AutoCarver/feature_selector.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.5/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-5.0.6/AutoCarver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.0.5
+Version: 5.0.6
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 \n</p>
 <p align="center">
     <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
```

### Comparing `AutoCarver-5.0.5/AutoCarver.egg-info/SOURCES.txt` & `AutoCarver-5.0.6/AutoCarver.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 AutoCarver/__init__.py
 AutoCarver/auto_carver.py
 AutoCarver/converters.py
 AutoCarver/feature_selector.py
 AutoCarver.egg-info/PKG-INFO
 AutoCarver.egg-info/SOURCES.txt
 AutoCarver.egg-info/dependency_links.txt
+AutoCarver.egg-info/requires.txt
 AutoCarver.egg-info/top_level.txt
 AutoCarver/discretizers/__init__.py
 AutoCarver/discretizers/discretizers.py
 AutoCarver/discretizers/utils/__init__.py
 AutoCarver/discretizers/utils/base_discretizers.py
 AutoCarver/discretizers/utils/grouped_list.py
 AutoCarver/discretizers/utils/qualitative_discretizers.py
```

### Comparing `AutoCarver-5.0.5/LICENSE` & `AutoCarver-5.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.5/PKG-INFO` & `AutoCarver-5.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.0.5
+Version: 5.0.6
 Summary: Automatic Bucketizing of Features with Optimal Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 \n</p>
 <p align="center">
     <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver?style=flat-square">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver?style=flat-square">
```

### Comparing `AutoCarver-5.0.5/README.md` & `AutoCarver-5.0.6/README.md`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.5/setup.py` & `AutoCarver-5.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,33 +6,42 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="AutoCarver",
-    version="5.0.5",
+    version="5.0.6",
     author="Mario DEFRANCE",
     author_email="defrancemario@gmail.com",
     description="Automatic Bucketizing of Features with Optimal Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mdefrance/AutoCarver",
     project_urls={
         "Bug Tracker": "https://github.com/mdefrance/AutoCarver/issues"
     },
     license="MIT",
-    # install_requires= # TODO,
+    install_requires=[
+        'pandas',
+        'numpy',
+        'scipy',
+        'scikit-learn',
+        'statsmodels',
+        'tqdm',
+        'matplotlib',
+        'seaborn',
+    ],
     packages=find_packages(),
     classifiers=[
         # ou 4 - Beta ou 5 - Production/Stable
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: Unix",
         # "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.9",
 )
```

### Comparing `AutoCarver-5.0.5/tests/test_auto_carver.py` & `AutoCarver-5.0.6/tests/test_auto_carver.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.5/tests/test_base_discretizers.py` & `AutoCarver-5.0.6/tests/test_base_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.5/tests/test_discretizers.py` & `AutoCarver-5.0.6/tests/test_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.5/tests/test_grouped_list.py` & `AutoCarver-5.0.6/tests/test_grouped_list.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.5/tests/test_qualitative_discretizers.py` & `AutoCarver-5.0.6/tests/test_qualitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.5/tests/test_quantitative_discretizers.py` & `AutoCarver-5.0.6/tests/test_quantitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.0.5/tests/test_type_discretizers.py` & `AutoCarver-5.0.6/tests/test_type_discretizers.py`

 * *Files identical despite different names*

