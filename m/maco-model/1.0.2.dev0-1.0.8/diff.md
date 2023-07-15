# Comparing `tmp/maco-model-1.0.2.dev0.tar.gz` & `tmp/maco-model-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maco-model-1.0.2.dev0.tar", last modified: Sat Jul 15 07:03:41 2023, max compression
+gzip compressed data, was "maco-model-1.0.8.tar", last modified: Sat Jul 15 07:09:36 2023, max compression
```

## Comparing `maco-model-1.0.2.dev0.tar` & `maco-model-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:03:41.833991 maco-model-1.0.2.dev0/
--rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-07-15 07:03:41.833991 maco-model-1.0.2.dev0/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:03:41.829991 maco-model-1.0.2.dev0/maco/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-15 07:03:12.000000 maco-model-1.0.2.dev0/maco/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2555 2023-07-15 07:03:12.000000 maco-model-1.0.2.dev0/maco/base_test.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7539 2023-07-15 07:03:12.000000 maco-model-1.0.2.dev0/maco/cli.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5598 2023-07-15 07:03:12.000000 maco-model-1.0.2.dev0/maco/collector.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2973 2023-07-15 07:03:12.000000 maco-model-1.0.2.dev0/maco/extractor.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:03:41.829991 maco-model-1.0.2.dev0/maco/model/
--rw-r--r--   0 vsts      (1001) docker     (122)       31 2023-07-15 07:03:12.000000 maco-model-1.0.2.dev0/maco/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18082 2023-07-15 07:03:12.000000 maco-model-1.0.2.dev0/maco/model/model.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:03:41.829991 maco-model-1.0.2.dev0/maco_model.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-07-15 07:03:41.000000 maco-model-1.0.2.dev0/maco_model.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      303 2023-07-15 07:03:41.000000 maco-model-1.0.2.dev0/maco_model.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-15 07:03:41.000000 maco-model-1.0.2.dev0/maco_model.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       17 2023-07-15 07:03:41.000000 maco-model-1.0.2.dev0/maco_model.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-07-15 07:03:41.000000 maco-model-1.0.2.dev0/maco_model.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-07-15 07:03:41.833991 maco-model-1.0.2.dev0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      388 2023-07-15 07:03:12.000000 maco-model-1.0.2.dev0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:09:36.825203 maco-model-1.0.8/
+-rw-r--r--   0 vsts      (1001) docker     (122)      101 2023-07-15 07:09:36.825203 maco-model-1.0.8/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:09:36.821203 maco-model-1.0.8/maco/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-15 07:09:09.000000 maco-model-1.0.8/maco/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2555 2023-07-15 07:09:09.000000 maco-model-1.0.8/maco/base_test.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7539 2023-07-15 07:09:09.000000 maco-model-1.0.8/maco/cli.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5598 2023-07-15 07:09:09.000000 maco-model-1.0.8/maco/collector.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2973 2023-07-15 07:09:09.000000 maco-model-1.0.8/maco/extractor.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:09:36.821203 maco-model-1.0.8/maco/model/
+-rw-r--r--   0 vsts      (1001) docker     (122)       31 2023-07-15 07:09:09.000000 maco-model-1.0.8/maco/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18082 2023-07-15 07:09:09.000000 maco-model-1.0.8/maco/model/model.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-15 07:09:36.825203 maco-model-1.0.8/maco_model.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)      101 2023-07-15 07:09:36.000000 maco-model-1.0.8/maco_model.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      303 2023-07-15 07:09:36.000000 maco-model-1.0.8/maco_model.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-15 07:09:36.000000 maco-model-1.0.8/maco_model.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       17 2023-07-15 07:09:36.000000 maco-model-1.0.8/maco_model.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-07-15 07:09:36.000000 maco-model-1.0.8/maco_model.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       38 2023-07-15 07:09:36.825203 maco-model-1.0.8/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      388 2023-07-15 07:09:09.000000 maco-model-1.0.8/setup.py
```

### Comparing `maco-model-1.0.2.dev0/maco/base_test.py` & `maco-model-1.0.8/maco/base_test.py`

 * *Files identical despite different names*

### Comparing `maco-model-1.0.2.dev0/maco/cli.py` & `maco-model-1.0.8/maco/cli.py`

 * *Files identical despite different names*

### Comparing `maco-model-1.0.2.dev0/maco/collector.py` & `maco-model-1.0.8/maco/collector.py`

 * *Files identical despite different names*

### Comparing `maco-model-1.0.2.dev0/maco/extractor.py` & `maco-model-1.0.8/maco/extractor.py`

 * *Files identical despite different names*

### Comparing `maco-model-1.0.2.dev0/maco/model/model.py` & `maco-model-1.0.8/maco/model/model.py`

 * *Files identical despite different names*

