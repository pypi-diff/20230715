# Comparing `tmp/tailwindpie-0.1.0.tar.gz` & `tmp/tailwindpie-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailwindpie-0.1.0.tar", last modified: Sat Jul 15 12:02:15 2023, max compression
+gzip compressed data, was "tailwindpie-0.1.1.tar", last modified: Sat Jul 15 12:51:36 2023, max compression
```

## Comparing `tailwindpie-0.1.0.tar` & `tailwindpie-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 yaqeen    (1000) yaqeen    (1000)        0 2023-07-15 12:02:15.484860 tailwindpie-0.1.0/
--rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)     1320 2023-06-23 10:16:48.000000 tailwindpie-0.1.0/LICENSE
--rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)      605 2023-07-15 12:02:15.484860 tailwindpie-0.1.0/PKG-INFO
--rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)     1783 2023-07-14 09:45:41.000000 tailwindpie-0.1.0/README.md
--rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)       38 2023-07-15 12:02:15.484860 tailwindpie-0.1.0/setup.cfg
--rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)      832 2023-07-15 11:55:55.000000 tailwindpie-0.1.0/setup.py
-drwxr-xr-x   0 yaqeen    (1000) yaqeen    (1000)        0 2023-07-15 12:02:15.481860 tailwindpie-0.1.0/tailwindpie/
--rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)       88 2023-07-15 11:01:50.000000 tailwindpie-0.1.0/tailwindpie/__init__.py
--rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)     1277 2023-07-15 11:11:50.000000 tailwindpie-0.1.0/tailwindpie/__main__.py
--rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)     4747 2023-07-15 12:02:09.000000 tailwindpie-0.1.0/tailwindpie/main.py
-drwxr-xr-x   0 yaqeen    (1000) yaqeen    (1000)        0 2023-07-15 12:02:15.483860 tailwindpie-0.1.0/tailwindpie.egg-info/
--rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)      605 2023-07-15 12:02:15.000000 tailwindpie-0.1.0/tailwindpie.egg-info/PKG-INFO
--rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)      306 2023-07-15 12:02:15.000000 tailwindpie-0.1.0/tailwindpie.egg-info/SOURCES.txt
--rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)        1 2023-07-15 12:02:15.000000 tailwindpie-0.1.0/tailwindpie.egg-info/dependency_links.txt
--rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)       50 2023-07-15 12:02:15.000000 tailwindpie-0.1.0/tailwindpie.egg-info/entry_points.txt
--rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)        5 2023-07-15 12:02:15.000000 tailwindpie-0.1.0/tailwindpie.egg-info/requires.txt
--rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)       12 2023-07-15 12:02:15.000000 tailwindpie-0.1.0/tailwindpie.egg-info/top_level.txt
+drwxr-xr-x   0 yaqeen    (1000) yaqeen    (1000)        0 2023-07-15 12:51:36.977079 tailwindpie-0.1.1/
+-rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)     1320 2023-06-23 10:16:48.000000 tailwindpie-0.1.1/LICENSE
+-rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)      609 2023-07-15 12:51:36.974079 tailwindpie-0.1.1/PKG-INFO
+-rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)     1783 2023-07-14 09:45:41.000000 tailwindpie-0.1.1/README.md
+-rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)       38 2023-07-15 12:51:36.977079 tailwindpie-0.1.1/setup.cfg
+-rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)      836 2023-07-15 12:51:25.000000 tailwindpie-0.1.1/setup.py
+drwxr-xr-x   0 yaqeen    (1000) yaqeen    (1000)        0 2023-07-15 12:51:36.972079 tailwindpie-0.1.1/tailwindpie/
+-rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)       88 2023-07-15 11:01:50.000000 tailwindpie-0.1.1/tailwindpie/__init__.py
+-rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)     1277 2023-07-15 11:11:50.000000 tailwindpie-0.1.1/tailwindpie/__main__.py
+-rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)     4747 2023-07-15 12:02:09.000000 tailwindpie-0.1.1/tailwindpie/main.py
+drwxr-xr-x   0 yaqeen    (1000) yaqeen    (1000)        0 2023-07-15 12:51:36.974079 tailwindpie-0.1.1/tailwindpie.egg-info/
+-rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)      609 2023-07-15 12:51:36.000000 tailwindpie-0.1.1/tailwindpie.egg-info/PKG-INFO
+-rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)      306 2023-07-15 12:51:36.000000 tailwindpie-0.1.1/tailwindpie.egg-info/SOURCES.txt
+-rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)        1 2023-07-15 12:51:36.000000 tailwindpie-0.1.1/tailwindpie.egg-info/dependency_links.txt
+-rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)       50 2023-07-15 12:51:36.000000 tailwindpie-0.1.1/tailwindpie.egg-info/entry_points.txt
+-rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)        5 2023-07-15 12:51:36.000000 tailwindpie-0.1.1/tailwindpie.egg-info/requires.txt
+-rw-r--r--   0 yaqeen    (1000) yaqeen    (1000)       12 2023-07-15 12:51:36.000000 tailwindpie-0.1.1/tailwindpie.egg-info/top_level.txt
```

### Comparing `tailwindpie-0.1.0/LICENSE` & `tailwindpie-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tailwindpie-0.1.0/PKG-INFO` & `tailwindpie-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tailwindpie
-Version: 0.1.0
+Version: 0.1.1
 Summary: easiest way to configure tailwind in python
-Home-page: https://github.com/Abdulmumin1/xologic
+Home-page: https://github.com/Abdulmumin1/tailwindpie
 Author: Abdulmumin Abdulkarim
 Author-email: avdorr12345@gmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `tailwindpie-0.1.0/README.md` & `tailwindpie-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tailwindpie-0.1.0/setup.py` & `tailwindpie-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name='tailwindpie',
-    version='0.1.0',
+    version='0.1.1',
     description='easiest way to configure tailwind in python',
-    url='https://github.com/Abdulmumin1/xologic',
+    url='https://github.com/Abdulmumin1/tailwindpie',
     author='Abdulmumin Abdulkarim',
     author_email='avdorr12345@gmail.com',
     license='BSD 2-clause',
     packages=['tailwindpie'],
     install_requires=['rich'],
     entry_points={
         'console_scripts': [
```

### Comparing `tailwindpie-0.1.0/tailwindpie/__main__.py` & `tailwindpie-0.1.1/tailwindpie/__main__.py`

 * *Files identical despite different names*

### Comparing `tailwindpie-0.1.0/tailwindpie/main.py` & `tailwindpie-0.1.1/tailwindpie/main.py`

 * *Files identical despite different names*

### Comparing `tailwindpie-0.1.0/tailwindpie.egg-info/PKG-INFO` & `tailwindpie-0.1.1/tailwindpie.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: tailwindpie
-Version: 0.1.0
+Version: 0.1.1
 Summary: easiest way to configure tailwind in python
-Home-page: https://github.com/Abdulmumin1/xologic
+Home-page: https://github.com/Abdulmumin1/tailwindpie
 Author: Abdulmumin Abdulkarim
 Author-email: avdorr12345@gmail.com
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
```

