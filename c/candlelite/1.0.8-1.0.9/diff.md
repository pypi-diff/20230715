# Comparing `tmp/candlelite-1.0.8.tar.gz` & `tmp/candlelite-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/candlelite-1.0.8.tar", last modified: Sat Jul 15 03:39:36 2023, max compression
+gzip compressed data, was "dist/candlelite-1.0.9.tar", last modified: Sat Jul 15 03:55:56 2023, max compression
```

## Comparing `candlelite-1.0.8.tar` & `candlelite-1.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-07-15 03:39:36.950417 candlelite-1.0.8/
--rw-r--r--   0 kzlknight   (501) staff       (20)      628 2023-07-15 03:39:36.949888 candlelite-1.0.8/PKG-INFO
--rw-r--r--   0 kzlknight   (501) staff       (20)       25 2023-02-21 10:35:06.000000 candlelite-1.0.8/README.md
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-07-15 03:39:36.939086 candlelite-1.0.8/candlelite/
--rw-r--r--   0 kzlknight   (501) staff       (20)      242 2023-07-15 03:37:10.000000 candlelite-1.0.8/candlelite/__init__.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-07-15 03:39:36.942957 candlelite-1.0.8/candlelite/calculate/
--rw-r--r--   0 kzlknight   (501) staff       (20)      204 2023-01-25 20:14:09.000000 candlelite-1.0.8/candlelite/calculate/__init__.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     1167 2023-07-15 03:30:24.000000 candlelite-1.0.8/candlelite/calculate/bar.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     1139 2023-07-15 03:37:10.000000 candlelite-1.0.8/candlelite/calculate/interval.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     5141 2023-01-25 19:36:00.000000 candlelite-1.0.8/candlelite/calculate/technical.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     6651 2023-01-25 20:11:14.000000 candlelite-1.0.8/candlelite/calculate/transform.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     5104 2023-01-26 21:55:48.000000 candlelite-1.0.8/candlelite/calculate/valid.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-07-15 03:39:36.943361 candlelite-1.0.8/candlelite/cmdline/
--rw-r--r--   0 kzlknight   (501) staff       (20)      975 2023-01-26 07:20:12.000000 candlelite-1.0.8/candlelite/cmdline/__init__.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-07-15 03:39:36.945028 candlelite-1.0.8/candlelite/crypto/
--rw-r--r--   0 kzlknight   (501) staff       (20)      101 2023-02-21 10:35:06.000000 candlelite-1.0.8/candlelite/crypto/__init__.py
--rw-r--r--   0 kzlknight   (501) staff       (20)    11177 2023-06-22 07:44:31.000000 candlelite-1.0.8/candlelite/crypto/_base.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      885 2023-01-29 21:17:12.000000 candlelite-1.0.8/candlelite/crypto/binace_lite.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      818 2023-01-25 21:49:55.000000 candlelite-1.0.8/candlelite/crypto/okx_lite.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-07-15 03:39:36.947348 candlelite-1.0.8/candlelite/exception/
--rw-r--r--   0 kzlknight   (501) staff       (20)      131 2023-01-25 19:19:56.000000 candlelite-1.0.8/candlelite/exception/__init__.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      235 2023-01-25 19:24:42.000000 candlelite-1.0.8/candlelite/exception/_base.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     1294 2023-05-02 04:09:34.000000 candlelite-1.0.8/candlelite/exception/candle.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      202 2023-01-25 19:25:08.000000 candlelite-1.0.8/candlelite/exception/execute.py
--rw-r--r--   0 kzlknight   (501) staff       (20)      813 2023-01-25 20:07:05.000000 candlelite-1.0.8/candlelite/exception/param.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-07-15 03:39:36.948891 candlelite-1.0.8/candlelite/io/
--rw-r--r--   0 kzlknight   (501) staff       (20)       93 2023-02-21 10:35:06.000000 candlelite-1.0.8/candlelite/io/__init__.py
--rw-r--r--   0 kzlknight   (501) staff       (20)    12243 2023-06-22 07:36:19.000000 candlelite-1.0.8/candlelite/io/load.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     8693 2023-05-01 14:46:48.000000 candlelite-1.0.8/candlelite/io/path.py
--rw-r--r--   0 kzlknight   (501) staff       (20)     7368 2023-03-06 06:06:56.000000 candlelite-1.0.8/candlelite/io/save.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-07-15 03:39:36.949362 candlelite-1.0.8/candlelite/settings/
--rw-r--r--   0 kzlknight   (501) staff       (20)     4485 2023-01-29 21:19:01.000000 candlelite-1.0.8/candlelite/settings/__init__.py
-drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-07-15 03:39:36.940647 candlelite-1.0.8/candlelite.egg-info/
--rw-r--r--   0 kzlknight   (501) staff       (20)      628 2023-07-15 03:39:36.000000 candlelite-1.0.8/candlelite.egg-info/PKG-INFO
--rw-r--r--   0 kzlknight   (501) staff       (20)      870 2023-07-15 03:39:36.000000 candlelite-1.0.8/candlelite.egg-info/SOURCES.txt
--rw-r--r--   0 kzlknight   (501) staff       (20)        1 2023-07-15 03:39:36.000000 candlelite-1.0.8/candlelite.egg-info/dependency_links.txt
--rw-r--r--   0 kzlknight   (501) staff       (20)       54 2023-07-15 03:39:36.000000 candlelite-1.0.8/candlelite.egg-info/entry_points.txt
--rw-r--r--   0 kzlknight   (501) staff       (20)       18 2023-07-15 03:39:36.000000 candlelite-1.0.8/candlelite.egg-info/requires.txt
--rw-r--r--   0 kzlknight   (501) staff       (20)       11 2023-07-15 03:39:36.000000 candlelite-1.0.8/candlelite.egg-info/top_level.txt
--rw-r--r--   0 kzlknight   (501) staff       (20)       38 2023-07-15 03:39:36.950564 candlelite-1.0.8/setup.cfg
--rw-r--r--   0 kzlknight   (501) staff       (20)     2835 2023-07-15 03:37:17.000000 candlelite-1.0.8/setup.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-07-15 03:55:56.970721 candlelite-1.0.9/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      628 2023-07-15 03:55:56.968996 candlelite-1.0.9/PKG-INFO
+-rw-r--r--   0 kzlknight   (501) staff       (20)       25 2023-02-21 10:35:06.000000 candlelite-1.0.9/README.md
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-07-15 03:55:56.952049 candlelite-1.0.9/candlelite/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      242 2023-07-15 03:55:33.000000 candlelite-1.0.9/candlelite/__init__.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-07-15 03:55:56.959605 candlelite-1.0.9/candlelite/calculate/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      204 2023-01-25 20:14:09.000000 candlelite-1.0.9/candlelite/calculate/__init__.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     1167 2023-07-15 03:55:21.000000 candlelite-1.0.9/candlelite/calculate/bar.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     1144 2023-07-15 03:54:51.000000 candlelite-1.0.9/candlelite/calculate/interval.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     5141 2023-01-25 19:36:00.000000 candlelite-1.0.9/candlelite/calculate/technical.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     6651 2023-01-25 20:11:14.000000 candlelite-1.0.9/candlelite/calculate/transform.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     5104 2023-01-26 21:55:48.000000 candlelite-1.0.9/candlelite/calculate/valid.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-07-15 03:55:56.960079 candlelite-1.0.9/candlelite/cmdline/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      975 2023-01-26 07:20:12.000000 candlelite-1.0.9/candlelite/cmdline/__init__.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-07-15 03:55:56.961905 candlelite-1.0.9/candlelite/crypto/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      101 2023-02-21 10:35:06.000000 candlelite-1.0.9/candlelite/crypto/__init__.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)    11177 2023-06-22 07:44:31.000000 candlelite-1.0.9/candlelite/crypto/_base.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      885 2023-01-29 21:17:12.000000 candlelite-1.0.9/candlelite/crypto/binace_lite.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      818 2023-01-25 21:49:55.000000 candlelite-1.0.9/candlelite/crypto/okx_lite.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-07-15 03:55:56.964899 candlelite-1.0.9/candlelite/exception/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      131 2023-01-25 19:19:56.000000 candlelite-1.0.9/candlelite/exception/__init__.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      235 2023-01-25 19:24:42.000000 candlelite-1.0.9/candlelite/exception/_base.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     1294 2023-05-02 04:09:34.000000 candlelite-1.0.9/candlelite/exception/candle.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      202 2023-01-25 19:25:08.000000 candlelite-1.0.9/candlelite/exception/execute.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)      813 2023-01-25 20:07:05.000000 candlelite-1.0.9/candlelite/exception/param.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-07-15 03:55:56.967445 candlelite-1.0.9/candlelite/io/
+-rw-r--r--   0 kzlknight   (501) staff       (20)       93 2023-02-21 10:35:06.000000 candlelite-1.0.9/candlelite/io/__init__.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)    12243 2023-06-22 07:36:19.000000 candlelite-1.0.9/candlelite/io/load.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     8693 2023-05-01 14:46:48.000000 candlelite-1.0.9/candlelite/io/path.py
+-rw-r--r--   0 kzlknight   (501) staff       (20)     7368 2023-03-06 06:06:56.000000 candlelite-1.0.9/candlelite/io/save.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-07-15 03:55:56.967998 candlelite-1.0.9/candlelite/settings/
+-rw-r--r--   0 kzlknight   (501) staff       (20)     4485 2023-01-29 21:19:01.000000 candlelite-1.0.9/candlelite/settings/__init__.py
+drwxr-xr-x   0 kzlknight   (501) staff       (20)        0 2023-07-15 03:55:56.955834 candlelite-1.0.9/candlelite.egg-info/
+-rw-r--r--   0 kzlknight   (501) staff       (20)      628 2023-07-15 03:55:56.000000 candlelite-1.0.9/candlelite.egg-info/PKG-INFO
+-rw-r--r--   0 kzlknight   (501) staff       (20)      870 2023-07-15 03:55:56.000000 candlelite-1.0.9/candlelite.egg-info/SOURCES.txt
+-rw-r--r--   0 kzlknight   (501) staff       (20)        1 2023-07-15 03:55:56.000000 candlelite-1.0.9/candlelite.egg-info/dependency_links.txt
+-rw-r--r--   0 kzlknight   (501) staff       (20)       54 2023-07-15 03:55:56.000000 candlelite-1.0.9/candlelite.egg-info/entry_points.txt
+-rw-r--r--   0 kzlknight   (501) staff       (20)       18 2023-07-15 03:55:56.000000 candlelite-1.0.9/candlelite.egg-info/requires.txt
+-rw-r--r--   0 kzlknight   (501) staff       (20)       11 2023-07-15 03:55:56.000000 candlelite-1.0.9/candlelite.egg-info/top_level.txt
+-rw-r--r--   0 kzlknight   (501) staff       (20)       38 2023-07-15 03:55:56.970933 candlelite-1.0.9/setup.cfg
+-rw-r--r--   0 kzlknight   (501) staff       (20)     2835 2023-07-15 03:55:36.000000 candlelite-1.0.9/setup.py
```

### Comparing `candlelite-1.0.8/PKG-INFO` & `candlelite-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: candlelite
-Version: 1.0.8
+Version: 1.0.9
 Summary: History candle database and utils
 Home-page: https://github.com/pyted/candlelite
 Author: pyted
 Author-email: pyted@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `candlelite-1.0.8/candlelite/calculate/bar.py` & `candlelite-1.0.9/candlelite/calculate/bar.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.8/candlelite/calculate/interval.py` & `candlelite-1.0.9/candlelite/calculate/interval.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     '''
     :param bar: 时间粒度 1m 3m 5m 15m 1h 2h 4h 1d ...
     :param MINUTE_BAR_INTERVAL: 每分钟的数字间隔，默认毫秒
     '''
     bar_int = int(bar[0:-1].strip())
     suffix = bar[-1].lower()
     if suffix == 's':
-        interval = (MINUTE_BAR_INTERVAL / 60) * bar_int
+        interval = int((MINUTE_BAR_INTERVAL / 60) * bar_int)
     elif suffix == 'm':
         interval = MINUTE_BAR_INTERVAL * bar_int
     elif suffix == 'h':
         interval = MINUTE_BAR_INTERVAL * 60 * bar_int
     elif suffix == 'd':
         interval = MINUTE_BAR_INTERVAL * 60 * 24 * bar_int
     elif suffix == 'w':
```

### Comparing `candlelite-1.0.8/candlelite/calculate/technical.py` & `candlelite-1.0.9/candlelite/calculate/technical.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.8/candlelite/calculate/transform.py` & `candlelite-1.0.9/candlelite/calculate/transform.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.8/candlelite/calculate/valid.py` & `candlelite-1.0.9/candlelite/calculate/valid.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.8/candlelite/cmdline/__init__.py` & `candlelite-1.0.9/candlelite/cmdline/__init__.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.8/candlelite/crypto/_base.py` & `candlelite-1.0.9/candlelite/crypto/_base.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.8/candlelite/crypto/binace_lite.py` & `candlelite-1.0.9/candlelite/crypto/binace_lite.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.8/candlelite/crypto/okx_lite.py` & `candlelite-1.0.9/candlelite/crypto/okx_lite.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.8/candlelite/exception/candle.py` & `candlelite-1.0.9/candlelite/exception/candle.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.8/candlelite/exception/param.py` & `candlelite-1.0.9/candlelite/exception/param.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.8/candlelite/io/load.py` & `candlelite-1.0.9/candlelite/io/load.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.8/candlelite/io/path.py` & `candlelite-1.0.9/candlelite/io/path.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.8/candlelite/io/save.py` & `candlelite-1.0.9/candlelite/io/save.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.8/candlelite/settings/__init__.py` & `candlelite-1.0.9/candlelite/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.8/candlelite.egg-info/PKG-INFO` & `candlelite-1.0.9/candlelite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: candlelite
-Version: 1.0.8
+Version: 1.0.9
 Summary: History candle database and utils
 Home-page: https://github.com/pyted/candlelite
 Author: pyted
 Author-email: pyted@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `candlelite-1.0.8/candlelite.egg-info/SOURCES.txt` & `candlelite-1.0.9/candlelite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `candlelite-1.0.8/setup.py` & `candlelite-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = 'candlelite'
 DESCRIPTION = 'History candle database and utils'
 URL = "https://github.com/pyted/candlelite"
 EMAIL = 'pyted@outlook.com'
 AUTHOR = 'pyted'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.0.8'
+VERSION = '1.0.9'
 
 REQUIRED = [
     'numpy',
     'pandas',
     'paux',
 ]
```

