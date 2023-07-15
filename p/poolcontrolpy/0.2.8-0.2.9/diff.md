# Comparing `tmp/poolcontrolpy-0.2.8.tar.gz` & `tmp/poolcontrolpy-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poolcontrolpy-0.2.8.tar", max compression
+gzip compressed data, was "poolcontrolpy-0.2.9.tar", max compression
```

## Comparing `poolcontrolpy-0.2.8.tar` & `poolcontrolpy-0.2.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1073 2023-06-08 12:23:30.579218 poolcontrolpy-0.2.8/LICENSE
--rwxr-xr-x   0        0        0     1237 2023-06-08 12:23:30.579218 poolcontrolpy-0.2.8/README.md
--rwxr-xr-x   0        0        0     1265 2023-06-08 12:24:14.147358 poolcontrolpy-0.2.8/pyproject.toml
--rwxr-xr-x   0        0        0      115 2023-06-08 12:23:30.583218 poolcontrolpy-0.2.8/src/poolcontrolpy/__init__.py
--rw-r--r--   0        0        0      770 2023-06-08 12:23:30.583218 poolcontrolpy-0.2.8/src/poolcontrolpy/exceptions.py
--rwxr-xr-x   0        0        0     4466 2023-06-08 12:23:30.583218 poolcontrolpy-0.2.8/src/poolcontrolpy/poolcontrolpy.py
--rw-r--r--   0        0        0     1784 1970-01-01 00:00:00.000000 poolcontrolpy-0.2.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1073 2023-07-15 19:09:44.042881 poolcontrolpy-0.2.9/LICENSE
+-rwxr-xr-x   0        0        0     1237 2023-07-15 19:09:44.042881 poolcontrolpy-0.2.9/README.md
+-rwxr-xr-x   0        0        0     1265 2023-07-15 19:10:21.727248 poolcontrolpy-0.2.9/pyproject.toml
+-rwxr-xr-x   0        0        0      115 2023-07-15 19:09:44.046881 poolcontrolpy-0.2.9/src/poolcontrolpy/__init__.py
+-rw-r--r--   0        0        0      770 2023-07-15 19:09:44.046881 poolcontrolpy-0.2.9/src/poolcontrolpy/exceptions.py
+-rwxr-xr-x   0        0        0     4466 2023-07-15 19:09:44.046881 poolcontrolpy-0.2.9/src/poolcontrolpy/poolcontrolpy.py
+-rw-r--r--   0        0        0     1784 1970-01-01 00:00:00.000000 poolcontrolpy-0.2.9/PKG-INFO
```

### Comparing `poolcontrolpy-0.2.8/LICENSE` & `poolcontrolpy-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `poolcontrolpy-0.2.8/README.md` & `poolcontrolpy-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `poolcontrolpy-0.2.8/pyproject.toml` & `poolcontrolpy-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poolcontrolpy"
-version = "0.2.8"
+version = "0.2.9"
 description = "Package for accessing nodejs-poolController"
 authors = ["Kevin Robinson"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `poolcontrolpy-0.2.8/src/poolcontrolpy/exceptions.py` & `poolcontrolpy-0.2.9/src/poolcontrolpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `poolcontrolpy-0.2.8/src/poolcontrolpy/poolcontrolpy.py` & `poolcontrolpy-0.2.9/src/poolcontrolpy/poolcontrolpy.py`

 * *Files identical despite different names*

### Comparing `poolcontrolpy-0.2.8/PKG-INFO` & `poolcontrolpy-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poolcontrolpy
-Version: 0.2.8
+Version: 0.2.9
 Summary: Package for accessing nodejs-poolController
 License: MIT
 Author: Kevin Robinson
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

