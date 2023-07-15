# Comparing `tmp/pymoutility-0.1.0.tar.gz` & `tmp/pymoutility-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymoutility-0.1.0.tar", max compression
+gzip compressed data, was "pymoutility-0.1.1.tar", max compression
```

## Comparing `pymoutility-0.1.0.tar` & `pymoutility-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1066 2023-07-14 20:03:52.073294 pymoutility-0.1.0/LICENSE
--rw-r--r--   0        0        0     4598 2023-07-14 20:03:52.073294 pymoutility-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-14 20:03:52.073294 pymoutility-0.1.0/pymoutility/__init__.py
--rw-r--r--   0        0        0       70 2023-07-14 20:03:52.073294 pymoutility-0.1.0/pymoutility/decorators.py
--rw-r--r--   0        0        0     5659 2023-07-14 20:03:52.077295 pymoutility-0.1.0/pymoutility/notebooks/Examples.ipynb
--rw-r--r--   0        0        0        0 2023-07-14 20:03:52.077295 pymoutility-0.1.0/pymoutility/src/__init__.py
--rw-r--r--   0        0        0     3470 2023-07-14 20:03:52.077295 pymoutility-0.1.0/pymoutility/src/debugger.py
--rw-r--r--   0        0        0        0 2023-07-14 20:03:52.077295 pymoutility-0.1.0/pymoutility/src/logger_setup.py
--rw-r--r--   0        0        0      637 2023-07-14 20:03:52.077295 pymoutility-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5293 1970-01-01 00:00:00.000000 pymoutility-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-15 05:12:34.267477 pymoutility-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4598 2023-07-15 05:12:34.267477 pymoutility-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-15 05:12:34.271477 pymoutility-0.1.1/pymoutility/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-15 05:12:34.271477 pymoutility-0.1.1/pymoutility/decorators.py
+-rw-r--r--   0        0        0     5659 2023-07-15 05:12:34.271477 pymoutility-0.1.1/pymoutility/notebooks/Examples.ipynb
+-rw-r--r--   0        0        0        0 2023-07-15 05:12:34.271477 pymoutility-0.1.1/pymoutility/src/__init__.py
+-rw-r--r--   0        0        0     3470 2023-07-15 05:12:34.271477 pymoutility-0.1.1/pymoutility/src/debugger.py
+-rw-r--r--   0        0        0        0 2023-07-15 05:12:34.271477 pymoutility-0.1.1/pymoutility/src/logger_setup.py
+-rw-r--r--   0        0        0      637 2023-07-15 05:12:55.711907 pymoutility-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5293 1970-01-01 00:00:00.000000 pymoutility-0.1.1/PKG-INFO
```

### Comparing `pymoutility-0.1.0/LICENSE` & `pymoutility-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymoutility-0.1.0/README.md` & `pymoutility-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pymoutility-0.1.0/pymoutility/notebooks/Examples.ipynb` & `pymoutility-0.1.1/pymoutility/notebooks/Examples.ipynb`

 * *Files identical despite different names*

### Comparing `pymoutility-0.1.0/pymoutility/src/debugger.py` & `pymoutility-0.1.1/pymoutility/src/debugger.py`

 * *Files identical despite different names*

### Comparing `pymoutility-0.1.0/pyproject.toml` & `pymoutility-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymoutility"
-version = "0.1.0"
+version = "0.1.1"
 description = "A handy collection of helper functions, decorators, and utilities designed to streamline and simplify your Python 🐍 development experience. It provides powerful tools to make your code cleaner, more readable, and easier to debug."
 authors = ["JasGujral <jasmeet.gujral@mostacktechnology.com>"]
 license = "./LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pymoutility-0.1.0/PKG-INFO` & `pymoutility-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymoutility
-Version: 0.1.0
+Version: 0.1.1
 Summary: A handy collection of helper functions, decorators, and utilities designed to streamline and simplify your Python 🐍 development experience. It provides powerful tools to make your code cleaner, more readable, and easier to debug.
 License: ./LICENSE
 Author: JasGujral
 Author-email: jasmeet.gujral@mostacktechnology.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

