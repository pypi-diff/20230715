# Comparing `tmp/eztils-0.4.2.tar.gz` & `tmp/eztils-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eztils-0.4.2.tar", max compression
+gzip compressed data, was "eztils-0.4.3.tar", max compression
```

## Comparing `eztils-0.4.2.tar` & `eztils-0.4.3.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0     1075 2023-07-14 01:17:51.780650 eztils-0.4.2/LICENSE
--rw-r--r--   0        0        0    12752 2023-07-14 23:03:04.291472 eztils-0.4.2/README.md
--rw-r--r--   0        0        0      542 2023-07-14 02:09:17.596159 eztils-0.4.2/eztils/__init__.py
--rw-r--r--   0        0        0      935 2023-07-14 23:03:49.090942 eztils-0.4.2/eztils/default/__init__.py
--rw-r--r--   0        0        0     3689 2023-07-14 23:03:49.090942 eztils-0.4.2/eztils/default/dict_operations.py
--rw-r--r--   0        0        0     2246 2023-07-14 21:46:13.733182 eztils-0.4.2/eztils/default/itertools.py
--rw-r--r--   0        0        0     2458 2023-07-14 23:07:36.740250 eztils-0.4.2/eztils/default/logging.py
--rw-r--r--   0        0        0      112 2023-07-14 02:09:16.540172 eztils-0.4.2/eztils/default/math.py
--rw-r--r--   0        0        0     1091 2023-07-14 01:58:12.704178 eztils-0.4.2/eztils/default/structures.py
--rw-r--r--   0        0        0     1099 2023-07-14 23:03:35.175106 eztils-0.4.2/eztils/torch/__init__.py
--rw-r--r--   0        0        0      155 2023-07-14 22:54:30.913527 eztils-0.4.2/eztils/torch/lightning.py
--rw-r--r--   0        0        0      173 2023-07-14 22:54:30.917527 eztils-0.4.2/eztils/torch/math.py
--rw-r--r--   0        0        0      962 2023-07-14 01:17:51.780650 eztils-0.4.2/eztils/torch/model_wrappers.py
--rw-r--r--   0        0        0     1420 2023-07-14 22:54:30.937527 eztils-0.4.2/eztils/torch/parameters.py
--rw-r--r--   0        0        0     2858 2023-07-14 23:03:35.175106 eztils-0.4.2/eztils/torch/to.py
--rw-r--r--   0        0        0     3501 2023-07-14 23:10:38.602099 eztils-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    13785 1970-01-01 00:00:00.000000 eztils-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-14 01:17:51.780650 eztils-0.4.3/LICENSE
+-rw-r--r--   0        0        0    12815 2023-07-15 07:19:31.991773 eztils-0.4.3/README.md
+-rw-r--r--   0        0        0      542 2023-07-14 02:09:17.596159 eztils-0.4.3/eztils/__init__.py
+-rw-r--r--   0        0        0     2021 2023-07-15 08:36:51.511267 eztils-0.4.3/eztils/default/__init__.py
+-rw-r--r--   0        0        0     3689 2023-07-15 06:11:10.377851 eztils-0.4.3/eztils/default/dict_operations.py
+-rw-r--r--   0        0        0     2246 2023-07-14 21:46:13.733182 eztils-0.4.3/eztils/default/itertools.py
+-rw-r--r--   0        0        0     2458 2023-07-14 23:07:36.740250 eztils-0.4.3/eztils/default/logging.py
+-rw-r--r--   0        0        0     1412 2023-07-15 08:36:51.519267 eztils-0.4.3/eztils/default/math.py
+-rw-r--r--   0        0        0     1091 2023-07-14 01:58:12.704178 eztils-0.4.3/eztils/default/structures.py
+-rw-r--r--   0        0        0     2346 2023-07-15 08:36:50.879275 eztils-0.4.3/eztils/git/__init__.py
+-rw-r--r--   0        0        0     1489 2023-07-15 08:36:51.539267 eztils-0.4.3/eztils/torch/__init__.py
+-rw-r--r--   0        0        0    15657 2023-07-15 08:36:51.763264 eztils-0.4.3/eztils/torch/distributions.py
+-rw-r--r--   0        0        0      155 2023-07-14 22:54:30.913527 eztils-0.4.3/eztils/torch/lightning.py
+-rw-r--r--   0        0        0      173 2023-07-14 22:54:30.917527 eztils-0.4.3/eztils/torch/math.py
+-rw-r--r--   0        0        0     2550 2023-07-15 08:36:51.535267 eztils-0.4.3/eztils/torch/modules.py
+-rw-r--r--   0        0        0     1420 2023-07-14 22:54:30.937527 eztils-0.4.3/eztils/torch/parameters.py
+-rw-r--r--   0        0        0     1668 2023-07-15 08:36:50.879275 eztils-0.4.3/eztils/torch/tensor_creators.py
+-rw-r--r--   0        0        0     2858 2023-07-14 23:03:35.175106 eztils-0.4.3/eztils/torch/to.py
+-rw-r--r--   0        0        0     3712 2023-07-15 08:38:50.197824 eztils-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    13848 1970-01-01 00:00:00.000000 eztils-0.4.3/PKG-INFO
```

### Comparing `eztils-0.4.2/LICENSE` & `eztils-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eztils-0.4.2/README.md` & `eztils-0.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # eztils
 
-# TODO add torchtyping?
 # TODO add tests
-
+# TODO add serialization to cloud or huggingface dataset
 <div align="center">
 
 [![Build status](https://github.com/ezhang7423/eztils/workflows/build/badge.svg?branch=master&event=push)](https://github.com/ezhang7423/eztils/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/eztils.svg)](https://pypi.org/project/eztils/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/ezhang7423/eztils/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/ezhang7423/eztils/blob/master/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/ezhang7423/eztils/releases)
 [![License](https://img.shields.io/github/license/ezhang7423/eztils)](https://github.com/ezhang7423/eztils/blob/master/LICENSE)
 
 eds utilities.
 
-torch, torchvision, and numpy are required but not specified, so as to be flexible with any environment this package is installed in.
+torch, torchvision, and torchtyping are required to use the torch package but not specified, so as to be flexible with any environment this package is installed in.
 
 </div>
 
 ## Installation
 
 `pip install eztils`
```

### Comparing `eztils-0.4.2/eztils/__init__.py` & `eztils-0.4.3/eztils/__init__.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.2/eztils/default/dict_operations.py` & `eztils-0.4.3/eztils/default/dict_operations.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.2/eztils/default/itertools.py` & `eztils-0.4.3/eztils/default/itertools.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.2/eztils/default/logging.py` & `eztils-0.4.3/eztils/default/logging.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.2/eztils/default/structures.py` & `eztils-0.4.3/eztils/default/structures.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.2/eztils/torch/parameters.py` & `eztils-0.4.3/eztils/torch/parameters.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.2/eztils/torch/to.py` & `eztils-0.4.3/eztils/torch/to.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.2/pyproject.toml` & `eztils-0.4.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = ["ezhang7423 <ezhang7423@student.palomar.edu>"]
 description = "eds utilities"
 homepage = "https://github.com/ezhang7423/eztils"
 license = "MIT"
 name = "eztils"
 readme = "README.md"
 repository = "https://github.com/ezhang7423/eztils"
-version = "0.4.2"
+version = "0.4.3"
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = [] #! Update me
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [
   #! Update me
@@ -52,14 +52,17 @@
 pylint = "^2.17.1"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-html = "^3.2.0"
 pyupgrade = "^3.3.1"
 ipython = "^8.11.0"
 
+# [tool.poetry.extras]
+# torch = ["torchtyping"]
+# TODO can't run this because torchtyping depends on torch. if only there was a way to get --no-deps to work: https://github.com/python-poetry/poetry/issues/3377
 
 [tool.black]
 # https://github.com/psf/black
 color = true
 line-length = 88
 target-version = ["py38"]
```

### Comparing `eztils-0.4.2/PKG-INFO` & `eztils-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eztils
-Version: 0.4.2
+Version: 0.4.3
 Summary: eds utilities
 Home-page: https://github.com/ezhang7423/eztils
 License: MIT
 Author: ezhang7423
 Author-email: ezhang7423@student.palomar.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -23,32 +23,31 @@
 Requires-Dist: rich (>=13.3.3,<14.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/ezhang7423/eztils
 Description-Content-Type: text/markdown
 
 # eztils
 
-# TODO add torchtyping?
 # TODO add tests
-
+# TODO add serialization to cloud or huggingface dataset
 <div align="center">
 
 [![Build status](https://github.com/ezhang7423/eztils/workflows/build/badge.svg?branch=master&event=push)](https://github.com/ezhang7423/eztils/actions?query=workflow%3Abuild)
 [![Python Version](https://img.shields.io/pypi/pyversions/eztils.svg)](https://pypi.org/project/eztils/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/ezhang7423/eztils/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/ezhang7423/eztils/blob/master/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/ezhang7423/eztils/releases)
 [![License](https://img.shields.io/github/license/ezhang7423/eztils)](https://github.com/ezhang7423/eztils/blob/master/LICENSE)
 
 eds utilities.
 
-torch, torchvision, and numpy are required but not specified, so as to be flexible with any environment this package is installed in.
+torch, torchvision, and torchtyping are required to use the torch package but not specified, so as to be flexible with any environment this package is installed in.
 
 </div>
 
 ## Installation
 
 `pip install eztils`
```

