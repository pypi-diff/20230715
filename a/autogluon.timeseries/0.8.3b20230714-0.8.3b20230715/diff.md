# Comparing `tmp/autogluon.timeseries-0.8.3b20230714.tar.gz` & `tmp/autogluon.timeseries-0.8.3b20230715.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-0.8.3b20230714.tar", last modified: Fri Jul 14 09:04:23 2023, max compression
+gzip compressed data, was "autogluon.timeseries-0.8.3b20230715.tar", last modified: Sat Jul 15 09:04:22 2023, max compression
```

## Comparing `autogluon.timeseries-0.8.3b20230714.tar` & `autogluon.timeseries-0.8.3b20230715.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:04:23.509597 autogluon.timeseries-0.8.3b20230714/
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-14 09:04:23.509597 autogluon.timeseries-0.8.3b20230714/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 09:04:23.509597 autogluon.timeseries-0.8.3b20230714/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:04:23.505597 autogluon.timeseries-0.8.3b20230714/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:04:23.505597 autogluon.timeseries-0.8.3b20230714/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:04:23.505597 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:04:23.505597 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:04:23.505597 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37845 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:04:23.505597 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:04:23.505597 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19492 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:04:23.505597 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17338 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)    16645 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:04:23.509597 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:04:23.509597 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:04:23.509597 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/gluonts/mx/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/gluonts/mx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/gluonts/mx/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/gluonts/mx/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:04:23.509597 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:04:23.509597 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/local/statsforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/local/statsmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:04:23.509597 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    49484 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:04:23.509597 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48122 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:04:23.509597 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/utils/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-14 09:03:44.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 09:04:23.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:04:23.505597 autogluon.timeseries-0.8.3b20230714/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-14 09:04:23.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-14 09:04:23.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:04:23.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 09:04:23.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-14 09:04:23.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 09:04:23.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:04:23.000000 autogluon.timeseries-0.8.3b20230714/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:04:22.247259 autogluon.timeseries-0.8.3b20230715/
+-rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-15 09:04:22.247259 autogluon.timeseries-0.8.3b20230715/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 09:04:22.247259 autogluon.timeseries-0.8.3b20230715/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:04:22.239259 autogluon.timeseries-0.8.3b20230715/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:04:22.239259 autogluon.timeseries-0.8.3b20230715/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:04:22.243259 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:04:22.243259 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:04:22.243259 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37845 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:04:22.243259 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:04:22.243259 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19492 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:04:22.243259 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17338 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16645 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:04:22.243259 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:04:22.243259 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:04:22.243259 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/gluonts/mx/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/gluonts/mx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/gluonts/mx/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/gluonts/mx/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:04:22.243259 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:04:22.247259 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/local/statsforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/local/statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:04:22.247259 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49484 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:04:22.247259 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48122 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:04:22.247259 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/utils/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-15 09:03:41.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-15 09:04:22.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:04:22.243259 autogluon.timeseries-0.8.3b20230715/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12682 2023-07-15 09:04:22.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-15 09:04:22.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 09:04:22.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-15 09:04:22.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-15 09:04:22.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-15 09:04:22.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 09:04:22.000000 autogluon.timeseries-0.8.3b20230715/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-0.8.3b20230714/PKG-INFO` & `autogluon.timeseries-0.8.3b20230715/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.8.3b20230714
+Version: 0.8.3b20230715
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.8.3b20230714/setup.py` & `autogluon.timeseries-0.8.3b20230715/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/__init__.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/evaluator.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/evaluator.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/gluonts/mx/__init__.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/gluonts/mx/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/gluonts/mx/callback.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/gluonts/mx/callback.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/gluonts/mx/models.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/gluonts/mx/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/local/__init__.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/local/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/local/statsmodels.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/local/statsmodels.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/models/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/predictor.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/utils/seasonality.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/utils/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-0.8.3b20230715/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-0.8.3b20230715/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.8.3b20230714
+Version: 0.8.3b20230715
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.8.3b20230714/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-0.8.3b20230715/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

