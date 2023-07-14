# Comparing `tmp/cjm-yolox-pytorch-0.0.96.tar.gz` & `tmp/cjm-yolox-pytorch-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cjm-yolox-pytorch-0.0.96.tar", last modified: Fri Jul 14 21:47:10 2023, max compression
+gzip compressed data, was "cjm-yolox-pytorch-0.0.97.tar", last modified: Fri Jul 14 23:34:58 2023, max compression
```

## Comparing `cjm-yolox-pytorch-0.0.96.tar` & `cjm-yolox-pytorch-0.0.97.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-14 21:47:10.478366 cjm-yolox-pytorch-0.0.96/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.96/LICENSE
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.96/MANIFEST.in
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-14 21:47:10.478204 cjm-yolox-pytorch-0.0.96/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-13 20:16:56.000000 cjm-yolox-pytorch-0.0.96/README.md
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-14 21:47:10.475723 cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       23 2023-07-14 21:46:58.000000 cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch/__init__.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    12639 2023-07-14 21:46:58.000000 cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch/_modidx.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    24672 2023-07-14 21:46:58.000000 cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch/loss.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    35626 2023-07-14 21:46:58.000000 cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch/model.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15312 2023-07-14 21:46:58.000000 cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch/simota.py
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     3149 2023-07-14 21:46:58.000000 cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch/utils.py
-drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-14 21:47:10.477859 cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch.egg-info/
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-14 21:47:10.000000 cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch.egg-info/PKG-INFO
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-14 21:47:10.000000 cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch.egg-info/SOURCES.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-14 21:47:10.000000 cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch.egg-info/dependency_links.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-14 21:47:10.000000 cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch.egg-info/entry_points.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch.egg-info/not-zip-safe
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       45 2023-07-14 21:47:10.000000 cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch.egg-info/requires.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-14 21:47:10.000000 cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch.egg-info/top_level.txt
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1067 2023-07-14 21:46:25.000000 cjm-yolox-pytorch-0.0.96/settings.ini
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-14 21:47:10.478416 cjm-yolox-pytorch-0.0.96/setup.cfg
--rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.96/setup.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-14 23:34:58.467374 cjm-yolox-pytorch-0.0.97/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1075 2023-06-22 23:01:16.000000 cjm-yolox-pytorch-0.0.97/LICENSE
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      111 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.97/MANIFEST.in
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-14 23:34:58.467202 cjm-yolox-pytorch-0.0.97/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1050 2023-07-13 20:16:56.000000 cjm-yolox-pytorch-0.0.97/README.md
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-14 23:34:58.464610 cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       23 2023-07-14 23:34:50.000000 cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch/__init__.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    12639 2023-07-14 23:34:50.000000 cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch/_modidx.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    24674 2023-07-14 23:34:50.000000 cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch/loss.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    35626 2023-07-14 23:34:50.000000 cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch/model.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)    15312 2023-07-14 23:34:50.000000 cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch/simota.py
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     3149 2023-07-14 23:34:50.000000 cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch/utils.py
+drwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        0 2023-07-14 23:34:58.466858 cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch.egg-info/
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1816 2023-07-14 23:34:58.000000 cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch.egg-info/PKG-INFO
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)      506 2023-07-14 23:34:58.000000 cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch.egg-info/SOURCES.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-07-14 23:34:58.000000 cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch.egg-info/dependency_links.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       56 2023-07-14 23:34:58.000000 cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch.egg-info/entry_points.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)        1 2023-06-23 01:14:13.000000 cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch.egg-info/not-zip-safe
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       45 2023-07-14 23:34:58.000000 cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch.egg-info/requires.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       18 2023-07-14 23:34:58.000000 cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch.egg-info/top_level.txt
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     1067 2023-07-14 23:34:09.000000 cjm-yolox-pytorch-0.0.97/settings.ini
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)       38 2023-07-14 23:34:58.467425 cjm-yolox-pytorch-0.0.97/setup.cfg
+-rwxrwxrwx   0 innom-dt  (1000) innom-dt  (1000)     2596 2023-04-27 10:12:58.000000 cjm-yolox-pytorch-0.0.97/setup.py
```

### Comparing `cjm-yolox-pytorch-0.0.96/LICENSE` & `cjm-yolox-pytorch-0.0.97/LICENSE`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.96/PKG-INFO` & `cjm-yolox-pytorch-0.0.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.96
+Version: 0.0.97
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.96/README.md` & `cjm-yolox-pytorch-0.0.97/README.md`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch/_modidx.py` & `cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch/_modidx.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch/loss.py` & `cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch/loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,24 +434,24 @@
 #         # Compute class loss
 #         loss_cls = self.class_loss_func(flatten_class_preds.view(-1, self.num_classes)[positive_masks],class_targets)
 
         # Compute bounding box loss
         if positive_masks.shape[0] > 0:
             loss_bbox = self.bbox_loss_func(flatten_decoded_bboxes.view(-1, 4)[positive_masks], bbox_targets)
         else:
-            loss_bbox = torch.tensor(0.).to(class_scores[0].device)
+            loss_bbox = torch.tensor(0.)#.to(class_scores[0].device)
 
         # Compute objectness loss
         loss_obj = self.objectness_loss_func(flatten_objectness_scores.view(-1, 1), objectness_targets)
 
         # Compute class loss
         if positive_masks.shape[0] > 0:
             loss_cls = self.class_loss_func(flatten_class_preds.view(-1, self.num_classes)[positive_masks], class_targets)
         else:
-            loss_cls = torch.tensor(0.).to(class_scores[0].device)
+            loss_cls = torch.tensor(0.)#.to(class_scores[0].device)
         
         # Calculate total number of samples
         num_total_samples = max(sum(num_positive_images), 1)
         
         # Scale losses
         loss_bbox = (loss_bbox * self.bbox_loss_weight) / num_total_samples
         loss_obj = (loss_obj * self.objectness_loss_weight) / num_total_samples
```

### Comparing `cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch/model.py` & `cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch/model.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch/simota.py` & `cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch/simota.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch/utils.py` & `cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `cjm-yolox-pytorch-0.0.96/cjm_yolox_pytorch.egg-info/PKG-INFO` & `cjm-yolox-pytorch-0.0.97/cjm_yolox_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cjm-yolox-pytorch
-Version: 0.0.96
+Version: 0.0.97
 Summary: A PyTorch implementation of the YOLOX object detection model based on the mmdetection implementation.
 Home-page: https://github.com/cj-mills/cjm-yolox-pytorch
 Author: cj-mills
 Author-email: millscj.mills2@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python torch
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cjm-yolox-pytorch-0.0.96/settings.ini` & `cjm-yolox-pytorch-0.0.97/settings.ini`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = cjm-yolox-pytorch
 lib_name = %(repo)s
-version = 0.0.96
+version = 0.0.97
 min_python = 3.9
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = cjm_yolox_pytorch
```

### Comparing `cjm-yolox-pytorch-0.0.96/setup.py` & `cjm-yolox-pytorch-0.0.97/setup.py`

 * *Files identical despite different names*

