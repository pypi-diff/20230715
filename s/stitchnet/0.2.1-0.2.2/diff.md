# Comparing `tmp/stitchnet-0.2.1.tar.gz` & `tmp/stitchnet-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stitchnet-0.2.1.tar", max compression
+gzip compressed data, was "stitchnet-0.2.2.tar", max compression
```

## Comparing `stitchnet-0.2.1.tar` & `stitchnet-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     3217 2023-07-15 19:50:25.824416 stitchnet-0.2.1/README.md
--rw-r--r--   0        0        0      749 2023-07-15 19:50:32.268524 stitchnet-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4575 2023-07-15 19:20:50.619006 stitchnet-0.2.1/stitchnet/__init__.py
--rw-r--r--   0        0        0        0 2022-08-11 16:21:49.761514 stitchnet-0.2.1/stitchnet/ensemble/__init__.py
--rw-r--r--   0        0        0     2825 2022-08-13 21:59:26.715969 stitchnet-0.2.1/stitchnet/ensemble/ensemble.py
--rw-r--r--   0        0        0        0 2022-08-11 16:21:49.761514 stitchnet-0.2.1/stitchnet/finetuning/__init__.py
--rw-r--r--   0        0        0     7865 2022-08-15 14:22:01.420281 stitchnet-0.2.1/stitchnet/finetuning/finetune.py
--rw-r--r--   0        0        0     6899 2022-08-15 11:37:11.000183 stitchnet-0.2.1/stitchnet/finetuning/finetune2.py
--rw-r--r--   0        0        0        0 2022-08-11 18:02:06.373025 stitchnet-0.2.1/stitchnet/plot/__init__.py
--rw-r--r--   0        0        0        0 2022-08-11 18:02:06.373025 stitchnet-0.2.1/stitchnet/plot/plotutils.py
--rw-r--r--   0        0        0     1559 2022-08-11 16:21:49.761514 stitchnet-0.2.1/stitchnet/stitchonnx/CKA.py
--rw-r--r--   0        0        0        0 2022-08-11 16:21:49.761514 stitchnet-0.2.1/stitchnet/stitchonnx/__init__.py
--rw-r--r--   0        0        0     1287 2022-08-11 16:21:49.761514 stitchnet-0.2.1/stitchnet/stitchonnx/ptCKA.py
--rw-r--r--   0        0        0      947 2022-08-12 05:48:18.123566 stitchnet-0.2.1/stitchnet/stitchonnx/render.py
--rw-r--r--   0        0        0     6915 2023-07-15 16:49:42.682547 stitchnet-0.2.1/stitchnet/stitchonnx/report.py
--rw-r--r--   0        0        0    64786 2023-07-15 19:24:45.663127 stitchnet-0.2.1/stitchnet/stitchonnx/utils.py
--rw-r--r--   0        0        0     3033 2023-07-15 19:25:23.937773 stitchnet-0.2.1/stitchnet/stitchonnx/viz.py
--rw-r--r--   0        0        0     4500 2023-07-15 19:50:39.344462 stitchnet-0.2.1/setup.py
--rw-r--r--   0        0        0     4313 2023-07-15 19:50:39.345024 stitchnet-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4153 2023-07-15 19:51:19.497307 stitchnet-0.2.2/README.md
+-rw-r--r--   0        0        0      749 2023-07-15 19:51:46.173744 stitchnet-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4575 2023-07-15 19:20:50.619006 stitchnet-0.2.2/stitchnet/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-11 16:21:49.761514 stitchnet-0.2.2/stitchnet/ensemble/__init__.py
+-rw-r--r--   0        0        0     2825 2022-08-13 21:59:26.715969 stitchnet-0.2.2/stitchnet/ensemble/ensemble.py
+-rw-r--r--   0        0        0        0 2022-08-11 16:21:49.761514 stitchnet-0.2.2/stitchnet/finetuning/__init__.py
+-rw-r--r--   0        0        0     7865 2022-08-15 14:22:01.420281 stitchnet-0.2.2/stitchnet/finetuning/finetune.py
+-rw-r--r--   0        0        0     6899 2022-08-15 11:37:11.000183 stitchnet-0.2.2/stitchnet/finetuning/finetune2.py
+-rw-r--r--   0        0        0        0 2022-08-11 18:02:06.373025 stitchnet-0.2.2/stitchnet/plot/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-11 18:02:06.373025 stitchnet-0.2.2/stitchnet/plot/plotutils.py
+-rw-r--r--   0        0        0     1559 2022-08-11 16:21:49.761514 stitchnet-0.2.2/stitchnet/stitchonnx/CKA.py
+-rw-r--r--   0        0        0        0 2022-08-11 16:21:49.761514 stitchnet-0.2.2/stitchnet/stitchonnx/__init__.py
+-rw-r--r--   0        0        0     1287 2022-08-11 16:21:49.761514 stitchnet-0.2.2/stitchnet/stitchonnx/ptCKA.py
+-rw-r--r--   0        0        0      947 2022-08-12 05:48:18.123566 stitchnet-0.2.2/stitchnet/stitchonnx/render.py
+-rw-r--r--   0        0        0     6915 2023-07-15 16:49:42.682547 stitchnet-0.2.2/stitchnet/stitchonnx/report.py
+-rw-r--r--   0        0        0    64786 2023-07-15 19:24:45.663127 stitchnet-0.2.2/stitchnet/stitchonnx/utils.py
+-rw-r--r--   0        0        0     3033 2023-07-15 19:25:23.937773 stitchnet-0.2.2/stitchnet/stitchonnx/viz.py
+-rw-r--r--   0        0        0     5437 2023-07-15 19:52:03.998531 stitchnet-0.2.2/setup.py
+-rw-r--r--   0        0        0     5249 2023-07-15 19:52:03.999135 stitchnet-0.2.2/PKG-INFO
```

### Comparing `stitchnet-0.2.1/README.md` & `stitchnet-0.2.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 StitchNet: Composing Neural Networks from Pre-Trained Fragments
 =============
 
+We propose StitchNet, a novel neural network creation paradigm that stitches together fragments (one or more consecutive network layers) from multiple pre-trained neural networks. StitchNet allows the creation of high-performing neural networks without the large compute and data requirements needed under traditional model creation processes via backpropagation training. We leverage Centered Kernel Alignment (CKA) as a compatibility measure to efficiently guide the selection of these fragments in composing a network for a given task tailored to specific accuracy needs and computing resource constraints. We then show that these fragments can be stitched together to create neural networks with comparable accuracy to traditionally trained networks at a fraction of computing resource and data requirements. Finally, we explore a novel on-the-fly personalized model creation and inference application enabled by this new paradigm.
 
 Installation
 =============
 
     pip install stitchnet
     
 Usage
```

### Comparing `stitchnet-0.2.1/pyproject.toml` & `stitchnet-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stitchnet"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 authors = ["Surat Teerapittayanon <steerapi@gmail.com>"]
 readme = "README.md"
 exclude = ["_*",".*","*.ipynb"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
```

### Comparing `stitchnet-0.2.1/stitchnet/__init__.py` & `stitchnet-0.2.2/stitchnet/__init__.py`

 * *Files identical despite different names*

### Comparing `stitchnet-0.2.1/stitchnet/ensemble/ensemble.py` & `stitchnet-0.2.2/stitchnet/ensemble/ensemble.py`

 * *Files identical despite different names*

### Comparing `stitchnet-0.2.1/stitchnet/finetuning/finetune.py` & `stitchnet-0.2.2/stitchnet/finetuning/finetune.py`

 * *Files identical despite different names*

### Comparing `stitchnet-0.2.1/stitchnet/finetuning/finetune2.py` & `stitchnet-0.2.2/stitchnet/finetuning/finetune2.py`

 * *Files identical despite different names*

### Comparing `stitchnet-0.2.1/stitchnet/stitchonnx/CKA.py` & `stitchnet-0.2.2/stitchnet/stitchonnx/CKA.py`

 * *Files identical despite different names*

### Comparing `stitchnet-0.2.1/stitchnet/stitchonnx/ptCKA.py` & `stitchnet-0.2.2/stitchnet/stitchonnx/ptCKA.py`

 * *Files identical despite different names*

### Comparing `stitchnet-0.2.1/stitchnet/stitchonnx/render.py` & `stitchnet-0.2.2/stitchnet/stitchonnx/render.py`

 * *Files identical despite different names*

### Comparing `stitchnet-0.2.1/stitchnet/stitchonnx/report.py` & `stitchnet-0.2.2/stitchnet/stitchonnx/report.py`

 * *Files identical despite different names*

### Comparing `stitchnet-0.2.1/stitchnet/stitchonnx/utils.py` & `stitchnet-0.2.2/stitchnet/stitchonnx/utils.py`

 * *Files identical despite different names*

### Comparing `stitchnet-0.2.1/stitchnet/stitchonnx/viz.py` & `stitchnet-0.2.2/stitchnet/stitchonnx/viz.py`

 * *Files identical despite different names*

### Comparing `stitchnet-0.2.1/PKG-INFO` & `stitchnet-0.2.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stitchnet
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Author: Surat Teerapittayanon
 Author-email: steerapi@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
@@ -27,14 +27,15 @@
 Requires-Dist: torchvision (>=0.13.1,<0.14.0)
 Requires-Dist: transformers (>=4.25.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 StitchNet: Composing Neural Networks from Pre-Trained Fragments
 =============
 
+We propose StitchNet, a novel neural network creation paradigm that stitches together fragments (one or more consecutive network layers) from multiple pre-trained neural networks. StitchNet allows the creation of high-performing neural networks without the large compute and data requirements needed under traditional model creation processes via backpropagation training. We leverage Centered Kernel Alignment (CKA) as a compatibility measure to efficiently guide the selection of these fragments in composing a network for a given task tailored to specific accuracy needs and computing resource constraints. We then show that these fragments can be stitched together to create neural networks with comparable accuracy to traditionally trained networks at a fraction of computing resource and data requirements. Finally, we explore a novel on-the-fly personalized model creation and inference application enabled by this new paradigm.
 
 Installation
 =============
 
     pip install stitchnet
     
 Usage
```

