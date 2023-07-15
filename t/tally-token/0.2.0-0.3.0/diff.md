# Comparing `tmp/tally-token-0.2.0.tar.gz` & `tmp/tally-token-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tally-token-0.2.0.tar", last modified: Sat Jul 15 01:35:28 2023, max compression
+gzip compressed data, was "tally-token-0.3.0.tar", last modified: Sat Jul 15 02:44:00 2023, max compression
```

## Comparing `tally-token-0.2.0.tar` & `tally-token-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:35:28.607541 tally-token-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-15 01:35:08.000000 tally-token-0.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:35:28.603541 tally-token-0.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-15 01:35:08.000000 tally-token-0.2.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-15 01:35:08.000000 tally-token-0.2.0/.github/renovate.json5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:35:28.603541 tally-token-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-15 01:35:08.000000 tally-token-0.2.0/.github/workflows/happy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-15 01:35:08.000000 tally-token-0.2.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-15 01:35:08.000000 tally-token-0.2.0/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-15 01:35:08.000000 tally-token-0.2.0/.github/workflows/spellcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-15 01:35:08.000000 tally-token-0.2.0/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-07-15 01:35:08.000000 tally-token-0.2.0/.gitignore.in
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-15 01:35:28.607541 tally-token-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-15 01:35:08.000000 tally-token-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    39018 2023-07-15 01:35:08.000000 tally-token-0.2.0/poetry.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-15 01:35:08.000000 tally-token-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-15 01:35:28.607541 tally-token-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:35:28.603541 tally-token-0.2.0/tally_token/
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-15 01:35:08.000000 tally-token-0.2.0/tally_token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-15 01:35:28.000000 tally-token-0.2.0/tally_token/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:35:28.607541 tally-token-0.2.0/tally_token.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-15 01:35:28.000000 tally-token-0.2.0/tally_token.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-15 01:35:28.000000 tally-token-0.2.0/tally_token.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 01:35:28.000000 tally-token-0.2.0/tally_token.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 01:35:28.000000 tally-token-0.2.0/tally_token.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:35:28.607541 tally-token-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-15 01:35:08.000000 tally-token-0.2.0/tests/test_basis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:44:00.908723 tally-token-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-15 02:43:40.000000 tally-token-0.3.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:44:00.908723 tally-token-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-15 02:43:40.000000 tally-token-0.3.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-15 02:43:40.000000 tally-token-0.3.0/.github/renovate.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:44:00.908723 tally-token-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-15 02:43:40.000000 tally-token-0.3.0/.github/workflows/happy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-15 02:43:40.000000 tally-token-0.3.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-15 02:43:40.000000 tally-token-0.3.0/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-15 02:43:40.000000 tally-token-0.3.0/.github/workflows/spellcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-15 02:43:40.000000 tally-token-0.3.0/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-07-15 02:43:40.000000 tally-token-0.3.0/.gitignore.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-07-15 02:44:00.908723 tally-token-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-07-15 02:43:40.000000 tally-token-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    39018 2023-07-15 02:43:40.000000 tally-token-0.3.0/poetry.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-15 02:43:40.000000 tally-token-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-15 02:44:00.908723 tally-token-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:44:00.908723 tally-token-0.3.0/tally_token/
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-15 02:43:40.000000 tally-token-0.3.0/tally_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-15 02:43:40.000000 tally-token-0.3.0/tally_token/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-15 02:44:00.000000 tally-token-0.3.0/tally_token/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:44:00.908723 tally-token-0.3.0/tally_token.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-07-15 02:44:00.000000 tally-token-0.3.0/tally_token.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-15 02:44:00.000000 tally-token-0.3.0/tally_token.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 02:44:00.000000 tally-token-0.3.0/tally_token.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-15 02:44:00.000000 tally-token-0.3.0/tally_token.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 02:44:00.000000 tally-token-0.3.0/tally_token.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:44:00.908723 tally-token-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-15 02:43:40.000000 tally-token-0.3.0/tests/test_basis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-15 02:43:40.000000 tally-token-0.3.0/tests/test_cli.py
```

### Comparing `tally-token-0.2.0/.github/workflows/pypi-publish.yml` & `tally-token-0.3.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `tally-token-0.2.0/.github/workflows/python-test.yml` & `tally-token-0.3.0/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `tally-token-0.2.0/.gitignore` & `tally-token-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tally-token-0.2.0/PKG-INFO` & `tally-token-0.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: tally-token
-Version: 0.2.0
-Summary: A library to split data into tokens
-Home-page: https://github.com/kitsuyui/python-tally-token
-Author: Yui Kitsu
-Author-email: kitsuyui+github@kitsuyui.com
-License: BSD-3-Clause
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Topic :: Security :: Cryptography
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # python-tally-token
 
 [![Python](https://img.shields.io/pypi/pyversions/tally-token.svg?style=plastic)](https://badge.fury.io/py/tally-token)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/tally-token.svg)](https://pypi.python.org/pypi/tally-token/)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 [![codecov](https://codecov.io/gh/kitsuyui/python-tally-token/branch/main/graph/badge.svg?token=OJ8QRXTTE9)](https://codecov.io/gh/kitsuyui/python-tally-token)
 
@@ -38,14 +18,44 @@
 
 ## Install
 
 ```sh
 $ pip install tally-token
 ```
 
+## CLI Usage
+
+```sh
+$ tally-token --help
+usage: tally-token [-h] {split,merge} ...
+
+positional arguments:
+  {split,merge}  Commands: split: split a file into multiple files merge: merge multiple files into a fileExample: tally-token split example.bin
+                 example.bin.1 example.bin.2 example.bin.3 tally-token merge example-merged.bin example.bin.1 example.bin.2 example.bin.3
+
+options:
+  -h, --help     show this help message and exit
+```
+
+### split
+
+You can use `split` to split a file into multiple files.
+
+```sh
+$ tally-token split something.bin split-1.bin split-2.bin split-3.bin
+```
+
+### merge
+
+You can use `merge` to merge multiple files into a file.
+
+```sh
+$ tally-token merge merged.bin split-1.bin split-2.bin split-3.bin
+```
+
 ## Example
 
 ### split
 
 You can use `split_text` to split text into tokens. `split_text` returns list of random bytes.
 
 ```python
```

#### html2text {}

```diff
@@ -1,36 +1,35 @@
-Metadata-Version: 2.1 Name: tally-token Version: 0.2.0 Summary: A library to
-split data into tokens Home-page: https://github.com/kitsuyui/python-tally-
-token Author: Yui Kitsu Author-email: kitsuyui+github@kitsuyui.com License:
-BSD-3-Clause Classifier: Development Status :: 3 - Alpha Classifier: License ::
-OSI Approved :: BSD License Classifier: Topic :: Security :: Cryptography
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.7 Description-Content-Type: text/markdown # python-tally-
-token [![Python](https://img.shields.io/pypi/pyversions/tally-
+# python-tally-token [![Python](https://img.shields.io/pypi/pyversions/tally-
 token.svg?style=plastic)](https://badge.fury.io/py/tally-token) [![PyPI version
 shields.io](https://img.shields.io/pypi/v/tally-token.svg)](https://
 pypi.python.org/pypi/tally-token/) [![License](https://img.shields.io/badge/
 License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-
 Clause) [![codecov](https://codecov.io/gh/kitsuyui/python-tally-token/branch/
 main/graph/badge.svg?token=OJ8QRXTTE9)](https://codecov.io/gh/kitsuyui/python-
 tally-token) ## What is this? tally-token is a Python library for split data
 into tokens with same length. [Tally](https://en.wikipedia.org/wiki/
 Tally_stick) is a historical object for prove something by splitting wood into
 tokens and matching tokens. [https://github.com/kitsuyui/python-tally-token/
 assets/2596972/103a0184-c508-4ce6-9ed3-1b1eb58bc6cc] > Medieval English split
 tally stick (front and reverse view). The stick is notched and inscribed to
 record a debt owed to the rural dean of Preston Candover, Hampshire, of a tithe
 of 20d each on 32 sheep, amounting to a total sum of Â£2 13s. 4d. # Usage ##
-Install ```sh $ pip install tally-token ``` ## Example ### split You can use
-`split_text` to split text into tokens. `split_text` returns list of random
-bytes. ```python >>> from tally_token import split_text >>> split_text("Hello,
-World!") [b'qQ\xa5\x97\x84\x88\xd7U%\xfb(k\xa1',
+Install ```sh $ pip install tally-token ``` ## CLI Usage ```sh $ tally-token --
+help usage: tally-token [-h] {split,merge} ... positional arguments:
+{split,merge} Commands: split: split a file into multiple files merge: merge
+multiple files into a fileExample: tally-token split example.bin example.bin.1
+example.bin.2 example.bin.3 tally-token merge example-merged.bin example.bin.1
+example.bin.2 example.bin.3 options: -h, --help show this help message and exit
+``` ### split You can use `split` to split a file into multiple files. ```sh $
+tally-token split something.bin split-1.bin split-2.bin split-3.bin ``` ###
+merge You can use `merge` to merge multiple files into a file. ```sh $ tally-
+token merge merged.bin split-1.bin split-2.bin split-3.bin ``` ## Example ###
+split You can use `split_text` to split text into tokens. `split_text` returns
+list of random bytes. ```python >>> from tally_token import split_text >>>
+split_text("Hello, World!") [b'qQ\xa5\x97\x84\x88\xd7U%\xfb(k\xa1',
 b'94\xc9\xfb\xeb\xa4\xf7\x02J\x89D\x0f\x80'] ``` ### merge You can use
 `merge_text` to merge tokens into text. `merge_text` returns cleartext.
 ```python >>> from tally_token import merge_text >>> merge_text(
 [b'qQ\xa5\x97\x84\x88\xd7U%\xfb(k\xa1',
 b'94\xc9\xfb\xeb\xa4\xf7\x02J\x89D\x0f\x80']) 'Hello, World!' ``` ### split
 with custom length ```python >>> from tally_token import split_text, merge_text
 >>> split_text("Hello, World!", 5) [b'N&\xce\\\xbc6dxp\x87\xa8#z',
```

### Comparing `tally-token-0.2.0/poetry.lock` & `tally-token-0.3.0/poetry.lock`

 * *Files identical despite different names*

### Comparing `tally-token-0.2.0/pyproject.toml` & `tally-token-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tally-token-0.2.0/setup.cfg` & `tally-token-0.3.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -24,11 +24,15 @@
 test_suite = tests
 python_requires = >= 3.7
 
 [options.package_data]
 * = README.md, LICENSE
 tally_token = py.typed, *.pyi
 
+[options.entry_points]
+console_scripts = 
+	tally-token = tally_token.__main__:main
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `tally-token-0.2.0/tally_token/__init__.py` & `tally-token-0.3.0/tally_token/__init__.py`

 * *Files identical despite different names*

### Comparing `tally-token-0.2.0/tally_token.egg-info/PKG-INFO` & `tally-token-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tally-token
-Version: 0.2.0
+Version: 0.3.0
 Summary: A library to split data into tokens
 Home-page: https://github.com/kitsuyui/python-tally-token
 Author: Yui Kitsu
 Author-email: kitsuyui+github@kitsuyui.com
 License: BSD-3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
@@ -38,14 +38,44 @@
 
 ## Install
 
 ```sh
 $ pip install tally-token
 ```
 
+## CLI Usage
+
+```sh
+$ tally-token --help
+usage: tally-token [-h] {split,merge} ...
+
+positional arguments:
+  {split,merge}  Commands: split: split a file into multiple files merge: merge multiple files into a fileExample: tally-token split example.bin
+                 example.bin.1 example.bin.2 example.bin.3 tally-token merge example-merged.bin example.bin.1 example.bin.2 example.bin.3
+
+options:
+  -h, --help     show this help message and exit
+```
+
+### split
+
+You can use `split` to split a file into multiple files.
+
+```sh
+$ tally-token split something.bin split-1.bin split-2.bin split-3.bin
+```
+
+### merge
+
+You can use `merge` to merge multiple files into a file.
+
+```sh
+$ tally-token merge merged.bin split-1.bin split-2.bin split-3.bin
+```
+
 ## Example
 
 ### split
 
 You can use `split_text` to split text into tokens. `split_text` returns list of random bytes.
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tally-token Version: 0.2.0 Summary: A library to
+Metadata-Version: 2.1 Name: tally-token Version: 0.3.0 Summary: A library to
 split data into tokens Home-page: https://github.com/kitsuyui/python-tally-
 token Author: Yui Kitsu Author-email: kitsuyui+github@kitsuyui.com License:
 BSD-3-Clause Classifier: Development Status :: 3 - Alpha Classifier: License ::
 OSI Approved :: BSD License Classifier: Topic :: Security :: Cryptography
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
@@ -19,18 +19,27 @@
 into tokens with same length. [Tally](https://en.wikipedia.org/wiki/
 Tally_stick) is a historical object for prove something by splitting wood into
 tokens and matching tokens. [https://github.com/kitsuyui/python-tally-token/
 assets/2596972/103a0184-c508-4ce6-9ed3-1b1eb58bc6cc] > Medieval English split
 tally stick (front and reverse view). The stick is notched and inscribed to
 record a debt owed to the rural dean of Preston Candover, Hampshire, of a tithe
 of 20d each on 32 sheep, amounting to a total sum of Â£2 13s. 4d. # Usage ##
-Install ```sh $ pip install tally-token ``` ## Example ### split You can use
-`split_text` to split text into tokens. `split_text` returns list of random
-bytes. ```python >>> from tally_token import split_text >>> split_text("Hello,
-World!") [b'qQ\xa5\x97\x84\x88\xd7U%\xfb(k\xa1',
+Install ```sh $ pip install tally-token ``` ## CLI Usage ```sh $ tally-token --
+help usage: tally-token [-h] {split,merge} ... positional arguments:
+{split,merge} Commands: split: split a file into multiple files merge: merge
+multiple files into a fileExample: tally-token split example.bin example.bin.1
+example.bin.2 example.bin.3 tally-token merge example-merged.bin example.bin.1
+example.bin.2 example.bin.3 options: -h, --help show this help message and exit
+``` ### split You can use `split` to split a file into multiple files. ```sh $
+tally-token split something.bin split-1.bin split-2.bin split-3.bin ``` ###
+merge You can use `merge` to merge multiple files into a file. ```sh $ tally-
+token merge merged.bin split-1.bin split-2.bin split-3.bin ``` ## Example ###
+split You can use `split_text` to split text into tokens. `split_text` returns
+list of random bytes. ```python >>> from tally_token import split_text >>>
+split_text("Hello, World!") [b'qQ\xa5\x97\x84\x88\xd7U%\xfb(k\xa1',
 b'94\xc9\xfb\xeb\xa4\xf7\x02J\x89D\x0f\x80'] ``` ### merge You can use
 `merge_text` to merge tokens into text. `merge_text` returns cleartext.
 ```python >>> from tally_token import merge_text >>> merge_text(
 [b'qQ\xa5\x97\x84\x88\xd7U%\xfb(k\xa1',
 b'94\xc9\xfb\xeb\xa4\xf7\x02J\x89D\x0f\x80']) 'Hello, World!' ``` ### split
 with custom length ```python >>> from tally_token import split_text, merge_text
 >>> split_text("Hello, World!", 5) [b'N&\xce\\\xbc6dxp\x87\xa8#z',
```

### Comparing `tally-token-0.2.0/tests/test_basis.py` & `tally-token-0.3.0/tests/test_basis.py`

 * *Files identical despite different names*

