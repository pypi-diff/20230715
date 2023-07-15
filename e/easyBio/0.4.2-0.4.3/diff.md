# Comparing `tmp/easyBio-0.4.2.tar.gz` & `tmp/easybio-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyBio-0.4.2.tar", last modified: Sat Jul 15 13:04:31 2023, max compression
+gzip compressed data, was "easybio-0.4.3.tar", last modified: Sat Jul 15 13:06:20 2023, max compression
```

## Comparing `easyBio-0.4.2.tar` & `easybio-0.4.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:04:31.860284 easyBio-0.4.2/
--rw-r--r--   0 root         (0) root         (0)      538 2023-07-15 13:04:31.860284 easyBio-0.4.2/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)       30 2023-04-21 05:50:43.000000 easyBio-0.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:04:31.856284 easyBio-0.4.2/easyBio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:04:31.860284 easyBio-0.4.2/easyBio/Utils/
--rw-rw-r--   0 root         (0) root         (0)      661 2023-07-07 11:47:13.000000 easyBio-0.4.2/easyBio/Utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2854 2023-07-07 09:45:10.000000 easyBio-0.4.2/easyBio/Utils/downLoadBAM.py
--rw-rw-r--   0 root         (0) root         (0)     2901 2023-07-07 02:09:13.000000 easyBio-0.4.2/easyBio/Utils/downLoadSRA.py
--rw-rw-r--   0 root         (0) root         (0)     8221 2023-07-07 02:07:55.000000 easyBio-0.4.2/easyBio/Utils/download.py
--rw-rw-r--   0 root         (0) root         (0)     4193 2023-07-07 11:51:19.000000 easyBio-0.4.2/easyBio/Utils/downloadUtils.py
--rw-rw-r--   0 root         (0) root         (0)     9077 2023-07-06 12:33:28.000000 easyBio-0.4.2/easyBio/Utils/easyBioUtils.py
--rw-rw-r--   0 root         (0) root         (0)     2216 2023-07-06 13:07:59.000000 easyBio-0.4.2/easyBio/Utils/easyCellranger.py
--rw-rw-r--   0 root         (0) root         (0)    12112 2023-07-14 10:32:06.000000 easyBio-0.4.2/easyBio/Utils/gsaDownLoadUtils.py
--rw-rw-r--   0 root         (0) root         (0)     2117 2023-04-26 10:50:17.000000 easyBio-0.4.2/easyBio/Utils/netUtils.py
--rw-rw-r--   0 root         (0) root         (0)     2594 2023-07-07 11:45:29.000000 easyBio-0.4.2/easyBio/Utils/runvelocityc.py
--rw-rw-r--   0 root         (0) root         (0)     7773 2023-07-14 10:39:20.000000 easyBio-0.4.2/easyBio/Utils/toFastq.py
--rw-rw-r--   0 root         (0) root         (0)     3735 2023-07-07 09:45:19.000000 easyBio-0.4.2/easyBio/Utils/toolsUtils.py
--rw-rw-r--   0 root         (0) root         (0)      426 2023-07-06 12:55:32.000000 easyBio-0.4.2/easyBio/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     6283 2023-07-12 07:12:26.000000 easyBio-0.4.2/easyBio/changeSRAName.py
--rw-rw-r--   0 root         (0) root         (0)     2136 2023-07-14 04:32:24.000000 easyBio-0.4.2/easyBio/downloadSRA.py
--rw-rw-r--   0 root         (0) root         (0)      200 2023-07-12 06:59:45.000000 easyBio-0.4.2/easyBio/easyBio.py
--rw-rw-r--   0 root         (0) root         (0)     2636 2023-07-14 04:40:35.000000 easyBio-0.4.2/easyBio/gsaPipline.py
--rw-rw-r--   0 root         (0) root         (0)     5024 2023-07-14 10:32:46.000000 easyBio-0.4.2/easyBio/pipline.py
--rw-rw-r--   0 root         (0) root         (0)     1324 2023-07-12 07:12:35.000000 easyBio-0.4.2/easyBio/run_cellranger.py
--rw-rw-r--   0 root         (0) root         (0)      110 2023-07-12 11:04:38.000000 easyBio-0.4.2/easyBio/run_test.py
--rw-rw-r--   0 root         (0) root         (0)     1247 2023-07-12 07:12:38.000000 easyBio-0.4.2/easyBio/runvelocyto.py
--rw-rw-r--   0 root         (0) root         (0)     1479 2023-07-12 07:12:42.000000 easyBio-0.4.2/easyBio/splitSRA.py
--rw-rw-r--   0 root         (0) root         (0)     1006 2023-04-29 17:25:20.000000 easyBio-0.4.2/easyBio/test.py
--rw-rw-r--   0 root         (0) root         (0)     2671 2023-07-12 07:12:49.000000 easyBio-0.4.2/easyBio/tidy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:04:31.856284 easyBio-0.4.2/easyBio.egg-info/
--rw-r--r--   0 root         (0) root         (0)      538 2023-07-15 13:04:31.000000 easyBio-0.4.2/easyBio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      831 2023-07-15 13:04:31.000000 easyBio-0.4.2/easyBio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 13:04:31.000000 easyBio-0.4.2/easyBio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      345 2023-07-15 13:04:31.000000 easyBio-0.4.2/easyBio.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 13:04:28.000000 easyBio-0.4.2/easyBio.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       27 2023-07-15 13:04:31.000000 easyBio-0.4.2/easyBio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-15 13:04:31.000000 easyBio-0.4.2/easyBio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-15 13:04:31.860284 easyBio-0.4.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1562 2023-07-15 13:03:59.000000 easyBio-0.4.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:06:20.789289 easybio-0.4.3/
+-rw-r--r--   0 root         (0) root         (0)      538 2023-07-15 13:06:20.789289 easybio-0.4.3/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)       30 2023-04-21 05:50:43.000000 easybio-0.4.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:06:20.789289 easybio-0.4.3/easyBio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:06:20.789289 easybio-0.4.3/easyBio/Utils/
+-rw-rw-r--   0 root         (0) root         (0)      661 2023-07-07 11:47:13.000000 easybio-0.4.3/easyBio/Utils/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2854 2023-07-07 09:45:10.000000 easybio-0.4.3/easyBio/Utils/downLoadBAM.py
+-rw-rw-r--   0 root         (0) root         (0)     2901 2023-07-07 02:09:13.000000 easybio-0.4.3/easyBio/Utils/downLoadSRA.py
+-rw-rw-r--   0 root         (0) root         (0)     8221 2023-07-07 02:07:55.000000 easybio-0.4.3/easyBio/Utils/download.py
+-rw-rw-r--   0 root         (0) root         (0)     4193 2023-07-07 11:51:19.000000 easybio-0.4.3/easyBio/Utils/downloadUtils.py
+-rw-rw-r--   0 root         (0) root         (0)     9077 2023-07-06 12:33:28.000000 easybio-0.4.3/easyBio/Utils/easyBioUtils.py
+-rw-rw-r--   0 root         (0) root         (0)     2216 2023-07-06 13:07:59.000000 easybio-0.4.3/easyBio/Utils/easyCellranger.py
+-rw-rw-r--   0 root         (0) root         (0)    12112 2023-07-14 10:32:06.000000 easybio-0.4.3/easyBio/Utils/gsaDownLoadUtils.py
+-rw-rw-r--   0 root         (0) root         (0)     2117 2023-04-26 10:50:17.000000 easybio-0.4.3/easyBio/Utils/netUtils.py
+-rw-rw-r--   0 root         (0) root         (0)     2594 2023-07-07 11:45:29.000000 easybio-0.4.3/easyBio/Utils/runvelocityc.py
+-rw-rw-r--   0 root         (0) root         (0)     7773 2023-07-14 10:39:20.000000 easybio-0.4.3/easyBio/Utils/toFastq.py
+-rw-rw-r--   0 root         (0) root         (0)     3735 2023-07-07 09:45:19.000000 easybio-0.4.3/easyBio/Utils/toolsUtils.py
+-rw-rw-r--   0 root         (0) root         (0)      426 2023-07-06 12:55:32.000000 easybio-0.4.3/easyBio/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     6283 2023-07-12 07:12:26.000000 easybio-0.4.3/easyBio/changeSRAName.py
+-rw-rw-r--   0 root         (0) root         (0)     2136 2023-07-14 04:32:24.000000 easybio-0.4.3/easyBio/downloadSRA.py
+-rw-rw-r--   0 root         (0) root         (0)      200 2023-07-12 06:59:45.000000 easybio-0.4.3/easyBio/easyBio.py
+-rw-rw-r--   0 root         (0) root         (0)     2636 2023-07-14 04:40:35.000000 easybio-0.4.3/easyBio/gsaPipline.py
+-rw-rw-r--   0 root         (0) root         (0)     5024 2023-07-14 10:32:46.000000 easybio-0.4.3/easyBio/pipline.py
+-rw-rw-r--   0 root         (0) root         (0)     1324 2023-07-12 07:12:35.000000 easybio-0.4.3/easyBio/run_cellranger.py
+-rw-rw-r--   0 root         (0) root         (0)      110 2023-07-12 11:04:38.000000 easybio-0.4.3/easyBio/run_test.py
+-rw-rw-r--   0 root         (0) root         (0)     1247 2023-07-12 07:12:38.000000 easybio-0.4.3/easyBio/runvelocyto.py
+-rw-rw-r--   0 root         (0) root         (0)     1479 2023-07-12 07:12:42.000000 easybio-0.4.3/easyBio/splitSRA.py
+-rw-rw-r--   0 root         (0) root         (0)     1006 2023-04-29 17:25:20.000000 easybio-0.4.3/easyBio/test.py
+-rw-rw-r--   0 root         (0) root         (0)     2671 2023-07-12 07:12:49.000000 easybio-0.4.3/easyBio/tidy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 13:06:20.789289 easybio-0.4.3/easybio.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)      538 2023-07-15 13:06:20.000000 easybio-0.4.3/easybio.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      831 2023-07-15 13:06:20.000000 easybio-0.4.3/easybio.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-15 13:06:20.000000 easybio-0.4.3/easybio.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)      345 2023-07-15 13:06:20.000000 easybio-0.4.3/easybio.egg-info/entry_points.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-14 10:41:43.000000 easybio-0.4.3/easybio.egg-info/not-zip-safe
+-rw-rw-r--   0 root         (0) root         (0)       27 2023-07-15 13:06:20.000000 easybio-0.4.3/easybio.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)        8 2023-07-15 13:06:20.000000 easybio-0.4.3/easybio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-15 13:06:20.789289 easybio-0.4.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1562 2023-07-15 13:05:23.000000 easybio-0.4.3/setup.py
```

### Comparing `easyBio-0.4.2/PKG-INFO` & `easybio-0.4.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: easyBio
-Version: 0.4.2
+Name: easybio
+Version: 0.4.3
 Summary: The purpose of the creation of this package is to make bioinformatics analysis simpler.
 Home-page: https://github.com/xleizi/easyBio_conda
 Author: Lei Cui
 Author-email: cuilei798@qq.com
 Maintainer: Lei Cui
 Maintainer-email: cuilei798@qq.com
 License: MIT License
```

### Comparing `easyBio-0.4.2/easyBio/Utils/__init__.py` & `easybio-0.4.3/easyBio/Utils/__init__.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/Utils/downLoadBAM.py` & `easybio-0.4.3/easyBio/Utils/downLoadBAM.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/Utils/downLoadSRA.py` & `easybio-0.4.3/easyBio/Utils/downLoadSRA.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/Utils/download.py` & `easybio-0.4.3/easyBio/Utils/download.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/Utils/downloadUtils.py` & `easybio-0.4.3/easyBio/Utils/downloadUtils.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/Utils/easyBioUtils.py` & `easybio-0.4.3/easyBio/Utils/easyBioUtils.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/Utils/easyCellranger.py` & `easybio-0.4.3/easyBio/Utils/easyCellranger.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/Utils/gsaDownLoadUtils.py` & `easybio-0.4.3/easyBio/Utils/gsaDownLoadUtils.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/Utils/netUtils.py` & `easybio-0.4.3/easyBio/Utils/netUtils.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/Utils/runvelocityc.py` & `easybio-0.4.3/easyBio/Utils/runvelocityc.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/Utils/toFastq.py` & `easybio-0.4.3/easyBio/Utils/toFastq.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/Utils/toolsUtils.py` & `easybio-0.4.3/easyBio/Utils/toolsUtils.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/changeSRAName.py` & `easybio-0.4.3/easyBio/changeSRAName.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/downloadSRA.py` & `easybio-0.4.3/easyBio/downloadSRA.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/gsaPipline.py` & `easybio-0.4.3/easyBio/gsaPipline.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/pipline.py` & `easybio-0.4.3/easyBio/pipline.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/run_cellranger.py` & `easybio-0.4.3/easyBio/run_cellranger.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/runvelocyto.py` & `easybio-0.4.3/easyBio/runvelocyto.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/splitSRA.py` & `easybio-0.4.3/easyBio/splitSRA.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/test.py` & `easybio-0.4.3/easyBio/test.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio/tidy.py` & `easybio-0.4.3/easyBio/tidy.py`

 * *Files identical despite different names*

### Comparing `easyBio-0.4.2/easyBio.egg-info/PKG-INFO` & `easybio-0.4.3/easybio.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: easyBio
-Version: 0.4.2
+Name: easybio
+Version: 0.4.3
 Summary: The purpose of the creation of this package is to make bioinformatics analysis simpler.
 Home-page: https://github.com/xleizi/easyBio_conda
 Author: Lei Cui
 Author-email: cuilei798@qq.com
 Maintainer: Lei Cui
 Maintainer-email: cuilei798@qq.com
 License: MIT License
```

### Comparing `easyBio-0.4.2/easyBio.egg-info/SOURCES.txt` & `easybio-0.4.3/easybio.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 easyBio/pipline.py
 easyBio/run_cellranger.py
 easyBio/run_test.py
 easyBio/runvelocyto.py
 easyBio/splitSRA.py
 easyBio/test.py
 easyBio/tidy.py
-easyBio.egg-info/PKG-INFO
-easyBio.egg-info/SOURCES.txt
-easyBio.egg-info/dependency_links.txt
-easyBio.egg-info/entry_points.txt
-easyBio.egg-info/not-zip-safe
-easyBio.egg-info/requires.txt
-easyBio.egg-info/top_level.txt
 easyBio/Utils/__init__.py
 easyBio/Utils/downLoadBAM.py
 easyBio/Utils/downLoadSRA.py
 easyBio/Utils/download.py
 easyBio/Utils/downloadUtils.py
 easyBio/Utils/easyBioUtils.py
 easyBio/Utils/easyCellranger.py
 easyBio/Utils/gsaDownLoadUtils.py
 easyBio/Utils/netUtils.py
 easyBio/Utils/runvelocityc.py
 easyBio/Utils/toFastq.py
-easyBio/Utils/toolsUtils.py
+easyBio/Utils/toolsUtils.py
+easybio.egg-info/PKG-INFO
+easybio.egg-info/SOURCES.txt
+easybio.egg-info/dependency_links.txt
+easybio.egg-info/entry_points.txt
+easybio.egg-info/not-zip-safe
+easybio.egg-info/requires.txt
+easybio.egg-info/top_level.txt
```

### Comparing `easyBio-0.4.2/setup.py` & `easybio-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
-VERSION = '0.4.2'
+VERSION = '0.4.3'
 
 setup(
-    name='easyBio',  # package name
+    name='easybio',  # package name
     version=VERSION,  # package version
     author='Lei Cui',
     author_email='cuilei798@qq.com',
     maintainer='Lei Cui',
     maintainer_email='cuilei798@qq.com',
     license='MIT License',
     platforms=["linux"],
```

