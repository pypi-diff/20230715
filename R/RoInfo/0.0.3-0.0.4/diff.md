# Comparing `tmp/RoInfo-0.0.3.tar.gz` & `tmp/RoInfo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RoInfo-0.0.3.tar", last modified: Sat Jul 15 06:05:42 2023, max compression
+gzip compressed data, was "RoInfo-0.0.4.tar", last modified: Sat Jul 15 06:49:54 2023, max compression
```

## Comparing `RoInfo-0.0.3.tar` & `RoInfo-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 06:05:42.026582 RoInfo-0.0.3/
--rw-rw-rw-   0        0        0      617 2023-07-15 06:05:42.018276 RoInfo-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-12 12:51:48.000000 RoInfo-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 06:05:41.980587 RoInfo-0.0.3/RoInfo/
--rw-rw-rw-   0        0        0     5042 2023-05-12 13:27:41.000000 RoInfo-0.0.3/RoInfo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 06:05:42.013227 RoInfo-0.0.3/RoInfo.egg-info/
--rw-rw-rw-   0        0        0      617 2023-07-15 06:05:41.000000 RoInfo-0.0.3/RoInfo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-07-15 06:05:41.000000 RoInfo-0.0.3/RoInfo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 06:05:41.000000 RoInfo-0.0.3/RoInfo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-15 06:05:41.000000 RoInfo-0.0.3/RoInfo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-15 06:05:41.000000 RoInfo-0.0.3/RoInfo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 06:05:42.026582 RoInfo-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      993 2023-05-12 12:54:26.000000 RoInfo-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 06:49:54.133301 RoInfo-0.0.4/
+-rw-rw-rw-   0        0        0      617 2023-07-15 06:49:54.121075 RoInfo-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-12 12:51:48.000000 RoInfo-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 06:49:54.050234 RoInfo-0.0.4/RoInfo/
+-rw-rw-rw-   0        0        0     5042 2023-05-12 13:27:41.000000 RoInfo-0.0.4/RoInfo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 06:49:54.116164 RoInfo-0.0.4/RoInfo.egg-info/
+-rw-rw-rw-   0        0        0      617 2023-07-15 06:49:53.000000 RoInfo-0.0.4/RoInfo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-07-15 06:49:53.000000 RoInfo-0.0.4/RoInfo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 06:49:53.000000 RoInfo-0.0.4/RoInfo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-15 06:49:53.000000 RoInfo-0.0.4/RoInfo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-15 06:49:53.000000 RoInfo-0.0.4/RoInfo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 06:49:54.134276 RoInfo-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      993 2023-07-15 06:47:26.000000 RoInfo-0.0.4/setup.py
```

### Comparing `RoInfo-0.0.3/PKG-INFO` & `RoInfo-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RoInfo
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Roblox API Wrapper for roblox.com
 Home-page: 
 Author: Ryan_shamu
 Author-email: Ryanshamu418@Gmail.com
 Keywords: Roblox,RoInfo,Roblox Web Api,Roblox Python,Roblox For Python,Roblox Api,Roblox Api Library,Roblox Bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `RoInfo-0.0.3/RoInfo/__init__.py` & `RoInfo-0.0.4/RoInfo/__init__.py`

 * *Files identical despite different names*

### Comparing `RoInfo-0.0.3/RoInfo.egg-info/PKG-INFO` & `RoInfo-0.0.4/RoInfo.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RoInfo
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Roblox API Wrapper for roblox.com
 Home-page: 
 Author: Ryan_shamu
 Author-email: Ryanshamu418@Gmail.com
 Keywords: Roblox,RoInfo,Roblox Web Api,Roblox Python,Roblox For Python,Roblox Api,Roblox Api Library,Roblox Bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `RoInfo-0.0.3/setup.py` & `RoInfo-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'A Roblox API Wrapper for roblox.com'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="RoInfo",
     version=VERSION,
```

