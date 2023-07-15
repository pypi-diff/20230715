# Comparing `tmp/daves_utilities-0.1.6.tar.gz` & `tmp/daves_utilities-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daves_utilities-0.1.6.tar", max compression
+gzip compressed data, was "daves_utilities-0.1.7.tar", max compression
```

## Comparing `daves_utilities-0.1.6.tar` & `daves_utilities-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1087 2022-12-31 15:33:52.562362 daves_utilities-0.1.6/LICENSE
--rw-r--r--   0        0        0       19 2022-12-31 15:33:52.565062 daves_utilities-0.1.6/README.md
--rw-r--r--   0        0        0     1370 2023-07-15 14:00:18.904466 daves_utilities-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      703 2023-07-15 13:59:58.779869 daves_utilities-0.1.6/src/daves_utilities/__init__.py
--rw-r--r--   0        0        0     2600 2023-07-15 13:59:00.262111 daves_utilities-0.1.6/src/daves_utilities/archive/fun_save.py
--rw-r--r--   0        0        0     1475 2023-07-15 13:21:21.764496 daves_utilities-0.1.6/src/daves_utilities/archive/is_equal.py
--rw-r--r--   0        0        0     3478 2023-01-01 15:53:17.727021 daves_utilities-0.1.6/src/daves_utilities/archive/print_structure.py
--rw-r--r--   0        0        0      554 2023-07-15 13:58:43.390194 daves_utilities-0.1.6/src/daves_utilities/david_secrets.py
--rw-r--r--   0        0        0     5184 2023-07-15 13:21:21.799335 daves_utilities-0.1.6/src/daves_utilities/iterator.py
--rw-r--r--   0        0        0     2285 1970-01-01 00:00:00.000000 daves_utilities-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1087 2022-12-31 15:33:52.562362 daves_utilities-0.1.7/LICENSE
+-rw-r--r--   0        0        0       19 2022-12-31 15:33:52.565062 daves_utilities-0.1.7/README.md
+-rw-r--r--   0        0        0     1370 2023-07-15 14:01:17.122596 daves_utilities-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      697 2023-07-15 14:01:05.585224 daves_utilities-0.1.7/src/daves_utilities/__init__.py
+-rw-r--r--   0        0        0     2600 2023-07-15 13:59:00.262111 daves_utilities-0.1.7/src/daves_utilities/archive/fun_save.py
+-rw-r--r--   0        0        0     1475 2023-07-15 13:21:21.764496 daves_utilities-0.1.7/src/daves_utilities/archive/is_equal.py
+-rw-r--r--   0        0        0     3478 2023-01-01 15:53:17.727021 daves_utilities-0.1.7/src/daves_utilities/archive/print_structure.py
+-rw-r--r--   0        0        0      554 2023-07-15 13:58:43.390194 daves_utilities-0.1.7/src/daves_utilities/david_secrets.py
+-rw-r--r--   0        0        0     5184 2023-07-15 13:21:21.799335 daves_utilities-0.1.7/src/daves_utilities/iterator.py
+-rw-r--r--   0        0        0     2285 1970-01-01 00:00:00.000000 daves_utilities-0.1.7/PKG-INFO
```

### Comparing `daves_utilities-0.1.6/LICENSE` & `daves_utilities-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.6/pyproject.toml` & `daves_utilities-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ########################################################################################
 # POETRY                                                                               #
 ########################################################################################
 [tool.poetry]
 name = "daves_utilities"
 authors = ["David Kuchelmeister"]
 description = "some useful function for myself"
-version = "0.1.6"
+version = "0.1.7"
 
 license = "MIT"
 
 repository = "https://github.com/kuchedav/daves_utilities"
 
 # README file(s) are used as the package description
 readme = ["README.md", "LICENSE"]
```

### Comparing `daves_utilities-0.1.6/src/daves_utilities/__init__.py` & `daves_utilities-0.1.7/src/daves_utilities/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Daves utilities is a collection of useful python functions which I would like to
 provide to anybody who is interested in using them.
 """
 from daves_utilities.archive.fun_save import fun_save
 from daves_utilities.archive.is_equal import is_equal
-from daves_utilities.archive.print_structure import print_structure
+from daves_utilities.archive.print_structure import print_str
 from daves_utilities.david_secrets import decrypt_message
 from daves_utilities.david_secrets import encrypt_message
 from daves_utilities.david_secrets import generate_key
 from daves_utilities.iterator import for_long
 
 __all__ = [
     "for_long",
```

### Comparing `daves_utilities-0.1.6/src/daves_utilities/archive/fun_save.py` & `daves_utilities-0.1.7/src/daves_utilities/archive/fun_save.py`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.6/src/daves_utilities/archive/is_equal.py` & `daves_utilities-0.1.7/src/daves_utilities/archive/is_equal.py`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.6/src/daves_utilities/archive/print_structure.py` & `daves_utilities-0.1.7/src/daves_utilities/archive/print_structure.py`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.6/src/daves_utilities/david_secrets.py` & `daves_utilities-0.1.7/src/daves_utilities/david_secrets.py`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.6/src/daves_utilities/iterator.py` & `daves_utilities-0.1.7/src/daves_utilities/iterator.py`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.6/PKG-INFO` & `daves_utilities-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daves-utilities
-Version: 0.1.6
+Version: 0.1.7
 Summary: some useful function for myself
 Home-page: https://github.com/kuchedav/daves_utilities
 License: MIT
 Keywords: packaging,poetry
 Author: David Kuchelmeister
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

