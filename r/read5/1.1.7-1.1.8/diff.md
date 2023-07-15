# Comparing `tmp/read5-1.1.7.tar.gz` & `tmp/read5-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "read5-1.1.7.tar", last modified: Fri Jul 14 19:03:11 2023, max compression
+gzip compressed data, was "read5-1.1.8.tar", last modified: Sat Jul 15 18:36:17 2023, max compression
```

## Comparing `read5-1.1.7.tar` & `read5-1.1.8.tar`

### file list

```diff
@@ -1,26 +1,41 @@
-drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-14 19:03:11.315812 read5-1.1.7/
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    35149 2023-04-26 15:37:10.000000 read5-1.1.7/LICENSE
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)       22 2023-04-26 15:39:17.000000 read5-1.1.7/MANIFEST.in
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     3377 2023-07-14 19:03:11.319812 read5-1.1.7/PKG-INFO
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     3541 2023-07-14 12:49:29.000000 read5-1.1.7/README.md
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     2509 2023-07-12 22:00:39.000000 read5-1.1.7/README.rst
-drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-14 19:03:11.335812 read5-1.1.7/read5/
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    20283 2023-07-14 12:44:04.000000 read5-1.1.7/read5/AbstractFileReader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      773 2023-07-12 15:11:37.000000 read5-1.1.7/read5/Exceptions.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    13183 2023-07-14 12:47:54.000000 read5-1.1.7/read5/Fast5Reader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    11653 2023-07-12 12:38:39.000000 read5-1.1.7/read5/Pod5Reader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      980 2023-07-12 12:52:52.000000 read5-1.1.7/read5/Reader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     8605 2023-07-12 12:39:08.000000 read5-1.1.7/read5/Slow5Reader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      148 2023-07-13 08:25:24.000000 read5-1.1.7/read5/__init__.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      497 2023-07-14 19:03:11.335812 read5-1.1.7/read5/_version.py
-drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-14 19:03:11.295812 read5-1.1.7/read5.egg-info/
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     3377 2023-07-14 19:03:10.000000 read5-1.1.7/read5.egg-info/PKG-INFO
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      404 2023-07-14 19:03:11.000000 read5-1.1.7/read5.egg-info/SOURCES.txt
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)        1 2023-07-14 19:03:11.000000 read5-1.1.7/read5.egg-info/dependency_links.txt
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)       88 2023-07-14 19:03:11.000000 read5-1.1.7/read5.egg-info/requires.txt
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)        6 2023-07-14 19:03:11.000000 read5-1.1.7/read5.egg-info/top_level.txt
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      208 2023-07-14 19:03:11.327812 read5-1.1.7/setup.cfg
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     1519 2023-07-12 21:25:01.000000 read5-1.1.7/setup.py
-drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-14 19:03:11.307812 read5-1.1.7/tests/
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    54377 2023-07-12 12:51:42.000000 read5-1.1.7/tests/test_FileReader.py
--rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    68611 2023-04-26 15:39:17.000000 read5-1.1.7/versioneer.py
+drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-15 18:36:17.643064 read5-1.1.8/
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    35149 2023-04-26 15:37:10.000000 read5-1.1.8/LICENSE
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)       33 2023-07-15 18:32:46.000000 read5-1.1.8/MANIFEST.in
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     3377 2023-07-15 18:36:17.647064 read5-1.1.8/PKG-INFO
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     3576 2023-07-14 20:09:57.000000 read5-1.1.8/README.md
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     2509 2023-07-12 22:00:39.000000 read5-1.1.8/README.rst
+drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-15 18:36:17.659064 read5-1.1.8/read5/
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    20283 2023-07-14 12:44:04.000000 read5-1.1.8/read5/AbstractFileReader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      773 2023-07-12 15:11:37.000000 read5-1.1.8/read5/Exceptions.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    13183 2023-07-14 12:47:54.000000 read5-1.1.8/read5/Fast5Reader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    11653 2023-07-12 12:38:39.000000 read5-1.1.8/read5/Pod5Reader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      980 2023-07-12 12:52:52.000000 read5-1.1.8/read5/Reader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     8605 2023-07-12 12:39:08.000000 read5-1.1.8/read5/Slow5Reader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      148 2023-07-15 08:28:26.000000 read5-1.1.8/read5/__init__.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      497 2023-07-15 18:36:17.659064 read5-1.1.8/read5/_version.py
+drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-15 18:36:17.139065 read5-1.1.8/read5.egg-info/
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     3377 2023-07-15 18:36:16.000000 read5-1.1.8/read5.egg-info/PKG-INFO
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      912 2023-07-15 18:36:16.000000 read5-1.1.8/read5.egg-info/SOURCES.txt
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)        1 2023-07-15 18:36:16.000000 read5-1.1.8/read5.egg-info/dependency_links.txt
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)       88 2023-07-15 18:36:16.000000 read5-1.1.8/read5.egg-info/requires.txt
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)        6 2023-07-15 18:36:16.000000 read5-1.1.8/read5.egg-info/top_level.txt
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      208 2023-07-15 18:36:17.651064 read5-1.1.8/setup.cfg
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)     1519 2023-07-12 21:25:01.000000 read5-1.1.8/setup.py
+drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-15 18:36:17.487064 read5-1.1.8/tests/
+drwxr-xr-x   0 yi98suv  (13381) bioinf3   (2904)        0 2023-07-15 18:36:17.619064 read5-1.1.8/tests/__pycache__/
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      161 2023-07-12 12:51:33.000000 read5-1.1.8/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      137 2023-07-12 11:48:27.000000 read5-1.1.8/tests/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    24897 2023-05-03 11:13:18.000000 read5-1.1.8/tests/__pycache__/testFileReader.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    92760 2023-05-08 13:37:55.000000 read5-1.1.8/tests/__pycache__/test_FileReader.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    93836 2023-07-12 12:51:48.000000 read5-1.1.8/tests/__pycache__/test_FileReader.cpython-310-pytest-7.4.0.pyc
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    47423 2023-07-12 12:20:31.000000 read5-1.1.8/tests/__pycache__/test_FileReader.cpython-310.pyc
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)   158376 2023-07-12 11:48:27.000000 read5-1.1.8/tests/__pycache__/test_FileReader.cpython-39-pytest-7.1.2.pyc
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      369 2023-05-02 15:11:08.000000 read5-1.1.8/tests/ids.txt
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)   325086 2023-05-02 12:32:46.000000 read5-1.1.8/tests/test.blow5
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      612 2023-05-02 12:34:49.000000 read5-1.1.8/tests/test.blow5.idx
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)   388942 2023-05-02 15:17:01.000000 read5-1.1.8/tests/test.fast5
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)   335512 2023-05-02 15:18:24.000000 read5-1.1.8/tests/test.pod5
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)  1432159 2023-05-02 12:32:36.000000 read5-1.1.8/tests/test.slow5
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)      612 2023-05-02 12:34:49.000000 read5-1.1.8/tests/test.slow5.idx
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    54377 2023-07-12 12:51:42.000000 read5-1.1.8/tests/test_FileReader.py
+-rw-r--r--   0 yi98suv  (13381) bioinf3   (2904)    68611 2023-04-26 15:39:17.000000 read5-1.1.8/versioneer.py
```

### Comparing `read5-1.1.7/LICENSE` & `read5-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `read5-1.1.7/PKG-INFO` & `read5-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: read5
-Version: 1.1.7
+Version: 1.1.8
 Summary: Wrapper to read fast5, slow5, blow5 and pod5 files.
 Home-page: https://github.com/JannesSP/read5
 Author: Jannes Spangenberg
 Author-email: jannes.spangenberg@uni-jena.de
 License: GNU General Public License v3
 Keywords: read5,slow5,blow5,fast5,pod5,ONT,Oxford Nanopore Technologies,Nanopore,raw data,wrapper
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `read5-1.1.7/README.md` & `read5-1.1.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ![Alt text](figures/logo.png)
 
 Read5 is a python wrapper to read fast5, slow5/blow5 and pod5 files using the same overloaded functions from different APIs.
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-teal.svg)](https://www.gnu.org/licenses/gpl-3.0)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/read5)
 
-![PyPI](https://img.shields.io/pypi/v/read5) ![PyPI - Downloads](https://img.shields.io/pypi/dm/read5) ![PyPI - Status](https://img.shields.io/pypi/status/read5)
+[![PyPI](https://img.shields.io/pypi/v/read5) ![PyPI - Downloads](https://img.shields.io/pypi/dm/read5) ![PyPI - Status](https://img.shields.io/pypi/status/read5)](https://pypi.org/project/read5/)
 
 
 [![Anaconda-Server Badge](https://anaconda.org/jannessp/read5/badges/version.svg)](https://anaconda.org/jannessp/read5) ![Conda](https://img.shields.io/conda/dn/jannessp/read5) [![Conda package](https://anaconda.org/jannessp/read5/badges/latest_release_date.svg)](https://anaconda.org/jannessp/read5) [![Conda package](https://anaconda.org/jannessp/read5/badges/platforms.svg)](https://anaconda.org/jannessp/read5)
  
 [![DOI](https://zenodo.org/badge/633012569.svg)](https://zenodo.org/badge/latestdoi/633012569)
 
 [![Twitter Follow](https://img.shields.io/twitter/follow/Ja_Spangenberg)](https://twitter.com/Ja_Spangenberg)
```

### Comparing `read5-1.1.7/README.rst` & `read5-1.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `read5-1.1.7/read5/AbstractFileReader.py` & `read5-1.1.8/read5/AbstractFileReader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.7/read5/Exceptions.py` & `read5-1.1.8/read5/Exceptions.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.7/read5/Fast5Reader.py` & `read5-1.1.8/read5/Fast5Reader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.7/read5/Pod5Reader.py` & `read5-1.1.8/read5/Pod5Reader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.7/read5/Reader.py` & `read5-1.1.8/read5/Reader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.7/read5/Slow5Reader.py` & `read5-1.1.8/read5/Slow5Reader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.7/read5.egg-info/PKG-INFO` & `read5-1.1.8/read5.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: read5
-Version: 1.1.7
+Version: 1.1.8
 Summary: Wrapper to read fast5, slow5, blow5 and pod5 files.
 Home-page: https://github.com/JannesSP/read5
 Author: Jannes Spangenberg
 Author-email: jannes.spangenberg@uni-jena.de
 License: GNU General Public License v3
 Keywords: read5,slow5,blow5,fast5,pod5,ONT,Oxford Nanopore Technologies,Nanopore,raw data,wrapper
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `read5-1.1.7/setup.py` & `read5-1.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.7/tests/test_FileReader.py` & `read5-1.1.8/tests/test_FileReader.py`

 * *Files identical despite different names*

### Comparing `read5-1.1.7/versioneer.py` & `read5-1.1.8/versioneer.py`

 * *Files identical despite different names*

