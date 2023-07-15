# Comparing `tmp/morecopy-0.2.4.tar.gz` & `tmp/morecopy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morecopy-0.2.4.tar", max compression
+gzip compressed data, was "morecopy-0.3.0.tar", max compression
```

## Comparing `morecopy-0.2.4.tar` & `morecopy-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1071 2021-12-16 12:45:38.101297 morecopy-0.2.4/LICENSE
--rw-r--r--   0        0        0     2003 2021-12-16 12:45:38.101297 morecopy-0.2.4/README.md
--rw-r--r--   0        0        0      148 2021-12-16 12:45:38.101297 morecopy-0.2.4/morecopy/__init__.py
--rw-r--r--   0        0        0     1714 2021-12-16 12:45:38.101297 morecopy-0.2.4/morecopy/copiers.py
--rw-r--r--   0        0        0      922 2021-12-16 12:45:38.101297 morecopy-0.2.4/morecopy/copy.py
--rw-r--r--   0        0        0        0 2021-12-16 12:45:38.101297 morecopy-0.2.4/morecopy/py.typed
--rw-r--r--   0        0        0      528 2021-12-16 12:45:38.101297 morecopy-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2660 2021-12-16 12:45:48.727595 morecopy-0.2.4/setup.py
--rw-r--r--   0        0        0     2641 2021-12-16 12:45:48.727940 morecopy-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-15 14:14:12.168914 morecopy-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2358 2023-07-15 14:14:12.168914 morecopy-0.3.0/README.md
+-rw-r--r--   0        0        0      180 2023-07-15 14:14:12.168914 morecopy-0.3.0/morecopy/__init__.py
+-rw-r--r--   0        0        0     1714 2023-07-15 14:14:12.168914 morecopy-0.3.0/morecopy/copiers.py
+-rw-r--r--   0        0        0      922 2023-07-15 14:14:12.168914 morecopy-0.3.0/morecopy/copy.py
+-rw-r--r--   0        0        0        0 2023-07-15 14:14:12.168914 morecopy-0.3.0/morecopy/py.typed
+-rw-r--r--   0        0        0      526 2023-07-15 14:14:12.168914 morecopy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2998 1970-01-01 00:00:00.000000 morecopy-0.3.0/PKG-INFO
```

### Comparing `morecopy-0.2.4/LICENSE` & `morecopy-0.3.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Akio Taniguchi
+Copyright (c) 2021-2023 Akio Taniguchi
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `morecopy-0.2.4/README.md` & `morecopy-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,32 @@
+Metadata-Version: 2.1
+Name: morecopy
+Version: 0.3.0
+Summary: Copy even immutable objects as much as possible
+Home-page: https://github.com/astropenguin/morecopy/
+License: MIT
+Keywords: copy,deepcopy
+Author: Akio Taniguchi
+Author-email: taniguchi@a.phys.nagoya-u.ac.jp
+Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
 # morecopy
 
-[![PyPI](https://img.shields.io/pypi/v/morecopy.svg?label=PyPI&style=flat-square)](https://pypi.org/project/morecopy/)
-[![Python](https://img.shields.io/pypi/pyversions/morecopy.svg?label=Python&color=yellow&style=flat-square)](https://pypi.org/project/morecopy/)
-[![Test](https://img.shields.io/github/workflow/status/astropenguin/morecopy/Tests?logo=github&label=Test&style=flat-square)](https://github.com/astropenguin/morecopy/actions)
-[![License](https://img.shields.io/badge/license-MIT-blue.svg?label=License&style=flat-square)](LICENSE)
-[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.5594444-blue?style=flat-square)](https://doi.org/10.5281/zenodo.5594444)
+[![Release](https://img.shields.io/pypi/v/morecopy?label=Release&color=cornflowerblue&style=flat-square)](https://pypi.org/project/morecopy/)
+[![Python](https://img.shields.io/pypi/pyversions/morecopy?label=Python&color=cornflowerblue&style=flat-square)](https://pypi.org/project/morecopy/)
+[![Downloads](https://img.shields.io/pypi/dm/morecopy?label=Downloads&color=cornflowerblue&style=flat-square)](https://pepy.tech/project/morecopy)
+[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.5594444-cornflowerblue?style=flat-square)](https://doi.org/10.5281/zenodo.5594444)
+[![Tests](https://img.shields.io/github/actions/workflow/status/astropenguin/morecopy/tests.yml?label=Tests&style=flat-square)](https://github.com/astropenguin/morecopy/actions)
 
 Copy even immutable objects as much as possible
 
 ## Overview
 
 morecopy is a Python package that enables copy of immutable objects so that a copied object is equivalent but not identical to the original:
 
@@ -19,14 +37,19 @@
 original = 1234567890
 copied = copy(original)
 
 original == copied # -> True
 original is copied # -> False
 ```
 
+> **Note**
+> In general, there is no need to copy immutable objects, so this package may not be necessary in most cases.
+> Also, some objects may not be copied even with this package:
+> In CPython, for example, integers from -5 to 256 are always uncopied for optimization.
+
 ## Installation
 
 ```shell
 $ pip install morecopy
 ```
 
 ## Supported immutable types
@@ -57,7 +80,8 @@
 from morecopy import copier_for
 
 
 @copier_for(int)
 def copy_int(integer: int) -> int:
     return eval(repr(integer))
 ```
+
```

### Comparing `morecopy-0.2.4/morecopy/copiers.py` & `morecopy-0.3.0/morecopy/copiers.py`

 * *Files identical despite different names*

### Comparing `morecopy-0.2.4/morecopy/copy.py` & `morecopy-0.3.0/morecopy/copy.py`

 * *Files identical despite different names*

### Comparing `morecopy-0.2.4/pyproject.toml` & `morecopy-0.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "morecopy"
-version = "0.2.4"
+version = "0.3.0"
 description = "Copy even immutable objects as much as possible"
 keywords = ["copy", "deepcopy"]
 authors = ["Akio Taniguchi <taniguchi@a.phys.nagoya-u.ac.jp>"]
 license = "MIT"
 readme = "README.md"
-homepage = "https://github.com/astropenguin/morecopy"
+homepage = "https://github.com/astropenguin/morecopy/"
 
 [tool.poetry.dependencies]
-python = ">=3.7, <3.11"
+python = ">=3.8, <3.12"
 
-[tool.poetry.dev-dependencies]
-black = "^21.12b"
-ipython = "^7.30"
-pytest = "^6.2"
+[tool.poetry.group.dev.dependencies]
+black = "^23.7"
+ipython = "^8.12"
+pytest = "^7.4"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `morecopy-0.2.4/setup.py` & `morecopy-0.3.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,68 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# morecopy
 
-packages = \
-['morecopy']
+[![Release](https://img.shields.io/pypi/v/morecopy?label=Release&color=cornflowerblue&style=flat-square)](https://pypi.org/project/morecopy/)
+[![Python](https://img.shields.io/pypi/pyversions/morecopy?label=Python&color=cornflowerblue&style=flat-square)](https://pypi.org/project/morecopy/)
+[![Downloads](https://img.shields.io/pypi/dm/morecopy?label=Downloads&color=cornflowerblue&style=flat-square)](https://pepy.tech/project/morecopy)
+[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.5594444-cornflowerblue?style=flat-square)](https://doi.org/10.5281/zenodo.5594444)
+[![Tests](https://img.shields.io/github/actions/workflow/status/astropenguin/morecopy/tests.yml?label=Tests&style=flat-square)](https://github.com/astropenguin/morecopy/actions)
 
-package_data = \
-{'': ['*']}
+Copy even immutable objects as much as possible
 
-setup_kwargs = {
-    'name': 'morecopy',
-    'version': '0.2.4',
-    'description': 'Copy even immutable objects as much as possible',
-    'long_description': '# morecopy\n\n[![PyPI](https://img.shields.io/pypi/v/morecopy.svg?label=PyPI&style=flat-square)](https://pypi.org/project/morecopy/)\n[![Python](https://img.shields.io/pypi/pyversions/morecopy.svg?label=Python&color=yellow&style=flat-square)](https://pypi.org/project/morecopy/)\n[![Test](https://img.shields.io/github/workflow/status/astropenguin/morecopy/Tests?logo=github&label=Test&style=flat-square)](https://github.com/astropenguin/morecopy/actions)\n[![License](https://img.shields.io/badge/license-MIT-blue.svg?label=License&style=flat-square)](LICENSE)\n[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.5594444-blue?style=flat-square)](https://doi.org/10.5281/zenodo.5594444)\n\nCopy even immutable objects as much as possible\n\n## Overview\n\nmorecopy is a Python package that enables copy of immutable objects so that a copied object is equivalent but not identical to the original:\n\n```python\nfrom morecopy import copy\n\n\noriginal = 1234567890\ncopied = copy(original)\n\noriginal == copied # -> True\noriginal is copied # -> False\n```\n\n## Installation\n\n```shell\n$ pip install morecopy\n```\n\n## Supported immutable types\n\nThe following types are supported.\nFor mutable types (e.g. `list`) or unsupported immutable types (e.g. `bool`, `NoneType`), `morecopy.copy` and `morecopy.deepcopy` are equivalent to `copy.copy` and `copy.deepcopy`, respectively.\n\nType | `morecopy.copy` | `morecopy.deepcopy`\n--- | --- | ---\n`int` | yes | n/a\n`float` | yes | n/a\n`complex` | yes | n/a\n`str` | yes | n/a\n`bytes` | yes | n/a\n`tuple` | yes | n/a\n`range` | yes | n/a\n`slice` | yes | n/a\n`frozenset` | yes | n/a\n`FunctionType` | yes | n/a\n`LambdaType` | yes | n/a\n\n## Custom immutable copier\n\nUsers can add a custom copy function (copier) for a type.\nFor example, the following code defines copy of integer by creating a copy function and registering it by the `copier_for` decorator.\n\n```python\nfrom morecopy import copier_for\n\n\n@copier_for(int)\ndef copy_int(integer: int) -> int:\n    return eval(repr(integer))\n```\n',
-    'author': 'Akio Taniguchi',
-    'author_email': 'taniguchi@a.phys.nagoya-u.ac.jp',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/astropenguin/morecopy',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.7,<3.11',
-}
+## Overview
 
+morecopy is a Python package that enables copy of immutable objects so that a copied object is equivalent but not identical to the original:
 
-setup(**setup_kwargs)
+```python
+from morecopy import copy
+
+
+original = 1234567890
+copied = copy(original)
+
+original == copied # -> True
+original is copied # -> False
+```
+
+> **Note**
+> In general, there is no need to copy immutable objects, so this package may not be necessary in most cases.
+> Also, some objects may not be copied even with this package:
+> In CPython, for example, integers from -5 to 256 are always uncopied for optimization.
+
+## Installation
+
+```shell
+$ pip install morecopy
+```
+
+## Supported immutable types
+
+The following types are supported.
+For mutable types (e.g. `list`) or unsupported immutable types (e.g. `bool`, `NoneType`), `morecopy.copy` and `morecopy.deepcopy` are equivalent to `copy.copy` and `copy.deepcopy`, respectively.
+
+Type | `morecopy.copy` | `morecopy.deepcopy`
+--- | --- | ---
+`int` | yes | n/a
+`float` | yes | n/a
+`complex` | yes | n/a
+`str` | yes | n/a
+`bytes` | yes | n/a
+`tuple` | yes | n/a
+`range` | yes | n/a
+`slice` | yes | n/a
+`frozenset` | yes | n/a
+`FunctionType` | yes | n/a
+`LambdaType` | yes | n/a
+
+## Custom immutable copier
+
+Users can add a custom copy function (copier) for a type.
+For example, the following code defines copy of integer by creating a copy function and registering it by the `copier_for` decorator.
+
+```python
+from morecopy import copier_for
+
+
+@copier_for(int)
+def copy_int(integer: int) -> int:
+    return eval(repr(integer))
+```
```

