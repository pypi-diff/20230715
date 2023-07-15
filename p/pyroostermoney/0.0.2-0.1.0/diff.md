# Comparing `tmp/pyroostermoney-0.0.2.tar.gz` & `tmp/pyroostermoney-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroostermoney-0.0.2.tar", last modified: Fri Jul 14 22:17:44 2023, max compression
+gzip compressed data, was "pyroostermoney-0.1.0.tar", last modified: Sat Jul 15 21:27:21 2023, max compression
```

## Comparing `pyroostermoney-0.0.2.tar` & `pyroostermoney-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:17:44.219524 pyroostermoney-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:17:44.215524 pyroostermoney-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:17:44.219524 pyroostermoney-0.0.2/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:17:44.219524 pyroostermoney-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-14 22:17:44.219524 pyroostermoney-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:17:44.219524 pyroostermoney-0.0.2/pyroostermoney/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/pyroostermoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/pyroostermoney/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:17:44.219524 pyroostermoney-0.0.2/pyroostermoney/services/
--rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/pyroostermoney/services/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/pyroostermoney/services/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/pyroostermoney/services/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/pyroostermoney/services/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:17:44.219524 pyroostermoney-0.0.2/pyroostermoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-14 22:17:44.000000 pyroostermoney-0.0.2/pyroostermoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-14 22:17:44.000000 pyroostermoney-0.0.2/pyroostermoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:17:44.000000 pyroostermoney-0.0.2/pyroostermoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 22:17:44.000000 pyroostermoney-0.0.2/pyroostermoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 22:17:44.000000 pyroostermoney-0.0.2/pyroostermoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-14 22:17:44.219524 pyroostermoney-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:27:21.334201 pyroostermoney-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:27:21.330201 pyroostermoney-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:27:21.334201 pyroostermoney-0.1.0/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:27:21.334201 pyroostermoney-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-15 21:27:21.334201 pyroostermoney-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:27:21.334201 pyroostermoney-0.1.0/pyroostermoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/pyroostermoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/pyroostermoney/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:27:21.334201 pyroostermoney-0.1.0/pyroostermoney/child/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/pyroostermoney/child/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/pyroostermoney/child/child.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/pyroostermoney/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/pyroostermoney/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/pyroostermoney/roostermoney.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:27:21.334201 pyroostermoney-0.1.0/pyroostermoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-15 21:27:21.000000 pyroostermoney-0.1.0/pyroostermoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-15 21:27:21.000000 pyroostermoney-0.1.0/pyroostermoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 21:27:21.000000 pyroostermoney-0.1.0/pyroostermoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 21:27:21.000000 pyroostermoney-0.1.0/pyroostermoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-15 21:27:21.000000 pyroostermoney-0.1.0/pyroostermoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-15 21:27:21.334201 pyroostermoney-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/setup.py
```

### Comparing `pyroostermoney-0.0.2/.github/scripts/release.py` & `pyroostermoney-0.1.0/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.0.2/.github/workflows/build.yml` & `pyroostermoney-0.1.0/.github/workflows/build.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-name: Publish to PyPI.org
-on: workflow_dispatch
+name: Python test and build
+on: [push]
 jobs:
   pypi:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v3
       - name: Set up Python
@@ -11,10 +11,14 @@
         with:
           python-version: '3.x'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install build
           pip install -r requirements.txt
+          pip install pylint
+      - name: Analysing the code with pylint
+        run: |
+          pylint $(git ls-files '*.py')
       - name: Build package
         run: python -m build
       - run: python3 -m pip install --upgrade build && python3 -m build
```

### Comparing `pyroostermoney-0.0.2/.gitignore` & `pyroostermoney-0.1.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -159,8 +159,11 @@
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 # test files
 test.py
 
 # vscode
-.vscode/
+.vscode/
+
+# old files
+*.old/
```

### Comparing `pyroostermoney-0.0.2/LICENSE` & `pyroostermoney-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.0.2/PKG-INFO` & `pyroostermoney-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.0.2
+Version: 0.1.0
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.0.2/pyroostermoney.egg-info/PKG-INFO` & `pyroostermoney-0.1.0/pyroostermoney.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.0.2
+Version: 0.1.0
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.0.2/pyroostermoney.egg-info/SOURCES.txt` & `pyroostermoney-0.1.0/pyroostermoney.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 setup.cfg
 setup.py
 .github/scripts/release.py
 .github/workflows/build.yml
 .github/workflows/publish.yml
 .github/workflows/release.yml
 pyroostermoney/__init__.py
+pyroostermoney/api.py
 pyroostermoney/const.py
+pyroostermoney/exceptions.py
+pyroostermoney/roostermoney.py
 pyroostermoney.egg-info/PKG-INFO
 pyroostermoney.egg-info/SOURCES.txt
 pyroostermoney.egg-info/dependency_links.txt
 pyroostermoney.egg-info/requires.txt
 pyroostermoney.egg-info/top_level.txt
-pyroostermoney/services/api.py
-pyroostermoney/services/errors.py
-pyroostermoney/services/login.py
-pyroostermoney/services/session.py
+pyroostermoney/child/__init__.py
+pyroostermoney/child/child.py
```

