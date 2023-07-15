# Comparing `tmp/muse-maskgit-pytorch-0.2.0.tar.gz` & `tmp/muse-maskgit-pytorch-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muse-maskgit-pytorch-0.2.0.tar", last modified: Sat Jul 15 17:04:51 2023, max compression
+gzip compressed data, was "muse-maskgit-pytorch-0.2.1.tar", last modified: Sat Jul 15 17:05:38 2023, max compression
```

## Comparing `muse-maskgit-pytorch-0.2.0.tar` & `muse-maskgit-pytorch-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:04:51.220769 muse-maskgit-pytorch-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-15 17:04:39.000000 muse-maskgit-pytorch-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-15 17:04:51.220769 muse-maskgit-pytorch-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-15 17:04:39.000000 muse-maskgit-pytorch-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:04:51.220769 muse-maskgit-pytorch-0.2.0/muse_maskgit_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-15 17:04:39.000000 muse-maskgit-pytorch-0.2.0/muse_maskgit_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24961 2023-07-15 17:04:39.000000 muse-maskgit-pytorch-0.2.0/muse_maskgit_pytorch/muse_maskgit_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-15 17:04:39.000000 muse-maskgit-pytorch-0.2.0/muse_maskgit_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)    12012 2023-07-15 17:04:39.000000 muse-maskgit-pytorch-0.2.0/muse_maskgit_pytorch/trainers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-07-15 17:04:39.000000 muse-maskgit-pytorch-0.2.0/muse_maskgit_pytorch/vqgan_vae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:04:51.220769 muse-maskgit-pytorch-0.2.0/muse_maskgit_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-15 17:04:51.000000 muse-maskgit-pytorch-0.2.0/muse_maskgit_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-15 17:04:51.000000 muse-maskgit-pytorch-0.2.0/muse_maskgit_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 17:04:51.000000 muse-maskgit-pytorch-0.2.0/muse_maskgit_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-15 17:04:51.000000 muse-maskgit-pytorch-0.2.0/muse_maskgit_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-15 17:04:51.000000 muse-maskgit-pytorch-0.2.0/muse_maskgit_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 17:04:51.220769 muse-maskgit-pytorch-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-15 17:04:39.000000 muse-maskgit-pytorch-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:05:38.934267 muse-maskgit-pytorch-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-15 17:05:26.000000 muse-maskgit-pytorch-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-15 17:05:38.934267 muse-maskgit-pytorch-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-15 17:05:26.000000 muse-maskgit-pytorch-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:05:38.934267 muse-maskgit-pytorch-0.2.1/muse_maskgit_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-15 17:05:26.000000 muse-maskgit-pytorch-0.2.1/muse_maskgit_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-15 17:05:26.000000 muse-maskgit-pytorch-0.2.1/muse_maskgit_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24961 2023-07-15 17:05:26.000000 muse-maskgit-pytorch-0.2.1/muse_maskgit_pytorch/muse_maskgit_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-15 17:05:26.000000 muse-maskgit-pytorch-0.2.1/muse_maskgit_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12012 2023-07-15 17:05:26.000000 muse-maskgit-pytorch-0.2.1/muse_maskgit_pytorch/trainers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-07-15 17:05:26.000000 muse-maskgit-pytorch-0.2.1/muse_maskgit_pytorch/vqgan_vae.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:05:38.934267 muse-maskgit-pytorch-0.2.1/muse_maskgit_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-15 17:05:38.000000 muse-maskgit-pytorch-0.2.1/muse_maskgit_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-15 17:05:38.000000 muse-maskgit-pytorch-0.2.1/muse_maskgit_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 17:05:38.000000 muse-maskgit-pytorch-0.2.1/muse_maskgit_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-15 17:05:38.000000 muse-maskgit-pytorch-0.2.1/muse_maskgit_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-15 17:05:38.000000 muse-maskgit-pytorch-0.2.1/muse_maskgit_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 17:05:38.934267 muse-maskgit-pytorch-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-15 17:05:26.000000 muse-maskgit-pytorch-0.2.1/setup.py
```

### Comparing `muse-maskgit-pytorch-0.2.0/LICENSE` & `muse-maskgit-pytorch-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `muse-maskgit-pytorch-0.2.0/PKG-INFO` & `muse-maskgit-pytorch-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muse-maskgit-pytorch
-Version: 0.2.0
+Version: 0.2.1
 Summary: MUSE - Text-to-Image Generation via Masked Generative Transformers, in Pytorch
 Home-page: https://github.com/lucidrains/muse-maskgit-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-image
 Classifier: Development Status :: 4 - Beta
```

### Comparing `muse-maskgit-pytorch-0.2.0/README.md` & `muse-maskgit-pytorch-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `muse-maskgit-pytorch-0.2.0/muse_maskgit_pytorch/muse_maskgit_pytorch.py` & `muse-maskgit-pytorch-0.2.1/muse_maskgit_pytorch/muse_maskgit_pytorch.py`

 * *Files identical despite different names*

### Comparing `muse-maskgit-pytorch-0.2.0/muse_maskgit_pytorch/t5.py` & `muse-maskgit-pytorch-0.2.1/muse_maskgit_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `muse-maskgit-pytorch-0.2.0/muse_maskgit_pytorch/trainers.py` & `muse-maskgit-pytorch-0.2.1/muse_maskgit_pytorch/trainers.py`

 * *Files identical despite different names*

### Comparing `muse-maskgit-pytorch-0.2.0/muse_maskgit_pytorch/vqgan_vae.py` & `muse-maskgit-pytorch-0.2.1/muse_maskgit_pytorch/vqgan_vae.py`

 * *Files identical despite different names*

### Comparing `muse-maskgit-pytorch-0.2.0/muse_maskgit_pytorch.egg-info/PKG-INFO` & `muse-maskgit-pytorch-0.2.1/muse_maskgit_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muse-maskgit-pytorch
-Version: 0.2.0
+Version: 0.2.1
 Summary: MUSE - Text-to-Image Generation via Masked Generative Transformers, in Pytorch
 Home-page: https://github.com/lucidrains/muse-maskgit-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-image
 Classifier: Development Status :: 4 - Beta
```

### Comparing `muse-maskgit-pytorch-0.2.0/setup.py` & `muse-maskgit-pytorch-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'muse-maskgit-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.2.0',
+  version = '0.2.1',
   license='MIT',
   description = 'MUSE - Text-to-Image Generation via Masked Generative Transformers, in Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/muse-maskgit-pytorch',
   keywords = [
```

