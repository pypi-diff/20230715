# Comparing `tmp/abi_parser-1.0.1.tar.gz` & `tmp/abi_parser-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abi_parser-1.0.1.tar", last modified: Sat Jul 15 00:16:37 2023, max compression
+gzip compressed data, was "abi_parser-1.0.2.tar", last modified: Sat Jul 15 00:16:57 2023, max compression
```

## Comparing `abi_parser-1.0.1.tar` & `abi_parser-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-15 00:16:37.540432 abi_parser-1.0.1/
--rw-r--r--   0 abhinavmir   (501) staff       (20)      735 2023-07-15 00:16:37.540282 abi_parser-1.0.1/PKG-INFO
--rw-r--r--   0 abhinavmir   (501) staff       (20)      524 2023-07-15 00:14:40.000000 abi_parser-1.0.1/README.md
-drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-15 00:16:37.539177 abi_parser-1.0.1/abi_parser/
--rw-r--r--   0 abhinavmir   (501) staff       (20)     4836 2023-07-15 00:08:15.000000 abi_parser-1.0.1/abi_parser/__init__.py
-drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-15 00:16:37.539848 abi_parser-1.0.1/abi_parser.egg-info/
--rw-r--r--   0 abhinavmir   (501) staff       (20)      735 2023-07-15 00:16:37.000000 abi_parser-1.0.1/abi_parser.egg-info/PKG-INFO
--rw-r--r--   0 abhinavmir   (501) staff       (20)      202 2023-07-15 00:16:37.000000 abi_parser-1.0.1/abi_parser.egg-info/SOURCES.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)        1 2023-07-15 00:16:37.000000 abi_parser-1.0.1/abi_parser.egg-info/dependency_links.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)       11 2023-07-15 00:16:37.000000 abi_parser-1.0.1/abi_parser.egg-info/top_level.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)       38 2023-07-15 00:16:37.540478 abi_parser-1.0.1/setup.cfg
--rw-r--r--   0 abhinavmir   (501) staff       (20)      481 2023-07-15 00:16:30.000000 abi_parser-1.0.1/setup.py
-drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-15 00:16:37.539976 abi_parser-1.0.1/tests/
--rw-r--r--   0 abhinavmir   (501) staff       (20)      360 2023-07-15 00:09:01.000000 abi_parser-1.0.1/tests/test_abi_parser.py
+drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-15 00:16:57.010833 abi_parser-1.0.2/
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      735 2023-07-15 00:16:57.010702 abi_parser-1.0.2/PKG-INFO
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      524 2023-07-15 00:14:40.000000 abi_parser-1.0.2/README.md
+drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-15 00:16:57.009526 abi_parser-1.0.2/abi_parser/
+-rw-r--r--   0 abhinavmir   (501) staff       (20)     4836 2023-07-15 00:08:15.000000 abi_parser-1.0.2/abi_parser/__init__.py
+drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-15 00:16:57.010305 abi_parser-1.0.2/abi_parser.egg-info/
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      735 2023-07-15 00:16:56.000000 abi_parser-1.0.2/abi_parser.egg-info/PKG-INFO
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      202 2023-07-15 00:16:56.000000 abi_parser-1.0.2/abi_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)        1 2023-07-15 00:16:56.000000 abi_parser-1.0.2/abi_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)       11 2023-07-15 00:16:56.000000 abi_parser-1.0.2/abi_parser.egg-info/top_level.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)       38 2023-07-15 00:16:57.010880 abi_parser-1.0.2/setup.cfg
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      481 2023-07-15 00:16:55.000000 abi_parser-1.0.2/setup.py
+drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-15 00:16:57.010427 abi_parser-1.0.2/tests/
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      360 2023-07-15 00:09:01.000000 abi_parser-1.0.2/tests/test_abi_parser.py
```

### Comparing `abi_parser-1.0.1/PKG-INFO` & `abi_parser-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abi_parser
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package to parse Ethereum contract ABI files
 Author: August Radjoe
 Author-email: atg271@gmail.com
 Description-Content-Type: text/markdown
 
 ### abi_parser
```

### Comparing `abi_parser-1.0.1/README.md` & `abi_parser-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `abi_parser-1.0.1/abi_parser/__init__.py` & `abi_parser-1.0.2/abi_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `abi_parser-1.0.1/abi_parser.egg-info/PKG-INFO` & `abi_parser-1.0.2/abi_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abi-parser
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package to parse Ethereum contract ABI files
 Author: August Radjoe
 Author-email: atg271@gmail.com
 Description-Content-Type: text/markdown
 
 ### abi_parser
```

