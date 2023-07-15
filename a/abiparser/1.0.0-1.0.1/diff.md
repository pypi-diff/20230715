# Comparing `tmp/abiparser-1.0.0.tar.gz` & `tmp/abiparser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abiparser-1.0.0.tar", last modified: Sat Jul 15 00:21:57 2023, max compression
+gzip compressed data, was "abiparser-1.0.1.tar", last modified: Sat Jul 15 00:25:15 2023, max compression
```

## Comparing `abiparser-1.0.0.tar` & `abiparser-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-15 00:21:57.975711 abiparser-1.0.0/
--rw-r--r--   0 abhinavmir   (501) staff       (20)      734 2023-07-15 00:21:57.975574 abiparser-1.0.0/PKG-INFO
--rw-r--r--   0 abhinavmir   (501) staff       (20)      524 2023-07-15 00:14:40.000000 abiparser-1.0.0/README.md
-drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-15 00:21:57.974637 abiparser-1.0.0/abiparser/
--rw-r--r--   0 abhinavmir   (501) staff       (20)     4836 2023-07-15 00:08:15.000000 abiparser-1.0.0/abiparser/__init__.py
-drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-15 00:21:57.975118 abiparser-1.0.0/abiparser.egg-info/
--rw-r--r--   0 abhinavmir   (501) staff       (20)      734 2023-07-15 00:21:57.000000 abiparser-1.0.0/abiparser.egg-info/PKG-INFO
--rw-r--r--   0 abhinavmir   (501) staff       (20)      197 2023-07-15 00:21:57.000000 abiparser-1.0.0/abiparser.egg-info/SOURCES.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)        1 2023-07-15 00:21:57.000000 abiparser-1.0.0/abiparser.egg-info/dependency_links.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)       10 2023-07-15 00:21:57.000000 abiparser-1.0.0/abiparser.egg-info/top_level.txt
--rw-r--r--   0 abhinavmir   (501) staff       (20)       38 2023-07-15 00:21:57.975753 abiparser-1.0.0/setup.cfg
--rw-r--r--   0 abhinavmir   (501) staff       (20)      479 2023-07-15 00:21:45.000000 abiparser-1.0.0/setup.py
-drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-15 00:21:57.975283 abiparser-1.0.0/tests/
--rw-r--r--   0 abhinavmir   (501) staff       (20)      360 2023-07-15 00:09:01.000000 abiparser-1.0.0/tests/test_abi_parser.py
+drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-15 00:25:15.182667 abiparser-1.0.1/
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      732 2023-07-15 00:25:15.182517 abiparser-1.0.1/PKG-INFO
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      522 2023-07-15 00:24:33.000000 abiparser-1.0.1/README.md
+drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-15 00:25:15.181601 abiparser-1.0.1/abiparser/
+-rw-r--r--   0 abhinavmir   (501) staff       (20)     4836 2023-07-15 00:08:15.000000 abiparser-1.0.1/abiparser/__init__.py
+drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-15 00:25:15.182208 abiparser-1.0.1/abiparser.egg-info/
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      732 2023-07-15 00:25:15.000000 abiparser-1.0.1/abiparser.egg-info/PKG-INFO
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      197 2023-07-15 00:25:15.000000 abiparser-1.0.1/abiparser.egg-info/SOURCES.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)        1 2023-07-15 00:25:15.000000 abiparser-1.0.1/abiparser.egg-info/dependency_links.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)       10 2023-07-15 00:25:15.000000 abiparser-1.0.1/abiparser.egg-info/top_level.txt
+-rw-r--r--   0 abhinavmir   (501) staff       (20)       38 2023-07-15 00:25:15.182714 abiparser-1.0.1/setup.cfg
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      479 2023-07-15 00:25:12.000000 abiparser-1.0.1/setup.py
+drwxr-xr-x   0 abhinavmir   (501) staff       (20)        0 2023-07-15 00:25:15.182331 abiparser-1.0.1/tests/
+-rw-r--r--   0 abhinavmir   (501) staff       (20)      359 2023-07-15 00:23:29.000000 abiparser-1.0.1/tests/test_abi_parser.py
```

### Comparing `abiparser-1.0.0/PKG-INFO` & `abiparser-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: abiparser
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package to parse Ethereum contract ABI files
 Author: August Radjoe
 Author-email: atg271@gmail.com
 Description-Content-Type: text/markdown
 
 ### abi_parser
 
 A simple way to parse your ABIs in Python.
 
 ### Installation
 
 ```bash
-pip install abi_parser
+pip install abiparser
 ```
 
 ```python
-from abi_parser import ContractABI
+from abiparser import ContractABI
 abi = ContractABI('<PATH TO ABI JSON'>)
 
 # name
 name = abi.name
 
 # functions
 functions = abi.functions
```

### Comparing `abiparser-1.0.0/README.md` & `abiparser-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ### abi_parser
 
 A simple way to parse your ABIs in Python.
 
 ### Installation
 
 ```bash
-pip install abi_parser
+pip install abiparser
 ```
 
 ```python
-from abi_parser import ContractABI
+from abiparser import ContractABI
 abi = ContractABI('<PATH TO ABI JSON'>)
 
 # name
 name = abi.name
 
 # functions
 functions = abi.functions
```

### Comparing `abiparser-1.0.0/abiparser/__init__.py` & `abiparser-1.0.1/abiparser/__init__.py`

 * *Files identical despite different names*

### Comparing `abiparser-1.0.0/abiparser.egg-info/PKG-INFO` & `abiparser-1.0.1/abiparser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: abiparser
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python package to parse Ethereum contract ABI files
 Author: August Radjoe
 Author-email: atg271@gmail.com
 Description-Content-Type: text/markdown
 
 ### abi_parser
 
 A simple way to parse your ABIs in Python.
 
 ### Installation
 
 ```bash
-pip install abi_parser
+pip install abiparser
 ```
 
 ```python
-from abi_parser import ContractABI
+from abiparser import ContractABI
 abi = ContractABI('<PATH TO ABI JSON'>)
 
 # name
 name = abi.name
 
 # functions
 functions = abi.functions
```

