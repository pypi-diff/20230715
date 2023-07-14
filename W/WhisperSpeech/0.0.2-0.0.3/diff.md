# Comparing `tmp/WhisperSpeech-0.0.2.tar.gz` & `tmp/WhisperSpeech-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WhisperSpeech-0.0.2.tar", last modified: Fri Jul 14 22:51:48 2023, max compression
+gzip compressed data, was "WhisperSpeech-0.0.3.tar", last modified: Fri Jul 14 23:19:33 2023, max compression
```

## Comparing `WhisperSpeech-0.0.2.tar` & `WhisperSpeech-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 22:51:48.598960 WhisperSpeech-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-05-15 17:24:12.000000 WhisperSpeech-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-15 17:24:12.000000 WhisperSpeech-0.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6789 2023-07-14 22:51:48.598960 WhisperSpeech-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5972 2023-07-13 17:54:10.000000 WhisperSpeech-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 22:51:48.598960 WhisperSpeech-0.0.2/WhisperSpeech.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6789 2023-07-14 22:51:48.000000 WhisperSpeech-0.0.2/WhisperSpeech.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      659 2023-07-14 22:51:48.000000 WhisperSpeech-0.0.2/WhisperSpeech.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 22:51:48.000000 WhisperSpeech-0.0.2/WhisperSpeech.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-14 22:51:48.000000 WhisperSpeech-0.0.2/WhisperSpeech.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 16:42:35.000000 WhisperSpeech-0.0.2/WhisperSpeech.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       97 2023-07-14 22:51:48.000000 WhisperSpeech-0.0.2/WhisperSpeech.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-14 22:51:48.000000 WhisperSpeech-0.0.2/WhisperSpeech.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1253 2023-07-14 22:51:41.000000 WhisperSpeech-0.0.2/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 22:51:48.598960 WhisperSpeech-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2560 2023-05-15 17:24:12.000000 WhisperSpeech-0.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 22:51:48.598960 WhisperSpeech-0.0.2/whisperspeech/
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/__init__.py
--rw-r--r--   0 root         (0) root         (0)    58342 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/_modidx.py
--rw-r--r--   0 root         (0) root         (0)     5422 2023-07-13 11:51:18.000000 WhisperSpeech-0.0.2/whisperspeech/a2a.py
--rw-r--r--   0 root         (0) root         (0)     1108 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/a2wav.py
--rw-r--r--   0 root         (0) root         (0)     1983 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/extract_acoustic.py
--rw-r--r--   0 root         (0) root         (0)     2570 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/extract_semb.py
--rw-r--r--   0 root         (0) root         (0)     9636 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/extract_stoks.py
--rw-r--r--   0 root         (0) root         (0)    10094 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/modules.py
--rw-r--r--   0 root         (0) root         (0)     1167 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    16932 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/s2a_delar_mup.py
--rw-r--r--   0 root         (0) root         (0)    12102 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/t2s_up.py
--rw-r--r--   0 root         (0) root         (0)     8705 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/train.py
--rw-r--r--   0 root         (0) root         (0)     9800 2023-07-14 22:45:12.000000 WhisperSpeech-0.0.2/whisperspeech/train_multi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 23:19:33.016052 WhisperSpeech-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-05-15 17:24:12.000000 WhisperSpeech-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-15 17:24:12.000000 WhisperSpeech-0.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6789 2023-07-14 23:19:33.016052 WhisperSpeech-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5972 2023-07-13 17:54:10.000000 WhisperSpeech-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 23:19:33.016052 WhisperSpeech-0.0.3/WhisperSpeech.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6789 2023-07-14 23:19:32.000000 WhisperSpeech-0.0.3/WhisperSpeech.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      659 2023-07-14 23:19:33.000000 WhisperSpeech-0.0.3/WhisperSpeech.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 23:19:32.000000 WhisperSpeech-0.0.3/WhisperSpeech.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-14 23:19:32.000000 WhisperSpeech-0.0.3/WhisperSpeech.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 16:42:35.000000 WhisperSpeech-0.0.3/WhisperSpeech.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       97 2023-07-14 23:19:32.000000 WhisperSpeech-0.0.3/WhisperSpeech.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-14 23:19:32.000000 WhisperSpeech-0.0.3/WhisperSpeech.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1253 2023-07-14 23:18:17.000000 WhisperSpeech-0.0.3/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 23:19:33.016052 WhisperSpeech-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-05-15 17:24:12.000000 WhisperSpeech-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 23:19:33.016052 WhisperSpeech-0.0.3/whisperspeech/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-14 23:18:25.000000 WhisperSpeech-0.0.3/whisperspeech/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    58342 2023-07-14 23:18:25.000000 WhisperSpeech-0.0.3/whisperspeech/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)     5422 2023-07-13 11:51:18.000000 WhisperSpeech-0.0.3/whisperspeech/a2a.py
+-rw-r--r--   0 root         (0) root         (0)     1108 2023-07-14 23:18:25.000000 WhisperSpeech-0.0.3/whisperspeech/a2wav.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-07-14 23:18:25.000000 WhisperSpeech-0.0.3/whisperspeech/extract_acoustic.py
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-07-14 23:18:25.000000 WhisperSpeech-0.0.3/whisperspeech/extract_semb.py
+-rw-r--r--   0 root         (0) root         (0)     9636 2023-07-14 23:18:25.000000 WhisperSpeech-0.0.3/whisperspeech/extract_stoks.py
+-rw-r--r--   0 root         (0) root         (0)    10096 2023-07-14 23:18:25.000000 WhisperSpeech-0.0.3/whisperspeech/modules.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-07-14 23:18:25.000000 WhisperSpeech-0.0.3/whisperspeech/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    16932 2023-07-14 23:18:25.000000 WhisperSpeech-0.0.3/whisperspeech/s2a_delar_mup.py
+-rw-r--r--   0 root         (0) root         (0)    12102 2023-07-14 23:18:25.000000 WhisperSpeech-0.0.3/whisperspeech/t2s_up.py
+-rw-r--r--   0 root         (0) root         (0)     8705 2023-07-14 23:18:25.000000 WhisperSpeech-0.0.3/whisperspeech/train.py
+-rw-r--r--   0 root         (0) root         (0)     9800 2023-07-14 23:18:25.000000 WhisperSpeech-0.0.3/whisperspeech/train_multi.py
```

### Comparing `WhisperSpeech-0.0.2/LICENSE` & `WhisperSpeech-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `WhisperSpeech-0.0.2/PKG-INFO` & `WhisperSpeech-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WhisperSpeech
-Version: 0.0.2
+Version: 0.0.3
 Summary: An Open Source text-to-speech system built by inverting Whisper
 Home-page: https://github.com/collabora/WhisperSpeech
 Author: Jakub Piotr Cłapa
 Author-email: jpc@collabora.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `WhisperSpeech-0.0.2/README.md` & `WhisperSpeech-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `WhisperSpeech-0.0.2/WhisperSpeech.egg-info/PKG-INFO` & `WhisperSpeech-0.0.3/WhisperSpeech.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WhisperSpeech
-Version: 0.0.2
+Version: 0.0.3
 Summary: An Open Source text-to-speech system built by inverting Whisper
 Home-page: https://github.com/collabora/WhisperSpeech
 Author: Jakub Piotr Cłapa
 Author-email: jpc@collabora.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `WhisperSpeech-0.0.2/WhisperSpeech.egg-info/SOURCES.txt` & `WhisperSpeech-0.0.3/WhisperSpeech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `WhisperSpeech-0.0.2/settings.ini` & `WhisperSpeech-0.0.3/settings.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = WhisperSpeech
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = whisperspeech
 nbs_path = nbs
```

### Comparing `WhisperSpeech-0.0.2/setup.py` & `WhisperSpeech-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `WhisperSpeech-0.0.2/whisperspeech/_modidx.py` & `WhisperSpeech-0.0.3/whisperspeech/_modidx.py`

 * *Files identical despite different names*

### Comparing `WhisperSpeech-0.0.2/whisperspeech/a2a.py` & `WhisperSpeech-0.0.3/whisperspeech/a2a.py`

 * *Files identical despite different names*

### Comparing `WhisperSpeech-0.0.2/whisperspeech/a2wav.py` & `WhisperSpeech-0.0.3/whisperspeech/a2wav.py`

 * *Files identical despite different names*

### Comparing `WhisperSpeech-0.0.2/whisperspeech/extract_acoustic.py` & `WhisperSpeech-0.0.3/whisperspeech/extract_acoustic.py`

 * *Files identical despite different names*

### Comparing `WhisperSpeech-0.0.2/whisperspeech/extract_semb.py` & `WhisperSpeech-0.0.3/whisperspeech/extract_semb.py`

 * *Files identical despite different names*

### Comparing `WhisperSpeech-0.0.2/whisperspeech/extract_stoks.py` & `WhisperSpeech-0.0.3/whisperspeech/extract_stoks.py`

 * *Files identical despite different names*

### Comparing `WhisperSpeech-0.0.2/whisperspeech/modules.py` & `WhisperSpeech-0.0.3/whisperspeech/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import numpy as np
 import math
 
 from torch import Tensor, nn
 import torch.nn.functional as F
 from typing import Dict, Iterable, Optional
 
-import xformers.ops as xops
+# import xformers.ops as xops
 
 # %% ../nbs/A. Neural modules.ipynb 3
 # Code in this file is mostly borrowed from
 # https://github.com/openai/whisper/blob/main/whisper/model.py
 # and is under the MIT License
 
 class LayerNorm(nn.LayerNorm):
```

### Comparing `WhisperSpeech-0.0.2/whisperspeech/pipeline.py` & `WhisperSpeech-0.0.3/whisperspeech/pipeline.py`

 * *Files identical despite different names*

### Comparing `WhisperSpeech-0.0.2/whisperspeech/s2a_delar_mup.py` & `WhisperSpeech-0.0.3/whisperspeech/s2a_delar_mup.py`

 * *Files identical despite different names*

### Comparing `WhisperSpeech-0.0.2/whisperspeech/t2s_up.py` & `WhisperSpeech-0.0.3/whisperspeech/t2s_up.py`

 * *Files identical despite different names*

### Comparing `WhisperSpeech-0.0.2/whisperspeech/train.py` & `WhisperSpeech-0.0.3/whisperspeech/train.py`

 * *Files identical despite different names*

### Comparing `WhisperSpeech-0.0.2/whisperspeech/train_multi.py` & `WhisperSpeech-0.0.3/whisperspeech/train_multi.py`

 * *Files identical despite different names*

