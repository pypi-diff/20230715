# Comparing `tmp/sherpa-onnx-1.5.1.tar.gz` & `tmp/sherpa-onnx-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa-onnx-1.5.1.tar", last modified: Thu Jul 13 07:13:09 2023, max compression
+gzip compressed data, was "sherpa-onnx-1.5.2.tar", last modified: Fri Jul 14 10:49:01 2023, max compression
```

## Comparing `sherpa-onnx-1.5.1.tar` & `sherpa-onnx-1.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:13:09.986547 sherpa-onnx-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-13 07:01:53.000000 sherpa-onnx-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-13 07:13:09.982547 sherpa-onnx-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-13 07:01:53.000000 sherpa-onnx-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 07:13:09.986547 sherpa-onnx-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-13 07:01:53.000000 sherpa-onnx-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:13:09.982547 sherpa-onnx-1.5.1/sherpa-onnx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:13:09.982547 sherpa-onnx-1.5.1/sherpa-onnx/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:13:09.982547 sherpa-onnx-1.5.1/sherpa-onnx/python/sherpa_onnx/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-13 07:13:09.000000 sherpa-onnx-1.5.1/sherpa-onnx/python/sherpa_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-13 07:01:53.000000 sherpa-onnx-1.5.1/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-07-13 07:01:53.000000 sherpa-onnx-1.5.1/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-13 07:01:53.000000 sherpa-onnx-1.5.1/sherpa-onnx/python/sherpa_onnx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 07:13:09.982547 sherpa-onnx-1.5.1/sherpa_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-13 07:13:09.000000 sherpa-onnx-1.5.1/sherpa_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-13 07:13:09.000000 sherpa-onnx-1.5.1/sherpa_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 07:13:09.000000 sherpa-onnx-1.5.1/sherpa_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 07:13:09.000000 sherpa-onnx-1.5.1/sherpa_onnx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-13 07:13:09.000000 sherpa-onnx-1.5.1/sherpa_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-13 07:13:09.000000 sherpa-onnx-1.5.1/sherpa_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:49:01.562237 sherpa-onnx-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-14 10:37:29.000000 sherpa-onnx-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-14 10:49:01.562237 sherpa-onnx-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-14 10:37:29.000000 sherpa-onnx-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:49:01.562237 sherpa-onnx-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-14 10:37:29.000000 sherpa-onnx-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:49:01.558237 sherpa-onnx-1.5.2/sherpa-onnx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:49:01.558237 sherpa-onnx-1.5.2/sherpa-onnx/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:49:01.562237 sherpa-onnx-1.5.2/sherpa-onnx/python/sherpa_onnx/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-14 10:49:01.000000 sherpa-onnx-1.5.2/sherpa-onnx/python/sherpa_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-07-14 10:37:29.000000 sherpa-onnx-1.5.2/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-07-14 10:37:29.000000 sherpa-onnx-1.5.2/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-14 10:37:29.000000 sherpa-onnx-1.5.2/sherpa-onnx/python/sherpa_onnx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:49:01.562237 sherpa-onnx-1.5.2/sherpa_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-14 10:49:01.000000 sherpa-onnx-1.5.2/sherpa_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-14 10:49:01.000000 sherpa-onnx-1.5.2/sherpa_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:49:01.000000 sherpa-onnx-1.5.2/sherpa_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:49:01.000000 sherpa-onnx-1.5.2/sherpa_onnx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 10:49:01.000000 sherpa-onnx-1.5.2/sherpa_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-14 10:49:01.000000 sherpa-onnx-1.5.2/sherpa_onnx.egg-info/top_level.txt
```

### Comparing `sherpa-onnx-1.5.1/LICENSE` & `sherpa-onnx-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.5.1/PKG-INFO` & `sherpa-onnx-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.5.1
+Version: 1.5.2
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

### Comparing `sherpa-onnx-1.5.1/setup.py` & `sherpa-onnx-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.5.1/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py` & `sherpa-onnx-1.5.2/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,15 @@
                 decoder_filename=decoder,
                 joiner_filename=joiner,
             ),
             tokens=tokens,
             num_threads=num_threads,
             debug=debug,
             provider=provider,
+            model_type="transducer",
         )
 
         feat_config = OfflineFeatureExtractorConfig(
             sampling_rate=sample_rate,
             feature_dim=feature_dim,
         )
 
@@ -145,14 +146,15 @@
         self = cls.__new__(cls)
         model_config = OfflineModelConfig(
             paraformer=OfflineParaformerModelConfig(model=paraformer),
             tokens=tokens,
             num_threads=num_threads,
             debug=debug,
             provider=provider,
+            model_type="paraformer",
         )
 
         feat_config = OfflineFeatureExtractorConfig(
             sampling_rate=sample_rate,
             feature_dim=feature_dim,
         )
 
@@ -207,14 +209,15 @@
         self = cls.__new__(cls)
         model_config = OfflineModelConfig(
             nemo_ctc=OfflineNemoEncDecCtcModelConfig(model=model),
             tokens=tokens,
             num_threads=num_threads,
             debug=debug,
             provider=provider,
+            model_type="nemo_ctc",
         )
 
         feat_config = OfflineFeatureExtractorConfig(
             sampling_rate=sample_rate,
             feature_dim=feature_dim,
         )
```

### Comparing `sherpa-onnx-1.5.1/sherpa-onnx/python/sherpa_onnx/online_recognizer.py` & `sherpa-onnx-1.5.2/sherpa-onnx/python/sherpa_onnx/online_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.5.1/sherpa-onnx/python/sherpa_onnx/utils.py` & `sherpa-onnx-1.5.2/sherpa-onnx/python/sherpa_onnx/utils.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.5.1/sherpa_onnx.egg-info/PKG-INFO` & `sherpa-onnx-1.5.2/sherpa_onnx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.5.1
+Version: 1.5.2
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

