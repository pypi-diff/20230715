# Comparing `tmp/lbstanza-wrappers-0.2.1.tar.gz` & `tmp/lbstanza-wrappers-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbstanza-wrappers-0.2.1.tar", last modified: Sat Jul 15 04:45:56 2023, max compression
+gzip compressed data, was "lbstanza-wrappers-0.2.2.tar", last modified: Sat Jul 15 04:50:44 2023, max compression
```

## Comparing `lbstanza-wrappers-0.2.1.tar` & `lbstanza-wrappers-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 callendorph  (1000) callendorph  (1000)        0 2023-07-15 04:45:56.290342 lbstanza-wrappers-0.2.1/
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)    35149 2023-07-15 04:37:49.000000 lbstanza-wrappers-0.2.1/LICENSE
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)     2586 2023-07-15 04:45:56.290342 lbstanza-wrappers-0.2.1/PKG-INFO
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)     2232 2023-07-15 04:37:49.000000 lbstanza-wrappers-0.2.1/README.md
--rwxrwxr-x   0 callendorph  (1000) callendorph  (1000)    30594 2023-07-15 04:45:38.000000 lbstanza-wrappers-0.2.1/convert2stanza.py
--rwxrwxr-x   0 callendorph  (1000) callendorph  (1000)      760 2023-07-15 04:37:49.000000 lbstanza-wrappers-0.2.1/dump-c-header.py
-drwxrwxr-x   0 callendorph  (1000) callendorph  (1000)        0 2023-07-15 04:45:56.290342 lbstanza-wrappers-0.2.1/lbstanza_wrappers.egg-info/
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)     2586 2023-07-15 04:45:56.000000 lbstanza-wrappers-0.2.1/lbstanza_wrappers.egg-info/PKG-INFO
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)      265 2023-07-15 04:45:56.000000 lbstanza-wrappers-0.2.1/lbstanza_wrappers.egg-info/SOURCES.txt
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)        1 2023-07-15 04:45:56.000000 lbstanza-wrappers-0.2.1/lbstanza_wrappers.egg-info/dependency_links.txt
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)       40 2023-07-15 04:45:56.000000 lbstanza-wrappers-0.2.1/lbstanza_wrappers.egg-info/requires.txt
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)        1 2023-07-15 04:45:56.000000 lbstanza-wrappers-0.2.1/lbstanza_wrappers.egg-info/top_level.txt
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)       38 2023-07-15 04:45:56.290342 lbstanza-wrappers-0.2.1/setup.cfg
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)      690 2023-07-15 04:45:38.000000 lbstanza-wrappers-0.2.1/setup.py
+drwxrwxr-x   0 callendorph  (1000) callendorph  (1000)        0 2023-07-15 04:50:43.996196 lbstanza-wrappers-0.2.2/
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)    35149 2023-07-15 04:37:49.000000 lbstanza-wrappers-0.2.2/LICENSE
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)     2586 2023-07-15 04:50:43.996196 lbstanza-wrappers-0.2.2/PKG-INFO
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)     2232 2023-07-15 04:37:49.000000 lbstanza-wrappers-0.2.2/README.md
+-rwxrwxr-x   0 callendorph  (1000) callendorph  (1000)    30594 2023-07-15 04:45:38.000000 lbstanza-wrappers-0.2.2/convert2stanza.py
+-rwxrwxr-x   0 callendorph  (1000) callendorph  (1000)      760 2023-07-15 04:37:49.000000 lbstanza-wrappers-0.2.2/dump-c-header.py
+drwxrwxr-x   0 callendorph  (1000) callendorph  (1000)        0 2023-07-15 04:50:43.996196 lbstanza-wrappers-0.2.2/lbstanza_wrappers.egg-info/
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)     2586 2023-07-15 04:50:43.000000 lbstanza-wrappers-0.2.2/lbstanza_wrappers.egg-info/PKG-INFO
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)      265 2023-07-15 04:50:43.000000 lbstanza-wrappers-0.2.2/lbstanza_wrappers.egg-info/SOURCES.txt
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)        1 2023-07-15 04:50:43.000000 lbstanza-wrappers-0.2.2/lbstanza_wrappers.egg-info/dependency_links.txt
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)       40 2023-07-15 04:50:43.000000 lbstanza-wrappers-0.2.2/lbstanza_wrappers.egg-info/requires.txt
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)        1 2023-07-15 04:50:43.000000 lbstanza-wrappers-0.2.2/lbstanza_wrappers.egg-info/top_level.txt
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)       38 2023-07-15 04:50:43.996196 lbstanza-wrappers-0.2.2/setup.cfg
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)      737 2023-07-15 04:49:44.000000 lbstanza-wrappers-0.2.2/setup.py
```

### Comparing `lbstanza-wrappers-0.2.1/LICENSE` & `lbstanza-wrappers-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lbstanza-wrappers-0.2.1/PKG-INFO` & `lbstanza-wrappers-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbstanza-wrappers
-Version: 0.2.1
+Version: 0.2.2
 Summary: Utility to create lbstanza wrappers from C headers
 Home-page: https://github.com/callendorph/lbstanza-wrappers
 Author: Carl Allendorph
 License: GPLv3
 Keywords: lbstanza wrappers utility
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lbstanza-wrappers-0.2.1/README.md` & `lbstanza-wrappers-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `lbstanza-wrappers-0.2.1/convert2stanza.py` & `lbstanza-wrappers-0.2.2/convert2stanza.py`

 * *Files identical despite different names*

### Comparing `lbstanza-wrappers-0.2.1/dump-c-header.py` & `lbstanza-wrappers-0.2.2/dump-c-header.py`

 * *Files identical despite different names*

### Comparing `lbstanza-wrappers-0.2.1/lbstanza_wrappers.egg-info/PKG-INFO` & `lbstanza-wrappers-0.2.2/lbstanza_wrappers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbstanza-wrappers
-Version: 0.2.1
+Version: 0.2.2
 Summary: Utility to create lbstanza wrappers from C headers
 Home-page: https://github.com/callendorph/lbstanza-wrappers
 Author: Carl Allendorph
 License: GPLv3
 Keywords: lbstanza wrappers utility
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lbstanza-wrappers-0.2.1/setup.py` & `lbstanza-wrappers-0.2.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os
 from setuptools import setup
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 def read(fname):
-	return open(os.path.join(os.path.dirname(__file__), fname)).read()
+	try:
+		return open(os.path.join(os.path.dirname(__file__), fname)).read()
+	except:
+		return "No Long Description"
 
 setup(
 	name="lbstanza-wrappers",
 	version=__version__,
 	description="Utility to create lbstanza wrappers from C headers",
 	long_description=read("long_description.rst"),
 	license="GPLv3",
```

