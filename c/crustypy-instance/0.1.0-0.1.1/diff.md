# Comparing `tmp/crustypy_instance-0.1.0.tar.gz` & `tmp/crustypy_instance-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crustypy_instance-0.1.0.tar", max compression
+gzip compressed data, was "crustypy_instance-0.1.1.tar", max compression
```

## Comparing `crustypy_instance-0.1.0.tar` & `crustypy_instance-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-07-14 20:27:56.220278 crustypy_instance-0.1.0/LICENSE
--rw-r--r--   0        0        0     5779 2023-07-14 20:27:56.220278 crustypy_instance-0.1.0/docs/README.md
--rw-r--r--   0        0        0     3285 2023-07-14 20:27:57.172284 crustypy_instance-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      107 2023-07-14 20:27:56.220278 crustypy_instance-0.1.0/src/crustypy_instance/__init__.py
--rw-r--r--   0        0        0      641 2023-07-14 20:27:56.220278 crustypy_instance-0.1.0/src/crustypy_instance/_crustypy_instance.py
--rw-r--r--   0        0        0        0 2023-07-14 20:27:56.220278 crustypy_instance-0.1.0/src/crustypy_instance/py.typed
--rw-r--r--   0        0        0     6953 1970-01-01 00:00:00.000000 crustypy_instance-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-14 22:38:52.989252 crustypy_instance-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5778 2023-07-14 22:38:52.989252 crustypy_instance-0.1.1/docs/README.md
+-rw-r--r--   0        0        0     3062 2023-07-14 22:38:53.885248 crustypy_instance-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-07-14 22:38:52.989252 crustypy_instance-0.1.1/src/crustypy_instance/__init__.py
+-rw-r--r--   0        0        0      641 2023-07-14 22:38:52.989252 crustypy_instance-0.1.1/src/crustypy_instance/_crustypy_instance.py
+-rw-r--r--   0        0        0        0 2023-07-14 22:38:52.989252 crustypy_instance-0.1.1/src/crustypy_instance/py.typed
+-rw-r--r--   0        0        0     6908 1970-01-01 00:00:00.000000 crustypy_instance-0.1.1/PKG-INFO
```

### Comparing `crustypy_instance-0.1.0/LICENSE` & `crustypy_instance-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crustypy_instance-0.1.0/docs/README.md` & `crustypy_instance-0.1.1/docs/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 [label-build]: https://img.shields.io/badge/%F0%9F%94%A7-build-darkblue?style=flat-square
 [label-tests]: https://img.shields.io/badge/%F0%9F%A7%AA-tests-darkblue?style=flat-square
 [label-standards]: https://img.shields.io/badge/%F0%9F%93%91-standards-darkblue?style=flat-square
 [label-code]: https://img.shields.io/badge/%F0%9F%92%BB-code-darkblue?style=flat-square
 [label-repo]: https://img.shields.io/badge/%F0%9F%93%81-repo-darkblue?style=flat-square
 
 <!-- Build -->
-[badge-actions]: https://img.shields.io/github/actions/workflow/status/MicaelJarniac/crustypy-instance/nox.yml?branch=main&style=flat-square
+[badge-actions]: https://img.shields.io/github/actions/workflow/status/MicaelJarniac/crustypy-instance/ci.yml?branch=main&style=flat-square
 [actions]: https://github.com/MicaelJarniac/crustypy-instance/actions
 [badge-semantic-release]: https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079?style=flat-square
 [semantic-release]: https://github.com/semantic-release/semantic-release
 [badge-pypi]: https://img.shields.io/pypi/v/crustypy-instance?style=flat-square
 [pypi]: https://pypi.org/project/crustypy-instance
 [badge-docs]: https://img.shields.io/readthedocs/crustypy-instance?style=flat-square
 [docs]: https://crustypy-instance.readthedocs.io
```

### Comparing `crustypy_instance-0.1.0/pyproject.toml` & `crustypy_instance-0.1.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "crustypy-instance"
-version = "0.1.0"
+version = "0.1.1"
 description = "Generated with CrustyPy."
 authors = ["Micael Jarniac <micael@jarniac.dev>"]
 license = "MIT"
 readme = "docs/README.md"
 packages = [{include = "crustypy_instance", from = "src"}]
 homepage = "https://github.com/MicaelJarniac/crustypy-instance"
 repository = "https://github.com/MicaelJarniac/crustypy-instance"
 documentation = "https://crustypy-instance.readthedocs.io"
 classifiers = [
   # Get more from http://pypi.python.org/pypi?%3Aaction=list_classifiers
   "Development Status :: 1 - Planning",
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
   "Operating System :: OS Independent",
-  "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
   "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 loguru = "^0.7.0"
@@ -63,16 +57,16 @@
 pre-commit = "^3.3.3"
 
 [tool.poetry.group.dev.dependencies]
 nox = "^2023.4.22"
 python-semantic-release = "^7.34.6"
 
 [tool.poetry.urls]
-"Changelog" = "https://github.com/AuthorName/python-project/blob/main/docs/CHANGELOG.md"
-"Bug Tracker" = "https://github.com/AuthorName/python-project/issues"
+"Changelog" = "https://github.com/MicaelJarniac/crustypy-instance/blob/main/docs/CHANGELOG.md"
+"Bug Tracker" = "https://github.com/MicaelJarniac/crustypy-instance/issues"
 
 [tool.ruff]
 # https://beta.ruff.rs/docs/rules
 line-length = 88  # Default
 select = ["ALL"]
 ignore = [
   "D203",
@@ -114,15 +108,18 @@
 warn_unused_ignores = false  # true
 show_column_numbers = true
 # show_error_context = true
 # pretty = true
 
 [tool.semantic_release]
 version_toml = ["pyproject.toml:tool.poetry.version"]
-build_command = "pip install poetry && poetry build"
+build_command = """
+  python -m pip install build~=0.10.0
+  python -m build .
+"""
 
 [tool.semantic_release.changelog]
 changelog_file = "docs/CHANGELOG.md"
 
 [tool.semantic_release.branches.main]
 match = "main"
```

### Comparing `crustypy_instance-0.1.0/src/crustypy_instance/_crustypy_instance.py` & `crustypy_instance-0.1.1/src/crustypy_instance/_crustypy_instance.py`

 * *Files identical despite different names*

### Comparing `crustypy_instance-0.1.0/PKG-INFO` & `crustypy_instance-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crustypy-instance
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generated with CrustyPy.
 Home-page: https://github.com/MicaelJarniac/crustypy-instance
 License: MIT
 Author: Micael Jarniac
 Author-email: micael@jarniac.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 1 - Planning
@@ -12,19 +12,18 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
-Project-URL: Bug Tracker, https://github.com/AuthorName/python-project/issues
-Project-URL: Changelog, https://github.com/AuthorName/python-project/blob/main/docs/CHANGELOG.md
+Project-URL: Bug Tracker, https://github.com/MicaelJarniac/crustypy-instance/issues
+Project-URL: Changelog, https://github.com/MicaelJarniac/crustypy-instance/blob/main/docs/CHANGELOG.md
 Project-URL: Documentation, https://crustypy-instance.readthedocs.io
 Project-URL: Repository, https://github.com/MicaelJarniac/crustypy-instance
 Description-Content-Type: text/markdown
 
 <div align="center">
 
   | | ![Badges][label-badges] |
@@ -43,15 +42,15 @@
 [label-build]: https://img.shields.io/badge/%F0%9F%94%A7-build-darkblue?style=flat-square
 [label-tests]: https://img.shields.io/badge/%F0%9F%A7%AA-tests-darkblue?style=flat-square
 [label-standards]: https://img.shields.io/badge/%F0%9F%93%91-standards-darkblue?style=flat-square
 [label-code]: https://img.shields.io/badge/%F0%9F%92%BB-code-darkblue?style=flat-square
 [label-repo]: https://img.shields.io/badge/%F0%9F%93%81-repo-darkblue?style=flat-square
 
 <!-- Build -->
-[badge-actions]: https://img.shields.io/github/actions/workflow/status/MicaelJarniac/crustypy-instance/nox.yml?branch=main&style=flat-square
+[badge-actions]: https://img.shields.io/github/actions/workflow/status/MicaelJarniac/crustypy-instance/ci.yml?branch=main&style=flat-square
 [actions]: https://github.com/MicaelJarniac/crustypy-instance/actions
 [badge-semantic-release]: https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079?style=flat-square
 [semantic-release]: https://github.com/semantic-release/semantic-release
 [badge-pypi]: https://img.shields.io/pypi/v/crustypy-instance?style=flat-square
 [pypi]: https://pypi.org/project/crustypy-instance
 [badge-docs]: https://img.shields.io/readthedocs/crustypy-instance?style=flat-square
 [docs]: https://crustypy-instance.readthedocs.io
```

