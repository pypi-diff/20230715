# Comparing `tmp/featdist-0.1.5.tar.gz` & `tmp/featdist-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featdist-0.1.5.tar", last modified: Wed Jul  5 07:36:40 2023, max compression
+gzip compressed data, was "featdist-0.1.6.tar", last modified: Sat Jul 15 06:53:22 2023, max compression
```

## Comparing `featdist-0.1.5.tar` & `featdist-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:36:40.052848 featdist-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-05 07:36:26.000000 featdist-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-05 07:36:40.052848 featdist-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-05 07:36:26.000000 featdist-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:36:40.052848 featdist-0.1.5/featdist/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-05 07:36:26.000000 featdist-0.1.5/featdist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18266 2023-07-05 07:36:26.000000 featdist-0.1.5/featdist/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 07:36:40.052848 featdist-0.1.5/featdist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-05 07:36:40.000000 featdist-0.1.5/featdist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-05 07:36:40.000000 featdist-0.1.5/featdist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 07:36:40.000000 featdist-0.1.5/featdist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 07:36:40.000000 featdist-0.1.5/featdist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-05 07:36:40.000000 featdist-0.1.5/featdist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 07:36:40.052848 featdist-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-05 07:36:26.000000 featdist-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:53:22.579005 featdist-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-15 06:53:13.000000 featdist-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-15 06:53:22.579005 featdist-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-15 06:53:13.000000 featdist-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:53:22.579005 featdist-0.1.6/featdist/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-15 06:53:13.000000 featdist-0.1.6/featdist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18346 2023-07-15 06:53:13.000000 featdist-0.1.6/featdist/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:53:22.579005 featdist-0.1.6/featdist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-15 06:53:22.000000 featdist-0.1.6/featdist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-15 06:53:22.000000 featdist-0.1.6/featdist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:53:22.000000 featdist-0.1.6/featdist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-15 06:53:22.000000 featdist-0.1.6/featdist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 06:53:22.000000 featdist-0.1.6/featdist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:53:22.579005 featdist-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-15 06:53:13.000000 featdist-0.1.6/setup.py
```

### Comparing `featdist-0.1.5/LICENSE` & `featdist-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `featdist-0.1.5/PKG-INFO` & `featdist-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featdist
-Version: 0.1.5
+Version: 0.1.6
 Summary: Train test target distribution function for machine learning
 Home-page: https://github.com/Hasan-Basri-Akcay/featdist
 Author: Hasan Basri Akcay
 Author-email: hasan.basri.akcay@gmail.com
 Keywords: python,data science,data analysis,exploratory data analysis,distribution,beginner
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
```

### Comparing `featdist-0.1.5/README.md` & `featdist-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `featdist-0.1.5/featdist/base.py` & `featdist-0.1.6/featdist/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     plt.show()
     df_stats.dropna(axis=1, inplace=True)
     if val is not None:  df_stats.sort_values('train_val_trend_corr', inplace=True, ascending=False), val.drop('bin', axis=1, inplace=True)
     if test is not None:  df_stats.sort_values('train_test_trend_corr', inplace=True, ascending=False), test.drop('bin', axis=1, inplace=True)
     return df_stats
 
 
-def categorical_ttt_dist(train=None, test=None, val=None, features=[], target='target', ncols=3, s='auto', agg_func='mean', figsize=16, ylim=(), sharey=False, anova=True):
+def categorical_ttt_dist(train=None, test=None, val=None, features=[], target='target', ncols=3, s='auto', agg_func='mean', labelrotation=0, figsize=16, ylim=(), sharey=False, anova=True):
     '''
     The Categorical Train Test Target Distribution function helps us to understand data distribution better. It can plot train, test, validation, and the target in 
     one graph for each feature.
 
     Args:
         train (DataFrame): the train dataframe containing features and target columns.
         test (DataFrame): the test dataframe containing features.
@@ -258,14 +258,15 @@
                     loc="upper left",
                 )
             at.patch.set_boxstyle("square, pad=0.0")
             ax.add_artist(at)
         
         ax.bar(train_counts.index, train_counts.values, alpha=alpha, label='train', color='tab:cyan')
         if test is not None: ax.bar(test_counts.index, test_counts.values, alpha=alpha, label='test', color='tab:red')
+        ax.tick_params(axis='x', labelrotation=labelrotation)
         ax2 = ax.twinx()
         ax2.scatter(train_group.index, train_group[target], label='train target rate', color='tab:purple', s=s)
         
         if val is not None:  
             val_group = val.groupby(feature).agg({target:agg_func})
             ax.bar(val_counts.index, val_counts.values, alpha=alpha, label='val', color='tab:gray')
             ax2.scatter(val_group.index, val_group[target], label='val target rate', color='tab:gray', s=s)
```

### Comparing `featdist-0.1.5/featdist.egg-info/PKG-INFO` & `featdist-0.1.6/featdist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featdist
-Version: 0.1.5
+Version: 0.1.6
 Summary: Train test target distribution function for machine learning
 Home-page: https://github.com/Hasan-Basri-Akcay/featdist
 Author: Hasan Basri Akcay
 Author-email: hasan.basri.akcay@gmail.com
 Keywords: python,data science,data analysis,exploratory data analysis,distribution,beginner
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
```

### Comparing `featdist-0.1.5/setup.py` & `featdist-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="featdist",
-    version="v0.1.5",
+    version="v0.1.6",
     author="Hasan Basri Akcay",
     author_email="hasan.basri.akcay@gmail.com",
     description="Train test target distribution function for machine learning",
     long_description=(
         "Featdist (Train Test Target Distribution) helps with feature understanding, "
         "calculating feature importances, feature comparison, feature debugging, and "
         "leakage detection"
```

