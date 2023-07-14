# Comparing `tmp/eztils-0.4.1.tar.gz` & `tmp/eztils-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eztils-0.4.1.tar", max compression
+gzip compressed data, was "eztils-0.4.2.tar", max compression
```

## Comparing `eztils-0.4.1.tar` & `eztils-0.4.2.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0     1075 2023-07-14 01:17:51.780650 eztils-0.4.1/LICENSE
--rw-r--r--   0        0        0    12710 2023-07-14 01:52:52.320035 eztils-0.4.1/README.md
--rw-r--r--   0        0        0      542 2023-07-14 02:09:17.596159 eztils-0.4.1/eztils/__init__.py
--rw-r--r--   0        0        0      879 2023-07-14 02:29:30.133442 eztils-0.4.1/eztils/default/__init__.py
--rw-r--r--   0        0        0     2341 2023-07-14 01:58:12.724178 eztils-0.4.1/eztils/default/logging.py
--rw-r--r--   0        0        0      112 2023-07-14 02:09:16.540172 eztils-0.4.1/eztils/default/math.py
--rw-r--r--   0        0        0     1091 2023-07-14 01:58:12.704178 eztils-0.4.1/eztils/default/structures.py
--rw-r--r--   0        0        0      265 2023-07-14 02:09:16.960167 eztils-0.4.1/eztils/torch/__init__.py
--rw-r--r--   0        0        0      688 2023-07-14 02:09:17.632159 eztils-0.4.1/eztils/torch/utils/__init__.py
--rw-r--r--   0        0        0     5667 2023-07-14 02:09:17.640159 eztils-0.4.1/eztils/torch/utils/arrays.py
--rw-r--r--   0        0        0      962 2023-07-14 01:17:51.780650 eztils-0.4.1/eztils/torch/utils/model_wrappers.py
--rw-r--r--   0        0        0     3457 2023-07-14 02:29:08.441706 eztils-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    13743 1970-01-01 00:00:00.000000 eztils-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-14 01:17:51.780650 eztils-0.4.2/LICENSE
+-rw-r--r--   0        0        0    12752 2023-07-14 23:03:04.291472 eztils-0.4.2/README.md
+-rw-r--r--   0        0        0      542 2023-07-14 02:09:17.596159 eztils-0.4.2/eztils/__init__.py
+-rw-r--r--   0        0        0      935 2023-07-14 23:03:49.090942 eztils-0.4.2/eztils/default/__init__.py
+-rw-r--r--   0        0        0     3689 2023-07-14 23:03:49.090942 eztils-0.4.2/eztils/default/dict_operations.py
+-rw-r--r--   0        0        0     2246 2023-07-14 21:46:13.733182 eztils-0.4.2/eztils/default/itertools.py
+-rw-r--r--   0        0        0     2458 2023-07-14 23:07:36.740250 eztils-0.4.2/eztils/default/logging.py
+-rw-r--r--   0        0        0      112 2023-07-14 02:09:16.540172 eztils-0.4.2/eztils/default/math.py
+-rw-r--r--   0        0        0     1091 2023-07-14 01:58:12.704178 eztils-0.4.2/eztils/default/structures.py
+-rw-r--r--   0        0        0     1099 2023-07-14 23:03:35.175106 eztils-0.4.2/eztils/torch/__init__.py
+-rw-r--r--   0        0        0      155 2023-07-14 22:54:30.913527 eztils-0.4.2/eztils/torch/lightning.py
+-rw-r--r--   0        0        0      173 2023-07-14 22:54:30.917527 eztils-0.4.2/eztils/torch/math.py
+-rw-r--r--   0        0        0      962 2023-07-14 01:17:51.780650 eztils-0.4.2/eztils/torch/model_wrappers.py
+-rw-r--r--   0        0        0     1420 2023-07-14 22:54:30.937527 eztils-0.4.2/eztils/torch/parameters.py
+-rw-r--r--   0        0        0     2858 2023-07-14 23:03:35.175106 eztils-0.4.2/eztils/torch/to.py
+-rw-r--r--   0        0        0     3501 2023-07-14 23:10:38.602099 eztils-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    13785 1970-01-01 00:00:00.000000 eztils-0.4.2/PKG-INFO
```

### Comparing `eztils-0.4.1/LICENSE` & `eztils-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eztils-0.4.1/README.md` & `eztils-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # eztils
 
+# TODO add torchtyping?
+# TODO add tests
+
 <div align="center">
 
 [![Build status](https://github.com/ezhang7423/eztils/workflows/build/badge.svg?branch=master&event=push)](https://github.com/ezhang7423/eztils/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/eztils.svg)](https://pypi.org/project/eztils/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/ezhang7423/eztils/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

### Comparing `eztils-0.4.1/eztils/__init__.py` & `eztils-0.4.2/eztils/__init__.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.1/eztils/default/__init__.py` & `eztils-0.4.2/eztils/default/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,10 +23,12 @@
     return os.path.dirname(getsourcefile(inspect_.stack()[1][0]))  # type: ignore
 
 
 def apply_dict(fn, d, *args, **kwargs):
     return {k: fn(v, *args, **kwargs) for k, v in d.items()}
 
 
+from .dict_operations import *
+from .itertools import *
 from .logging import *
 from .math import *
 from .structures import *
```

### Comparing `eztils-0.4.1/eztils/default/logging.py` & `eztils-0.4.2/eztils/default/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from datetime import datetime
 
 import numpy as np
-import torch
 from rich.console import Console
 from rich.tree import Tree
 
 console = Console()
 
 
 def print_creator(color):
@@ -20,14 +19,21 @@
 bold = print_creator("bold")
 blue = print_creator("blue")
 purple = print_creator("purple")
 orange = print_creator("orange")
 
 
 def inspect(obj, list_expand=3):
+    try:
+        import torch
+
+        torch_exists = True
+    except ImportError:
+        torch_exists = False
+
     console = Console(record=True)
 
     class TreeWrapper:
         def __init__(self) -> None:
             self.tree = None
 
         def add(self, label):
@@ -55,15 +61,15 @@
             list_node = root.add(f"{type_fmt(obj)}[{len(obj)}]")
             if len(obj) == 0:
                 return
             for i in range(min(list_expand, len(obj))):
                 add_children(obj[i], list_node)
             if len(obj) > list_expand:
                 list_node.add("...")
-        elif isinstance(obj, torch.Tensor):
+        elif torch_exists and isinstance(obj, torch.Tensor):
             root.add(f"tensor[[blue]{tuple(obj.shape)}; {obj.dtype}[/blue]]")
         else:
             repr = str(obj)
             if len(repr) > 100:
                 repr = repr[:100] + "..."
             root.add(f"{type_fmt(obj)}: [blue]{repr}[/blue]")
```

### Comparing `eztils-0.4.1/eztils/default/structures.py` & `eztils-0.4.2/eztils/default/structures.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.1/eztils/torch/utils/__init__.py` & `eztils-0.4.2/eztils/torch/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,40 @@
+"""eds utilities"""
+
+# import often used modules
 import random
+from pathlib import Path
 
 import numpy as np
 import torch
-
-# helpers functions
+from einops import rearrange as rea
+from einops import reduce
+from torch import einsum, nn
+from torch.nn import functional as F
+from torchvision.utils import save_image
+
+# globals
+USE_GPU = False
+DTYPE = torch.float
+GPU_ID = 0
+DEVICE = None
+
+
+def set_gpu_mode(mode, gpu_id=0):
+    global USE_GPU
+    global DEVICE
+    global GPU_ID
+    GPU_ID = gpu_id
+    USE_GPU = mode
+    DEVICE = torch.device("cuda:" + str(gpu_id) if USE_GPU else "cpu")
+    if USE_GPU:
+        torch.cuda.set_device(gpu_id)
 
 
-def register_buffer(
-    self, name, val
-):  # register as same type as weights for lightning modules
-    self.register_buffer(name, val.type(self.dtype))
+# helper functions
 
 
 def seed_everything(seed):
     """
     Set the seed for all the possible random number generators
     for global packages.
     :param seed:
@@ -24,11 +45,12 @@
     np.random.seed(seed)
     torch.manual_seed(seed)
 
     if torch.cuda.is_available():
         torch.cuda.manual_seed_all(seed)
 
 
-from ...default.logging import *
-from ...default.structures import *
-from .arrays import *
+from .lightning import *
+from .math import *
 from .model_wrappers import *
+from .parameters import *
+from .to import *
```

### Comparing `eztils-0.4.1/eztils/torch/utils/model_wrappers.py` & `eztils-0.4.2/eztils/torch/model_wrappers.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.1/pyproject.toml` & `eztils-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = ["ezhang7423 <ezhang7423@student.palomar.edu>"]
 description = "eds utilities"
 homepage = "https://github.com/ezhang7423/eztils"
 license = "MIT"
 name = "eztils"
 readme = "README.md"
 repository = "https://github.com/ezhang7423/eztils"
-version = "0.4.1"
+version = "0.4.2"
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = [] #! Update me
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [
   #! Update me
@@ -23,14 +23,15 @@
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 rich = "^13.3.3"
 numpy = "^1.24.3"
 loguru = "^0.7.0"
```

### Comparing `eztils-0.4.1/PKG-INFO` & `eztils-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eztils
-Version: 0.4.1
+Version: 0.4.2
 Summary: eds utilities
 Home-page: https://github.com/ezhang7423/eztils
 License: MIT
 Author: ezhang7423
 Author-email: ezhang7423@student.palomar.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -23,14 +23,17 @@
 Requires-Dist: rich (>=13.3.3,<14.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/ezhang7423/eztils
 Description-Content-Type: text/markdown
 
 # eztils
 
+# TODO add torchtyping?
+# TODO add tests
+
 <div align="center">
 
 [![Build status](https://github.com/ezhang7423/eztils/workflows/build/badge.svg?branch=master&event=push)](https://github.com/ezhang7423/eztils/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/eztils.svg)](https://pypi.org/project/eztils/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/ezhang7423/eztils/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

