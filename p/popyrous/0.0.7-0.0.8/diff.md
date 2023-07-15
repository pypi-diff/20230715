# Comparing `tmp/popyrous-0.0.7.tar.gz` & `tmp/popyrous-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popyrous-0.0.7.tar", last modified: Sat Jan 21 19:47:32 2023, max compression
+gzip compressed data, was "popyrous-0.0.8.tar", last modified: Sat Jul 15 18:30:03 2023, max compression
```

## Comparing `popyrous-0.0.7.tar` & `popyrous-0.0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-01-21 19:47:32.626402 popyrous-0.0.7/
--rw-rw-rw-   0        0        0     1072 2023-01-20 07:48:00.000000 popyrous-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0     9278 2023-01-21 19:47:32.627399 popyrous-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     8531 2023-01-21 19:46:18.000000 popyrous-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-01-21 19:47:32.608463 popyrous-0.0.7/popyrous/
--rw-rw-rw-   0        0        0      304 2023-01-21 19:46:08.000000 popyrous-0.0.7/popyrous/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-21 19:47:32.619427 popyrous-0.0.7/popyrous/matlab/
--rw-rw-rw-   0        0        0       22 2023-01-19 13:24:02.000000 popyrous-0.0.7/popyrous/matlab/__init__.py
--rw-rw-rw-   0        0        0     2537 2023-01-19 13:24:24.000000 popyrous-0.0.7/popyrous/matlab/matlab.py
-drwxrwxrwx   0        0        0        0 2023-01-21 19:47:32.620424 popyrous-0.0.7/popyrous/ml/
--rw-rw-rw-   0        0        0       15 2023-01-21 13:53:00.000000 popyrous-0.0.7/popyrous/ml/__init__.py
--rw-rw-rw-   0        0        0     4333 2023-01-21 13:54:45.000000 popyrous-0.0.7/popyrous/ml/confusion_matrix.py
-drwxrwxrwx   0        0        0        0 2023-01-21 19:47:32.621420 popyrous-0.0.7/popyrous/packages/
--rw-rw-rw-   0        0        0       47 2023-01-19 11:52:33.000000 popyrous-0.0.7/popyrous/packages/__init__.py
--rw-rw-rw-   0        0        0     6288 2023-01-19 11:55:04.000000 popyrous-0.0.7/popyrous/packages/packages.py
-drwxrwxrwx   0        0        0        0 2023-01-21 19:47:32.624410 popyrous-0.0.7/popyrous/timeseries/
--rw-rw-rw-   0        0        0      185 2023-01-20 20:11:43.000000 popyrous-0.0.7/popyrous/timeseries/__init__.py
--rw-rw-rw-   0        0        0     7172 2023-01-21 12:14:16.000000 popyrous-0.0.7/popyrous/timeseries/cwt.py
--rw-rw-rw-   0        0        0    21072 2023-01-21 19:43:36.000000 popyrous-0.0.7/popyrous/timeseries/datasets.py
--rw-rw-rw-   0        0        0    73409 2023-01-21 10:52:22.000000 popyrous-0.0.7/popyrous/timeseries/experiment.py
--rw-rw-rw-   0        0        0     1781 2023-01-19 13:48:53.000000 popyrous-0.0.7/popyrous/timeseries/filt.py
--rw-rw-rw-   0        0        0     2686 2023-01-19 16:08:55.000000 popyrous-0.0.7/popyrous/timeseries/metrics.py
--rw-rw-rw-   0        0        0     1862 2022-08-06 15:20:20.000000 popyrous-0.0.7/popyrous/timeseries/recipe_577504_1.py
--rw-rw-rw-   0        0        0     4342 2023-01-19 13:33:36.000000 popyrous-0.0.7/popyrous/timeseries/sliding_window.py
--rw-rw-rw-   0        0        0      459 2023-01-19 16:12:28.000000 popyrous-0.0.7/popyrous/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-21 19:47:32.625406 popyrous-0.0.7/popyrous/web/
--rw-rw-rw-   0        0        0       24 2023-01-19 12:24:39.000000 popyrous-0.0.7/popyrous/web/__init__.py
--rw-rw-rw-   0        0        0     8751 2023-01-19 13:10:54.000000 popyrous-0.0.7/popyrous/web/download.py
-drwxrwxrwx   0        0        0        0 2023-01-21 19:47:32.626402 popyrous-0.0.7/popyrous/zipfiles/
--rw-rw-rw-   0        0        0       24 2023-01-19 13:21:58.000000 popyrous-0.0.7/popyrous/zipfiles/__init__.py
--rw-rw-rw-   0        0        0     1791 2023-01-19 13:28:12.000000 popyrous-0.0.7/popyrous/zipfiles/zipfiles.py
-drwxrwxrwx   0        0        0        0 2023-01-21 19:47:32.618429 popyrous-0.0.7/popyrous.egg-info/
--rw-rw-rw-   0        0        0     9278 2023-01-21 19:47:32.000000 popyrous-0.0.7/popyrous.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      779 2023-01-21 19:47:32.000000 popyrous-0.0.7/popyrous.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-21 19:47:32.000000 popyrous-0.0.7/popyrous.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-01-21 19:47:32.000000 popyrous-0.0.7/popyrous.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-01-21 19:47:32.000000 popyrous-0.0.7/popyrous.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-01-21 19:47:32.630389 popyrous-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1532 2023-01-21 19:46:46.000000 popyrous-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:30:03.386049 popyrous-0.0.8/
+-rw-rw-rw-   0        0        0     1072 2023-01-20 07:48:00.000000 popyrous-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     9279 2023-07-15 18:30:03.387223 popyrous-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     8532 2023-07-15 18:28:58.000000 popyrous-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 18:30:03.368582 popyrous-0.0.8/popyrous/
+-rw-rw-rw-   0        0        0      304 2023-01-21 19:46:08.000000 popyrous-0.0.8/popyrous/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:30:03.378077 popyrous-0.0.8/popyrous/matlab/
+-rw-rw-rw-   0        0        0       22 2023-01-19 13:24:02.000000 popyrous-0.0.8/popyrous/matlab/__init__.py
+-rw-rw-rw-   0        0        0     2537 2023-01-19 13:24:24.000000 popyrous-0.0.8/popyrous/matlab/matlab.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:30:03.379073 popyrous-0.0.8/popyrous/ml/
+-rw-rw-rw-   0        0        0       15 2023-01-21 13:53:00.000000 popyrous-0.0.8/popyrous/ml/__init__.py
+-rw-rw-rw-   0        0        0     4333 2023-01-21 13:54:45.000000 popyrous-0.0.8/popyrous/ml/confusion_matrix.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:30:03.380069 popyrous-0.0.8/popyrous/packages/
+-rw-rw-rw-   0        0        0       47 2023-01-19 11:52:33.000000 popyrous-0.0.8/popyrous/packages/__init__.py
+-rw-rw-rw-   0        0        0     6288 2023-01-19 11:55:04.000000 popyrous-0.0.8/popyrous/packages/packages.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:30:03.384057 popyrous-0.0.8/popyrous/timeseries/
+-rw-rw-rw-   0        0        0      185 2023-01-20 20:11:43.000000 popyrous-0.0.8/popyrous/timeseries/__init__.py
+-rw-rw-rw-   0        0        0     7172 2023-01-21 12:14:16.000000 popyrous-0.0.8/popyrous/timeseries/cwt.py
+-rw-rw-rw-   0        0        0    21072 2023-01-21 19:43:36.000000 popyrous-0.0.8/popyrous/timeseries/datasets.py
+-rw-rw-rw-   0        0        0    74704 2023-05-01 19:23:41.000000 popyrous-0.0.8/popyrous/timeseries/experiment.py
+-rw-rw-rw-   0        0        0     1781 2023-01-19 13:48:53.000000 popyrous-0.0.8/popyrous/timeseries/filt.py
+-rw-rw-rw-   0        0        0     2686 2023-01-19 16:08:55.000000 popyrous-0.0.8/popyrous/timeseries/metrics.py
+-rw-rw-rw-   0        0        0     1862 2022-08-06 15:20:20.000000 popyrous-0.0.8/popyrous/timeseries/recipe_577504_1.py
+-rw-rw-rw-   0        0        0     4342 2023-01-19 13:33:36.000000 popyrous-0.0.8/popyrous/timeseries/sliding_window.py
+-rw-rw-rw-   0        0        0      459 2023-01-19 16:12:28.000000 popyrous-0.0.8/popyrous/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:30:03.385053 popyrous-0.0.8/popyrous/web/
+-rw-rw-rw-   0        0        0       24 2023-01-19 12:24:39.000000 popyrous-0.0.8/popyrous/web/__init__.py
+-rw-rw-rw-   0        0        0     8751 2023-01-19 13:10:54.000000 popyrous-0.0.8/popyrous/web/download.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:30:03.386049 popyrous-0.0.8/popyrous/zipfiles/
+-rw-rw-rw-   0        0        0       24 2023-01-19 13:21:58.000000 popyrous-0.0.8/popyrous/zipfiles/__init__.py
+-rw-rw-rw-   0        0        0     1791 2023-01-19 13:28:12.000000 popyrous-0.0.8/popyrous/zipfiles/zipfiles.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:30:03.377062 popyrous-0.0.8/popyrous.egg-info/
+-rw-rw-rw-   0        0        0     9279 2023-07-15 18:30:03.000000 popyrous-0.0.8/popyrous.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      779 2023-07-15 18:30:03.000000 popyrous-0.0.8/popyrous.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 18:30:03.000000 popyrous-0.0.8/popyrous.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-07-15 18:30:03.000000 popyrous-0.0.8/popyrous.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-15 18:30:03.000000 popyrous-0.0.8/popyrous.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-15 18:30:03.391404 popyrous-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1532 2023-07-15 18:29:18.000000 popyrous-0.0.8/setup.py
```

### Comparing `popyrous-0.0.7/LICENSE.txt` & `popyrous-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.7/PKG-INFO` & `popyrous-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popyrous
-Version: 0.0.7
+Version: 0.0.8
 Summary: Pouya's Python routines. A collection of useful Python routines for everyday and professional life.
 Home-page: https://github.com/pniaz20/popyrous
 Author: Pouya P. Niaz
 Author-email: <pniaz20@ku.edu.tr>
 License: MIT
 Keywords: python,routines,matlab,zipfile,packages,time series,filtering,download,web
 Classifier: Development Status :: 3 - Alpha
@@ -18,16 +18,16 @@
 License-File: LICENSE.txt
 
 # Popyrous
 
 (Pouya's Python Routines) A collection of useful Python routines for science, research, development, and everyday life.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 0.0.7  
-Last Update: 21 Jan, 2023
+Version: 0.0.8  
+Last Update: July 15, 2023
 
 This is a collection of Python routines for the following purposes:
 
 - Checking for packages and installing missing ones iwithin scripts without the need for Jupyter and symbols like "!" and "%".
 - Reading and writing `.mat` files coming to/from MathWorks MATLAB software.
 - Building and manipulating time series data using sliding windows, low-pass filtering, etc.
 - Building flexible and easy-to-use datasets for data analysis or machine learning out of structured time series experiments (multiple subjects, conditions, repetitions, etc.).
```

### Comparing `popyrous-0.0.7/README.md` & `popyrous-0.0.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Popyrous
 
 (Pouya's Python Routines) A collection of useful Python routines for science, research, development, and everyday life.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 0.0.7  
-Last Update: 21 Jan, 2023
+Version: 0.0.8  
+Last Update: July 15, 2023
 
 This is a collection of Python routines for the following purposes:
 
 - Checking for packages and installing missing ones iwithin scripts without the need for Jupyter and symbols like "!" and "%".
 - Reading and writing `.mat` files coming to/from MathWorks MATLAB software.
 - Building and manipulating time series data using sliding windows, low-pass filtering, etc.
 - Building flexible and easy-to-use datasets for data analysis or machine learning out of structured time series experiments (multiple subjects, conditions, repetitions, etc.).
```

### Comparing `popyrous-0.0.7/popyrous/matlab/matlab.py` & `popyrous-0.0.8/popyrous/matlab/matlab.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.7/popyrous/ml/confusion_matrix.py` & `popyrous-0.0.8/popyrous/ml/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.7/popyrous/packages/packages.py` & `popyrous-0.0.8/popyrous/packages/packages.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.7/popyrous/timeseries/cwt.py` & `popyrous-0.0.8/popyrous/timeseries/cwt.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.7/popyrous/timeseries/datasets.py` & `popyrous-0.0.8/popyrous/timeseries/datasets.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.7/popyrous/timeseries/experiment.py` & `popyrous-0.0.8/popyrous/timeseries/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 SEED = 42
 
 import numpy as np
 import pandas as pd
 from sklearn.model_selection import train_test_split
+import warnings
 
 if __name__ == "popyrous.timeseries.experiment":
     from . datasets import make_squeezed_dataset, make_unsqueezed_dataset
     from . filt import butter_lowpass_filter_forward
     from . recipe_577504_1 import total_size
 else:
     from datasets import make_squeezed_dataset, make_unsqueezed_dataset
@@ -376,22 +377,32 @@
                             is_test_arr[subj, ctrl, trial] = None
                             if verbosity == 2: print("[skip]")
                             continue
                     
                     # Update the array that stores if the trial is for training or testing        
                     is_test_arr[subj, ctrl, trial] = is_test
                     
-                    # Extract relevant columns of the data
+                    # Extract relevant trial of the data
                     data_trial = self.dataframe
                     if self.subjects_column:
                         data_trial = data_trial[data_trial[self.subjects_column] == subj+1]
                     if self.conditions_column:
                         data_trial = data_trial[data_trial[self.conditions_column] == ctrl+1]
                     if self.trials_column:
                         data_trial = data_trial[data_trial[self.trials_column] == trial+1]
+                    if len(data_trial) == 0: # There is no data in this particular trial
+                        print("")
+                        x_arrays[subj, ctrl, trial] = []
+                        y_arrays[subj, ctrl, trial] = []
+                        data_arrays_orig[subj, ctrl, trial] = {}
+                        data_arrays_processed[subj, ctrl, trial] = {}
+                        is_test_arr[subj, ctrl, trial] = None
+                        print("")
+                        warnings.warn("No data found for subject %d, condition %d, trial %d. Skipping ..."%(subj+1, ctrl+1, trial+1), RuntimeWarning)
+                        continue
                     if verbosity == 2: print(data_trial.shape, end="")
                     
                     # Input Preprocessing
                     data_in = data_trial[self.input_cols] if self.input_cols else data_trial
                     if self.input_preprocessor:
                         x = self.input_preprocessor(data_in)
                     else:
@@ -908,22 +919,32 @@
                         
                 is_test_arr[subj, ctrl, trial] = is_test
                 # data_trial = dataframe[
                 #     (dataframe[subjects_column] == subj+1) & \
                 #     (dataframe[conditions_column] == ctrl+1) & \
                 #     (dataframe[trials_column] == trial+1)]
                 
-                # Extract relevant columns of the data
+                # Extract relevant trial of the data
                 data_trial = dataframe
                 if subjects_column:
                     data_trial = data_trial[data_trial[subjects_column] == subj+1]
                 if conditions_column:
                     data_trial = data_trial[data_trial[conditions_column] == ctrl+1]
                 if trials_column:
                     data_trial = data_trial[data_trial[trials_column] == trial+1]
+                if len(data_trial) == 0: # There is no data in this particular trial
+                    print("")
+                    x_arrays[subj, ctrl, trial] = []
+                    y_arrays[subj, ctrl, trial] = []
+                    data_arrays_orig[subj, ctrl, trial] = {}
+                    data_arrays_processed[subj, ctrl, trial] = {}
+                    is_test_arr[subj, ctrl, trial] = None
+                    print("")
+                    warnings.warn("No data found for subject %d, condition %d, trial %d. Skipping ..."%(subj+1, ctrl+1, trial+1), RuntimeWarning)
+                    continue
                 if verbosity == 2: print(data_trial.shape, end="")
                 
                 # Input Preprocessing
                 data_in = data_trial[input_cols] if input_cols else data_trial
                 if input_preprocessor:
                     x = input_preprocessor(data_in)
                 else:
```

### Comparing `popyrous-0.0.7/popyrous/timeseries/filt.py` & `popyrous-0.0.8/popyrous/timeseries/filt.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.7/popyrous/timeseries/metrics.py` & `popyrous-0.0.8/popyrous/timeseries/metrics.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.7/popyrous/timeseries/recipe_577504_1.py` & `popyrous-0.0.8/popyrous/timeseries/recipe_577504_1.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.7/popyrous/timeseries/sliding_window.py` & `popyrous-0.0.8/popyrous/timeseries/sliding_window.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.7/popyrous/web/download.py` & `popyrous-0.0.8/popyrous/web/download.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.7/popyrous/zipfiles/zipfiles.py` & `popyrous-0.0.8/popyrous/zipfiles/zipfiles.py`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.7/popyrous.egg-info/PKG-INFO` & `popyrous-0.0.8/popyrous.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popyrous
-Version: 0.0.7
+Version: 0.0.8
 Summary: Pouya's Python routines. A collection of useful Python routines for everyday and professional life.
 Home-page: https://github.com/pniaz20/popyrous
 Author: Pouya P. Niaz
 Author-email: <pniaz20@ku.edu.tr>
 License: MIT
 Keywords: python,routines,matlab,zipfile,packages,time series,filtering,download,web
 Classifier: Development Status :: 3 - Alpha
@@ -18,16 +18,16 @@
 License-File: LICENSE.txt
 
 # Popyrous
 
 (Pouya's Python Routines) A collection of useful Python routines for science, research, development, and everyday life.
 
 Author: Pouya P. Niaz (<pniaz20@ku.edu.tr> , <pouya.p.niaz@gmail.com>)  
-Version: 0.0.7  
-Last Update: 21 Jan, 2023
+Version: 0.0.8  
+Last Update: July 15, 2023
 
 This is a collection of Python routines for the following purposes:
 
 - Checking for packages and installing missing ones iwithin scripts without the need for Jupyter and symbols like "!" and "%".
 - Reading and writing `.mat` files coming to/from MathWorks MATLAB software.
 - Building and manipulating time series data using sliding windows, low-pass filtering, etc.
 - Building flexible and easy-to-use datasets for data analysis or machine learning out of structured time series experiments (multiple subjects, conditions, repetitions, etc.).
```

### Comparing `popyrous-0.0.7/popyrous.egg-info/SOURCES.txt` & `popyrous-0.0.8/popyrous.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `popyrous-0.0.7/setup.py` & `popyrous-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
-VERSION = '0.0.7' 
+VERSION = '0.0.8' 
 DESCRIPTION = "Pouya's Python routines. A collection of useful Python routines for everyday and professional life."
 
 # Setting up
 setup(
        # the name must match the folder name
         name="popyrous", 
         version=VERSION,
```

