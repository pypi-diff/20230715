# Comparing `tmp/toodaloo-0.0.2.tar.gz` & `tmp/toodaloo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toodaloo-0.0.2.tar", last modified: Mon Jul 10 14:17:02 2023, max compression
+gzip compressed data, was "toodaloo-0.0.3.tar", last modified: Sat Jul 15 10:22:46 2023, max compression
```

## Comparing `toodaloo-0.0.2.tar` & `toodaloo-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 thibault   (501) staff       (20)        0 2023-07-10 14:17:02.877569 toodaloo-0.0.2/
--rw-r--r--   0 thibault   (501) staff       (20)     1081 2023-07-10 14:02:37.000000 toodaloo-0.0.2/LICENSE
--rw-r--r--   0 thibault   (501) staff       (20)      618 2023-07-10 14:17:02.877451 toodaloo-0.0.2/PKG-INFO
--rw-r--r--   0 thibault   (501) staff       (20)       38 2023-07-10 14:17:02.877609 toodaloo-0.0.2/setup.cfg
--rw-r--r--   0 thibault   (501) staff       (20)      752 2023-07-10 14:15:23.000000 toodaloo-0.0.2/setup.py
-drwxr-xr-x   0 thibault   (501) staff       (20)        0 2023-07-10 14:17:02.876671 toodaloo-0.0.2/src/
-drwxr-xr-x   0 thibault   (501) staff       (20)        0 2023-07-10 14:17:02.877267 toodaloo-0.0.2/src/toodaloo.egg-info/
--rw-r--r--   0 thibault   (501) staff       (20)      618 2023-07-10 14:17:02.000000 toodaloo-0.0.2/src/toodaloo.egg-info/PKG-INFO
--rw-r--r--   0 thibault   (501) staff       (20)      176 2023-07-10 14:17:02.000000 toodaloo-0.0.2/src/toodaloo.egg-info/SOURCES.txt
--rw-r--r--   0 thibault   (501) staff       (20)        1 2023-07-10 14:17:02.000000 toodaloo-0.0.2/src/toodaloo.egg-info/dependency_links.txt
--rw-r--r--   0 thibault   (501) staff       (20)        9 2023-07-10 14:17:02.000000 toodaloo-0.0.2/src/toodaloo.egg-info/top_level.txt
--rw-r--r--   0 thibault   (501) staff       (20)     1048 2023-07-10 14:15:23.000000 toodaloo-0.0.2/src/toodaloo.py
+drwxr-xr-x   0 thibault   (501) staff       (20)        0 2023-07-15 10:22:46.122418 toodaloo-0.0.3/
+-rw-r--r--   0 thibault   (501) staff       (20)     1081 2023-07-15 10:09:33.000000 toodaloo-0.0.3/LICENSE
+-rw-r--r--   0 thibault   (501) staff       (20)      567 2023-07-15 10:22:46.122303 toodaloo-0.0.3/PKG-INFO
+-rw-r--r--   0 thibault   (501) staff       (20)       38 2023-07-15 10:22:46.122456 toodaloo-0.0.3/setup.cfg
+-rw-r--r--   0 thibault   (501) staff       (20)      701 2023-07-15 10:21:52.000000 toodaloo-0.0.3/setup.py
+drwxr-xr-x   0 thibault   (501) staff       (20)        0 2023-07-15 10:22:46.121642 toodaloo-0.0.3/src/
+drwxr-xr-x   0 thibault   (501) staff       (20)        0 2023-07-15 10:22:46.122133 toodaloo-0.0.3/src/toodaloo.egg-info/
+-rw-r--r--   0 thibault   (501) staff       (20)      567 2023-07-15 10:22:46.000000 toodaloo-0.0.3/src/toodaloo.egg-info/PKG-INFO
+-rw-r--r--   0 thibault   (501) staff       (20)      176 2023-07-15 10:22:46.000000 toodaloo-0.0.3/src/toodaloo.egg-info/SOURCES.txt
+-rw-r--r--   0 thibault   (501) staff       (20)        1 2023-07-15 10:22:46.000000 toodaloo-0.0.3/src/toodaloo.egg-info/dependency_links.txt
+-rw-r--r--   0 thibault   (501) staff       (20)        9 2023-07-15 10:22:46.000000 toodaloo-0.0.3/src/toodaloo.egg-info/top_level.txt
+-rw-r--r--   0 thibault   (501) staff       (20)     1354 2023-07-15 10:22:37.000000 toodaloo-0.0.3/src/toodaloo.py
```

### Comparing `toodaloo-0.0.2/LICENSE` & `toodaloo-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `toodaloo-0.0.2/PKG-INFO` & `toodaloo-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: toodaloo
-Version: 0.0.2
-Summary: Toodaloo Library
-Home-page: https://github.com/Thibault00/toodetest
+Version: 0.0.3
+Summary: requesty Library
 Author: Thibault Jaigu
 Author-email: thibault.jaigu@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `toodaloo-0.0.2/setup.py` & `toodaloo-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from setuptools import setup
 
 setup(
     name='toodaloo',
-    version='0.0.2',
+    version='0.0.3',
     author='Thibault Jaigu',
     author_email='thibault.jaigu@gmail.com',
-    description='Toodaloo Library',
+    description='requesty Library',
     py_modules=["toodaloo"],
     package_dir={'': 'src'},
     long_description='The best boefies library in the world',
-    url='https://github.com/Thibault00/toodetest',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

### Comparing `toodaloo-0.0.2/src/toodaloo.egg-info/PKG-INFO` & `toodaloo-0.0.3/src/toodaloo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: toodaloo
-Version: 0.0.2
-Summary: Toodaloo Library
-Home-page: https://github.com/Thibault00/toodetest
+Version: 0.0.3
+Summary: requesty Library
 Author: Thibault Jaigu
 Author-email: thibault.jaigu@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

