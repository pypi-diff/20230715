# Comparing `tmp/dxlib-0.2.1.tar.gz` & `tmp/dxlib-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxlib-0.2.1.tar", last modified: Sat Jul 15 08:03:30 2023, max compression
+gzip compressed data, was "dxlib-0.2.2.tar", last modified: Sat Jul 15 08:07:01 2023, max compression
```

## Comparing `dxlib-0.2.1.tar` & `dxlib-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:30.506143 dxlib-0.2.1/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1716 2023-07-15 08:03:30.503141 dxlib-0.2.1/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      981 2023-07-15 07:58:15.000000 dxlib-0.2.1/README.md
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:29.868367 dxlib-0.2.1/dxlib/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       95 2023-07-15 07:58:04.000000 dxlib-0.2.1/dxlib/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:30.079595 dxlib-0.2.1/dxlib/api/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       73 2023-07-15 07:58:04.000000 dxlib-0.2.1/dxlib/api/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1304 2023-07-15 07:58:04.000000 dxlib-0.2.1/dxlib/api/alphavantage.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:44.000000 dxlib-0.2.1/dxlib/api/logger.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:34.000000 dxlib-0.2.1/dxlib/api/terminal.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:30.152861 dxlib-0.2.1/dxlib/core/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:09.000000 dxlib-0.2.1/dxlib/core/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      387 2023-07-15 07:58:04.000000 dxlib-0.2.1/dxlib/core/euler_method.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      262 2023-07-15 07:58:04.000000 dxlib-0.2.1/dxlib/core/finite_differences.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:30.201993 dxlib-0.2.1/dxlib/data/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       21 2023-07-15 07:58:04.000000 dxlib-0.2.1/dxlib/data/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1805 2023-07-15 07:58:04.000000 dxlib-0.2.1/dxlib/data/utils.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:30.250433 dxlib-0.2.1/dxlib/db/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-13 23:57:17.000000 dxlib-0.2.1/dxlib/db/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:30.339354 dxlib-0.2.1/dxlib/db/sql/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-06-30 10:14:59.000000 dxlib-0.2.1/dxlib/db/sql/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      148 2023-07-15 07:58:04.000000 dxlib-0.2.1/dxlib/db/sql/create.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      730 2023-07-15 07:58:04.000000 dxlib-0.2.1/dxlib/db/sql/queries.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     4241 2023-07-15 07:58:05.000000 dxlib-0.2.1/dxlib/db/utils.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:30.413000 dxlib-0.2.1/dxlib/models/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:31.000000 dxlib-0.2.1/dxlib/models/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       86 2023-07-15 07:58:05.000000 dxlib-0.2.1/dxlib/models/options.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-04-28 17:50:38.000000 dxlib-0.2.1/dxlib/models/pricing.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:30.435020 dxlib-0.2.1/dxlib/research/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:50:59.000000 dxlib-0.2.1/dxlib/research/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:30.481295 dxlib-0.2.1/dxlib/simulation/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:15.000000 dxlib-0.2.1/dxlib/simulation/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     7903 2023-07-15 07:58:05.000000 dxlib-0.2.1/dxlib/simulation/backtesting.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:29.979701 dxlib-0.2.1/dxlib.egg-info/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1716 2023-07-15 08:03:29.000000 dxlib-0.2.1/dxlib.egg-info/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      668 2023-07-15 08:03:29.000000 dxlib-0.2.1/dxlib.egg-info/SOURCES.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-07-15 08:03:29.000000 dxlib-0.2.1/dxlib.egg-info/dependency_links.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      106 2023-07-15 08:03:29.000000 dxlib-0.2.1/dxlib.egg-info/requires.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-07-15 08:03:29.000000 dxlib-0.2.1/dxlib.egg-info/top_level.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-07-15 08:03:30.507144 dxlib-0.2.1/setup.cfg
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1328 2023-07-15 07:44:19.000000 dxlib-0.2.1/setup.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:01.489526 dxlib-0.2.2/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1716 2023-07-15 08:07:01.485527 dxlib-0.2.2/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      981 2023-07-15 07:58:15.000000 dxlib-0.2.2/README.md
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:00.748446 dxlib-0.2.2/dxlib/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       95 2023-07-15 07:58:04.000000 dxlib-0.2.2/dxlib/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:00.943402 dxlib-0.2.2/dxlib/api/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       73 2023-07-15 07:58:04.000000 dxlib-0.2.2/dxlib/api/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1304 2023-07-15 07:58:04.000000 dxlib-0.2.2/dxlib/api/alphavantage.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:44.000000 dxlib-0.2.2/dxlib/api/logger.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:34.000000 dxlib-0.2.2/dxlib/api/terminal.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:01.004352 dxlib-0.2.2/dxlib/core/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:09.000000 dxlib-0.2.2/dxlib/core/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      387 2023-07-15 07:58:04.000000 dxlib-0.2.2/dxlib/core/euler_method.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      262 2023-07-15 07:58:04.000000 dxlib-0.2.2/dxlib/core/finite_differences.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:01.045473 dxlib-0.2.2/dxlib/data/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       21 2023-07-15 07:58:04.000000 dxlib-0.2.2/dxlib/data/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1805 2023-07-15 07:58:04.000000 dxlib-0.2.2/dxlib/data/utils.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:01.085093 dxlib-0.2.2/dxlib/db/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-13 23:57:17.000000 dxlib-0.2.2/dxlib/db/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:01.207764 dxlib-0.2.2/dxlib/db/sql/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-06-30 10:14:59.000000 dxlib-0.2.2/dxlib/db/sql/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      148 2023-07-15 07:58:04.000000 dxlib-0.2.2/dxlib/db/sql/create.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      730 2023-07-15 07:58:04.000000 dxlib-0.2.2/dxlib/db/sql/queries.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     4241 2023-07-15 07:58:05.000000 dxlib-0.2.2/dxlib/db/utils.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:01.309940 dxlib-0.2.2/dxlib/models/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:31.000000 dxlib-0.2.2/dxlib/models/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       86 2023-07-15 07:58:05.000000 dxlib-0.2.2/dxlib/models/options.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-04-28 17:50:38.000000 dxlib-0.2.2/dxlib/models/pricing.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:01.342987 dxlib-0.2.2/dxlib/research/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:50:59.000000 dxlib-0.2.2/dxlib/research/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:01.412618 dxlib-0.2.2/dxlib/simulation/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:15.000000 dxlib-0.2.2/dxlib/simulation/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     7903 2023-07-15 07:58:05.000000 dxlib-0.2.2/dxlib/simulation/backtesting.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:01.451979 dxlib-0.2.2/dxlib/visualization/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:06:43.000000 dxlib-0.2.2/dxlib/visualization/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:00.865293 dxlib-0.2.2/dxlib.egg-info/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1716 2023-07-15 08:07:00.000000 dxlib-0.2.2/dxlib.egg-info/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      700 2023-07-15 08:07:00.000000 dxlib-0.2.2/dxlib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-07-15 08:07:00.000000 dxlib-0.2.2/dxlib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      106 2023-07-15 08:07:00.000000 dxlib-0.2.2/dxlib.egg-info/requires.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-07-15 08:07:00.000000 dxlib-0.2.2/dxlib.egg-info/top_level.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-07-15 08:07:01.491034 dxlib-0.2.2/setup.cfg
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1328 2023-07-15 07:44:19.000000 dxlib-0.2.2/setup.py
```

### Comparing `dxlib-0.2.1/PKG-INFO` & `dxlib-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxlib
-Version: 0.2.1
+Version: 0.2.2
 Summary: Quantitative Methods for Finance
 Home-page: https://github.com/delphos-quant/dxlib
 Author: Rafael Zimmer
 Author-email: rzimmerde@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dxlib-0.2.1/README.md` & `dxlib-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.1/dxlib/api/alphavantage.py` & `dxlib-0.2.2/dxlib/api/alphavantage.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.1/dxlib/data/utils.py` & `dxlib-0.2.2/dxlib/data/utils.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.1/dxlib/db/sql/queries.py` & `dxlib-0.2.2/dxlib/db/sql/queries.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.1/dxlib/db/utils.py` & `dxlib-0.2.2/dxlib/db/utils.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.1/dxlib/simulation/backtesting.py` & `dxlib-0.2.2/dxlib/simulation/backtesting.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.1/dxlib.egg-info/PKG-INFO` & `dxlib-0.2.2/dxlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxlib
-Version: 0.2.1
+Version: 0.2.2
 Summary: Quantitative Methods for Finance
 Home-page: https://github.com/delphos-quant/dxlib
 Author: Rafael Zimmer
 Author-email: rzimmerde@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dxlib-0.2.1/dxlib.egg-info/SOURCES.txt` & `dxlib-0.2.2/dxlib.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -21,8 +21,9 @@
 dxlib/db/sql/create.py
 dxlib/db/sql/queries.py
 dxlib/models/__init__.py
 dxlib/models/options.py
 dxlib/models/pricing.py
 dxlib/research/__init__.py
 dxlib/simulation/__init__.py
-dxlib/simulation/backtesting.py
+dxlib/simulation/backtesting.py
+dxlib/visualization/__init__.py
```

### Comparing `dxlib-0.2.1/setup.py` & `dxlib-0.2.2/setup.py`

 * *Files identical despite different names*

