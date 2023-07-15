# Comparing `tmp/dl-hf-model-0.1.0a0.tar.gz` & `tmp/dl-hf-model-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dl-hf-model-0.1.0a0.tar", max compression
+gzip compressed data, was "dl-hf-model-0.1.0a1.tar", max compression
```

## Comparing `dl-hf-model-0.1.0a0.tar` & `dl-hf-model-0.1.0a1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      106 2023-07-15 08:39:14.904537 dl-hf-model-0.1.0a0/dl_hf_model/__init__.py
--rw-r--r--   0        0        0      951 2023-07-15 08:39:14.920127 dl-hf-model-0.1.0a0/dl_hf_model/__main__.py
--rw-r--r--   0        0        0     1064 2023-07-15 11:54:53.395182 dl-hf-model-0.1.0a0/dl_hf_model/dl_hf_model.py
--rw-r--r--   0        0        0     1085 2023-07-15 08:39:14.795160 dl-hf-model-0.1.0a0/LICENSE
--rw-r--r--   0        0        0     1864 2023-07-15 11:53:30.993190 dl-hf-model-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0      984 2023-07-15 08:44:47.671253 dl-hf-model-0.1.0a0/README.md
--rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 dl-hf-model-0.1.0a0/setup.py
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 dl-hf-model-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0      106 2023-07-15 13:03:08.213508 dl-hf-model-0.1.0a1/dl_hf_model/__init__.py
+-rw-r--r--   0        0        0      951 2023-07-15 08:39:14.920127 dl-hf-model-0.1.0a1/dl_hf_model/__main__.py
+-rw-r--r--   0        0        0     1338 2023-07-15 13:05:00.116438 dl-hf-model-0.1.0a1/dl_hf_model/dl_hf_model.py
+-rw-r--r--   0        0        0     1085 2023-07-15 08:39:14.795160 dl-hf-model-0.1.0a1/LICENSE
+-rw-r--r--   0        0        0     1858 2023-07-15 13:02:53.003086 dl-hf-model-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0      984 2023-07-15 08:44:47.671253 dl-hf-model-0.1.0a1/README.md
+-rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 dl-hf-model-0.1.0a1/setup.py
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 dl-hf-model-0.1.0a1/PKG-INFO
```

### Comparing `dl-hf-model-0.1.0a0/dl_hf_model/__main__.py` & `dl-hf-model-0.1.0a1/dl_hf_model/__main__.py`

 * *Files identical despite different names*

### Comparing `dl-hf-model-0.1.0a0/LICENSE` & `dl-hf-model-0.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `dl-hf-model-0.1.0a0/pyproject.toml` & `dl-hf-model-0.1.0a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dl-hf-model"
-version = "0.1.0-alpha.0"
+version = "0.1.0a1"
 description = "Download and cache a hf model for a given url, save to models dir"
 authors = ["ffreemt"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ffreemt/dl-hf-model"
 
 [tool.poetry.dependencies]
```

### Comparing `dl-hf-model-0.1.0a0/README.md` & `dl-hf-model-0.1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `dl-hf-model-0.1.0a0/setup.py` & `dl-hf-model-0.1.0a1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'typer>=0.4.1,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['dl-hf-model = dl_hf_model.__main__:app']}
 
 setup_kwargs = {
     'name': 'dl-hf-model',
-    'version': '0.1.0a0',
+    'version': '0.1.0a1',
     'description': 'Download and cache a hf model for a given url, save to models dir',
     'long_description': '# dl-hf-model\n[![pytest](https://github.com/ffreemt/dl-hf-model/actions/workflows/routine-tests.yml/badge.svg)](https://github.com/ffreemt/dl-hf-model/actions)[![python](https://img.shields.io/static/v1?label=python+&message=3.8%2B&color=blue)](https://www.python.org/downloads/)[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)[![PyPI version](https://badge.fury.io/py/dl_hf_model.svg)](https://badge.fury.io/py/dl_hf_model)\n\nDownload and cache a huggingface model given a url, save to models dir\n\n## Install it\n\n```shell\npip install dl-hf-model\n# pip install git+https://github.com/ffreemt/dl-hf-model\n# poetry add git+https://github.com/ffreemt/dl-hf-model\n# git clone https://github.com/ffreemt/dl-hf-model && cd dl-hf-model\n```\n\n## Use it\n```python\nfrom dl_hf_model import dl_hf_model\n\n```\n',
     'author': 'ffreemt',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ffreemt/dl-hf-model',
```

### Comparing `dl-hf-model-0.1.0a0/PKG-INFO` & `dl-hf-model-0.1.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dl-hf-model
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: Download and cache a hf model for a given url, save to models dir
 Home-page: https://github.com/ffreemt/dl-hf-model
 License: MIT
 Author: ffreemt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

