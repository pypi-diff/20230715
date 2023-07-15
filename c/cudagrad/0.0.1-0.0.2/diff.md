# Comparing `tmp/cudagrad-0.0.1.tar.gz` & `tmp/cudagrad-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cudagrad-0.0.1.tar", last modified: Sat Jul 15 19:04:44 2023, max compression
+gzip compressed data, was "cudagrad-0.0.2.tar", last modified: Sat Jul 15 20:18:47 2023, max compression
```

## Comparing `cudagrad-0.0.1.tar` & `cudagrad-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-15 19:04:44.021302 cudagrad-0.0.1/
--rw-r--r--   0 ryan       (501) staff       (20)     2182 2023-07-15 18:25:47.000000 cudagrad-0.0.1/LICENSE
--rw-r--r--   0 ryan       (501) staff       (20)     3699 2023-07-15 19:04:44.021189 cudagrad-0.0.1/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     3171 2023-07-15 18:25:47.000000 cudagrad-0.0.1/README.md
--rw-r--r--   0 ryan       (501) staff       (20)      732 2023-07-15 19:00:24.000000 cudagrad-0.0.1/pyproject.toml
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-15 19:04:44.021337 cudagrad-0.0.1/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     1300 2023-07-15 19:00:40.000000 cudagrad-0.0.1/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-15 19:04:44.019939 cudagrad-0.0.1/src/
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-15 19:04:44.020852 cudagrad-0.0.1/src/cudagrad.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     3699 2023-07-15 19:04:44.000000 cudagrad-0.0.1/src/cudagrad.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      282 2023-07-15 19:04:44.000000 cudagrad-0.0.1/src/cudagrad.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-15 19:04:44.000000 cudagrad-0.0.1/src/cudagrad.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-15 18:58:31.000000 cudagrad-0.0.1/src/cudagrad.egg-info/not-zip-safe
--rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-15 19:04:44.000000 cudagrad-0.0.1/src/cudagrad.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-15 19:04:44.000000 cudagrad-0.0.1/src/cudagrad.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)      858 2023-07-15 18:31:47.000000 cudagrad-0.0.1/src/main.cpp
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-15 19:04:44.020967 cudagrad-0.0.1/tests/
--rw-r--r--   0 ryan       (501) staff       (20)      108 2023-07-15 18:31:48.000000 cudagrad-0.0.1/tests/test.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-15 20:18:47.828782 cudagrad-0.0.2/
+-rw-r--r--   0 ryan       (501) staff       (20)     3481 2023-07-15 20:18:47.828668 cudagrad-0.0.2/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     2980 2023-07-15 19:49:48.000000 cudagrad-0.0.2/README.md
+-rw-r--r--   0 ryan       (501) staff       (20)      732 2023-07-15 20:15:50.000000 cudagrad-0.0.2/pyproject.toml
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-15 20:18:47.828816 cudagrad-0.0.2/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     1285 2023-07-15 20:18:01.000000 cudagrad-0.0.2/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-15 20:18:47.827340 cudagrad-0.0.2/src/
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-15 20:18:47.828213 cudagrad-0.0.2/src/cudagrad.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3481 2023-07-15 20:18:47.000000 cudagrad-0.0.2/src/cudagrad.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      274 2023-07-15 20:18:47.000000 cudagrad-0.0.2/src/cudagrad.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-15 20:18:47.000000 cudagrad-0.0.2/src/cudagrad.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-15 20:18:22.000000 cudagrad-0.0.2/src/cudagrad.egg-info/not-zip-safe
+-rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-15 20:18:47.000000 cudagrad-0.0.2/src/cudagrad.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-15 20:18:47.000000 cudagrad-0.0.2/src/cudagrad.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)      858 2023-07-15 18:31:47.000000 cudagrad-0.0.2/src/main.cpp
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-15 20:18:47.828315 cudagrad-0.0.2/tests/
+-rw-r--r--   0 ryan       (501) staff       (20)      108 2023-07-15 20:14:26.000000 cudagrad-0.0.2/tests/test.py
```

### Comparing `cudagrad-0.0.1/pyproject.toml` & `cudagrad-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel", "pybind11>=2.10.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cudagrad"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Ryan Moore", email="moorethreads@hey.com" },
 ]
 description = "A small autograd engine"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cudagrad-0.0.1/setup.py` & `cudagrad-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Available at setup time due to pyproject.toml
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 # The main interface is through Pybind11Extension.
 # * You can add cxx_std=11/14/17, and then build_ext can be removed.
 # * You can set include_pybind11=false to add the include directory yourself,
 #   say from a submodule.
 #
 # Note:
@@ -20,18 +20,18 @@
         define_macros = [('VERSION_INFO', __version__)],
         ),
 ]
 
 setup(
     name="cudagrad",
     version=__version__,
-    author="Sylvain Corlay",
-    author_email="sylvain.corlay@gmail.com",
-    url="https://github.com/pybind/cudagrad",
-    description="A test project using pybind11",
+    author="Ryan Moore",
+    author_email="moorethreads@hey.com",
+    url="https://github.com/yrom1/cudagrad",
+    description="A small autograd engine",
     long_description="",
     ext_modules=ext_modules,
     extras_require={"test": "pytest"},
     # Currently, build_ext only provides an optional "highest supported C++
     # level" feature, but in the future it may provide more features.
     cmdclass={"build_ext": build_ext},
     zip_safe=False,
```

### Comparing `cudagrad-0.0.1/src/main.cpp` & `cudagrad-0.0.2/src/main.cpp`

 * *Files identical despite different names*

