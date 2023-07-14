# Comparing `tmp/genomap-1.0.8.tar.gz` & `tmp/genomap-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomap-1.0.8.tar", last modified: Fri Jul 14 23:10:08 2023, max compression
+gzip compressed data, was "genomap-1.0.9.tar", last modified: Fri Jul 14 23:35:45 2023, max compression
```

## Comparing `genomap-1.0.8.tar` & `genomap-1.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:08.524754 genomap-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-14 23:08:20.000000 genomap-1.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-14 23:08:20.000000 genomap-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-14 23:10:08.524754 genomap-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-14 23:08:20.000000 genomap-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:08.520754 genomap-1.0.8/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-14 23:08:20.000000 genomap-1.0.8/data/TM_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:08.520754 genomap-1.0.8/genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:08.524754 genomap-1.0.8/genomap/bregman_genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/bregman_genomap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/bregman_genomap/bregman_genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:08.524754 genomap-1.0.8/genomap/genoMOI/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/genoMOI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/genoMOI/genoMOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:08.524754 genomap-1.0.8/genomap/genoTraj/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/genoTraj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/genoTraj/genoTraj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:08.524754 genomap-1.0.8/genomap/genoVis/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/genoVis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/genoVis/genoVis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:08.524754 genomap-1.0.8/genomap/genomapOPT/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/genomapOPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/genomapOPT/genomapOPT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:08.524754 genomap-1.0.8/genomap/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/utils/ConvDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/utils/ConvIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/utils/FcDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/utils/FcIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/utils/class_discriminative_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/utils/gTraj_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/utils/group_centroid_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-14 23:08:20.000000 genomap-1.0.8/genomap/utils/utils_MOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:08.524754 genomap-1.0.8/genomap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-14 23:10:08.000000 genomap-1.0.8/genomap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-14 23:10:08.000000 genomap-1.0.8/genomap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:10:08.000000 genomap-1.0.8/genomap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 23:10:08.000000 genomap-1.0.8/genomap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 23:10:08.000000 genomap-1.0.8/genomap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-14 23:08:20.000000 genomap-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 23:10:08.524754 genomap-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-14 23:08:20.000000 genomap-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:35:45.564506 genomap-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-14 23:33:21.000000 genomap-1.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-14 23:33:21.000000 genomap-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-14 23:35:45.564506 genomap-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-07-14 23:33:21.000000 genomap-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:35:45.560506 genomap-1.0.9/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-14 23:33:21.000000 genomap-1.0.9/data/TM_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:35:45.560506 genomap-1.0.9/genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:35:45.560506 genomap-1.0.9/genomap/bregman_genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/bregman_genomap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/bregman_genomap/bregman_genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:35:45.560506 genomap-1.0.9/genomap/genoMOI/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/genoMOI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/genoMOI/genoMOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:35:45.564506 genomap-1.0.9/genomap/genoTraj/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/genoTraj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/genoTraj/genoTraj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:35:45.564506 genomap-1.0.9/genomap/genoVis/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/genoVis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/genoVis/genoVis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:35:45.564506 genomap-1.0.9/genomap/genomapOPT/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/genomapOPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/genomapOPT/genomapOPT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:35:45.564506 genomap-1.0.9/genomap/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/utils/ConvDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/utils/ConvIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/utils/FcDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/utils/FcIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/utils/class_discriminative_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/utils/gTraj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/utils/group_centroid_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-14 23:33:21.000000 genomap-1.0.9/genomap/utils/utils_MOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:35:45.560506 genomap-1.0.9/genomap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-07-14 23:35:45.000000 genomap-1.0.9/genomap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-14 23:35:45.000000 genomap-1.0.9/genomap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:35:45.000000 genomap-1.0.9/genomap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-14 23:35:45.000000 genomap-1.0.9/genomap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 23:35:45.000000 genomap-1.0.9/genomap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-14 23:33:21.000000 genomap-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 23:35:45.564506 genomap-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-14 23:33:21.000000 genomap-1.0.9/setup.py
```

### Comparing `genomap-1.0.8/LICENSE.txt` & `genomap-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.0.8/PKG-INFO` & `genomap-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genomap
-Version: 1.0.8
+Version: 1.0.9
 Summary: Genomap converts tabular gene expression data into spatially meaningful images.
 Home-page: https://github.com/xinglab-ai/genomap
 Author: Md Tauhidul Islam
 Author-email: tauhid@stanford.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -81,23 +81,23 @@
 data=dx['X3']
 gt_data = sio.loadmat('cellsPsudo.mat')
 Y_time = np.squeeze(gt_data['newGT'])
 
 
 outGenoTraj=compute_genoTraj(data)
 
-dx = sio.loadmat('MOIdata/dataBaronX.mat')
+dx = sio.loadmat('dataBaronX.mat')
 data=dx['dataBaron']
-dx = sio.loadmat('MOIdata/dataMuraroX.mat')
+dx = sio.loadmat('dataMuraroX.mat')
 data2=dx['dataMuraro']
-dx = sio.loadmat('MOIdata/dataScapleX.mat')
+dx = sio.loadmat('dataScapleX.mat')
 data3=dx['dataScaple']
-dx = sio.loadmat('MOIdata/dataWangX.mat')
+dx = sio.loadmat('dataWangX.mat')
 data4=dx['dataWang']
-dx = sio.loadmat('MOIdata/dataXinX.mat')
+dx = sio.loadmat('dataXinX.mat')
 data5=dx['dataXin']
 
 resVis=compute_genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
 ```
 
 # Citation
```

### Comparing `genomap-1.0.8/README.md` & `genomap-1.0.9/genomap.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: genomap
+Version: 1.0.9
+Summary: Genomap converts tabular gene expression data into spatially meaningful images.
+Home-page: https://github.com/xinglab-ai/genomap
+Author: Md Tauhidul Islam
+Author-email: tauhid@stanford.edu
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Genomap creates images from gene expression data
 
 Genomap is an entropy-based cartography strategy to contrive the high dimensional gene expression data into a configured image format with explicit integration of the genomic interactions. This unique cartography casts the gene-gene interactions into a spatial configuration and enables us to extract the deep genomic interaction features and discover underlying discriminative patterns of the data. For a wide variety of applications (cell clustering and recognition, gene signature extraction, single-cell data integration, cellular trajectory analysis, dimensionality reduction, and visualization), genomap drastically improves the accuracy of data analyses as compared to state-of-the-art techniques.
 
 ## Required packages
 
 scipy, scikit-learn, pot, numpy
@@ -68,23 +81,23 @@
 data=dx['X3']
 gt_data = sio.loadmat('cellsPsudo.mat')
 Y_time = np.squeeze(gt_data['newGT'])
 
 
 outGenoTraj=compute_genoTraj(data)
 
-dx = sio.loadmat('MOIdata/dataBaronX.mat')
+dx = sio.loadmat('dataBaronX.mat')
 data=dx['dataBaron']
-dx = sio.loadmat('MOIdata/dataMuraroX.mat')
+dx = sio.loadmat('dataMuraroX.mat')
 data2=dx['dataMuraro']
-dx = sio.loadmat('MOIdata/dataScapleX.mat')
+dx = sio.loadmat('dataScapleX.mat')
 data3=dx['dataScaple']
-dx = sio.loadmat('MOIdata/dataWangX.mat')
+dx = sio.loadmat('dataWangX.mat')
 data4=dx['dataWang']
-dx = sio.loadmat('MOIdata/dataXinX.mat')
+dx = sio.loadmat('dataXinX.mat')
 data5=dx['dataXin']
 
 resVis=compute_genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
 ```
 
 # Citation
```

### Comparing `genomap-1.0.8/genomap/bregman_genomap/bregman_genomap.py` & `genomap-1.0.9/genomap/bregman_genomap/bregman_genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.8/genomap/genoMOI/genoMOI.py` & `genomap-1.0.9/genomap/genoMOI/genoMOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.8/genomap/genoTraj/genoTraj.py` & `genomap-1.0.9/genomap/genoTraj/genoTraj.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.8/genomap/genoVis/genoVis.py` & `genomap-1.0.9/genomap/genoVis/genoVis.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.8/genomap/genomap.py` & `genomap-1.0.9/genomap/genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.8/genomap/genomapOPT/genomapOPT.py` & `genomap-1.0.9/genomap/genomapOPT/genomapOPT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.8/genomap/utils/ConvDEC.py` & `genomap-1.0.9/genomap/utils/ConvDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.8/genomap/utils/ConvIDEC.py` & `genomap-1.0.9/genomap/utils/ConvIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.8/genomap/utils/FcDEC.py` & `genomap-1.0.9/genomap/utils/FcDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.8/genomap/utils/FcIDEC.py` & `genomap-1.0.9/genomap/utils/FcIDEC.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.8/genomap/utils/class_discriminative_opt.py` & `genomap-1.0.9/genomap/utils/class_discriminative_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.8/genomap/utils/gTraj_utils.py` & `genomap-1.0.9/genomap/utils/gTraj_utils.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.8/genomap/utils/group_centroid_opt.py` & `genomap-1.0.9/genomap/utils/group_centroid_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.8/genomap/utils/metrics.py` & `genomap-1.0.9/genomap/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.8/genomap/utils/utils_MOI.py` & `genomap-1.0.9/genomap/utils/utils_MOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.8/genomap.egg-info/PKG-INFO` & `genomap-1.0.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: genomap
-Version: 1.0.8
-Summary: Genomap converts tabular gene expression data into spatially meaningful images.
-Home-page: https://github.com/xinglab-ai/genomap
-Author: Md Tauhidul Islam
-Author-email: tauhid@stanford.edu
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Genomap creates images from gene expression data
 
 Genomap is an entropy-based cartography strategy to contrive the high dimensional gene expression data into a configured image format with explicit integration of the genomic interactions. This unique cartography casts the gene-gene interactions into a spatial configuration and enables us to extract the deep genomic interaction features and discover underlying discriminative patterns of the data. For a wide variety of applications (cell clustering and recognition, gene signature extraction, single-cell data integration, cellular trajectory analysis, dimensionality reduction, and visualization), genomap drastically improves the accuracy of data analyses as compared to state-of-the-art techniques.
 
 ## Required packages
 
 scipy, scikit-learn, pot, numpy
@@ -81,23 +68,23 @@
 data=dx['X3']
 gt_data = sio.loadmat('cellsPsudo.mat')
 Y_time = np.squeeze(gt_data['newGT'])
 
 
 outGenoTraj=compute_genoTraj(data)
 
-dx = sio.loadmat('MOIdata/dataBaronX.mat')
+dx = sio.loadmat('dataBaronX.mat')
 data=dx['dataBaron']
-dx = sio.loadmat('MOIdata/dataMuraroX.mat')
+dx = sio.loadmat('dataMuraroX.mat')
 data2=dx['dataMuraro']
-dx = sio.loadmat('MOIdata/dataScapleX.mat')
+dx = sio.loadmat('dataScapleX.mat')
 data3=dx['dataScaple']
-dx = sio.loadmat('MOIdata/dataWangX.mat')
+dx = sio.loadmat('dataWangX.mat')
 data4=dx['dataWang']
-dx = sio.loadmat('MOIdata/dataXinX.mat')
+dx = sio.loadmat('dataXinX.mat')
 data5=dx['dataXin']
 
 resVis=compute_genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
 ```
 
 # Citation
```

### Comparing `genomap-1.0.8/genomap.egg-info/SOURCES.txt` & `genomap-1.0.9/genomap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.0.8/setup.py` & `genomap-1.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="genomap",
-    version="1.0.8",
+    version="1.0.9",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="Genomap converts tabular gene expression data into spatially meaningful images.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/genomap",
     classifiers=[
```

