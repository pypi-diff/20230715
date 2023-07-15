# Comparing `tmp/donfig-0.8.0.tar.gz` & `tmp/donfig-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donfig-0.8.0.tar", last modified: Thu Jul 13 13:29:35 2023, max compression
+gzip compressed data, was "donfig-0.8.1.tar", last modified: Sat Jul 15 03:07:15 2023, max compression
```

## Comparing `donfig-0.8.0.tar` & `donfig-0.8.1.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:29:35.322126 donfig-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-13 13:29:27.000000 donfig-0.8.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-13 13:29:27.000000 donfig-0.8.0/DASK_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-13 13:29:27.000000 donfig-0.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-13 13:29:27.000000 donfig-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-13 13:29:35.322126 donfig-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-13 13:29:27.000000 donfig-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:29:35.322126 donfig-0.8.0/donfig/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-13 13:29:27.000000 donfig-0.8.0/donfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-13 13:29:27.000000 donfig-0.8.0/donfig/_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    24644 2023-07-13 13:29:27.000000 donfig-0.8.0/donfig/config_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-13 13:29:27.000000 donfig-0.8.0/donfig/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-13 13:29:35.322126 donfig-0.8.0/donfig/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:29:35.322126 donfig-0.8.0/donfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-13 13:29:35.000000 donfig-0.8.0/donfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-13 13:29:35.000000 donfig-0.8.0/donfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:29:35.000000 donfig-0.8.0/donfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-13 13:29:35.000000 donfig-0.8.0/donfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-13 13:29:35.000000 donfig-0.8.0/donfig.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-13 13:29:27.000000 donfig-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-13 13:29:35.322126 donfig-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-13 13:29:27.000000 donfig-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:07:15.431938 donfig-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-15 03:07:03.000000 donfig-0.8.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-15 03:07:03.000000 donfig-0.8.1/DASK_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-15 03:07:03.000000 donfig-0.8.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-15 03:07:03.000000 donfig-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-15 03:07:15.431938 donfig-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-07-15 03:07:03.000000 donfig-0.8.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:07:15.427938 donfig-0.8.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-15 03:07:03.000000 donfig-0.8.1/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:07:15.431938 donfig-0.8.1/donfig/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-15 03:07:03.000000 donfig-0.8.1/donfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-15 03:07:03.000000 donfig-0.8.1/donfig/_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24644 2023-07-15 03:07:03.000000 donfig-0.8.1/donfig/config_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:07:15.431938 donfig-0.8.1/donfig/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 03:07:03.000000 donfig-0.8.1/donfig/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19003 2023-07-15 03:07:03.000000 donfig-0.8.1/donfig/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-15 03:07:03.000000 donfig-0.8.1/donfig/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-15 03:07:03.000000 donfig-0.8.1/donfig/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-15 03:07:15.431938 donfig-0.8.1/donfig/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:07:15.431938 donfig-0.8.1/donfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-07-15 03:07:15.000000 donfig-0.8.1/donfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-15 03:07:15.000000 donfig-0.8.1/donfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 03:07:15.000000 donfig-0.8.1/donfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-15 03:07:15.000000 donfig-0.8.1/donfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-15 03:07:15.000000 donfig-0.8.1/donfig.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-15 03:07:03.000000 donfig-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-15 03:07:15.431938 donfig-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-15 03:07:03.000000 donfig-0.8.1/setup.py
```

### Comparing `donfig-0.8.0/AUTHORS.md` & `donfig-0.8.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `donfig-0.8.0/DASK_LICENSE.txt` & `donfig-0.8.1/DASK_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `donfig-0.8.0/LICENSE.txt` & `donfig-0.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `donfig-0.8.0/PKG-INFO` & `donfig-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: donfig
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python package for configuring a python package
 Maintainer-email: David Hoese <david.hoese@ssec.wisc.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/pytroll/donfig
 Keywords: task-scheduling parallel numpy pandas pydata
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `donfig-0.8.0/README.rst` & `donfig-0.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `donfig-0.8.0/donfig/_lock.py` & `donfig-0.8.1/donfig/_lock.py`

 * *Files identical despite different names*

### Comparing `donfig-0.8.0/donfig/config_obj.py` & `donfig-0.8.1/donfig/config_obj.py`

 * *Files identical despite different names*

### Comparing `donfig-0.8.0/donfig/utils.py` & `donfig-0.8.1/donfig/utils.py`

 * *Files identical despite different names*

### Comparing `donfig-0.8.0/donfig.egg-info/PKG-INFO` & `donfig-0.8.1/donfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: donfig
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python package for configuring a python package
 Maintainer-email: David Hoese <david.hoese@ssec.wisc.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/pytroll/donfig
 Keywords: task-scheduling parallel numpy pandas pydata
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `donfig-0.8.0/pyproject.toml` & `donfig-0.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,19 @@
     "sphinx>=4.0.0",
     "numpydoc",
     "pytest",
     "cloudpickle",
 ]
 
 [tool.setuptools]
-packages = ["donfig"]
 include-package-data = true
 
+[tool.setuptools.packages]
+find = {}
+
 [tool.mypy]
 # Silence errors about Python 3.9-style delayed type annotations on Python 3.8
 python_version = "3.9"
 # See https://github.com/python/mypy/issues/12286 for automatic multi-platform support
 platform = "linux"
 # platform = win32
 # platform = darwin
```

### Comparing `donfig-0.8.0/setup.py` & `donfig-0.8.1/setup.py`

 * *Files identical despite different names*

