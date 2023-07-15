# Comparing `tmp/types-aiobotocore-dynamodb-2.5.1.tar.gz` & `tmp/types-aiobotocore-dynamodb-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dynamodb-2.5.1.tar", last modified: Wed Jun 28 01:43:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-dynamodb-2.5.2.tar", last modified: Sat Jul  8 01:43:33 2023, max compression
```

## Comparing `types-aiobotocore-dynamodb-2.5.1.tar` & `types-aiobotocore-dynamodb-2.5.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:24.850128 types-aiobotocore-dynamodb-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 01:29:29.000000 types-aiobotocore-dynamodb-2.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28333 2023-06-28 01:43:24.850128 types-aiobotocore-dynamodb-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26764 2023-06-28 01:29:29.000000 types-aiobotocore-dynamodb-2.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 01:43:24.850128 types-aiobotocore-dynamodb-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-28 01:29:29.000000 types-aiobotocore-dynamodb-2.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:24.842128 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-28 01:29:29.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-28 01:29:29.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-28 01:29:29.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56380 2023-06-28 01:29:30.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    56311 2023-06-28 01:29:29.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-06-28 01:29:31.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-06-28 01:29:31.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-06-28 01:29:30.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-06-28 01:29:30.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 01:29:29.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29167 2023-06-28 01:29:30.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    29138 2023-06-28 01:29:30.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   152204 2023-06-28 01:29:34.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   152051 2023-06-28 01:29:32.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-28 01:29:29.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-28 01:29:30.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-28 01:29:30.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 01:43:24.850128 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28333 2023-06-28 01:43:24.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-28 01:43:24.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:24.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 01:43:24.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 01:43:24.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-28 01:43:24.000000 types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:33.074045 types-aiobotocore-dynamodb-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:29:08.000000 types-aiobotocore-dynamodb-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28333 2023-07-08 01:43:33.074045 types-aiobotocore-dynamodb-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26764 2023-07-08 01:29:08.000000 types-aiobotocore-dynamodb-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:33.074045 types-aiobotocore-dynamodb-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-08 01:29:08.000000 types-aiobotocore-dynamodb-2.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:33.070045 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-08 01:29:08.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-08 01:29:08.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-08 01:29:08.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56380 2023-07-08 01:29:09.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56311 2023-07-08 01:29:08.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-07-08 01:29:10.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-07-08 01:29:10.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-07-08 01:29:10.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-07-08 01:29:10.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:29:08.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29167 2023-07-08 01:29:10.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29138 2023-07-08 01:29:09.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   152204 2023-07-08 01:29:14.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152051 2023-07-08 01:29:12.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:29:08.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-08 01:29:10.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-08 01:29:10.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:33.074045 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28333 2023-07-08 01:43:32.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-08 01:43:32.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:32.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:43:32.000000 types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dynamodb-2.5.1/LICENSE` & `types-aiobotocore-dynamodb-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.1/PKG-INFO` & `types-aiobotocore-dynamodb-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodb
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.DynamoDB 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dynamodb?color=blue)](https://pypistats.org/packages/types-aiobotocore-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DynamoDB 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[aiobotocore.DynamoDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dynamodb-2.5.1/README.md` & `types-aiobotocore-dynamodb-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dynamodb?color=blue)](https://pypistats.org/packages/types-aiobotocore-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DynamoDB 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[aiobotocore.DynamoDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dynamodb-2.5.1/setup.py` & `types-aiobotocore-dynamodb-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dynamodb",
-    version="2.5.1",
+    version="2.5.2",
     packages=["types_aiobotocore_dynamodb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DynamoDB 2.5.1 service generated with mypy-boto3-builder"
+        "Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder"
         " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

### Comparing `types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/__init__.py` & `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/__init__.pyi` & `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/__main__.py` & `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DynamoDB 2.5.1\nVersion:         2.5.1\nBuilder version:"
+        "Type annotations for aiobotocore.DynamoDB 2.5.2\nVersion:         2.5.2\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.1")
+    print("2.5.2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/client.py` & `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/client.pyi` & `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/literals.py` & `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/literals.pyi` & `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/paginator.py` & `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/paginator.pyi` & `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/service_resource.py` & `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/service_resource.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/service_resource.pyi` & `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/type_defs.py` & `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/type_defs.pyi` & `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/waiter.py` & `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb/waiter.pyi` & `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb.egg-info/PKG-INFO` & `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodb
-Version: 2.5.1
-Summary: Type annotations for aiobotocore.DynamoDB 2.5.1 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2
+Summary: Type annotations for aiobotocore.DynamoDB 2.5.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dynamodb?color=blue)](https://pypistats.org/packages/types-aiobotocore-dynamodb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DynamoDB 2.5.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
+[aiobotocore.DynamoDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `types-aiobotocore-dynamodb-2.5.1/types_aiobotocore_dynamodb.egg-info/SOURCES.txt` & `types-aiobotocore-dynamodb-2.5.2/types_aiobotocore_dynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

