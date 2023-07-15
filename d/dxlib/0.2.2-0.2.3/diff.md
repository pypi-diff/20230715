# Comparing `tmp/dxlib-0.2.2.tar.gz` & `tmp/dxlib-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxlib-0.2.2.tar", last modified: Sat Jul 15 08:07:01 2023, max compression
+gzip compressed data, was "dxlib-0.2.3.tar", last modified: Sat Jul 15 09:58:55 2023, max compression
```

## Comparing `dxlib-0.2.2.tar` & `dxlib-0.2.3.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:01.489526 dxlib-0.2.2/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1716 2023-07-15 08:07:01.485527 dxlib-0.2.2/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      981 2023-07-15 07:58:15.000000 dxlib-0.2.2/README.md
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:00.748446 dxlib-0.2.2/dxlib/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       95 2023-07-15 07:58:04.000000 dxlib-0.2.2/dxlib/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:00.943402 dxlib-0.2.2/dxlib/api/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       73 2023-07-15 07:58:04.000000 dxlib-0.2.2/dxlib/api/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1304 2023-07-15 07:58:04.000000 dxlib-0.2.2/dxlib/api/alphavantage.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:44.000000 dxlib-0.2.2/dxlib/api/logger.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:34.000000 dxlib-0.2.2/dxlib/api/terminal.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:01.004352 dxlib-0.2.2/dxlib/core/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:09.000000 dxlib-0.2.2/dxlib/core/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      387 2023-07-15 07:58:04.000000 dxlib-0.2.2/dxlib/core/euler_method.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      262 2023-07-15 07:58:04.000000 dxlib-0.2.2/dxlib/core/finite_differences.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:01.045473 dxlib-0.2.2/dxlib/data/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       21 2023-07-15 07:58:04.000000 dxlib-0.2.2/dxlib/data/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1805 2023-07-15 07:58:04.000000 dxlib-0.2.2/dxlib/data/utils.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:01.085093 dxlib-0.2.2/dxlib/db/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-13 23:57:17.000000 dxlib-0.2.2/dxlib/db/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:01.207764 dxlib-0.2.2/dxlib/db/sql/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-06-30 10:14:59.000000 dxlib-0.2.2/dxlib/db/sql/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      148 2023-07-15 07:58:04.000000 dxlib-0.2.2/dxlib/db/sql/create.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      730 2023-07-15 07:58:04.000000 dxlib-0.2.2/dxlib/db/sql/queries.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     4241 2023-07-15 07:58:05.000000 dxlib-0.2.2/dxlib/db/utils.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:01.309940 dxlib-0.2.2/dxlib/models/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:31.000000 dxlib-0.2.2/dxlib/models/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       86 2023-07-15 07:58:05.000000 dxlib-0.2.2/dxlib/models/options.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-04-28 17:50:38.000000 dxlib-0.2.2/dxlib/models/pricing.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:01.342987 dxlib-0.2.2/dxlib/research/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:50:59.000000 dxlib-0.2.2/dxlib/research/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:01.412618 dxlib-0.2.2/dxlib/simulation/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:15.000000 dxlib-0.2.2/dxlib/simulation/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     7903 2023-07-15 07:58:05.000000 dxlib-0.2.2/dxlib/simulation/backtesting.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:01.451979 dxlib-0.2.2/dxlib/visualization/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:06:43.000000 dxlib-0.2.2/dxlib/visualization/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:07:00.865293 dxlib-0.2.2/dxlib.egg-info/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1716 2023-07-15 08:07:00.000000 dxlib-0.2.2/dxlib.egg-info/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      700 2023-07-15 08:07:00.000000 dxlib-0.2.2/dxlib.egg-info/SOURCES.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-07-15 08:07:00.000000 dxlib-0.2.2/dxlib.egg-info/dependency_links.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      106 2023-07-15 08:07:00.000000 dxlib-0.2.2/dxlib.egg-info/requires.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-07-15 08:07:00.000000 dxlib-0.2.2/dxlib.egg-info/top_level.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-07-15 08:07:01.491034 dxlib-0.2.2/setup.cfg
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1328 2023-07-15 07:44:19.000000 dxlib-0.2.2/setup.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:55.435587 dxlib-0.2.3/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1716 2023-07-15 09:58:55.432585 dxlib-0.2.3/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      981 2023-07-15 07:58:15.000000 dxlib-0.2.3/README.md
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:54.746892 dxlib-0.2.3/dxlib/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       95 2023-07-15 07:58:04.000000 dxlib-0.2.3/dxlib/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:54.944587 dxlib-0.2.3/dxlib/api/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       73 2023-07-15 07:58:04.000000 dxlib-0.2.3/dxlib/api/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1304 2023-07-15 07:58:04.000000 dxlib-0.2.3/dxlib/api/alphavantage.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:44.000000 dxlib-0.2.3/dxlib/api/logger.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:34.000000 dxlib-0.2.3/dxlib/api/terminal.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:55.018837 dxlib-0.2.3/dxlib/core/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:09.000000 dxlib-0.2.3/dxlib/core/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      387 2023-07-15 07:58:04.000000 dxlib-0.2.3/dxlib/core/euler_method.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      262 2023-07-15 07:58:04.000000 dxlib-0.2.3/dxlib/core/finite_differences.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:55.068677 dxlib-0.2.3/dxlib/data/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       21 2023-07-15 07:58:04.000000 dxlib-0.2.3/dxlib/data/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     2150 2023-07-15 09:26:56.000000 dxlib-0.2.3/dxlib/data/utils.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:55.118496 dxlib-0.2.3/dxlib/db/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-13 23:57:17.000000 dxlib-0.2.3/dxlib/db/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:55.211680 dxlib-0.2.3/dxlib/db/sql/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-06-30 10:14:59.000000 dxlib-0.2.3/dxlib/db/sql/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      148 2023-07-15 07:58:04.000000 dxlib-0.2.3/dxlib/db/sql/create.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      730 2023-07-15 07:58:04.000000 dxlib-0.2.3/dxlib/db/sql/queries.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     4241 2023-07-15 07:58:05.000000 dxlib-0.2.3/dxlib/db/utils.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:55.312093 dxlib-0.2.3/dxlib/models/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:31.000000 dxlib-0.2.3/dxlib/models/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     2338 2023-07-15 08:38:49.000000 dxlib-0.2.3/dxlib/models/options.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-04-28 17:50:38.000000 dxlib-0.2.3/dxlib/models/pricing.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:26:00.000000 dxlib-0.2.3/dxlib/models/systematic_trading.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:55.336120 dxlib-0.2.3/dxlib/research/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:50:59.000000 dxlib-0.2.3/dxlib/research/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:55.384850 dxlib-0.2.3/dxlib/simulation/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:15.000000 dxlib-0.2.3/dxlib/simulation/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     7903 2023-07-15 07:58:05.000000 dxlib-0.2.3/dxlib/simulation/backtesting.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:55.410540 dxlib-0.2.3/dxlib/visualization/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:06:43.000000 dxlib-0.2.3/dxlib/visualization/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 09:58:54.842620 dxlib-0.2.3/dxlib.egg-info/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1716 2023-07-15 09:58:54.000000 dxlib-0.2.3/dxlib.egg-info/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      735 2023-07-15 09:58:54.000000 dxlib-0.2.3/dxlib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-07-15 09:58:54.000000 dxlib-0.2.3/dxlib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       96 2023-07-15 09:58:54.000000 dxlib-0.2.3/dxlib.egg-info/requires.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-07-15 09:58:54.000000 dxlib-0.2.3/dxlib.egg-info/top_level.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-07-15 09:58:55.436589 dxlib-0.2.3/setup.cfg
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1328 2023-07-15 07:44:19.000000 dxlib-0.2.3/setup.py
```

### Comparing `dxlib-0.2.2/PKG-INFO` & `dxlib-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxlib
-Version: 0.2.2
+Version: 0.2.3
 Summary: Quantitative Methods for Finance
 Home-page: https://github.com/delphos-quant/dxlib
 Author: Rafael Zimmer
 Author-email: rzimmerde@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dxlib-0.2.2/README.md` & `dxlib-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.2/dxlib/api/alphavantage.py` & `dxlib-0.2.3/dxlib/api/alphavantage.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.2/dxlib/data/utils.py` & `dxlib-0.2.3/dxlib/data/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 import csv
+import os
 import pandas
 
 
+def read_data(symbol):
+    if os.path.exists(f"{symbol}.csv"):
+        try:
+            security = pandas.read_csv(f"{symbol}.csv", index_col=0, parse_dates=True)
+            security.index = pandas.to_datetime(security.index)
+            return security
+        except pandas.errors.EmptyDataError:
+            pass
+    return None
+
+
 def append_to_csv(data, csv_file='stock_data.csv'):
     if isinstance(data, list):
         try:
             with open(csv_file, 'r') as file:
                 is_empty = len(file.readline().strip()) == 0
         except FileNotFoundError:
             is_empty = True
```

### Comparing `dxlib-0.2.2/dxlib/db/sql/queries.py` & `dxlib-0.2.3/dxlib/db/sql/queries.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.2/dxlib/db/utils.py` & `dxlib-0.2.3/dxlib/db/utils.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.2/dxlib/simulation/backtesting.py` & `dxlib-0.2.3/dxlib/simulation/backtesting.py`

 * *Files identical despite different names*

### Comparing `dxlib-0.2.2/dxlib.egg-info/PKG-INFO` & `dxlib-0.2.3/dxlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxlib
-Version: 0.2.2
+Version: 0.2.3
 Summary: Quantitative Methods for Finance
 Home-page: https://github.com/delphos-quant/dxlib
 Author: Rafael Zimmer
 Author-email: rzimmerde@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dxlib-0.2.2/dxlib.egg-info/SOURCES.txt` & `dxlib-0.2.3/dxlib.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -19,11 +19,12 @@
 dxlib/db/utils.py
 dxlib/db/sql/__init__.py
 dxlib/db/sql/create.py
 dxlib/db/sql/queries.py
 dxlib/models/__init__.py
 dxlib/models/options.py
 dxlib/models/pricing.py
+dxlib/models/systematic_trading.py
 dxlib/research/__init__.py
 dxlib/simulation/__init__.py
 dxlib/simulation/backtesting.py
 dxlib/visualization/__init__.py
```

### Comparing `dxlib-0.2.2/setup.py` & `dxlib-0.2.3/setup.py`

 * *Files identical despite different names*

