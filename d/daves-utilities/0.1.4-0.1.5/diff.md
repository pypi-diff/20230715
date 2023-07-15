# Comparing `tmp/daves_utilities-0.1.4.tar.gz` & `tmp/daves_utilities-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daves_utilities-0.1.4.tar", max compression
+gzip compressed data, was "daves_utilities-0.1.5.tar", max compression
```

## Comparing `daves_utilities-0.1.4.tar` & `daves_utilities-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1087 2022-12-31 15:33:52.562362 daves_utilities-0.1.4/LICENSE
--rw-r--r--   0        0        0       19 2022-12-31 15:33:52.565062 daves_utilities-0.1.4/README.md
--rw-r--r--   0        0        0     1370 2023-07-15 13:53:38.624030 daves_utilities-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      419 2023-07-15 13:45:38.727093 daves_utilities-0.1.4/src/daves_utilities/__init__.py
--rw-r--r--   0        0        0     1475 2023-07-15 13:21:21.764496 daves_utilities-0.1.4/src/daves_utilities/archive/is_equal.py
--rw-r--r--   0        0        0     3478 2023-01-01 15:53:17.727021 daves_utilities-0.1.4/src/daves_utilities/archive/print_structure.py
--rw-r--r--   0        0        0      554 2023-07-15 13:21:21.747226 daves_utilities-0.1.4/src/daves_utilities/david_secrets.py
--rw-r--r--   0        0        0     5184 2023-07-15 13:21:21.799335 daves_utilities-0.1.4/src/daves_utilities/iterator.py
--rw-r--r--   0        0        0     2285 1970-01-01 00:00:00.000000 daves_utilities-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1087 2022-12-31 15:33:52.562362 daves_utilities-0.1.5/LICENSE
+-rw-r--r--   0        0        0       19 2022-12-31 15:33:52.565062 daves_utilities-0.1.5/README.md
+-rw-r--r--   0        0        0     1370 2023-07-15 13:56:04.230500 daves_utilities-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      410 2023-07-15 13:55:46.565253 daves_utilities-0.1.5/src/daves_utilities/__init__.py
+-rw-r--r--   0        0        0     1475 2023-07-15 13:21:21.764496 daves_utilities-0.1.5/src/daves_utilities/archive/is_equal.py
+-rw-r--r--   0        0        0     3478 2023-01-01 15:53:17.727021 daves_utilities-0.1.5/src/daves_utilities/archive/print_structure.py
+-rw-r--r--   0        0        0      554 2023-07-15 13:21:21.747226 daves_utilities-0.1.5/src/daves_utilities/david_secrets.py
+-rw-r--r--   0        0        0     5184 2023-07-15 13:21:21.799335 daves_utilities-0.1.5/src/daves_utilities/iterator.py
+-rw-r--r--   0        0        0     2285 1970-01-01 00:00:00.000000 daves_utilities-0.1.5/PKG-INFO
```

### Comparing `daves_utilities-0.1.4/LICENSE` & `daves_utilities-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.4/pyproject.toml` & `daves_utilities-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ########################################################################################
 # POETRY                                                                               #
 ########################################################################################
 [tool.poetry]
 name = "daves_utilities"
 authors = ["David Kuchelmeister"]
 description = "some useful function for myself"
-version = "0.1.4"
+version = "0.1.5"
 
 license = "MIT"
 
 repository = "https://github.com/kuchedav/daves_utilities"
 
 # README file(s) are used as the package description
 readme = ["README.md", "LICENSE"]
```

### Comparing `daves_utilities-0.1.4/src/daves_utilities/archive/is_equal.py` & `daves_utilities-0.1.5/src/daves_utilities/archive/is_equal.py`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.4/src/daves_utilities/archive/print_structure.py` & `daves_utilities-0.1.5/src/daves_utilities/archive/print_structure.py`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.4/src/daves_utilities/david_secrets.py` & `daves_utilities-0.1.5/src/daves_utilities/david_secrets.py`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.4/src/daves_utilities/iterator.py` & `daves_utilities-0.1.5/src/daves_utilities/iterator.py`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.4/PKG-INFO` & `daves_utilities-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daves-utilities
-Version: 0.1.4
+Version: 0.1.5
 Summary: some useful function for myself
 Home-page: https://github.com/kuchedav/daves_utilities
 License: MIT
 Keywords: packaging,poetry
 Author: David Kuchelmeister
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

