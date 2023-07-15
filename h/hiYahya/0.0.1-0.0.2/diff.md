# Comparing `tmp/hiYahya-0.0.1.tar.gz` & `tmp/hiYahya-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiYahya-0.0.1.tar", last modified: Sat Jul 15 18:11:42 2023, max compression
+gzip compressed data, was "hiYahya-0.0.2.tar", last modified: Sat Jul 15 18:47:45 2023, max compression
```

## Comparing `hiYahya-0.0.1.tar` & `hiYahya-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 noorhashem   (501) staff       (20)        0 2023-07-15 18:11:42.080961 hiYahya-0.0.1/
--rw-r--r--   0 noorhashem   (501) staff       (20)      547 2023-07-15 18:11:42.080831 hiYahya-0.0.1/PKG-INFO
-drwxr-xr-x   0 noorhashem   (501) staff       (20)        0 2023-07-15 18:11:42.080088 hiYahya-0.0.1/hiYahya.egg-info/
--rw-r--r--   0 noorhashem   (501) staff       (20)      547 2023-07-15 18:11:42.000000 hiYahya-0.0.1/hiYahya.egg-info/PKG-INFO
--rw-r--r--   0 noorhashem   (501) staff       (20)      176 2023-07-15 18:11:42.000000 hiYahya-0.0.1/hiYahya.egg-info/SOURCES.txt
--rw-r--r--   0 noorhashem   (501) staff       (20)        1 2023-07-15 18:11:42.000000 hiYahya-0.0.1/hiYahya.egg-info/dependency_links.txt
--rw-r--r--   0 noorhashem   (501) staff       (20)       13 2023-07-15 18:11:42.000000 hiYahya-0.0.1/hiYahya.egg-info/top_level.txt
--rw-r--r--   0 noorhashem   (501) staff       (20)       38 2023-07-15 18:11:42.081009 hiYahya-0.0.1/setup.cfg
--rw-r--r--   0 noorhashem   (501) staff       (20)      790 2023-07-15 18:09:52.000000 hiYahya-0.0.1/setup.py
-drwxr-xr-x   0 noorhashem   (501) staff       (20)        0 2023-07-15 18:11:42.080526 hiYahya-0.0.1/yahyapackage/
--rw-r--r--   0 noorhashem   (501) staff       (20)       20 2023-07-15 17:03:10.000000 hiYahya-0.0.1/yahyapackage/__init__.py
--rw-r--r--   0 noorhashem   (501) staff       (20)       36 2023-07-15 17:02:58.000000 hiYahya-0.0.1/yahyapackage/hi.py
+drwxr-xr-x   0 noorhashem   (501) staff       (20)        0 2023-07-15 18:47:45.349328 hiYahya-0.0.2/
+-rw-r--r--   0 noorhashem   (501) staff       (20)      547 2023-07-15 18:47:45.349188 hiYahya-0.0.2/PKG-INFO
+drwxr-xr-x   0 noorhashem   (501) staff       (20)        0 2023-07-15 18:47:45.348212 hiYahya-0.0.2/hiYahya.egg-info/
+-rw-r--r--   0 noorhashem   (501) staff       (20)      547 2023-07-15 18:47:45.000000 hiYahya-0.0.2/hiYahya.egg-info/PKG-INFO
+-rw-r--r--   0 noorhashem   (501) staff       (20)      181 2023-07-15 18:47:45.000000 hiYahya-0.0.2/hiYahya.egg-info/SOURCES.txt
+-rw-r--r--   0 noorhashem   (501) staff       (20)        1 2023-07-15 18:47:45.000000 hiYahya-0.0.2/hiYahya.egg-info/dependency_links.txt
+-rw-r--r--   0 noorhashem   (501) staff       (20)       13 2023-07-15 18:47:45.000000 hiYahya-0.0.2/hiYahya.egg-info/top_level.txt
+-rw-r--r--   0 noorhashem   (501) staff       (20)       38 2023-07-15 18:47:45.349381 hiYahya-0.0.2/setup.cfg
+-rw-r--r--   0 noorhashem   (501) staff       (20)      790 2023-07-15 18:47:34.000000 hiYahya-0.0.2/setup.py
+drwxr-xr-x   0 noorhashem   (501) staff       (20)        0 2023-07-15 18:47:45.348801 hiYahya-0.0.2/yahyapackage/
+-rw-r--r--   0 noorhashem   (501) staff       (20)       25 2023-07-15 18:44:49.000000 hiYahya-0.0.2/yahyapackage/__init__.py
+-rw-r--r--   0 noorhashem   (501) staff       (20)       59 2023-07-15 18:36:42.000000 hiYahya-0.0.2/yahyapackage/hiYahya.py
```

### Comparing `hiYahya-0.0.1/PKG-INFO` & `hiYahya-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiYahya
-Version: 0.0.1
+Version: 0.0.2
 Summary: Saying hi to Yahya
 Home-page: UNKNOWN
 Author: Noor Hashem
 Author-email: noor.hashem@hotmail.com
 License: UNKNOWN
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `hiYahya-0.0.1/hiYahya.egg-info/PKG-INFO` & `hiYahya-0.0.2/hiYahya.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiYahya
-Version: 0.0.1
+Version: 0.0.2
 Summary: Saying hi to Yahya
 Home-page: UNKNOWN
 Author: Noor Hashem
 Author-email: noor.hashem@hotmail.com
 License: UNKNOWN
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `hiYahya-0.0.1/setup.py` & `hiYahya-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Saying hi to Yahya'
 LONG_DESCRIPTION = 'Saying hi to Yahya'
 
 # Setting up
 setup(
     name="hiYahya",
     version=VERSION,
```

