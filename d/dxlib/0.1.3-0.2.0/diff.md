# Comparing `tmp/dxlib-0.1.3.tar.gz` & `tmp/dxlib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxlib-0.1.3.tar", last modified: Sat Jul 15 07:40:36 2023, max compression
+gzip compressed data, was "dxlib-0.2.0.tar", last modified: Sat Jul 15 07:42:08 2023, max compression
```

## Comparing `dxlib-0.1.3.tar` & `dxlib-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:40:36.023488 dxlib-0.1.3/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1262 2023-07-15 07:40:36.020979 dxlib-0.1.3/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      526 2023-04-20 14:34:27.000000 dxlib-0.1.3/README.md
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:40:35.576889 dxlib-0.1.3/dxlib/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       19 2023-07-15 07:24:40.000000 dxlib-0.1.3/dxlib/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:40:35.865722 dxlib-0.1.3/dxlib/api/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       76 2023-07-15 05:54:39.000000 dxlib-0.1.3/dxlib/api/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1345 2023-07-15 07:08:40.000000 dxlib-0.1.3/dxlib/api/__main__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1343 2023-07-15 05:57:39.000000 dxlib-0.1.3/dxlib/api/alphavantage.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      569 2023-07-15 03:43:22.000000 dxlib-0.1.3/dxlib/api/logger.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      315 2023-07-15 04:34:42.000000 dxlib-0.1.3/dxlib/api/terminal.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1857 2023-07-15 04:12:02.000000 dxlib-0.1.3/dxlib/api/utils.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1448 2023-07-14 03:22:23.000000 dxlib-0.1.3/dxlib/app.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:40:35.910823 dxlib-0.1.3/dxlib/db/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-13 23:57:17.000000 dxlib-0.1.3/dxlib/db/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:40:35.996744 dxlib-0.1.3/dxlib/db/sql/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-06-30 10:14:59.000000 dxlib-0.1.3/dxlib/db/sql/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      153 2023-06-30 10:10:39.000000 dxlib-0.1.3/dxlib/db/sql/create.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      761 2023-06-30 10:14:21.000000 dxlib-0.1.3/dxlib/db/sql/queries.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     4361 2023-07-14 00:49:31.000000 dxlib-0.1.3/dxlib/db/utils.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      404 2023-04-20 14:41:16.000000 dxlib-0.1.3/dxlib/euler_method.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      274 2023-04-20 14:39:35.000000 dxlib-0.1.3/dxlib/finite_differences.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:40:35.715585 dxlib-0.1.3/dxlib.egg-info/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1262 2023-07-15 07:40:35.000000 dxlib-0.1.3/dxlib.egg-info/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      485 2023-07-15 07:40:35.000000 dxlib-0.1.3/dxlib.egg-info/SOURCES.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-07-15 07:40:35.000000 dxlib-0.1.3/dxlib.egg-info/dependency_links.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      119 2023-07-15 07:40:35.000000 dxlib-0.1.3/dxlib.egg-info/requires.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-07-15 07:40:35.000000 dxlib-0.1.3/dxlib.egg-info/top_level.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-07-15 07:40:36.023488 dxlib-0.1.3/setup.cfg
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1328 2023-07-15 07:28:39.000000 dxlib-0.1.3/setup.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:42:08.768211 dxlib-0.2.0/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1262 2023-07-15 07:42:08.765200 dxlib-0.2.0/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      526 2023-04-20 14:34:27.000000 dxlib-0.2.0/README.md
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:42:08.358830 dxlib-0.2.0/dxlib/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       19 2023-07-15 07:24:40.000000 dxlib-0.2.0/dxlib/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:42:08.636952 dxlib-0.2.0/dxlib/api/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       76 2023-07-15 05:54:39.000000 dxlib-0.2.0/dxlib/api/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1345 2023-07-15 07:08:40.000000 dxlib-0.2.0/dxlib/api/__main__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1343 2023-07-15 05:57:39.000000 dxlib-0.2.0/dxlib/api/alphavantage.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      569 2023-07-15 03:43:22.000000 dxlib-0.2.0/dxlib/api/logger.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      315 2023-07-15 04:34:42.000000 dxlib-0.2.0/dxlib/api/terminal.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1857 2023-07-15 04:12:02.000000 dxlib-0.2.0/dxlib/api/utils.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1448 2023-07-14 03:22:23.000000 dxlib-0.2.0/dxlib/app.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:42:08.676041 dxlib-0.2.0/dxlib/db/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-13 23:57:17.000000 dxlib-0.2.0/dxlib/db/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:42:08.746335 dxlib-0.2.0/dxlib/db/sql/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-06-30 10:14:59.000000 dxlib-0.2.0/dxlib/db/sql/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      153 2023-06-30 10:10:39.000000 dxlib-0.2.0/dxlib/db/sql/create.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      761 2023-06-30 10:14:21.000000 dxlib-0.2.0/dxlib/db/sql/queries.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     4361 2023-07-14 00:49:31.000000 dxlib-0.2.0/dxlib/db/utils.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      404 2023-04-20 14:41:16.000000 dxlib-0.2.0/dxlib/euler_method.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      274 2023-04-20 14:39:35.000000 dxlib-0.2.0/dxlib/finite_differences.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:42:08.484872 dxlib-0.2.0/dxlib.egg-info/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1262 2023-07-15 07:42:07.000000 dxlib-0.2.0/dxlib.egg-info/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      485 2023-07-15 07:42:08.000000 dxlib-0.2.0/dxlib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-07-15 07:42:07.000000 dxlib-0.2.0/dxlib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      119 2023-07-15 07:42:07.000000 dxlib-0.2.0/dxlib.egg-info/requires.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-07-15 07:42:07.000000 dxlib-0.2.0/dxlib.egg-info/top_level.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-07-15 07:42:08.768211 dxlib-0.2.0/setup.cfg
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1328 2023-07-15 07:28:39.000000 dxlib-0.2.0/setup.py
```

### Comparing `dxlib-0.1.3/PKG-INFO` & `dxlib-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxlib
-Version: 0.1.3
+Version: 0.2.0
 Summary: Quantitative Methods for Finance
 Home-page: https://github.com/delphos-quant/dxlib
 Author: Rafael Zimmer
 Author-email: rzimmerde@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dxlib-0.1.3/README.md` & `dxlib-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dxlib-0.1.3/dxlib/api/__main__.py` & `dxlib-0.2.0/dxlib/api/__main__.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.1.3/dxlib/api/alphavantage.py` & `dxlib-0.2.0/dxlib/api/alphavantage.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.1.3/dxlib/api/logger.py` & `dxlib-0.2.0/dxlib/api/logger.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.1.3/dxlib/api/utils.py` & `dxlib-0.2.0/dxlib/api/utils.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.1.3/dxlib/app.py` & `dxlib-0.2.0/dxlib/app.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.1.3/dxlib/db/sql/queries.py` & `dxlib-0.2.0/dxlib/db/sql/queries.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.1.3/dxlib/db/utils.py` & `dxlib-0.2.0/dxlib/db/utils.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.1.3/dxlib.egg-info/PKG-INFO` & `dxlib-0.2.0/dxlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxlib
-Version: 0.1.3
+Version: 0.2.0
 Summary: Quantitative Methods for Finance
 Home-page: https://github.com/delphos-quant/dxlib
 Author: Rafael Zimmer
 Author-email: rzimmerde@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dxlib-0.1.3/setup.py` & `dxlib-0.2.0/setup.py`

 * *Files identical despite different names*

