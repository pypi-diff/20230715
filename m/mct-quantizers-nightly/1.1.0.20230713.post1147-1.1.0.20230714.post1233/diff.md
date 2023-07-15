# Comparing `tmp/mct-quantizers-nightly-1.1.0.20230713.post1147.tar.gz` & `tmp/mct-quantizers-nightly-1.1.0.20230714.post1233.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-quantizers-nightly-1.1.0.20230713.post1147.tar", last modified: Thu Jul 13 00:11:47 2023, max compression
+gzip compressed data, was "mct-quantizers-nightly-1.1.0.20230714.post1233.tar", last modified: Fri Jul 14 00:12:35 2023, max compression
```

## Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147.tar` & `mct-quantizers-nightly-1.1.0.20230714.post1233.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.900499 mct-quantizers-nightly-1.1.0.20230713.post1147/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-13 00:11:47.900499 mct-quantizers-nightly-1.1.0.20230713.post1147/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.896499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.896499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/base_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/get_all_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/quant_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/quant_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.896499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.896499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.896499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.900499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8551 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/validation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.900499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.900499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.900499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.900499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-13 00:11:32.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:11:47.900499 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-07-13 00:11:47.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-13 00:11:47.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 00:11:47.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-13 00:11:47.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 00:11:47.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-13 00:11:47.900499 mct-quantizers-nightly-1.1.0.20230713.post1147/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-13 00:11:47.000000 mct-quantizers-nightly-1.1.0.20230713.post1147/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:12:35.188732 mct-quantizers-nightly-1.1.0.20230714.post1233/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-07-14 00:12:35.188732 mct-quantizers-nightly-1.1.0.20230714.post1233/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:12:35.184732 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:12:35.184732 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/common/base_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/common/get_all_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/common/quant_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/common/quant_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:12:35.184732 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:12:35.184732 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:12:35.184732 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:12:35.184732 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/validation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:12:35.184732 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:12:35.188732 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:12:35.188732 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:12:35.188732 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-07-14 00:12:19.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 00:12:35.188732 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-07-14 00:12:34.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-07-14 00:12:35.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 00:12:34.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 00:12:34.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 00:12:34.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-14 00:12:35.188732 mct-quantizers-nightly-1.1.0.20230714.post1233/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-14 00:12:33.000000 mct-quantizers-nightly-1.1.0.20230714.post1233/setup.py
```

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/LICENSE.md` & `mct-quantizers-nightly-1.1.0.20230714.post1233/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/PKG-INFO` & `mct-quantizers-nightly-1.1.0.20230714.post1233/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.1.0.20230713.post1147
+Version: 1.1.0.20230714.post1233
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT) Quantizers
         
         The MCT Quantizers library is an open-source library developed by researchers and engineers working at Sony Semiconductor Israel. 
         
@@ -58,17 +58,16 @@
         pip install mct-quantizers-nightly
         ```
         
         ### Requirements
         
         To use MCT Quantizers, you need to have one of the supported frameworks, Tensorflow or PyTorch, installed.
         
-        For use with Tensorflow, please install the following packages:
-        [tensorflow](https://www.tensorflow.org/install), 
-        [tensorflow-model-optimization](https://www.tensorflow.org/model_optimization/guide/install)
+        For use with Tensorflow, please install the following package:
+        [tensorflow](https://www.tensorflow.org/install),
         
         For use with PyTorch, please install the following package:
         [torch](https://pytorch.org/)
         
         You can also use the [requirements](requirements.txt) file to set up your environment.
         
         ## License
```

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/README.md` & `mct-quantizers-nightly-1.1.0.20230714.post1233/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,16 @@
 pip install mct-quantizers-nightly
 ```
 
 ### Requirements
 
 To use MCT Quantizers, you need to have one of the supported frameworks, Tensorflow or PyTorch, installed.
 
-For use with Tensorflow, please install the following packages:
-[tensorflow](https://www.tensorflow.org/install), 
-[tensorflow-model-optimization](https://www.tensorflow.org/model_optimization/guide/install)
+For use with Tensorflow, please install the following package:
+[tensorflow](https://www.tensorflow.org/install),
 
 For use with PyTorch, please install the following package:
 [torch](https://pytorch.org/)
 
 You can also use the [requirements](requirements.txt) file to set up your environment.
 
 ## License
```

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/__init__.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/__init__.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/base_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/common/base_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/constants.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/get_all_subclasses.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/common/get_all_subclasses.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/get_quantizers.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/common/get_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/quant_info.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/common/quant_info.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/common/quant_utils.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/__init__.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/activation_quantization_holder.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/load_model.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantize_wrapper.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizer_utils.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/__init__.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         WeightsSymmetricInferableQuantizer
 
     @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                     quantization_method=[QuantizationMethod.POWER_OF_TWO],
                     identifier=QuantizerID.INFERABLE)
     class WeightsPOTInferableQuantizer(WeightsSymmetricInferableQuantizer):
         """
-        Class for quantizing weights using power-of-two quantizer
+        Class for quantizing weights using unsigned power-of-two quantizer.
         """
 
         def __init__(self,
                      num_bits: int,
                      threshold: List[float],
                      per_channel: bool,
                      channel_axis: int = None,
```

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         WeightsUniformInferableQuantizer
 
     @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                     quantization_method=[QuantizationMethod.SYMMETRIC],
                     identifier=QuantizerID.INFERABLE)
     class WeightsSymmetricInferableQuantizer(WeightsUniformInferableQuantizer):
         """
-        Class for quantizing weights using a symmetric quantizer
+        Class for quantizing weights using unsigned symmetric quantizer.
         """
         def __init__(self,
                      num_bits: int,
                      threshold: List[float],
                      per_channel: bool,
                      channel_axis: int = None,
                      input_rank: int = None
```

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         validate_adjusted_min_max_ranges
 
     @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                     quantization_method=[QuantizationMethod.UNIFORM],
                     identifier=QuantizerID.INFERABLE)
     class WeightsUniformInferableQuantizer(BaseKerasInferableQuantizer):
         """
-        Class for quantizing weights using a uniform quantizer
+        Class for quantizing weights using unsigned uniform quantizer
         """
         def __init__(self,
                      num_bits: int,
                      min_range: List[float],
                      max_range: List[float],
                      per_channel: bool,
                      channel_axis: int = None,
```

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/keras/validation_functions.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/keras/validation_functions.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/logger.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/logger.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/__init__.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/activation_quantization_holder.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/load_model.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantize_wrapper.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizer_utils.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/__init__.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         WeightsSymmetricInferableQuantizer
 
     @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                     quantization_method=[QuantizationMethod.POWER_OF_TWO],
                     identifier=QuantizerID.INFERABLE)
     class WeightsPOTInferableQuantizer(WeightsSymmetricInferableQuantizer):
         """
-        Class for quantizing weights using power-of-two quantizer
+        Class for quantizing weights using unsigned power-of-two quantizer.
         """
 
         def __init__(self,
                      num_bits: int,
                      threshold: np.ndarray,
                      per_channel: bool,
                      channel_axis: int = None
```

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     from mct_quantizers.pytorch.quantizer_utils import to_torch_tensor, get_working_device
 
     @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                     quantization_method=[QuantizationMethod.SYMMETRIC],
                     identifier=QuantizerID.INFERABLE)
     class WeightsSymmetricInferableQuantizer(BaseSymmetricInferableQuantizer):
         """
-        Class for quantizing weights using a symmetric quantizer
+        Class for quantizing weights using unsigned symmetric quantizer.
         """
 
         def __init__(self,
                      num_bits: int,
                      threshold: np.ndarray,
                      per_channel: bool,
                      channel_axis: int = None
```

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     from mct_quantizers.pytorch.quantizer_utils import fix_range_to_include_zero, get_working_device, to_torch_tensor
 
     @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                     quantization_method=[QuantizationMethod.UNIFORM],
                     identifier=QuantizerID.INFERABLE)
     class WeightsUniformInferableQuantizer(BaseUniformInferableQuantizer):
         """
-        Class for quantizing weights using a uniform quantizer
+        Class for quantizing weights using unsigned uniform quantizer.
         """
 
         def __init__(self,
                      num_bits: int,
                      min_range: np.ndarray,
                      max_range: np.ndarray,
                      per_channel: bool,
```

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers_nightly.egg-info/PKG-INFO` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers_nightly.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers-nightly
-Version: 1.1.0.20230713.post1147
+Version: 1.1.0.20230714.post1233
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT) Quantizers
         
         The MCT Quantizers library is an open-source library developed by researchers and engineers working at Sony Semiconductor Israel. 
         
@@ -58,17 +58,16 @@
         pip install mct-quantizers-nightly
         ```
         
         ### Requirements
         
         To use MCT Quantizers, you need to have one of the supported frameworks, Tensorflow or PyTorch, installed.
         
-        For use with Tensorflow, please install the following packages:
-        [tensorflow](https://www.tensorflow.org/install), 
-        [tensorflow-model-optimization](https://www.tensorflow.org/model_optimization/guide/install)
+        For use with Tensorflow, please install the following package:
+        [tensorflow](https://www.tensorflow.org/install),
         
         For use with PyTorch, please install the following package:
         [torch](https://pytorch.org/)
         
         You can also use the [requirements](requirements.txt) file to set up your environment.
         
         ## License
```

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/mct_quantizers_nightly.egg-info/SOURCES.txt` & `mct-quantizers-nightly-1.1.0.20230714.post1233/mct_quantizers_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-quantizers-nightly-1.1.0.20230713.post1147/setup.py` & `mct-quantizers-nightly-1.1.0.20230714.post1233/setup.py`

 * *Files identical despite different names*

