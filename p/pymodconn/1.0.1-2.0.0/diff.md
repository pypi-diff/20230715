# Comparing `tmp/pymodconn-1.0.1.tar.gz` & `tmp/pymodconn-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodconn-1.0.1.tar", last modified: Tue Jul 11 11:11:08 2023, max compression
+gzip compressed data, was "pymodconn-2.0.0.tar", last modified: Sat Jul 15 20:51:49 2023, max compression
```

## Comparing `pymodconn-1.0.1.tar` & `pymodconn-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:11:08.200735 pymodconn-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 11:10:56.000000 pymodconn-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-11 11:11:08.200735 pymodconn-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-11 11:10:56.000000 pymodconn-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:11:08.200735 pymodconn-1.0.1/pymodconn/
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/Decoder_class_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/Encoder_class_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/MHA_block_class_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/RNN_block_class_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/TCN_addnorm_class_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/cit_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:11:08.200735 pymodconn-1.0.1/pymodconn/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/configs/configs_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/keras_tcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/model_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/model_gen_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pymodconn/utils_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:11:08.200735 pymodconn-1.0.1/pymodconn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-07-11 11:11:08.000000 pymodconn-1.0.1/pymodconn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-11 11:11:08.000000 pymodconn-1.0.1/pymodconn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:11:08.000000 pymodconn-1.0.1/pymodconn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 11:11:08.000000 pymodconn-1.0.1/pymodconn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 11:10:56.000000 pymodconn-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-11 11:11:08.200735 pymodconn-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-11 11:10:56.000000 pymodconn-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:51:49.925483 pymodconn-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-15 20:51:38.000000 pymodconn-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25228 2023-07-15 20:51:49.925483 pymodconn-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24549 2023-07-15 20:51:38.000000 pymodconn-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:51:49.925483 pymodconn-2.0.0/pymodconn/
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-15 20:51:39.000000 pymodconn-2.0.0/pymodconn/Decoder_class_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-15 20:51:39.000000 pymodconn-2.0.0/pymodconn/Encoder_class_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-07-15 20:51:39.000000 pymodconn-2.0.0/pymodconn/MHA_block_class_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-07-15 20:51:39.000000 pymodconn-2.0.0/pymodconn/RNN_block_class_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-15 20:51:39.000000 pymodconn-2.0.0/pymodconn/TCN_addnorm_class_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-15 20:51:39.000000 pymodconn-2.0.0/pymodconn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-07-15 20:51:39.000000 pymodconn-2.0.0/pymodconn/cit_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:51:49.925483 pymodconn-2.0.0/pymodconn/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-15 20:51:39.000000 pymodconn-2.0.0/pymodconn/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-15 20:51:39.000000 pymodconn-2.0.0/pymodconn/configs/configs_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-07-15 20:51:39.000000 pymodconn-2.0.0/pymodconn/keras_tcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-07-15 20:51:39.000000 pymodconn-2.0.0/pymodconn/model_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-07-15 20:51:39.000000 pymodconn-2.0.0/pymodconn/model_gen_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-07-15 20:51:39.000000 pymodconn-2.0.0/pymodconn/utils_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:51:49.925483 pymodconn-2.0.0/pymodconn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25228 2023-07-15 20:51:49.000000 pymodconn-2.0.0/pymodconn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-15 20:51:49.000000 pymodconn-2.0.0/pymodconn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 20:51:49.000000 pymodconn-2.0.0/pymodconn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-15 20:51:49.000000 pymodconn-2.0.0/pymodconn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-15 20:51:39.000000 pymodconn-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-15 20:51:49.925483 pymodconn-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-15 20:51:39.000000 pymodconn-2.0.0/setup.py
```

### Comparing `pymodconn-1.0.1/LICENSE` & `pymodconn-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.1/pymodconn/Decoder_class_layer.py` & `pymodconn-2.0.0/pymodconn/Decoder_class_layer.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.1/pymodconn/Encoder_class_layer.py` & `pymodconn-2.0.0/pymodconn/Encoder_class_layer.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.1/pymodconn/MHA_block_class_function.py` & `pymodconn-2.0.0/pymodconn/MHA_block_class_function.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.1/pymodconn/RNN_block_class_function.py` & `pymodconn-2.0.0/pymodconn/RNN_block_class_function.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.1/pymodconn/TCN_addnorm_class_function.py` & `pymodconn-2.0.0/pymodconn/TCN_addnorm_class_function.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.1/pymodconn/cit_block.py` & `pymodconn-2.0.0/pymodconn/cit_block.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.1/pymodconn/configs/configs_init.py` & `pymodconn-2.0.0/pymodconn/configs/configs_init.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.1/pymodconn/keras_tcn.py` & `pymodconn-2.0.0/pymodconn/keras_tcn.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.1/pymodconn/model_gen.py` & `pymodconn-2.0.0/pymodconn/model_gen.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.1/pymodconn/model_gen_utils.py` & `pymodconn-2.0.0/pymodconn/model_gen_utils.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.1/pymodconn/utils_layers.py` & `pymodconn-2.0.0/pymodconn/utils_layers.py`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.1/pymodconn.egg-info/SOURCES.txt` & `pymodconn-2.0.0/pymodconn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymodconn-1.0.1/setup.cfg` & `pymodconn-2.0.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pymodconn
-version = 1.0.1
+version = 2.0.0
 author = Gaurav Chaudhary
 author_email = gaurav.chaudhary@ntnu.no
 description = Develops sequence to sequence control-oriented deep neural networks in a highly modular way.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/gaurav306/pymodconn
 classifiers =
```

