# Comparing `tmp/genomap-1.1.0.tar.gz` & `tmp/genomap-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomap-1.1.0.tar", last modified: Sat Jul 15 00:11:54 2023, max compression
+gzip compressed data, was "genomap-1.1.1.tar", last modified: Sat Jul 15 00:41:23 2023, max compression
```

## Comparing `genomap-1.1.0.tar` & `genomap-1.1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:11:54.434137 genomap-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-15 00:10:00.000000 genomap-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-15 00:10:00.000000 genomap-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-15 00:11:54.434137 genomap-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-15 00:10:00.000000 genomap-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:11:54.430137 genomap-1.1.0/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-15 00:10:00.000000 genomap-1.1.0/data/TM_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:11:54.430137 genomap-1.1.0/genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:11:54.434137 genomap-1.1.0/genomap/bregman_genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/bregman_genomap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/bregman_genomap/bregman_genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:11:54.434137 genomap-1.1.0/genomap/genoMOI/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/genoMOI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/genoMOI/genoMOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:11:54.434137 genomap-1.1.0/genomap/genoTraj/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/genoTraj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/genoTraj/genoTraj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:11:54.434137 genomap-1.1.0/genomap/genoVis/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/genoVis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/genoVis/genoVis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:11:54.434137 genomap-1.1.0/genomap/genomapOPT/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/genomapOPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/genomapOPT/genomapOPT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:11:54.434137 genomap-1.1.0/genomap/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/utils/ConvDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/utils/ConvIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/utils/FcDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/utils/FcIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/utils/class_discriminative_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/utils/gTraj_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/utils/group_centroid_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-15 00:10:00.000000 genomap-1.1.0/genomap/utils/utils_MOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:11:54.434137 genomap-1.1.0/genomap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-15 00:11:54.000000 genomap-1.1.0/genomap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-15 00:11:54.000000 genomap-1.1.0/genomap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 00:11:54.000000 genomap-1.1.0/genomap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-15 00:11:54.000000 genomap-1.1.0/genomap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 00:11:54.000000 genomap-1.1.0/genomap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-15 00:10:00.000000 genomap-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 00:11:54.434137 genomap-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-15 00:10:00.000000 genomap-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.029401 genomap-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-15 00:38:59.000000 genomap-1.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-15 00:38:59.000000 genomap-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-15 00:41:23.029401 genomap-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-15 00:39:00.000000 genomap-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.025400 genomap-1.1.1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-15 00:39:00.000000 genomap-1.1.1/data/TM_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.025400 genomap-1.1.1/genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.025400 genomap-1.1.1/genomap/bregman_genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/bregman_genomap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/bregman_genomap/bregman_genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.025400 genomap-1.1.1/genomap/genoMOI/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/genoMOI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/genoMOI/genoMOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.025400 genomap-1.1.1/genomap/genoTraj/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/genoTraj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/genoTraj/genoTraj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.025400 genomap-1.1.1/genomap/genoVis/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/genoVis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/genoVis/genoVis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.025400 genomap-1.1.1/genomap/genomapOPT/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/genomapOPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/genomapOPT/genomapOPT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.029401 genomap-1.1.1/genomap/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/ConvDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/ConvIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/FcDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/FcIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/class_discriminative_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/gTraj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/group_centroid_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-15 00:39:00.000000 genomap-1.1.1/genomap/utils/utils_MOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:41:23.025400 genomap-1.1.1/genomap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-15 00:41:22.000000 genomap-1.1.1/genomap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-15 00:41:22.000000 genomap-1.1.1/genomap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 00:41:22.000000 genomap-1.1.1/genomap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-15 00:41:22.000000 genomap-1.1.1/genomap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 00:41:22.000000 genomap-1.1.1/genomap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-15 00:39:00.000000 genomap-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 00:41:23.029401 genomap-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-15 00:39:00.000000 genomap-1.1.1/setup.py
```

### Comparing `genomap-1.1.0/LICENSE.txt` & `genomap-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.1.0/PKG-INFO` & `genomap-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.1.0
+Version: 1.1.1
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `genomap-1.1.0/README.md` & `genomap-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `genomap-1.1.0/genomap/bregman_genomap/bregman_genomap.py` & `genomap-1.1.1/genomap/bregman_genomap/bregman_genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.0/genomap/genoMOI/genoMOI.py` & `genomap-1.1.1/genomap/genoMOI/genoMOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.0/genomap/genoTraj/genoTraj.py` & `genomap-1.1.1/genomap/genoTraj/genoTraj.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.0/genomap/genoVis/genoVis.py` & `genomap-1.1.1/genomap/genoVis/genoVis.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.0/genomap/genomap.py` & `genomap-1.1.1/genomap/genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.0/genomap/genomapOPT/genomapOPT.py` & `genomap-1.1.1/genomap/genomapOPT/genomapOPT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.0/genomap/utils/ConvDEC.py` & `genomap-1.1.1/genomap/utils/ConvDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.0/genomap/utils/ConvIDEC.py` & `genomap-1.1.1/genomap/utils/ConvIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.0/genomap/utils/FcDEC.py` & `genomap-1.1.1/genomap/utils/FcDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.0/genomap/utils/FcIDEC.py` & `genomap-1.1.1/genomap/utils/FcIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.0/genomap/utils/class_discriminative_opt.py` & `genomap-1.1.1/genomap/utils/class_discriminative_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.0/genomap/utils/gTraj_utils.py` & `genomap-1.1.1/genomap/utils/gTraj_utils.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.0/genomap/utils/group_centroid_opt.py` & `genomap-1.1.1/genomap/utils/group_centroid_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.0/genomap/utils/metrics.py` & `genomap-1.1.1/genomap/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.0/genomap/utils/utils_MOI.py` & `genomap-1.1.1/genomap/utils/utils_MOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.1.0/genomap.egg-info/PKG-INFO` & `genomap-1.1.1/genomap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.1.0
+Version: 1.1.1
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `genomap-1.1.0/genomap.egg-info/SOURCES.txt` & `genomap-1.1.1/genomap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.1.0/setup.py` & `genomap-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="genomap",
-    version="1.1.0",
+    version="1.1.1",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="Genomap converts tabular gene expression data into spatially meaningful images.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/genomap",
     classifiers=[
```

