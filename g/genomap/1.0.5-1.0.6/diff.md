# Comparing `tmp/genomap-1.0.5.tar.gz` & `tmp/genomap-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genomap-1.0.5.tar", last modified: Fri Jul 14 21:26:22 2023, max compression
+gzip compressed data, was "genomap-1.0.6.tar", last modified: Fri Jul 14 22:43:31 2023, max compression
```

## Comparing `genomap-1.0.5.tar` & `genomap-1.0.6.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:26:22.305258 genomap-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-14 21:24:47.000000 genomap-1.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-14 21:24:47.000000 genomap-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-14 21:26:22.305258 genomap-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-14 21:24:47.000000 genomap-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:26:22.301258 genomap-1.0.5/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-14 21:24:47.000000 genomap-1.0.5/data/TM_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:26:22.301258 genomap-1.0.5/genomap/
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/ConvDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/ConvIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)    13513 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/FcDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/FcIDEC.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:26:22.305258 genomap-1.0.5/genomap/bregman_genomap/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/bregman_genomap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/bregman_genomap/bregman_genomap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/class_discriminative_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/gTraj_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:26:22.305258 genomap-1.0.5/genomap/genoMOI/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/genoMOI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/genoMOI/genoMOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:26:22.305258 genomap-1.0.5/genomap/genoTraj/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/genoTraj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/genoTraj/genoTraj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:26:22.305258 genomap-1.0.5/genomap/genoVis/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/genoVis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/genoVis/genoVis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/genomap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:26:22.305258 genomap-1.0.5/genomap/genomapOPT/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/genomapOPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/genomapOPT/genomapOPT.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/group_centroid_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-14 21:24:47.000000 genomap-1.0.5/genomap/utils_MOI.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:26:22.305258 genomap-1.0.5/genomap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-14 21:26:22.000000 genomap-1.0.5/genomap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-14 21:26:22.000000 genomap-1.0.5/genomap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 21:26:22.000000 genomap-1.0.5/genomap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 21:26:22.000000 genomap-1.0.5/genomap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 21:26:22.000000 genomap-1.0.5/genomap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-14 21:24:47.000000 genomap-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 21:26:22.305258 genomap-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-14 21:24:47.000000 genomap-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:43:31.953069 genomap-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-14 22:41:58.000000 genomap-1.0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-14 22:41:58.000000 genomap-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-14 22:43:31.953069 genomap-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-14 22:41:58.000000 genomap-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:43:31.949069 genomap-1.0.6/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-14 22:41:58.000000 genomap-1.0.6/data/TM_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:43:31.949069 genomap-1.0.6/genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:43:31.949069 genomap-1.0.6/genomap/bregman_genomap/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/bregman_genomap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125058 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/bregman_genomap/bregman_genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:43:31.953069 genomap-1.0.6/genomap/genoMOI/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/genoMOI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/genoMOI/genoMOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:43:31.953069 genomap-1.0.6/genomap/genoTraj/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/genoTraj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/genoTraj/genoTraj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:43:31.953069 genomap-1.0.6/genomap/genoVis/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/genoVis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/genoVis/genoVis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/genomap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:43:31.953069 genomap-1.0.6/genomap/genomapOPT/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/genomapOPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/genomapOPT/genomapOPT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:43:31.953069 genomap-1.0.6/genomap/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/utils/ConvDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/utils/ConvIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/utils/FcDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/utils/FcIDEC.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/utils/class_discriminative_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/utils/gTraj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/utils/group_centroid_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-14 22:41:58.000000 genomap-1.0.6/genomap/utils/utils_MOI.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:43:31.949069 genomap-1.0.6/genomap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-14 22:43:31.000000 genomap-1.0.6/genomap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-14 22:43:31.000000 genomap-1.0.6/genomap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:43:31.000000 genomap-1.0.6/genomap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 22:43:31.000000 genomap-1.0.6/genomap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 22:43:31.000000 genomap-1.0.6/genomap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-14 22:41:58.000000 genomap-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 22:43:31.953069 genomap-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-14 22:41:58.000000 genomap-1.0.6/setup.py
```

### Comparing `genomap-1.0.5/LICENSE.txt` & `genomap-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `genomap-1.0.5/PKG-INFO` & `genomap-1.0.6/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,95 @@
-Metadata-Version: 2.1
-Name: genomap
-Version: 1.0.5
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
 
-# Required packages
+## Required packages
 
 scipy, scikit-learn, pot, numpy
 
 If you face any issues with packages, please check the environment section of our Code-Ocean capsule (https://doi.org/10.24433/CO.0640398.v1), where you can check the package versions.
 
-# How to use genomap
+## How to use genomap
 
 The easiest way to start with genomap is to install it from pypi using 
 
 ```python
 pip install genomap
 ```
 The data should be in cell (row) x gene (column) format. Genomap construction needs only one parameter: the size of the genomap (row and column number). The row and column number can be any number starting from 1. You can create square or rectangular genomaps. The number of genes in your dataset should be less than or equal to the number of pixels in the genomap. Genomap construction is very fast and you should get the genomaps within a few seconds.
 
-# Sample data
+## Sample data
+
+To run the example codes below, you will need to download data files from [here](https://drive.google.com/drive/folders/1xq3bBgVP0NCMD7bGTXit0qRkL8fbutZ6?usp=drive_link).
 
-To run the example code below, you will need to download the required data file. You can download it from [here](https://drive.google.com/file/d/1kkbI9_6zD80Jr5OhMkGlcdMOeWcRfz7b/view?usp=drive_link).
+## Example codes
 
-# Example code
+### Example 1 - Construct a genomap
 
 ```python
 import pandas as pd # Please install pandas and matplotlib before you run this example
-
 import matplotlib.pyplot as plt
-
 import scipy
-
 import genomap as gp
 
 data = pd.read_csv('TM_data.csv', header=None, delim_whitespace=False)
-
 colNum=31 # Column number of genomap
-
 rowNum=31 # Row number of genomap
 
 dataNorm=scipy.stats.zscore(data,axis=0,ddof=1) # Normalization of the data
 
 genoMaps=gp.construct_genomap(dataNorm,rowNum,colNum) # Construction of genomaps
 
 findI=genoMaps[0,:,:,:]
 
 plt.figure(1) # Plot the first genomap
-
 plt.imshow(findI, origin = 'lower', extent = [0, 10, 0, 10], aspect = 1)
-
 plt.title('Genomap of a cell from TM dataset')
 ```
 
+### Example 2 - Try out genoVis, genoTraj and genoMOI
+
+```python
+import scipy.io as sio
+import numpy as np
+from genomap.genoVis import compute_genoVis
+from genomap.genoTraj import compute_genoTraj
+from genomap.genoMOI import compute_genoMOI
+
+dx = sio.loadmat('reducedData_divseq.mat')
+data=dx['X']
+gt_data = sio.loadmat('GT_divseq.mat')
+y = np.squeeze(gt_data['GT'])
+n_clusters = len(np.unique(y))
+
+
+resVis=compute_genoVis(data,n_clusters=n_clusters, colNum=33,rowNum=33)
+
+dx = sio.loadmat('organoidData.mat')
+data=dx['X3']
+gt_data = sio.loadmat('cellsPsudo.mat')
+Y_time = np.squeeze(gt_data['newGT'])
+
+
+outGenoTraj=compute_genoTraj(data)
+
+dx = sio.loadmat('MOIdata/dataBaronX.mat')
+data=dx['dataBaron']
+dx = sio.loadmat('MOIdata/dataMuraroX.mat')
+data2=dx['dataMuraro']
+dx = sio.loadmat('MOIdata/dataScapleX.mat')
+data3=dx['dataScaple']
+dx = sio.loadmat('MOIdata/dataWangX.mat')
+data4=dx['dataWang']
+dx = sio.loadmat('MOIdata/dataXinX.mat')
+data5=dx['dataXin']
+
+resVis=compute_genoMOI(data, data2, data3, data4, data5, colNum=44, rowNum=44)
+```
+
 # Citation
 
 If you use the genomap code, please cite our Nature Communications paper: https://www.nature.com/articles/s41467-023-36383-6
 
 Islam, M.T., Xing, L. Cartography of Genomic Interactions Enables Deep Analysis of Single-Cell Expression Data. Nat Commun 14, 679 (2023). https://doi.org/10.1038/s41467-023-36383-6
```

### Comparing `genomap-1.0.5/genomap/ConvDEC.py` & `genomap-1.0.6/genomap/utils/ConvDEC.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 Author:
     Xifeng Guo. 2018.6.30
 """
 
 from tensorflow.keras.layers import Conv2D, Conv2DTranspose, Dense, Flatten, Reshape, InputLayer
 from tensorflow.keras.models import Sequential, Model
 from tensorflow.keras.preprocessing.image import ImageDataGenerator
-from FcDEC import FcDEC, ClusteringLayer
-
+from .FcDEC import FcDEC, ClusteringLayer
 
 def CAE(input_shape=(28, 28, 1), filters=[32, 64, 128, 10]):
     model = Sequential()
     if input_shape[0] % 8 == 0:
         pad3 = 'same'
     else:
         pad3 = 'valid'
```

### Comparing `genomap-1.0.5/genomap/ConvIDEC.py` & `genomap-1.0.6/genomap/utils/ConvIDEC.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     - Xifeng Guo, En Zhu, Xinwang Liu, and Jianping Yin. Deep Embedded Clustering with Data Augmentation. ACML 2018.
 
 Author:
     Xifeng Guo. 2018.6.30
 """
 
 from tensorflow.keras.models import Model
-from ConvDEC import ConvDEC
+from .ConvDEC import ConvDEC
 
 
 class ConvIDEC(ConvDEC):
     def __init__(self,
                  input_shape,
                  filters=[32, 64, 128, 10],
                  n_clusters=10):
```

### Comparing `genomap-1.0.5/genomap/FcDEC.py` & `genomap-1.0.6/genomap/utils/FcDEC.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import tensorflow.keras.backend as K
 from tensorflow.keras.layers import Layer, InputSpec, Input, Dense
 from tensorflow.keras.models import Model
 from tensorflow.keras import callbacks
 from tensorflow.keras.initializers import VarianceScaling
 from tensorflow.keras.preprocessing.image import ImageDataGenerator
 from sklearn.cluster import KMeans
-import metrics
+from .metrics import *
 
 
 def autoencoder(dims, act='relu'):
     """
     Fully connected auto-encoder model, symmetric.
     Arguments:
         dims: list of number of units in each layer of encoder. dims[0] is input dim, dims[-1] is units in hidden layer.
```

### Comparing `genomap-1.0.5/genomap/FcIDEC.py` & `genomap-1.0.6/genomap/utils/FcIDEC.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     - Xifeng Guo, En Zhu, Xinwang Liu, and Jianping Yin. Deep Embedded Clustering with Data Augmentation. ACML 2018.
 
 Author:
     Xifeng Guo. 2018.6.30
 """
 
 from tensorflow.keras.models import Model
-from FcDEC import FcDEC
+from .FcDEC import FcDEC
 
 
 class FcIDEC(FcDEC):
     def __init__(self, dims, n_clusters=10, alpha=1.0):
         super(FcIDEC, self).__init__(dims, n_clusters, alpha)
         self.model = Model(inputs=self.autoencoder.input,
                            outputs=[self.model.output, self.autoencoder.output])
```

### Comparing `genomap-1.0.5/genomap/bregman_genomap/bregman_genomap.py` & `genomap-1.0.6/genomap/bregman_genomap/bregman_genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.5/genomap/class_discriminative_opt.py` & `genomap-1.0.6/genomap/utils/class_discriminative_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.5/genomap/gTraj_utils.py` & `genomap-1.0.6/genomap/utils/gTraj_utils.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.5/genomap/genoMOI/genoMOI.py` & `genomap-1.0.6/genomap/genoMOI/genoMOI.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 """
 Created on Wed Jul 12 16:11:15 2023
 
 @author: Md Tauhidul Islam, Ph.D., Dept. of Radiation Oncology, Stanford University
 """
 
 from tensorflow.keras.optimizers import Adam
-from genomap.ConvIDEC import ConvIDEC
+from utils.ConvIDEC import ConvIDEC
 # from ConvIDEC import ConvIDEC
 from sklearn.feature_selection import VarianceThreshold
 from genomap.genomap import construct_genomap
 import umap
-from genomap.gTraj_utils import nearest_divisible_by_four
+from utils.gTraj_utils import nearest_divisible_by_four
 # from gTraj_utils import nearest_divisible_by_four
-from genomap.utils_MOI import *
+from utils.utils_MOI import *
 # from utils_MOI import * 
 
 def compute_genoMOI(*arrays,n_clusters=None, colNum, rowNum):  
 
 # arrays: number of arrays such as array1,array2
 # n_clusters: number of data classes
 # colNum and rowNum: column are rwo number of genomaps
```

### Comparing `genomap-1.0.5/genomap/genoTraj/genoTraj.py` & `genomap-1.0.6/genomap/genoTraj/genoTraj.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 Created on Wed Jul 12 15:14:53 2023
 
 @author: Windows
 """
 
 import phate
 import numpy as np
-from genomap.class_discriminative_opt import ClassDiscriminative_OPT
+from utils.class_discriminative_opt import ClassDiscriminative_OPT
 import scipy
-from genomap.gTraj_utils import compute_cluster_distances, nearest_divisible_by_four
+from utils.gTraj_utils import compute_cluster_distances, nearest_divisible_by_four
 from tensorflow.keras.optimizers import Adam
-from genomap.ConvIDEC import ConvIDEC
+from utils.ConvIDEC import ConvIDEC
 from sklearn.feature_selection import VarianceThreshold
 from genomap.genomap import construct_genomap
 # from gTraj_utils import nearest_divisible_by_four
 
 def apply_genoTraj(data, y_pred):
 # data: input data
 # y_pred: predicted pseudo labels
```

### Comparing `genomap-1.0.5/genomap/genoVis/genoVis.py` & `genomap-1.0.6/genomap/genoVis/genoVis.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 """
 Created on Wed Jul 12 16:11:15 2023
 
 @author: Md Tauhidul Islam, Ph.D., Dept. of Radiation Oncology, Stanford University
 """
 
 from tensorflow.keras.optimizers import Adam
-from genomap.ConvIDEC import ConvIDEC
+from utils.ConvIDEC import ConvIDEC
 from sklearn.feature_selection import VarianceThreshold
 from genomap.genomap import construct_genomap
 import umap
 # from gTraj_utils import nearest_divisible_by_four
-from genomap.gTraj_utils import nearest_divisible_by_four
+from utils.gTraj_utils import nearest_divisible_by_four
 import scanpy as sc
 import numpy as np
 import pandas as pd
 
 def compute_genoVis(data,n_clusters=None, colNum=32,rowNum=32,batch_size=64,verbose=1,
                     pretrain_epochs=100,maxiter=300):
 # rowNum and colNum are the row and column numbers of constructed genomaps
```

### Comparing `genomap-1.0.5/genomap/genomap.py` & `genomap-1.0.6/genomap/genomap.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.5/genomap/genomapOPT/genomapOPT.py` & `genomap-1.0.6/genomap/genomapOPT/genomapOPT.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.5/genomap/group_centroid_opt.py` & `genomap-1.0.6/genomap/utils/group_centroid_opt.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.5/genomap/metrics.py` & `genomap-1.0.6/genomap/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.5/genomap/utils_MOI.py` & `genomap-1.0.6/genomap/utils/utils_MOI.py`

 * *Files identical despite different names*

### Comparing `genomap-1.0.5/genomap.egg-info/SOURCES.txt` & `genomap-1.0.6/genomap.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 data/TM_data.csv
-genomap/ConvDEC.py
-genomap/ConvIDEC.py
-genomap/FcDEC.py
-genomap/FcIDEC.py
 genomap/__init__.py
-genomap/class_discriminative_opt.py
-genomap/gTraj_utils.py
 genomap/genomap.py
-genomap/group_centroid_opt.py
-genomap/metrics.py
-genomap/utils_MOI.py
 genomap.egg-info/PKG-INFO
 genomap.egg-info/SOURCES.txt
 genomap.egg-info/dependency_links.txt
 genomap.egg-info/requires.txt
 genomap.egg-info/top_level.txt
 genomap/bregman_genomap/__init__.py
 genomap/bregman_genomap/bregman_genomap.py
 genomap/genoMOI/__init__.py
 genomap/genoMOI/genoMOI.py
 genomap/genoTraj/__init__.py
 genomap/genoTraj/genoTraj.py
 genomap/genoVis/__init__.py
 genomap/genoVis/genoVis.py
 genomap/genomapOPT/__init__.py
-genomap/genomapOPT/genomapOPT.py
+genomap/genomapOPT/genomapOPT.py
+genomap/utils/ConvDEC.py
+genomap/utils/ConvIDEC.py
+genomap/utils/FcDEC.py
+genomap/utils/FcIDEC.py
+genomap/utils/__init__.py
+genomap/utils/class_discriminative_opt.py
+genomap/utils/gTraj_utils.py
+genomap/utils/group_centroid_opt.py
+genomap/utils/metrics.py
+genomap/utils/utils_MOI.py
```

### Comparing `genomap-1.0.5/setup.py` & `genomap-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="genomap",
-    version="1.0.5",
+    version="1.0.6",
     author="Md Tauhidul Islam",
     author_email="tauhid@stanford.edu",
     description="Genomap converts tabular gene expression data into spatially meaningful images.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xinglab-ai/genomap",
     classifiers=[
```

