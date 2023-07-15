# Comparing `tmp/prolog_primitives-1.1.2.tar.gz` & `tmp/prolog_primitives-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prolog_primitives-1.1.2.tar", last modified: Fri Jul 14 18:08:17 2023, max compression
+gzip compressed data, was "prolog_primitives-1.2.0.tar", last modified: Sat Jul 15 16:27:09 2023, max compression
```

## Comparing `prolog_primitives-1.1.2.tar` & `prolog_primitives-1.2.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.694581 prolog_primitives-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-14 18:08:17.694581 prolog_primitives-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 18:08:17.000000 prolog_primitives-1.1.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.682581 prolog_primitives-1.1.2/prolog_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.686581 prolog_primitives-1.1.2/prolog_primitives/basic/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/basic/DBManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/basic/DistributedElements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/basic/PrimitiveWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/basic/Session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/basic/SubRequestEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/basic/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/basic/filterKbPrimitive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/basic/nt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.686581 prolog_primitives-1.1.2/prolog_primitives/generatedProto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/generatedProto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/generatedProto/basicMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/generatedProto/errorsMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/generatedProto/primitiveService_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-14 18:07:51.000000 prolog_primitives-1.1.2/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.686581 prolog_primitives-1.1.2/prolog_primitives/ml_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.690581 prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/fold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/randomSplit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/theoryToDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.690581 prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.690581 prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/score.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.694581 prolog_primitives-1.1.2/prolog_primitives/ml_lib/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/schema/schemaClass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/schema/theoryToSchema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.694581 prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/one_hot_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/schema_trasformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/transformationClass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:08:17.682581 prolog_primitives-1.1.2/prolog_primitives.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-14 18:08:17.000000 prolog_primitives-1.1.2/prolog_primitives.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-14 18:08:17.000000 prolog_primitives-1.1.2/prolog_primitives.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:08:17.000000 prolog_primitives-1.1.2/prolog_primitives.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:08:17.000000 prolog_primitives-1.1.2/prolog_primitives.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-14 18:08:17.000000 prolog_primitives-1.1.2/prolog_primitives.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 18:08:17.000000 prolog_primitives-1.1.2/prolog_primitives.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 18:08:17.694581 prolog_primitives-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-14 18:06:40.000000 prolog_primitives-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.495995 prolog_primitives-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-15 16:27:09.495995 prolog_primitives-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-15 16:27:09.000000 prolog_primitives-1.2.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.487995 prolog_primitives-1.2.0/prolog_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.487995 prolog_primitives-1.2.0/prolog_primitives/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/basic/DBManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/basic/DistributedElements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/basic/PrimitiveWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/basic/Session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/basic/SubRequestEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/basic/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/basic/filterKbPrimitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/basic/nt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.487995 prolog_primitives-1.2.0/prolog_primitives/generatedProto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/generatedProto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7223 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/generatedProto/basicMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/generatedProto/basicMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/generatedProto/errorsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/generatedProto/errorsMessages_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9189 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/generatedProto/primitiveService_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-15 16:26:44.000000 prolog_primitives-1.2.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.487995 prolog_primitives-1.2.0/prolog_primitives/ml_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.491995 prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/fold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/randomSplit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/theoryToDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.491995 prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.491995 prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.495995 prolog_primitives-1.2.0/prolog_primitives/ml_lib/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/schema/schemaClass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/schema/theoryToSchema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.495995 prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/one_hot_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/schema_trasformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/transformationClass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:27:09.487995 prolog_primitives-1.2.0/prolog_primitives.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-15 16:27:09.000000 prolog_primitives-1.2.0/prolog_primitives.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-15 16:27:09.000000 prolog_primitives-1.2.0/prolog_primitives.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 16:27:09.000000 prolog_primitives-1.2.0/prolog_primitives.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 16:27:09.000000 prolog_primitives-1.2.0/prolog_primitives.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-15 16:27:09.000000 prolog_primitives-1.2.0/prolog_primitives.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 16:27:09.000000 prolog_primitives-1.2.0/prolog_primitives.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 16:27:09.495995 prolog_primitives-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-15 16:25:32.000000 prolog_primitives-1.2.0/setup.py
```

### Comparing `prolog_primitives-1.1.2/LICENSE` & `prolog_primitives-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/PKG-INFO` & `prolog_primitives-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog_primitives
-Version: 1.1.2
+Version: 1.2.0
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-1.1.2/prolog_primitives/basic/DBManager.py` & `prolog_primitives-1.2.0/prolog_primitives/basic/DBManager.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/basic/DistributedElements.py` & `prolog_primitives-1.2.0/prolog_primitives/basic/DistributedElements.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/basic/PrimitiveWrapper.py` & `prolog_primitives-1.2.0/prolog_primitives/basic/PrimitiveWrapper.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/basic/Session.py` & `prolog_primitives-1.2.0/prolog_primitives/basic/Session.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/basic/SubRequestEvent.py` & `prolog_primitives-1.2.0/prolog_primitives/basic/SubRequestEvent.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/basic/Utils.py` & `prolog_primitives-1.2.0/prolog_primitives/basic/Utils.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/basic/filterKbPrimitive.py` & `prolog_primitives-1.2.0/prolog_primitives/basic/filterKbPrimitive.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/basic/nt.py` & `prolog_primitives-1.2.0/prolog_primitives/basic/nt.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/generatedProto/basicMessages_pb2.py` & `prolog_primitives-1.2.0/prolog_primitives/generatedProto/basicMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/generatedProto/errorsMessages_pb2.py` & `prolog_primitives-1.2.0/prolog_primitives/generatedProto/errorsMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/generatedProto/primitiveService_pb2.py` & `prolog_primitives-1.2.0/prolog_primitives/generatedProto/primitiveService_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py` & `prolog_primitives-1.2.0/prolog_primitives/generatedProto/primitiveService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py` & `prolog_primitives-1.2.0/prolog_primitives/generatedProto/sideEffectsMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/collections.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/collections.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/cell.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/cell.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/column.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/column.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/fold.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/fold.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/randomSplit.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/randomSplit.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/row.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/row.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/theoryToDataset.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/theoryToDataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,25 +22,25 @@
             for i in request.inspectKb(
                 primitiveMsg.InspectKbMsg.STATIC,
                 [(primitiveMsg.InspectKbMsg.STARTS_WITH, str(Utils.parseArgumentMsg(schema_name)))]):    
                 if(i == None and len(data) == 0):
                     yield request.replyFail()
                 elif(i != None):
                     i = Utils.parseStructMsg(i.arguments[0].struct)
-                    for j in zip(schema.attributes, i.arguments):
-                        value = j[0].typeCastElement(str(j[1]))
+                    for attr, arg in zip(schema.attributes, i.arguments):
+                        value = attr.typeCastElement(arg)
                         if(value == None):
                             yield request.replyError(primitiveMsg.ErrorMsg(
-                                message = "One of " + j[0].name + " was not the correct type",
+                                message = "One of " + attr.name + " was not the correct type",
                                 context=request.context,
                                 resolutionException = errorMsg.ResolutionExceptionMsg()
                             ))
                             raise Exception("Wrong typecasting in attributes")
                         else:
-                            data[j[0].name].append(value)
+                            data[attr.name].append(value)
             
             dataset = Dataset.from_dict(data).with_format("tf")
             datasetId = SharedCollections().addDataset(dataset, schemaId)
             yield request.replySuccess(substitutions={
                 dataset_ref.var: Utils.buildConstantArgumentMsg(datasetId)
                 }, hasNext=False)
         else:
```

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/dataset/theory_from_Dataset.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/launcher.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/launcher.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/denseLayer.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,17 @@
             topology: list = SharedCollections().getTopology(Utils.parseArgumentMsg(topology_in_ref))
             
             activation = str(Utils.parseArgumentMsg(activation))
             if(activation == "identity"):
                 activation = None
 
             dense = tf.keras.layers.Dense(
-                units=int(Utils.parseArgumentMsg(size)),
+                units=Utils.parseArgumentMsg(size),
                 activation=activation,
-                name="dense_"+str(len(topology)))
+                name=f"dense_{len(topology)}")
             topology.append(dense)
             
             id = SharedCollections().addTopology(topology)
             yield request.replySuccess(substitutions={
                 topology_out_ref.var: Utils.buildConstantArgumentMsg(id)
                 }, hasNext=False)
         else:
```

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/inputLayer.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         size = request.arguments[0]
         topology_ref = request.arguments[1]
         
         if(not size.HasField('var') and topology_ref.HasField('var')):
             size = int(Utils.parseArgumentMsg(size))
-            id = SharedCollections().addTopology([tf.keras.Input(shape=(size,), name="input")])
+            id = SharedCollections().addTopology([tf.keras.layers.Input(shape=(size,), name="input")])
             yield request.replySuccess(substitutions={
                 topology_ref.var: Utils.buildConstantArgumentMsg(id)
                 }, hasNext=False)
         else:
             yield request.replyFail()
```

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/neuralNetwork.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,21 +10,15 @@
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         topology_ref = request.arguments[0]
         predictor_ref = request.arguments[1]
         
         if(not topology_ref.HasField('var') and predictor_ref.HasField('var')):
             topology = SharedCollections().getTopology(Utils.parseArgumentMsg(topology_ref))
             
-            output = topology[0]
-            for i in topology[1:]:
-                output = i(output)
-            
-            model = tf.keras.Model(
-                inputs=[topology[0]], outputs = [output]
-            )
+            model = tf.keras.Sequential(topology)
             
             id = SharedCollections().addModel(model)
             yield request.replySuccess(substitutions={
                 predictor_ref.var: Utils.buildConstantArgumentMsg(id)
                 }, hasNext=False)
         else:
             yield request.replyFail()
```

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/neuralNetwork/outputLayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
             topology: list = SharedCollections().getTopology(Utils.parseArgumentMsg(topology_in_ref))
             
             activation = str(Utils.parseArgumentMsg(activation))
             if(activation == "identity"):
                 activation = None
 
             output = tf.keras.layers.Dense(
-                units=int(Utils.parseArgumentMsg(size)),
+                units=Utils.parseArgumentMsg(size),
                 activation=activation,
                 name="output")
             topology.append(output)
             id = SharedCollections().addTopology(topology)
             yield request.replySuccess(substitutions={
                 topology_out_ref.var: Utils.buildConstantArgumentMsg(id)
                 }, hasNext=False)
```

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/classify.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/classify.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/predict.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/predict.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,20 +24,20 @@
                 schemaId = SharedCollections().getSchemaIdFromDataset(datasetId)
                 schema = SharedCollections().getSchema(schemaId)
                 data = list()
                 for attr in dataset.column_names:
                     if(not attr in schema.targets):
                         data.append(tf.cast(dataset[attr], tf.float32))
                 data = tf.stack(data, axis = 1)
+                
+                predictions = model.predict(x=data)
                 result = {}
-                for attr in schema.targets:
-                    result[attr] = []
-                for row in model.predict(x=data):
-                    for attr, y in zip(schema.targets, row):
-                        result[attr].append(y)
+                for target, values in zip(schema.targets, tf.reshape(predictions, (len(schema.targets), len(predictions)))):
+                    result[target] = values
+
                 dataset = Dataset.from_dict(result).with_format("tf")
                 datasetId = SharedCollections().addDataset(dataset, schemaId)
             
                 yield request.replySuccess(substitutions={
                     prediction_ref.var: Utils.buildConstantArgumentMsg(datasetId)
                     }, hasNext=False)
             else:
```

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/score.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/score.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/predictors/train.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/predictors/train.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,23 +14,21 @@
     }
     for struct in structs:
         if(struct.functor == "max_epoch"):
             params['epoch'] = int(struct.arguments[0])
         elif(struct.functor == "batch_size"):
             params['batch'] = int(struct.arguments[0])
         elif(struct.functor == "learning_rate"):
-            params['learning_rate'] = float(struct.arguments[0])
+            params['learning_rate'] = struct.arguments[0]
         elif(struct.functor == "loss"):
             loss = struct.arguments[0]
-            if(loss == "mse"):
-                params['loss'] = "mse"
-            elif(loss == "mae"):
-                params['loss'] = "mae"
-            elif(loss == "cross_entropy"):
+            if(loss == "cross_entropy"):
                 params['loss'] = tf.keras.losses.BinaryCrossentropy()
+            else: 
+                params['loss'] = loss
     return params
 
 class __Train(DistributedElements.DistributedPrimitive):
     
     def solve(self, request: DistributedElements.DistributedRequest) -> Generator[DistributedElements.DistributedResponse, None, None]:
         predictor_in_ref = request.arguments[0]
         dataset_ref = request.arguments[1]
@@ -41,35 +39,37 @@
            not params.HasField('var') and predictor_out_ref.HasField('var')):
             model: tf.keras.Model = SharedCollections().getModel(Utils.parseArgumentMsg(predictor_in_ref))
             datasetId = Utils.parseArgumentMsg(dataset_ref)
             dataset: Dataset = SharedCollections().getDataset(datasetId)
             schema = SharedCollections().getSchema(SharedCollections().getSchemaIdFromDataset(datasetId))
             
             params = Utils.parseArgumentMsg(params)
-            if(type(params) is list[Utils.Struct]):
+            if(type(params) is list):
                 params = parseParams(params)
             else:
-                params = parseParams(dict())
+                params = parseParams(list())
             input = list()
             output = list()
             for attr in dataset.column_names:
                 if(attr in schema.targets):
                     output.append(tf.cast(dataset[attr], tf.float32))
                 else:
                     input.append(tf.cast(dataset[attr], tf.float32))
+            
             output = tf.stack(output, axis = 1)
             input = tf.stack(input, axis = 1)
             optimizer = tf.keras.optimizers.Adam(learning_rate=params["learning_rate"])
             
             model.compile(
                 loss = params["loss"],
                 optimizer=optimizer,
-                metrics=['mae', 'mse'],
+                metrics=['mae'],
             )
-            model.fit(x=input,y=output, batch_size=params["batch"], epochs=params["epoch"])
+            model.fit(x=input,y=output,  epochs=params["epoch"], validation_split=0.05)
+            
             id = SharedCollections().addModel(model)
             yield request.replySuccess(substitutions={
                 predictor_out_ref.var: Utils.buildConstantArgumentMsg(id)
                 }, hasNext=False)
         else:
             yield request.replyFail()
```

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/schema/schema.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/schema/schema.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/schema/schemaClass.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/schema/schemaClass.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/schema/theoryToSchema.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/schema/theoryToSchema.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/drop.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/drop.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/fit.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/fit.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/normalization.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/normalization.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/one_hot_encode.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/one_hot_encode.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/schema_trasformation.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/schema_trasformation.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/transform.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/transform.py`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/prolog_primitives/ml_lib/transformations/transformationClass.py` & `prolog_primitives-1.2.0/prolog_primitives/ml_lib/transformations/transformationClass.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,15 @@
         
     def apply(self, inputs):
         output = {}
         for attr, layers in self.__layers.items():
             output[attr] = tf.reshape(inputs[attr], (len(inputs[attr]), 1))
             for layer in layers:  
                 output[attr] = layer.applier(output[attr])
+            output[attr] = tf.reshape(output[attr], len(inputs[attr]))
         return Dataset.from_dict(output)
         
     def invert(self, inputs):
         output = {}
         for attr, layers in self.__layers.items():
             reversedList = list(layers)
             reversedList.reverse()
```

### Comparing `prolog_primitives-1.1.2/prolog_primitives.egg-info/PKG-INFO` & `prolog_primitives-1.2.0/prolog_primitives.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prolog-primitives
-Version: 1.1.2
+Version: 1.2.0
 Summary: description here
 Home-page: https://github.com/lorenzo-osimani/prolog_primitives/
 Author: Lorenzo Osimani
 Author-email: lorenzo.osimani@studio.unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/lorenzo-osimani/prolog_primitives/issues
 Project-URL: Source, https://github.com/lorenzo-osimani/prolog_primitives/
```

### Comparing `prolog_primitives-1.1.2/prolog_primitives.egg-info/SOURCES.txt` & `prolog_primitives-1.2.0/prolog_primitives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prolog_primitives-1.1.2/setup.py` & `prolog_primitives-1.2.0/setup.py`

 * *Files identical despite different names*

