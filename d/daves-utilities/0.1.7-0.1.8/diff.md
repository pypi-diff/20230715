# Comparing `tmp/daves_utilities-0.1.7.tar.gz` & `tmp/daves_utilities-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daves_utilities-0.1.7.tar", max compression
+gzip compressed data, was "daves_utilities-0.1.8.tar", max compression
```

## Comparing `daves_utilities-0.1.7.tar` & `daves_utilities-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1087 2022-12-31 15:33:52.562362 daves_utilities-0.1.7/LICENSE
--rw-r--r--   0        0        0       19 2022-12-31 15:33:52.565062 daves_utilities-0.1.7/README.md
--rw-r--r--   0        0        0     1370 2023-07-15 14:01:17.122596 daves_utilities-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      697 2023-07-15 14:01:05.585224 daves_utilities-0.1.7/src/daves_utilities/__init__.py
--rw-r--r--   0        0        0     2600 2023-07-15 13:59:00.262111 daves_utilities-0.1.7/src/daves_utilities/archive/fun_save.py
--rw-r--r--   0        0        0     1475 2023-07-15 13:21:21.764496 daves_utilities-0.1.7/src/daves_utilities/archive/is_equal.py
--rw-r--r--   0        0        0     3478 2023-01-01 15:53:17.727021 daves_utilities-0.1.7/src/daves_utilities/archive/print_structure.py
--rw-r--r--   0        0        0      554 2023-07-15 13:58:43.390194 daves_utilities-0.1.7/src/daves_utilities/david_secrets.py
--rw-r--r--   0        0        0     5184 2023-07-15 13:21:21.799335 daves_utilities-0.1.7/src/daves_utilities/iterator.py
--rw-r--r--   0        0        0     2285 1970-01-01 00:00:00.000000 daves_utilities-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1087 2022-12-31 15:33:52.562362 daves_utilities-0.1.8/LICENSE
+-rw-r--r--   0        0        0       19 2022-12-31 15:33:52.565062 daves_utilities-0.1.8/README.md
+-rw-r--r--   0        0        0     1416 2023-07-15 14:08:56.677392 daves_utilities-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      697 2023-07-15 14:01:05.585224 daves_utilities-0.1.8/src/daves_utilities/__init__.py
+-rw-r--r--   0        0        0     2600 2023-07-15 13:59:00.262111 daves_utilities-0.1.8/src/daves_utilities/archive/fun_save.py
+-rw-r--r--   0        0        0     1475 2023-07-15 13:21:21.764496 daves_utilities-0.1.8/src/daves_utilities/archive/is_equal.py
+-rw-r--r--   0        0        0     3478 2023-01-01 15:53:17.727021 daves_utilities-0.1.8/src/daves_utilities/archive/print_structure.py
+-rw-r--r--   0        0        0      554 2023-07-15 13:58:43.390194 daves_utilities-0.1.8/src/daves_utilities/david_secrets.py
+-rw-r--r--   0        0        0     5184 2023-07-15 13:21:21.799335 daves_utilities-0.1.8/src/daves_utilities/iterator.py
+-rw-r--r--   0        0        0     2372 1970-01-01 00:00:00.000000 daves_utilities-0.1.8/PKG-INFO
```

### Comparing `daves_utilities-0.1.7/LICENSE` & `daves_utilities-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.7/pyproject.toml` & `daves_utilities-0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ########################################################################################
 # POETRY                                                                               #
 ########################################################################################
 [tool.poetry]
 name = "daves_utilities"
 authors = ["David Kuchelmeister"]
 description = "some useful function for myself"
-version = "0.1.7"
+version = "0.1.8"
 
 license = "MIT"
 
 repository = "https://github.com/kuchedav/daves_utilities"
 
 # README file(s) are used as the package description
 readme = ["README.md", "LICENSE"]
@@ -48,7 +48,9 @@
 build = "^0.10.0"
 setuptools-scm = "^7.1.0"
 numpy = "^1.25.1"
 pre-commit = "^3.3.3"
 pandas = "2.0.2"
 polars = "^0.18.7"
 progressbar2 = "^4.2.0"
+cryptography = "^41.0.2"
+progressbar = "^2.5"
```

### Comparing `daves_utilities-0.1.7/src/daves_utilities/__init__.py` & `daves_utilities-0.1.8/src/daves_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.7/src/daves_utilities/archive/fun_save.py` & `daves_utilities-0.1.8/src/daves_utilities/archive/fun_save.py`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.7/src/daves_utilities/archive/is_equal.py` & `daves_utilities-0.1.8/src/daves_utilities/archive/is_equal.py`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.7/src/daves_utilities/archive/print_structure.py` & `daves_utilities-0.1.8/src/daves_utilities/archive/print_structure.py`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.7/src/daves_utilities/david_secrets.py` & `daves_utilities-0.1.8/src/daves_utilities/david_secrets.py`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.7/src/daves_utilities/iterator.py` & `daves_utilities-0.1.8/src/daves_utilities/iterator.py`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.7/PKG-INFO` & `daves_utilities-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: daves-utilities
-Version: 0.1.7
+Version: 0.1.8
 Summary: some useful function for myself
 Home-page: https://github.com/kuchedav/daves_utilities
 License: MIT
 Keywords: packaging,poetry
 Author: David Kuchelmeister
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: build (>=0.10.0,<0.11.0)
 Requires-Dist: coverage (>=7.2.7,<8.0.0)
+Requires-Dist: cryptography (>=41.0.2,<42.0.0)
 Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: mypy (>=1.4.1,<2.0.0)
 Requires-Dist: numpy (>=1.25.1,<2.0.0)
 Requires-Dist: pandas (==2.0.2)
 Requires-Dist: polars (>=0.18.7,<0.19.0)
 Requires-Dist: pre-commit (>=3.3.3,<4.0.0)
 Requires-Dist: pre-commit-hooks (>=4.4.0,<5.0.0)
+Requires-Dist: progressbar (>=2.5,<3.0)
 Requires-Dist: progressbar2 (>=4.2.0,<5.0.0)
 Requires-Dist: pyupgrade (>=3.9.0,<4.0.0)
 Requires-Dist: reorder-python-imports (>=3.10.0,<4.0.0)
 Requires-Dist: setuptools-scm (>=7.1.0,<8.0.0)
 Requires-Dist: tox (>=4.6.4,<5.0.0)
 Requires-Dist: twine (>=4.0.2,<5.0.0)
 Requires-Dist: wheel (>=0.40.0,<0.41.0)
```

