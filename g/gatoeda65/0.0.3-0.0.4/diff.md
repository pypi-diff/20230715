# Comparing `tmp/gatoeda65-0.0.3.tar.gz` & `tmp/gatoeda65-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gatoeda65-0.0.3.tar", last modified: Sat Jul  1 23:02:01 2023, max compression
+gzip compressed data, was "gatoeda65-0.0.4.tar", last modified: Sat Jul 15 00:28:28 2023, max compression
```

## Comparing `gatoeda65-0.0.3.tar` & `gatoeda65-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 gato      (1000) gato      (1000)        0 2023-07-01 23:02:01.463043 gatoeda65-0.0.3/
--rw-rw-r--   0 gato      (1000) gato      (1000)     1068 2023-07-01 17:25:51.000000 gatoeda65-0.0.3/LICENSE
--rw-rw-r--   0 gato      (1000) gato      (1000)      695 2023-07-01 23:02:01.463043 gatoeda65-0.0.3/PKG-INFO
--rw-rw-r--   0 gato      (1000) gato      (1000)      279 2023-07-01 19:45:58.000000 gatoeda65-0.0.3/README.md
-drwxrwxr-x   0 gato      (1000) gato      (1000)        0 2023-07-01 23:02:01.463043 gatoeda65-0.0.3/exploratory_data_analysis/
--rw-rw-r--   0 gato      (1000) gato      (1000)      793 2023-07-01 22:56:25.000000 gatoeda65-0.0.3/exploratory_data_analysis/__init__.py
--rw-rw-r--   0 gato      (1000) gato      (1000)      668 2023-07-01 19:44:35.000000 gatoeda65-0.0.3/exploratory_data_analysis/data.py
--rw-rw-r--   0 gato      (1000) gato      (1000)    13466 2023-07-01 20:11:34.000000 gatoeda65-0.0.3/exploratory_data_analysis/eda_functions.py
--rwxrwxr-x   0 gato      (1000) gato      (1000)     2320 2023-07-01 19:44:35.000000 gatoeda65-0.0.3/exploratory_data_analysis/tester.py
-drwxrwxr-x   0 gato      (1000) gato      (1000)        0 2023-07-01 23:02:01.463043 gatoeda65-0.0.3/gatoeda65.egg-info/
--rw-rw-r--   0 gato      (1000) gato      (1000)      695 2023-07-01 23:02:01.000000 gatoeda65-0.0.3/gatoeda65.egg-info/PKG-INFO
--rw-rw-r--   0 gato      (1000) gato      (1000)      341 2023-07-01 23:02:01.000000 gatoeda65-0.0.3/gatoeda65.egg-info/SOURCES.txt
--rw-rw-r--   0 gato      (1000) gato      (1000)        1 2023-07-01 23:02:01.000000 gatoeda65-0.0.3/gatoeda65.egg-info/dependency_links.txt
--rw-rw-r--   0 gato      (1000) gato      (1000)       50 2023-07-01 23:02:01.000000 gatoeda65-0.0.3/gatoeda65.egg-info/requires.txt
--rw-rw-r--   0 gato      (1000) gato      (1000)       26 2023-07-01 23:02:01.000000 gatoeda65-0.0.3/gatoeda65.egg-info/top_level.txt
--rw-rw-r--   0 gato      (1000) gato      (1000)       38 2023-07-01 23:02:01.463043 gatoeda65-0.0.3/setup.cfg
--rw-rw-r--   0 gato      (1000) gato      (1000)     1213 2023-07-01 21:32:16.000000 gatoeda65-0.0.3/setup.py
+drwxrwxr-x   0 gato      (1000) gato      (1000)        0 2023-07-15 00:28:28.051204 gatoeda65-0.0.4/
+-rw-rw-r--   0 gato      (1000) gato      (1000)     1068 2023-07-01 17:25:51.000000 gatoeda65-0.0.4/LICENSE
+-rw-rw-r--   0 gato      (1000) gato      (1000)      695 2023-07-15 00:28:28.051204 gatoeda65-0.0.4/PKG-INFO
+-rw-rw-r--   0 gato      (1000) gato      (1000)      279 2023-07-01 19:45:58.000000 gatoeda65-0.0.4/README.md
+drwxrwxr-x   0 gato      (1000) gato      (1000)        0 2023-07-15 00:28:28.051204 gatoeda65-0.0.4/exploratory_data_analysis/
+-rw-rw-r--   0 gato      (1000) gato      (1000)      793 2023-07-01 23:22:38.000000 gatoeda65-0.0.4/exploratory_data_analysis/__init__.py
+-rw-rw-r--   0 gato      (1000) gato      (1000)      668 2023-07-01 23:22:38.000000 gatoeda65-0.0.4/exploratory_data_analysis/data.py
+-rw-rw-r--   0 gato      (1000) gato      (1000)    14987 2023-07-15 00:27:34.000000 gatoeda65-0.0.4/exploratory_data_analysis/eda_functions.py
+-rwxrwxr-x   0 gato      (1000) gato      (1000)     2320 2023-07-01 23:22:38.000000 gatoeda65-0.0.4/exploratory_data_analysis/tester.py
+drwxrwxr-x   0 gato      (1000) gato      (1000)        0 2023-07-15 00:28:28.051204 gatoeda65-0.0.4/gatoeda65.egg-info/
+-rw-rw-r--   0 gato      (1000) gato      (1000)      695 2023-07-15 00:28:27.000000 gatoeda65-0.0.4/gatoeda65.egg-info/PKG-INFO
+-rw-rw-r--   0 gato      (1000) gato      (1000)      341 2023-07-15 00:28:28.000000 gatoeda65-0.0.4/gatoeda65.egg-info/SOURCES.txt
+-rw-rw-r--   0 gato      (1000) gato      (1000)        1 2023-07-15 00:28:27.000000 gatoeda65-0.0.4/gatoeda65.egg-info/dependency_links.txt
+-rw-rw-r--   0 gato      (1000) gato      (1000)       50 2023-07-15 00:28:27.000000 gatoeda65-0.0.4/gatoeda65.egg-info/requires.txt
+-rw-rw-r--   0 gato      (1000) gato      (1000)       26 2023-07-15 00:28:27.000000 gatoeda65-0.0.4/gatoeda65.egg-info/top_level.txt
+-rw-rw-r--   0 gato      (1000) gato      (1000)       38 2023-07-15 00:28:28.051204 gatoeda65-0.0.4/setup.cfg
+-rw-rw-r--   0 gato      (1000) gato      (1000)     1213 2023-07-15 00:27:53.000000 gatoeda65-0.0.4/setup.py
```

### Comparing `gatoeda65-0.0.3/LICENSE` & `gatoeda65-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gatoeda65-0.0.3/PKG-INFO` & `gatoeda65-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gatoeda65
-Version: 0.0.3
+Version: 0.0.4
 Summary: Functions for exploratory data analysis
 Author: GatoMario (Mario Hevia Cavieres)
 Author-email: mario.hevia@gmail.com
 Keywords: python,EDA,exploratory data analysis
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gatoeda65-0.0.3/exploratory_data_analysis/__init__.py` & `gatoeda65-0.0.4/exploratory_data_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `gatoeda65-0.0.3/exploratory_data_analysis/data.py` & `gatoeda65-0.0.4/exploratory_data_analysis/data.py`

 * *Files identical despite different names*

### Comparing `gatoeda65-0.0.3/exploratory_data_analysis/eda_functions.py` & `gatoeda65-0.0.4/exploratory_data_analysis/eda_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from scipy import stats
 from scipy.stats import skew
 from scipy.stats import kurtosis
 import statsmodels.api as sm
+from sklearn.utils import resample
 
 import math
 import pandas as pd
 import numpy as np
 
 ## Graphs
 import matplotlib.pyplot as plt
@@ -109,15 +110,14 @@
     invalid_list =\
     [np.nan, None, [], {}, 'NaN', 'Null','NULL'\
      ,'None','NA','?','-', '--','.','', ' ', '   ']
     
     invalids = []
     uniques = []
     result = pd.DataFrame({
-        'column': df.columns,
         'nulls': df.isnull().sum(),
     })
     for c in df.columns:
         invalids.append(df[c].isin(invalid_list).sum())
         uniques.append(df[c].unique())
     result['invalids'] = invalids
     result['unique_item'] = uniques
@@ -400,8 +400,59 @@
     ## qqplot from stats
     sm.qqplot(df[col], fit=True, line='45')
     
     plt.show()
     
 
 ################################################################################
+####################UpSampleMinorityClass#######################################
+
+def upsample_minority_class(data, feature):
+    
+    '''
+    Take a pandas df and one binary feature.
+    identify the minority class,
+    upsamples the minority in a binary class in a DataFrame 
+    to match the size of the majority class.
+
+      Args:
+        data: The DataFrame to be upsampled, pandas Data Frame.
+        feature: the columns name, string.
+        
+      Returns:
+        A DataFrame with the minority class upsampled.
+    '''
+    
+    ## Identify data points from majority and minority classes
+    
+    class_1 = data[feature].value_counts().index[0]
+    class_2 = data[feature].value_counts().index[1]
+    
+    majority_class = None
+    minority_class = None
+
+    if class_1 > class_2:
+        majority_class = class_1
+        minority_class = class_2
+    else: 
+        majority_class = class_2
+        minority_class = class_1
+
+    
+    data_majority = data[data[feature] == majority_class]
+    data_minority = data[data[feature] == minority_class]
+    
+    n_samples = len(data_majority)
+                              
+    data_minority_upsampled = resample(
+          data_minority,
+          replace=True,
+          n_samples=n_samples,
+          random_state=None)
+
+    data_upsampled = pd.concat([data_majority, \
+                                data_minority_upsampled]).reset_index(drop=True)
+
+    return data_upsampled
+
+################################################################################
 ################################################################################
```

### Comparing `gatoeda65-0.0.3/exploratory_data_analysis/tester.py` & `gatoeda65-0.0.4/exploratory_data_analysis/tester.py`

 * *Files identical despite different names*

### Comparing `gatoeda65-0.0.3/gatoeda65.egg-info/PKG-INFO` & `gatoeda65-0.0.4/gatoeda65.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gatoeda65
-Version: 0.0.3
+Version: 0.0.4
 Summary: Functions for exploratory data analysis
 Author: GatoMario (Mario Hevia Cavieres)
 Author-email: mario.hevia@gmail.com
 Keywords: python,EDA,exploratory data analysis
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gatoeda65-0.0.3/setup.py` & `gatoeda65-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, 'README.md'), encoding='utf-8') as fh:
     long_description = '\n' + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Functions for exploratory data analysis'
 LONG_DESCRIPTION = 'A set of functions that help to clean and analyse data builded on top of pandas, numpy, matplot.pyplot, seaborn, statsmodels, and scipy.'
 
 # Setting up
 setup(
     name='gatoeda65',
     version=VERSION,
```

