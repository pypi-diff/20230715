# Comparing `tmp/rss_parser-1.0.0.tar.gz` & `tmp/rss_parser-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rss_parser-1.0.0.tar", max compression
+gzip compressed data, was "rss_parser-1.1.0.tar", max compression
```

## Comparing `rss_parser-1.0.0.tar` & `rss_parser-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    35151 2023-05-31 18:08:42.610093 rss_parser-1.0.0/LICENSE
--rw-r--r--   0        0        0     5717 2023-05-31 18:08:42.610093 rss_parser-1.0.0/README.md
--rw-r--r--   0        0        0     2378 2023-05-31 18:08:42.610093 rss_parser-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       28 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/__init__.py
--rw-r--r--   0        0        0     1158 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/_parser.py
--rw-r--r--   0        0        0      885 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/__init__.py
--rw-r--r--   0        0        0     4854 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/channel.py
--rw-r--r--   0        0        0     1074 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/image.py
--rw-r--r--   0        0        0     1475 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/item.py
--rw-r--r--   0        0        0      321 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/rss.py
--rw-r--r--   0        0        0      751 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/text_input.py
--rw-r--r--   0        0        0       99 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/types/__init__.py
--rw-r--r--   0        0        0      934 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/types/date.py
--rw-r--r--   0        0        0     4666 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/types/tag.py
--rw-r--r--   0        0        0      140 2023-05-31 18:08:42.610093 rss_parser-1.0.0/rss_parser/models/utils.py
--rw-r--r--   0        0        0     7076 1970-01-01 00:00:00.000000 rss_parser-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35151 2023-07-15 00:15:24.290161 rss_parser-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5655 2023-07-15 00:15:24.290161 rss_parser-1.1.0/README.md
+-rw-r--r--   0        0        0     2376 2023-07-15 00:15:24.294161 rss_parser-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-07-15 00:15:24.294161 rss_parser-1.1.0/rss_parser/__init__.py
+-rw-r--r--   0        0        0     1158 2023-07-15 00:15:24.294161 rss_parser-1.1.0/rss_parser/_parser.py
+-rw-r--r--   0        0        0      885 2023-07-15 00:15:24.294161 rss_parser-1.1.0/rss_parser/models/__init__.py
+-rw-r--r--   0        0        0     4854 2023-07-15 00:15:24.294161 rss_parser-1.1.0/rss_parser/models/channel.py
+-rw-r--r--   0        0        0     1074 2023-07-15 00:15:24.294161 rss_parser-1.1.0/rss_parser/models/image.py
+-rw-r--r--   0        0        0     1475 2023-07-15 00:15:24.294161 rss_parser-1.1.0/rss_parser/models/item.py
+-rw-r--r--   0        0        0      321 2023-07-15 00:15:24.294161 rss_parser-1.1.0/rss_parser/models/rss.py
+-rw-r--r--   0        0        0      751 2023-07-15 00:15:24.294161 rss_parser-1.1.0/rss_parser/models/text_input.py
+-rw-r--r--   0        0        0       99 2023-07-15 00:15:24.294161 rss_parser-1.1.0/rss_parser/models/types/__init__.py
+-rw-r--r--   0        0        0      934 2023-07-15 00:15:24.294161 rss_parser-1.1.0/rss_parser/models/types/date.py
+-rw-r--r--   0        0        0     4666 2023-07-15 00:15:24.294161 rss_parser-1.1.0/rss_parser/models/types/tag.py
+-rw-r--r--   0        0        0      140 2023-07-15 00:15:24.294161 rss_parser-1.1.0/rss_parser/models/utils.py
+-rw-r--r--   0        0        0        0 2023-07-15 00:15:24.294161 rss_parser-1.1.0/rss_parser/py.typed
+-rw-r--r--   0        0        0     6928 1970-01-01 00:00:00.000000 rss_parser-1.1.0/PKG-INFO
```

### Comparing `rss_parser-1.0.0/LICENSE` & `rss_parser-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rss_parser-1.0.0/README.md` & `rss_parser-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Rss parser
 
 [![Downloads](https://pepy.tech/badge/rss-parser)](https://pepy.tech/project/rss-parser)
-[![Downloads](https://pepy.tech/badge/rss-parser/month)](https://pepy.tech/project/rss-parser/month)
-[![Downloads](https://pepy.tech/badge/rss-parser/week)](https://pepy.tech/project/rss-parser/week)
+[![Downloads](https://pepy.tech/badge/rss-parser/month)](https://pepy.tech/project/rss-parser)
+[![Downloads](https://pepy.tech/badge/rss-parser/week)](https://pepy.tech/project/rss-parser)
 
 [![PyPI version](https://img.shields.io/pypi/v/rss-parser)](https://pypi.org/project/rss-parser)
 [![Python versions](https://img.shields.io/pypi/pyversions/rss-parser)](https://pypi.org/project/rss-parser)
 [![Wheel status](https://img.shields.io/pypi/wheel/rss-parser)](https://pypi.org/project/rss-parser)
 [![License](https://img.shields.io/pypi/l/rss-parser?color=success)](https://github.com/dhvcc/rss-parser/blob/master/LICENSE)
-[![GitHub Pages](https://badgen.net/github/status/dhvcc/rss-parser/gh-pages?label=docs)](https://dhvcc.github.io/rss-parser#documentation)
 
+![Docs](https://github.com/dhvcc/rss-parser/actions/workflows/pages/pages-build-deployment/badge.svg)
 ![CI](https://github.com/dhvcc/rss-parser/actions/workflows/ci.yml/badge.svg?branch=master)
-![PyPi publish](https://github.com/dhvcc/rss-parser/actions/workflows/publish_to_pypi.yml/badge.svg?branch=master)
+![PyPi publish](https://github.com/dhvcc/rss-parser/actions/workflows/publish_to_pypi.yml/badge.svg)
 
 ## About
 
 `rss-parser` is typed python RSS parsing module built using [pydantic](https://github.com/pydantic/pydantic) and [xmltodict](https://github.com/martinblech/xmltodict)
 
 ## Installation
```

### Comparing `rss_parser-1.0.0/pyproject.toml` & `rss_parser-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rss-parser"
-version = "1.0.0"
+version = "1.1.0"
 description = "Typed pythonic RSS parser"
 authors = ["dhvcc <1337kwiz@gmail.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 keywords = [
     "python",
     "python3",
@@ -25,36 +25,38 @@
     "Typing :: Typed",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
 ]
-packages = [{include = "rss_parser"}]
+packages = [
+    {include = "rss_parser"},
+    {include = "rss_parser/py.typed"},
+]
 
 
 [tool.poetry.urls]
 "Homepage" = "https://dhvcc.github.io/rss-parser"
 "Source" = "https://github.com/dhvcc/rss-parser"
 "Bug Tracker" = "https://github.com/dhvcc/rss-parser/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = ">=1.6.1"
-pytest = "^7.1.2"
+pydantic = "^1.10"
 xmltodict = "^0.13.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "*"
 black = "^22.3.0"
 pre-commit = "^2.12.0"
 ruff = "*"
 rich = "*"
+pytest = "^7.4.0"
 
 [tool.pytest.ini_options]
 addopts = "-color=yes"
 
 [tool.black]
 line-length = 120
 target-version = ["py38"]
```

### Comparing `rss_parser-1.0.0/rss_parser/_parser.py` & `rss_parser-1.1.0/rss_parser/_parser.py`

 * *Files identical despite different names*

### Comparing `rss_parser-1.0.0/rss_parser/models/__init__.py` & `rss_parser-1.1.0/rss_parser/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rss_parser-1.0.0/rss_parser/models/channel.py` & `rss_parser-1.1.0/rss_parser/models/channel.py`

 * *Files identical despite different names*

### Comparing `rss_parser-1.0.0/rss_parser/models/image.py` & `rss_parser-1.1.0/rss_parser/models/image.py`

 * *Files identical despite different names*

### Comparing `rss_parser-1.0.0/rss_parser/models/item.py` & `rss_parser-1.1.0/rss_parser/models/item.py`

 * *Files identical despite different names*

### Comparing `rss_parser-1.0.0/rss_parser/models/text_input.py` & `rss_parser-1.1.0/rss_parser/models/text_input.py`

 * *Files identical despite different names*

### Comparing `rss_parser-1.0.0/rss_parser/models/types/date.py` & `rss_parser-1.1.0/rss_parser/models/types/date.py`

 * *Files identical despite different names*

### Comparing `rss_parser-1.0.0/rss_parser/models/types/tag.py` & `rss_parser-1.1.0/rss_parser/models/types/tag.py`

 * *Files identical despite different names*

### Comparing `rss_parser-1.0.0/PKG-INFO` & `rss_parser-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rss-parser
-Version: 1.0.0
+Version: 1.1.0
 Summary: Typed pythonic RSS parser
 License: GPL-3.0
 Keywords: python,python3,cli,rss,parser,gplv3,typed,typed-python
 Author: dhvcc
 Author-email: 1337kwiz@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,41 +13,39 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Typing :: Typed
-Requires-Dist: pydantic (>=1.6.1)
-Requires-Dist: pytest (>=7.1.2,<8.0.0)
+Requires-Dist: pydantic (>=1.10,<2.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Project-URL: Bug Tracker, https://github.com/dhvcc/rss-parser/issues
 Project-URL: Homepage, https://dhvcc.github.io/rss-parser
 Project-URL: Source, https://github.com/dhvcc/rss-parser
 Description-Content-Type: text/markdown
 
 # Rss parser
 
 [![Downloads](https://pepy.tech/badge/rss-parser)](https://pepy.tech/project/rss-parser)
-[![Downloads](https://pepy.tech/badge/rss-parser/month)](https://pepy.tech/project/rss-parser/month)
-[![Downloads](https://pepy.tech/badge/rss-parser/week)](https://pepy.tech/project/rss-parser/week)
+[![Downloads](https://pepy.tech/badge/rss-parser/month)](https://pepy.tech/project/rss-parser)
+[![Downloads](https://pepy.tech/badge/rss-parser/week)](https://pepy.tech/project/rss-parser)
 
 [![PyPI version](https://img.shields.io/pypi/v/rss-parser)](https://pypi.org/project/rss-parser)
 [![Python versions](https://img.shields.io/pypi/pyversions/rss-parser)](https://pypi.org/project/rss-parser)
 [![Wheel status](https://img.shields.io/pypi/wheel/rss-parser)](https://pypi.org/project/rss-parser)
 [![License](https://img.shields.io/pypi/l/rss-parser?color=success)](https://github.com/dhvcc/rss-parser/blob/master/LICENSE)
-[![GitHub Pages](https://badgen.net/github/status/dhvcc/rss-parser/gh-pages?label=docs)](https://dhvcc.github.io/rss-parser#documentation)
 
+![Docs](https://github.com/dhvcc/rss-parser/actions/workflows/pages/pages-build-deployment/badge.svg)
 ![CI](https://github.com/dhvcc/rss-parser/actions/workflows/ci.yml/badge.svg?branch=master)
-![PyPi publish](https://github.com/dhvcc/rss-parser/actions/workflows/publish_to_pypi.yml/badge.svg?branch=master)
+![PyPi publish](https://github.com/dhvcc/rss-parser/actions/workflows/publish_to_pypi.yml/badge.svg)
 
 ## About
 
 `rss-parser` is typed python RSS parsing module built using [pydantic](https://github.com/pydantic/pydantic) and [xmltodict](https://github.com/martinblech/xmltodict)
 
 ## Installation
```

