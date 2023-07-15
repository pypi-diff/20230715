# Comparing `tmp/dxlib-0.1.1.tar.gz` & `tmp/dxlib-0.1.209.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxlib-0.1.1.tar", last modified: Thu Apr 20 14:52:20 2023, max compression
+gzip compressed data, was "dxlib-0.1.209.tar", last modified: Sat Jul 15 06:55:37 2023, max compression
```

## Comparing `dxlib-0.1.1.tar` & `dxlib-0.1.209.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-04-20 14:53:44.377639 dxlib-0.1.1/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1262 2023-04-20 14:53:44.377639 dxlib-0.1.1/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      526 2023-04-20 14:34:27.000000 dxlib-0.1.1/README.md
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-04-20 14:53:44.205763 dxlib-0.1.1/dxlib/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      102 2023-04-20 14:41:28.000000 dxlib-0.1.1/dxlib/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      404 2023-04-20 14:41:16.000000 dxlib-0.1.1/dxlib/euler_method.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      274 2023-04-20 14:39:35.000000 dxlib-0.1.1/dxlib/finite_differences.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-04-20 14:53:44.346383 dxlib-0.1.1/dxlib.egg-info/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1262 2023-04-20 14:53:43.000000 dxlib-0.1.1/dxlib.egg-info/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      230 2023-04-20 14:53:44.000000 dxlib-0.1.1/dxlib.egg-info/SOURCES.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-04-20 14:53:43.000000 dxlib-0.1.1/dxlib.egg-info/dependency_links.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       17 2023-04-20 14:53:43.000000 dxlib-0.1.1/dxlib.egg-info/requires.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-04-20 14:53:43.000000 dxlib-0.1.1/dxlib.egg-info/top_level.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-04-20 14:53:44.377639 dxlib-0.1.1/setup.cfg
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1400 2023-04-20 14:52:57.000000 dxlib-0.1.1/setup.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 06:55:37.373043 dxlib-0.1.209/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1264 2023-07-15 06:55:37.369042 dxlib-0.1.209/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      526 2023-04-20 14:34:27.000000 dxlib-0.1.209/README.md
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 06:55:37.218274 dxlib-0.1.209/dxlib.egg-info/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1264 2023-07-15 06:55:36.000000 dxlib-0.1.209/dxlib.egg-info/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      235 2023-07-15 06:55:37.000000 dxlib-0.1.209/dxlib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-07-15 06:55:36.000000 dxlib-0.1.209/dxlib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      119 2023-07-15 06:55:36.000000 dxlib-0.1.209/dxlib.egg-info/requires.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        4 2023-07-15 06:55:36.000000 dxlib-0.1.209/dxlib.egg-info/top_level.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-07-15 06:55:37.374043 dxlib-0.1.209/setup.cfg
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1305 2023-07-15 06:14:29.000000 dxlib-0.1.209/setup.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 06:55:37.336035 dxlib-0.1.209/src/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       12 2023-07-15 06:53:11.000000 dxlib-0.1.209/src/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1448 2023-07-14 03:22:23.000000 dxlib-0.1.209/src/app.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      404 2023-04-20 14:41:16.000000 dxlib-0.1.209/src/euler_method.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      274 2023-04-20 14:39:35.000000 dxlib-0.1.209/src/finite_differences.py
```

### Comparing `dxlib-0.1.1/PKG-INFO` & `dxlib-0.1.209/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxlib
-Version: 0.1.1
+Version: 0.1.209
 Summary: Quantitative Methods for Finance
 Home-page: https://github.com/delphos-quant/dxlib
 Author: Rafael Zimmer
 Author-email: rzimmerde@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dxlib-0.1.1/README.md` & `dxlib-0.1.209/README.md`

 * *Files identical despite different names*

### Comparing `dxlib-0.1.1/dxlib.egg-info/PKG-INFO` & `dxlib-0.1.209/dxlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxlib
-Version: 0.1.1
+Version: 0.1.209
 Summary: Quantitative Methods for Finance
 Home-page: https://github.com/delphos-quant/dxlib
 Author: Rafael Zimmer
 Author-email: rzimmerde@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dxlib-0.1.1/setup.py` & `dxlib-0.1.209/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# Always prefer setuptools over distutils
-from setuptools import setup, find_packages
-
-# To use a consistent encoding
-from codecs import open
+import os
 from os import path
+from setuptools import setup
+from codecs import open
 
-# The directory containing this file
 HERE = path.abspath(path.dirname(__file__))
 
-# Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
-# This call to self.setup() does all the work
+with open('requirements.txt') as f:
+    requirements = f.read().splitlines()
+
+version = os.getenv("DXLIB_VERSION", "0.1.0")
+
 setup(
     name="dxlib",
-    version="0.1.1",
+    version=version,
     description="Quantitative Methods for Finance",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/delphos-quant/dxlib",
     author="Rafael Zimmer",
     author_email="rzimmerde@gmail.com",
     license="MIT",
@@ -31,11 +31,11 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent"
     ],
-    packages=["dxlib"],
+    packages=['src'],
     include_package_data=True,
-    install_requires=["numpy", "matplotlib"]
-)
+    install_requires=requirements,
+)
```

