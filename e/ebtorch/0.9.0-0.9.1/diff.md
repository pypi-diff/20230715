# Comparing `tmp/ebtorch-0.9.0.tar.gz` & `tmp/ebtorch-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebtorch-0.9.0.tar", last modified: Mon Jun 19 15:54:46 2023, max compression
+gzip compressed data, was "ebtorch-0.9.1.tar", last modified: Sat Jul 15 10:45:58 2023, max compression
```

## Comparing `ebtorch-0.9.0.tar` & `ebtorch-0.9.1.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:54:46.591891 ebtorch-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-06-19 15:54:32.000000 ebtorch-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-19 15:54:46.591891 ebtorch-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-19 15:54:32.000000 ebtorch-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:54:46.579891 ebtorch-0.9.0/ebtorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:54:46.583891 ebtorch-0.9.0/ebtorch/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/logging/avgmeter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/logging/logcsv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:54:46.587891 ebtorch-0.9.0/ebtorch/nn/
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/conv2drp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/convolutional_flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/coordconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/debuglayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/fieldtransform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:54:46.587891 ebtorch-0.9.0/ebtorch/nn/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/functional/inner_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/kwta.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/laplacenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/mish.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/nnsemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/reshapelayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/serf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/serlu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/sinlu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/smelu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:54:46.587891 ebtorch-0.9.0/ebtorch/nn/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/utils/adverutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/utils/autoclip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/utils/onlyutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/utils/patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/nn/utils/reprutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:54:46.587891 ebtorch-0.9.0/ebtorch/optim/
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/optim/adahessian.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/optim/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/optim/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/optim/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/optim/lookahead.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/optim/radam.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-19 15:54:32.000000 ebtorch-0.9.0/ebtorch/optim/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 15:54:46.583891 ebtorch-0.9.0/ebtorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-19 15:54:46.000000 ebtorch-0.9.0/ebtorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-19 15:54:46.000000 ebtorch-0.9.0/ebtorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:54:46.000000 ebtorch-0.9.0/ebtorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 15:54:46.000000 ebtorch-0.9.0/ebtorch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 15:54:46.000000 ebtorch-0.9.0/ebtorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 15:54:46.591891 ebtorch-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-19 15:54:32.000000 ebtorch-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:45:58.324609 ebtorch-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-15 10:45:44.000000 ebtorch-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-15 10:45:58.320608 ebtorch-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-15 10:45:44.000000 ebtorch-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:45:58.312608 ebtorch-0.9.1/ebtorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:45:58.316608 ebtorch-0.9.1/ebtorch/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/logging/avgmeter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/logging/logcsv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:45:58.320608 ebtorch-0.9.1/ebtorch/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13998 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/conv2drp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/convolutional_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/coordconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/debuglayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/fieldtransform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:45:58.320608 ebtorch-0.9.1/ebtorch/nn/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/functional/inner_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/kwta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/laplacenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/mish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/nnsemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/reshapelayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/serf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/serlu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/sinlu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/smelu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:45:58.320608 ebtorch-0.9.1/ebtorch/nn/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/utils/adverutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/utils/autoclip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/utils/onlyutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/utils/patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/nn/utils/reprutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:45:58.320608 ebtorch-0.9.1/ebtorch/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/optim/adahessian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/optim/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/optim/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/optim/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/optim/lookahead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/optim/lookaround.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/optim/radam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-07-15 10:45:44.000000 ebtorch-0.9.1/ebtorch/optim/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:45:58.316608 ebtorch-0.9.1/ebtorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-15 10:45:58.000000 ebtorch-0.9.1/ebtorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-15 10:45:58.000000 ebtorch-0.9.1/ebtorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 10:45:58.000000 ebtorch-0.9.1/ebtorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 10:45:58.000000 ebtorch-0.9.1/ebtorch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 10:45:58.000000 ebtorch-0.9.1/ebtorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 10:45:58.324609 ebtorch-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-15 10:45:44.000000 ebtorch-0.9.1/setup.py
```

### Comparing `ebtorch-0.9.0/PKG-INFO` & `ebtorch-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebtorch
-Version: 0.9.0
+Version: 0.9.1
 Summary: Collection of PyTorch additions, extensions, utilities, uses and abuses
 Home-page: https://github.com/emaballarin/ebtorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: Apache-2.0
 Keywords: Deep Learning,Machine Learning
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebtorch Version: 0.9.0 Summary: Collection of
+Metadata-Version: 2.1 Name: ebtorch Version: 0.9.1 Summary: Collection of
 PyTorch additions, extensions, utilities, uses and abuses Home-page: https://
 github.com/emaballarin/ebtorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: Apache-2.0 Keywords: Deep Learning,Machine
 Learning Classifier: Development Status :: 3 - Alpha Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Environment ::
 Console Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
```

### Comparing `ebtorch-0.9.0/ebtorch/__init__.py` & `ebtorch-0.9.1/ebtorch/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 del pixelwise_bce_sum
 
 # Deletions (from .optim)
 del AdaHessian
 del Adan
 del Lion
 del Lookahead
+del Lookaround
 del RAdam
 del SAM
 del ralah_optim
 del wfneal
 
 # Deletions (from .logging)
 del AverageMeter
```

### Comparing `ebtorch-0.9.0/ebtorch/logging/__init__.py` & `ebtorch-0.9.1/ebtorch/nn/reshapelayers.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # ==============================================================================
 #
-# Copyright 2020-* Emanuele Ballarin <emanuele@ballarin.cc>
-# All Rights Reserved. Unless otherwise explicitly stated.
+# Copyright (c) 2020-* Emanuele Ballarin <emanuele@ballarin.cc>
+#                      All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # ==============================================================================
-#
 # SPDX-License-Identifier: Apache-2.0
-# Imports (specific)
-from .avgmeter import AverageMeter
-from .logcsv import LogCSV
-
-# Deletions (from .)
-del avgmeter
-del logcsv
+from torch import nn
+
+
+class ReshapeLayer(nn.Module):
+    def __init__(self, shape: tuple):
+        super().__init__()
+        self.shape = shape
+
+    def forward(self, x):
+        return x.reshape(self.shape)
+
+
+class FlatChannelize2DLayer(nn.Module):
+    def __init__(self):
+        super().__init__()
+
+    def forward(self, x):  # Do not make static!
+        return x.reshape(*x.shape, 1, 1)
```

### Comparing `ebtorch-0.9.0/ebtorch/logging/logcsv.py` & `ebtorch-0.9.1/ebtorch/logging/logcsv.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# ==============================================================================
+# ------------------------------------------------------------------------------
 #
-# Copyright (c) 2020-* Emanuele Ballarin <emanuele@ballarin.cc>
-#                      All Rights Reserved.
+#  Copyright (c) 2020-2023 Emanuele Ballarin <emanuele@ballarin.cc>
+#  Released under the terms of the MIT License
+#  (see: https://url.ballarin.cc/mitlicense)
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
+# ------------------------------------------------------------------------------
 #
-#     https://www.apache.org/licenses/LICENSE-2.0
+# SPDX-License-Identifier: MIT
 #
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-# ==============================================================================
-# SPDX-License-Identifier: Apache-2.0
+# ------------------------------------------------------------------------------
 # IMPORTS
 import csv
 from pathlib import Path
 from typing import Union
 
 
 class LogCSV:
```

### Comparing `ebtorch-0.9.0/ebtorch/nn/architectures.py` & `ebtorch-0.9.1/ebtorch/nn/architectures.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/nn/conv2drp.py` & `ebtorch-0.9.1/ebtorch/nn/conv2drp.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/nn/convolutional_flatten.py` & `ebtorch-0.9.1/ebtorch/nn/convolutional_flatten.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/nn/coordconv.py` & `ebtorch-0.9.1/ebtorch/nn/coordconv.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/nn/debuglayers.py` & `ebtorch-0.9.1/ebtorch/nn/debuglayers.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/nn/fieldtransform.py` & `ebtorch-0.9.1/ebtorch/nn/fieldtransform.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/nn/functional/inner_functional.py` & `ebtorch-0.9.1/ebtorch/nn/functional/inner_functional.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/nn/kwta.py` & `ebtorch-0.9.1/ebtorch/nn/kwta.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/nn/laplacenet.py` & `ebtorch-0.9.1/ebtorch/nn/laplacenet.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/nn/mish.py` & `ebtorch-0.9.1/ebtorch/nn/mish.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/nn/nnsemble.py` & `ebtorch-0.9.1/ebtorch/nn/nnsemble.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/nn/reshapelayers.py` & `ebtorch-0.9.1/ebtorch/nn/serlu.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # ==============================================================================
 #
-# Copyright (c) 2020-* Emanuele Ballarin <emanuele@ballarin.cc>
+# Copyright (c) 2021-* Emanuele Ballarin <emanuele@ballarin.cc>
 #                      All Rights Reserved.
+#                      [maintainance, adaptation, extension]
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,25 +16,31 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # ==============================================================================
 # SPDX-License-Identifier: Apache-2.0
+# IMPORTS
 from torch import nn
+from torch import Tensor
 
+from .functional import serlu as fserlu
 
-class ReshapeLayer(nn.Module):
-    def __init__(self, shape: tuple):
-        super().__init__()
-        self.shape = shape
 
-    def forward(self, x):
-        return x.reshape(self.shape)
+# CLASSES
+
 
+class SERLU(nn.Module):
+    """
+    Applies the SERLU function element-wise,
+    defined after [Zhang & Li, 2018]
+    """
 
-class FlatChannelize2DLayer(nn.Module):
-    def __init__(self):
+    def __init__(self, lambd: float = 1.07862, alph: float = 2.90427) -> None:
         super().__init__()
+        self._lambd: float
+        self._alph: float
+        self._lambd, self._alph = lambd, alph
 
-    def forward(self, x):  # Do not make static!
-        return x.reshape(*x.shape, 1, 1)
+    def forward(self, x_input: Tensor) -> Tensor:
+        return fserlu(x_input, lambd=self._lambd, alph=self._alph)
```

### Comparing `ebtorch-0.9.0/ebtorch/nn/serf.py` & `ebtorch-0.9.1/ebtorch/nn/serf.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/nn/sinlu.py` & `ebtorch-0.9.1/ebtorch/nn/sinlu.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/nn/utils/adverutils.py` & `ebtorch-0.9.1/ebtorch/nn/utils/adverutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/nn/utils/autoclip.py` & `ebtorch-0.9.1/ebtorch/nn/utils/autoclip.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/nn/utils/onlyutils.py` & `ebtorch-0.9.1/ebtorch/nn/utils/onlyutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/nn/utils/patches.py` & `ebtorch-0.9.1/ebtorch/nn/utils/patches.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/nn/utils/reprutils.py` & `ebtorch-0.9.1/ebtorch/nn/utils/reprutils.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/optim/__init__.py` & `ebtorch-0.9.1/ebtorch/optim/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,18 +23,20 @@
 # Imports (specific)
 from .adahessian import AdaHessian
 from .adan import Adan
 from .custom import ralah_optim
 from .custom import wfneal
 from .lion import Lion
 from .lookahead import Lookahead
+from .lookaround import Lookaround
 from .radam import RAdam
 from .sam import SAM
 
 # Deletions (from .)
 del adahessian
 del adan
 del custom
 del lion
 del lookahead
+del lookaround
 del radam
 del sam
```

### Comparing `ebtorch-0.9.0/ebtorch/optim/adahessian.py` & `ebtorch-0.9.1/ebtorch/optim/adahessian.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-# ==============================================================================
+# ------------------------------------------------------------------------------
 #
 # Copyright (c) 2020 David Samuel. All Rights Reserved. MIT Licensed.
 #                    [orig. code: https://github.com/davda54/ada-hessian ;
 #                     license text: https://github.com/davda54/ada-hessian/blob/master/LICENSE]
 #
-# ==============================================================================
+# ------------------------------------------------------------------------------
 #
 # Copyright (c) 2020 Zhewei Yao, Amir Gholami, Sheng Shen, Mustafa Mustafa,
 #                    Kurt Keutzer, Michael W. Mahoney
 #                    Behnam Neyshabur. All Rights Reserved. MIT Licensed.
 #                    [orig. work: https://arxiv.org/abs/2006.00719;
 #                     orig. code: https://github.com/amirgholami/ADAHESSIAN;
 #                     license text: https://github.com/amirgholami/ADAHESSIAN/blob/master/LICENSE]
 #
-# ==============================================================================
+# ------------------------------------------------------------------------------
 #
-# Copyright (c) 2023-* Emanuele Ballarin <emanuele@ballarin.cc>
-#                      All Rights Reserved.
-#                      [maintainance, adaptation, extension]
+#  Copyright (c) 2020-2023 Emanuele Ballarin <emanuele@ballarin.cc>
+#  Released under the terms of the MIT License
+#  (see: https://url.ballarin.cc/mitlicense)
+#
+# ------------------------------------------------------------------------------
 #
-# ==============================================================================
 # SPDX-License-Identifier: MIT
-# SPDX-License-Identifier: Apache-2.0
+#
+# ------------------------------------------------------------------------------
 import torch
 
 hessian_step_literal: str = "hessian step"
 
 
 class AdaHessian(torch.optim.Optimizer):
     """
```

### Comparing `ebtorch-0.9.0/ebtorch/optim/adan.py` & `ebtorch-0.9.1/ebtorch/optim/adan.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/optim/custom.py` & `ebtorch-0.9.1/ebtorch/optim/custom.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/optim/lion.py` & `ebtorch-0.9.1/ebtorch/optim/lion.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/optim/lookahead.py` & `ebtorch-0.9.1/ebtorch/optim/lookahead.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/optim/radam.py` & `ebtorch-0.9.1/ebtorch/optim/radam.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch/optim/sam.py` & `ebtorch-0.9.1/ebtorch/optim/sam.py`

 * *Files identical despite different names*

### Comparing `ebtorch-0.9.0/ebtorch.egg-info/PKG-INFO` & `ebtorch-0.9.1/ebtorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebtorch
-Version: 0.9.0
+Version: 0.9.1
 Summary: Collection of PyTorch additions, extensions, utilities, uses and abuses
 Home-page: https://github.com/emaballarin/ebtorch
 Author: Emanuele Ballarin
 Author-email: emanuele@ballarin.cc
 License: Apache-2.0
 Keywords: Deep Learning,Machine Learning
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ebtorch Version: 0.9.0 Summary: Collection of
+Metadata-Version: 2.1 Name: ebtorch Version: 0.9.1 Summary: Collection of
 PyTorch additions, extensions, utilities, uses and abuses Home-page: https://
 github.com/emaballarin/ebtorch Author: Emanuele Ballarin Author-email:
 emanuele@ballarin.cc License: Apache-2.0 Keywords: Deep Learning,Machine
 Learning Classifier: Development Status :: 3 - Alpha Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Environment ::
 Console Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: Apache Software License Requires-Python: >=3.8 Description-
```

### Comparing `ebtorch-0.9.0/ebtorch.egg-info/SOURCES.txt` & `ebtorch-0.9.1/ebtorch.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -36,9 +36,10 @@
 ebtorch/nn/utils/reprutils.py
 ebtorch/optim/__init__.py
 ebtorch/optim/adahessian.py
 ebtorch/optim/adan.py
 ebtorch/optim/custom.py
 ebtorch/optim/lion.py
 ebtorch/optim/lookahead.py
+ebtorch/optim/lookaround.py
 ebtorch/optim/radam.py
 ebtorch/optim/sam.py
```

