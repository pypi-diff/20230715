# Comparing `tmp/easytester-0.1.tar.gz` & `tmp/easytester-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytester-0.1.tar", last modified: Sat Jul 15 03:46:48 2023, max compression
+gzip compressed data, was "easytester-0.2.tar", last modified: Sat Jul 15 11:46:49 2023, max compression
```

## Comparing `easytester-0.1.tar` & `easytester-0.2.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxr-x   0 ham       (1000) ham       (1000)        0 2023-07-15 03:46:48.049142 easytester-0.1/
--rw-rw-r--   0 ham       (1000) ham       (1000)     6427 2023-07-15 03:46:48.049142 easytester-0.1/PKG-INFO
--rw-rw-r--   0 ham       (1000) ham       (1000)     5933 2023-07-14 22:26:00.000000 easytester-0.1/README.md
-drwxrwxr-x   0 ham       (1000) ham       (1000)        0 2023-07-15 03:46:48.049142 easytester-0.1/easytester.egg-info/
--rw-rw-r--   0 ham       (1000) ham       (1000)     6427 2023-07-15 03:46:47.000000 easytester-0.1/easytester.egg-info/PKG-INFO
--rw-rw-r--   0 ham       (1000) ham       (1000)      187 2023-07-15 03:46:47.000000 easytester-0.1/easytester.egg-info/SOURCES.txt
--rw-rw-r--   0 ham       (1000) ham       (1000)        1 2023-07-15 03:46:47.000000 easytester-0.1/easytester.egg-info/dependency_links.txt
--rw-rw-r--   0 ham       (1000) ham       (1000)       44 2023-07-15 03:46:47.000000 easytester-0.1/easytester.egg-info/requires.txt
--rw-rw-r--   0 ham       (1000) ham       (1000)        1 2023-07-15 03:46:47.000000 easytester-0.1/easytester.egg-info/top_level.txt
--rw-rw-r--   0 ham       (1000) ham       (1000)       38 2023-07-15 03:46:48.049142 easytester-0.1/setup.cfg
--rw-rw-r--   0 ham       (1000) ham       (1000)      744 2023-07-15 03:28:33.000000 easytester-0.1/setup.py
+drwxrwxr-x   0 ham       (1000) ham       (1000)        0 2023-07-15 11:46:49.441429 easytester-0.2/
+-rw-rw-r--   0 ham       (1000) ham       (1000)     6427 2023-07-15 11:46:49.441429 easytester-0.2/PKG-INFO
+-rw-rw-r--   0 ham       (1000) ham       (1000)     5933 2023-07-15 11:22:52.000000 easytester-0.2/README.md
+drwxrwxr-x   0 ham       (1000) ham       (1000)        0 2023-07-15 11:46:49.441429 easytester-0.2/easytester/
+-rw-rw-r--   0 ham       (1000) ham       (1000)        0 2023-07-15 11:24:56.000000 easytester-0.2/easytester/__init__.py
+-rw-rw-r--   0 ham       (1000) ham       (1000)     2342 2023-07-15 11:22:57.000000 easytester-0.2/easytester/move.py
+-rw-rw-r--   0 ham       (1000) ham       (1000)     2102 2023-07-15 11:22:40.000000 easytester-0.2/easytester/utils.py
+drwxrwxr-x   0 ham       (1000) ham       (1000)        0 2023-07-15 11:46:49.441429 easytester-0.2/easytester.egg-info/
+-rw-rw-r--   0 ham       (1000) ham       (1000)     6427 2023-07-15 11:46:49.000000 easytester-0.2/easytester.egg-info/PKG-INFO
+-rw-rw-r--   0 ham       (1000) ham       (1000)      249 2023-07-15 11:46:49.000000 easytester-0.2/easytester.egg-info/SOURCES.txt
+-rw-rw-r--   0 ham       (1000) ham       (1000)        1 2023-07-15 11:46:49.000000 easytester-0.2/easytester.egg-info/dependency_links.txt
+-rw-rw-r--   0 ham       (1000) ham       (1000)       44 2023-07-15 11:46:49.000000 easytester-0.2/easytester.egg-info/requires.txt
+-rw-rw-r--   0 ham       (1000) ham       (1000)       11 2023-07-15 11:46:49.000000 easytester-0.2/easytester.egg-info/top_level.txt
+-rw-rw-r--   0 ham       (1000) ham       (1000)       38 2023-07-15 11:46:49.441429 easytester-0.2/setup.cfg
+-rw-rw-r--   0 ham       (1000) ham       (1000)      744 2023-07-15 11:46:39.000000 easytester-0.2/setup.py
```

### Comparing `easytester-0.1/PKG-INFO` & `easytester-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytester
-Version: 0.1
+Version: 0.2
 Summary: A simple and easy-to-use testing library for web and mobile applications
 Home-page: https://github.com/Hamsterrrrr/EasyTest
 Author: hamsterrrrr
 Author-email: radzabovibragim80@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easytester-0.1/README.md` & `easytester-0.2/README.md`

 * *Files identical despite different names*

### Comparing `easytester-0.1/easytester.egg-info/PKG-INFO` & `easytester-0.2/easytester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytester
-Version: 0.1
+Version: 0.2
 Summary: A simple and easy-to-use testing library for web and mobile applications
 Home-page: https://github.com/Hamsterrrrr/EasyTest
 Author: hamsterrrrr
 Author-email: radzabovibragim80@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easytester-0.1/setup.py` & `easytester-0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='easytester',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     description='A simple and easy-to-use testing library for web and mobile applications',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='hamsterrrrr',
     author_email='radzabovibragim80@gmail.com',
     url='https://github.com/Hamsterrrrr/EasyTest',
```

