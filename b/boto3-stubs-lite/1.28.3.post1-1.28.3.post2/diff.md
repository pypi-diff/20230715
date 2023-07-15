# Comparing `tmp/boto3-stubs-lite-1.28.3.post1.tar.gz` & `tmp/boto3-stubs-lite-1.28.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto3-stubs-lite-1.28.3.post1.tar", last modified: Fri Jul 14 16:18:03 2023, max compression
+gzip compressed data, was "boto3-stubs-lite-1.28.3.post2.tar", last modified: Sat Jul 15 06:38:36 2023, max compression
```

## Comparing `boto3-stubs-lite-1.28.3.post1.tar` & `boto3-stubs-lite-1.28.3.post2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.863833 boto3-stubs-lite-1.28.3.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 16:15:15.000000 boto3-stubs-lite-1.28.3.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    77448 2023-07-14 16:18:03.863833 boto3-stubs-lite-1.28.3.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    66011 2023-07-14 16:15:15.000000 boto3-stubs-lite-1.28.3.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.855832 boto3-stubs-lite-1.28.3.post1/boto3-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/compat.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.855832 boto3-stubs-lite-1.28.3.post1/boto3-stubs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/docs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/docs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.863833 boto3-stubs-lite-1.28.3.post1/boto3-stubs/dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/dynamodb/conditions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/dynamodb/table.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/dynamodb/transform.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/dynamodb/types.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.863833 boto3-stubs-lite-1.28.3.post1/boto3-stubs/ec2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/ec2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/ec2/createtags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/ec2/deletetags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:15:15.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.863833 boto3-stubs-lite-1.28.3.post1/boto3-stubs/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/resources/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/resources/action.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/resources/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/resources/collection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/resources/factory.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/resources/model.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/resources/params.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/resources/response.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.863833 boto3-stubs-lite-1.28.3.post1/boto3-stubs/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/s3/inject.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/s3/transfer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/session.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-14 16:15:13.000000 boto3-stubs-lite-1.28.3.post1/boto3-stubs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 16:18:03.863833 boto3-stubs-lite-1.28.3.post1/boto3_stubs_lite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    77448 2023-07-14 16:18:03.000000 boto3-stubs-lite-1.28.3.post1/boto3_stubs_lite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-14 16:18:03.000000 boto3-stubs-lite-1.28.3.post1/boto3_stubs_lite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:03.000000 boto3-stubs-lite-1.28.3.post1/boto3_stubs_lite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 16:18:03.000000 boto3-stubs-lite-1.28.3.post1/boto3_stubs_lite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)    33283 2023-07-14 16:18:03.000000 boto3-stubs-lite-1.28.3.post1/boto3_stubs_lite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 16:18:03.000000 boto3-stubs-lite-1.28.3.post1/boto3_stubs_lite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 16:18:03.863833 boto3-stubs-lite-1.28.3.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    46055 2023-07-14 16:15:14.000000 boto3-stubs-lite-1.28.3.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:36.714478 boto3-stubs-lite-1.28.3.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 06:35:42.000000 boto3-stubs-lite-1.28.3.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    77448 2023-07-15 06:38:36.714478 boto3-stubs-lite-1.28.3.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    66011 2023-07-15 06:35:42.000000 boto3-stubs-lite-1.28.3.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:36.710478 boto3-stubs-lite-1.28.3.post2/boto3-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/compat.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:36.710478 boto3-stubs-lite-1.28.3.post2/boto3-stubs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/docs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/docs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:36.710478 boto3-stubs-lite-1.28.3.post2/boto3-stubs/dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/dynamodb/conditions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/dynamodb/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/dynamodb/transform.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/dynamodb/types.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:36.710478 boto3-stubs-lite-1.28.3.post2/boto3-stubs/ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/ec2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/ec2/createtags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/ec2/deletetags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:35:42.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:36.710478 boto3-stubs-lite-1.28.3.post2/boto3-stubs/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/resources/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/resources/action.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/resources/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/resources/collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/resources/factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/resources/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/resources/params.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/resources/response.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:36.710478 boto3-stubs-lite-1.28.3.post2/boto3-stubs/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/s3/inject.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/s3/transfer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/boto3-stubs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:38:36.714478 boto3-stubs-lite-1.28.3.post2/boto3_stubs_lite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    77448 2023-07-15 06:38:36.000000 boto3-stubs-lite-1.28.3.post2/boto3_stubs_lite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-15 06:38:36.000000 boto3-stubs-lite-1.28.3.post2/boto3_stubs_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:36.000000 boto3-stubs-lite-1.28.3.post2/boto3_stubs_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:38:36.000000 boto3-stubs-lite-1.28.3.post2/boto3_stubs_lite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)    33283 2023-07-15 06:38:36.000000 boto3-stubs-lite-1.28.3.post2/boto3_stubs_lite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 06:38:36.000000 boto3-stubs-lite-1.28.3.post2/boto3_stubs_lite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:38:36.714478 boto3-stubs-lite-1.28.3.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    46055 2023-07-15 06:35:41.000000 boto3-stubs-lite-1.28.3.post2/setup.py
```

### Comparing `boto3-stubs-lite-1.28.3.post1/LICENSE` & `boto3-stubs-lite-1.28.3.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/PKG-INFO` & `boto3-stubs-lite-1.28.3.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: boto3-stubs-lite
-Version: 1.28.3.post1
-Summary: Type annotations for boto3 1.28.3 generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3 1.28.3 generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -400,15 +400,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.7](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [boto3-stubs-lite docs](https://youtype.github.io/boto3_stubs_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
```

### Comparing `boto3-stubs-lite-1.28.3.post1/README.md` & `boto3-stubs-lite-1.28.3.post2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.7](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [boto3-stubs-lite docs](https://youtype.github.io/boto3_stubs_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
```

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3-stubs/__init__.pyi` & `boto3-stubs-lite-1.28.3.post2/boto3-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3-stubs/docs/utils.pyi` & `boto3-stubs-lite-1.28.3.post2/boto3-stubs/docs/utils.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3-stubs/dynamodb/conditions.pyi` & `boto3-stubs-lite-1.28.3.post2/boto3-stubs/dynamodb/conditions.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3-stubs/dynamodb/table.pyi` & `boto3-stubs-lite-1.28.3.post2/boto3-stubs/dynamodb/table.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3-stubs/dynamodb/transform.pyi` & `boto3-stubs-lite-1.28.3.post2/boto3-stubs/dynamodb/transform.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3-stubs/dynamodb/types.pyi` & `boto3-stubs-lite-1.28.3.post2/boto3-stubs/dynamodb/types.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3-stubs/exceptions.pyi` & `boto3-stubs-lite-1.28.3.post2/boto3-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3-stubs/resources/action.pyi` & `boto3-stubs-lite-1.28.3.post2/boto3-stubs/resources/action.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3-stubs/resources/base.pyi` & `boto3-stubs-lite-1.28.3.post2/boto3-stubs/resources/base.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3-stubs/resources/collection.pyi` & `boto3-stubs-lite-1.28.3.post2/boto3-stubs/resources/collection.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3-stubs/resources/model.pyi` & `boto3-stubs-lite-1.28.3.post2/boto3-stubs/resources/model.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3-stubs/resources/params.pyi` & `boto3-stubs-lite-1.28.3.post2/boto3-stubs/resources/params.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3-stubs/resources/response.pyi` & `boto3-stubs-lite-1.28.3.post2/boto3-stubs/resources/response.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3-stubs/s3/inject.pyi` & `boto3-stubs-lite-1.28.3.post2/boto3-stubs/s3/inject.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3-stubs/s3/transfer.pyi` & `boto3-stubs-lite-1.28.3.post2/boto3-stubs/s3/transfer.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3-stubs/session.pyi` & `boto3-stubs-lite-1.28.3.post2/boto3-stubs/session.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3-stubs/utils.pyi` & `boto3-stubs-lite-1.28.3.post2/boto3-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3_stubs_lite.egg-info/PKG-INFO` & `boto3-stubs-lite-1.28.3.post2/boto3_stubs_lite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: boto3-stubs-lite
-Version: 1.28.3.post1
-Summary: Type annotations for boto3 1.28.3 generated with mypy-boto3-builder 7.14.7
+Version: 1.28.3.post2
+Summary: Type annotations for boto3 1.28.3 generated with mypy-boto3-builder 7.15.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -400,15 +400,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.7](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [boto3-stubs-lite docs](https://youtype.github.io/boto3_stubs_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
```

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3_stubs_lite.egg-info/SOURCES.txt` & `boto3-stubs-lite-1.28.3.post2/boto3_stubs_lite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/boto3_stubs_lite.egg-info/requires.txt` & `boto3-stubs-lite-1.28.3.post2/boto3_stubs_lite.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `boto3-stubs-lite-1.28.3.post1/setup.py` & `boto3-stubs-lite-1.28.3.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="boto3-stubs-lite",
-    version="1.28.3.post1",
+    version="1.28.3.post2",
     packages=["boto3-stubs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3 1.28.3 generated with mypy-boto3-builder 7.14.7",
+    description="Type annotations for boto3 1.28.3 generated with mypy-boto3-builder 7.15.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

