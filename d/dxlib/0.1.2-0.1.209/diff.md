# Comparing `tmp/dxlib-0.1.2.tar.gz` & `tmp/dxlib-0.1.209.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxlib-0.1.2.tar", last modified: Sat Jul 15 07:35:53 2023, max compression
+gzip compressed data, was "dxlib-0.1.209.tar", last modified: Sat Jul 15 06:55:37 2023, max compression
```

## Comparing `dxlib-0.1.2.tar` & `dxlib-0.1.209.tar`

### file list

```diff
@@ -1,30 +1,16 @@
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:35:53.831825 dxlib-0.1.2/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1262 2023-07-15 07:35:53.828817 dxlib-0.1.2/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      526 2023-04-20 14:34:27.000000 dxlib-0.1.2/README.md
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:35:53.414990 dxlib-0.1.2/dxlib/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       19 2023-07-15 07:24:40.000000 dxlib-0.1.2/dxlib/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:35:53.698380 dxlib-0.1.2/dxlib/api/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       76 2023-07-15 05:54:39.000000 dxlib-0.1.2/dxlib/api/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1345 2023-07-15 07:08:40.000000 dxlib-0.1.2/dxlib/api/__main__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1343 2023-07-15 05:57:39.000000 dxlib-0.1.2/dxlib/api/alphavantage.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      569 2023-07-15 03:43:22.000000 dxlib-0.1.2/dxlib/api/logger.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      315 2023-07-15 04:34:42.000000 dxlib-0.1.2/dxlib/api/terminal.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1857 2023-07-15 04:12:02.000000 dxlib-0.1.2/dxlib/api/utils.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1448 2023-07-14 03:22:23.000000 dxlib-0.1.2/dxlib/app.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:35:53.738356 dxlib-0.1.2/dxlib/db/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-13 23:57:17.000000 dxlib-0.1.2/dxlib/db/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:35:53.808680 dxlib-0.1.2/dxlib/db/sql/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-06-30 10:14:59.000000 dxlib-0.1.2/dxlib/db/sql/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      153 2023-06-30 10:10:39.000000 dxlib-0.1.2/dxlib/db/sql/create.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      761 2023-06-30 10:14:21.000000 dxlib-0.1.2/dxlib/db/sql/queries.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     4361 2023-07-14 00:49:31.000000 dxlib-0.1.2/dxlib/db/utils.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      404 2023-04-20 14:41:16.000000 dxlib-0.1.2/dxlib/euler_method.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      274 2023-04-20 14:39:35.000000 dxlib-0.1.2/dxlib/finite_differences.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:35:53.545379 dxlib-0.1.2/dxlib.egg-info/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1262 2023-07-15 07:35:52.000000 dxlib-0.1.2/dxlib.egg-info/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      485 2023-07-15 07:35:53.000000 dxlib-0.1.2/dxlib.egg-info/SOURCES.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-07-15 07:35:52.000000 dxlib-0.1.2/dxlib.egg-info/dependency_links.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      119 2023-07-15 07:35:52.000000 dxlib-0.1.2/dxlib.egg-info/requires.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-07-15 07:35:52.000000 dxlib-0.1.2/dxlib.egg-info/top_level.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-07-15 07:35:53.831825 dxlib-0.1.2/setup.cfg
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1328 2023-07-15 07:28:39.000000 dxlib-0.1.2/setup.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 06:55:37.373043 dxlib-0.1.209/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1264 2023-07-15 06:55:37.369042 dxlib-0.1.209/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      526 2023-04-20 14:34:27.000000 dxlib-0.1.209/README.md
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 06:55:37.218274 dxlib-0.1.209/dxlib.egg-info/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1264 2023-07-15 06:55:36.000000 dxlib-0.1.209/dxlib.egg-info/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      235 2023-07-15 06:55:37.000000 dxlib-0.1.209/dxlib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-07-15 06:55:36.000000 dxlib-0.1.209/dxlib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      119 2023-07-15 06:55:36.000000 dxlib-0.1.209/dxlib.egg-info/requires.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        4 2023-07-15 06:55:36.000000 dxlib-0.1.209/dxlib.egg-info/top_level.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-07-15 06:55:37.374043 dxlib-0.1.209/setup.cfg
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1305 2023-07-15 06:14:29.000000 dxlib-0.1.209/setup.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 06:55:37.336035 dxlib-0.1.209/src/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       12 2023-07-15 06:53:11.000000 dxlib-0.1.209/src/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1448 2023-07-14 03:22:23.000000 dxlib-0.1.209/src/app.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      404 2023-04-20 14:41:16.000000 dxlib-0.1.209/src/euler_method.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      274 2023-04-20 14:39:35.000000 dxlib-0.1.209/src/finite_differences.py
```

### Comparing `dxlib-0.1.2/PKG-INFO` & `dxlib-0.1.209/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxlib
-Version: 0.1.2
+Version: 0.1.209
 Summary: Quantitative Methods for Finance
 Home-page: https://github.com/delphos-quant/dxlib
 Author: Rafael Zimmer
 Author-email: rzimmerde@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dxlib-0.1.2/README.md` & `dxlib-0.1.209/README.md`

 * *Files identical despite different names*

### Comparing `dxlib-0.1.2/dxlib/app.py` & `dxlib-0.1.209/src/app.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.1.2/dxlib.egg-info/PKG-INFO` & `dxlib-0.1.209/dxlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxlib
-Version: 0.1.2
+Version: 0.1.209
 Summary: Quantitative Methods for Finance
 Home-page: https://github.com/delphos-quant/dxlib
 Author: Rafael Zimmer
 Author-email: rzimmerde@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dxlib-0.1.2/setup.py` & `dxlib-0.1.209/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from os import path
+from setuptools import setup
 from codecs import open
-from setuptools import setup, find_packages
 
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 with open('requirements.txt') as f:
@@ -31,11 +31,11 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent"
     ],
-    packages=find_packages(),
+    packages=['src'],
     include_package_data=True,
     install_requires=requirements,
 )
```

