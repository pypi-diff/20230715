# Comparing `tmp/notebooklog-0.0.1.tar.gz` & `tmp/notebooklog-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebooklog-0.0.1.tar", last modified: Wed Apr 12 03:15:17 2023, max compression
+gzip compressed data, was "notebooklog-0.0.2.tar", last modified: Sat Jul 15 01:09:22 2023, max compression
```

## Comparing `notebooklog-0.0.1.tar` & `notebooklog-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:15:17.480222 notebooklog-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 03:14:43.000000 notebooklog-0.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-12 03:14:43.000000 notebooklog-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-12 03:14:43.000000 notebooklog-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-12 03:15:17.480222 notebooklog-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-12 03:14:43.000000 notebooklog-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:15:17.476221 notebooklog-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-12 03:14:43.000000 notebooklog-0.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-12 03:14:43.000000 notebooklog-0.0.1/docs/changelog.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     7079 2023-04-12 03:14:43.000000 notebooklog-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-12 03:14:43.000000 notebooklog-0.0.1/docs/contents.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-12 03:14:43.000000 notebooklog-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-12 03:14:43.000000 notebooklog-0.0.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-12 03:14:43.000000 notebooklog-0.0.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 03:14:43.000000 notebooklog-0.0.1/docs/notebooklog.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:15:17.476221 notebooklog-0.0.1/notebooklog/
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-04-12 03:14:43.000000 notebooklog-0.0.1/notebooklog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:15:17.480222 notebooklog-0.0.1/notebooklog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-12 03:15:17.000000 notebooklog-0.0.1/notebooklog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-12 03:15:17.000000 notebooklog-0.0.1/notebooklog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 03:15:17.000000 notebooklog-0.0.1/notebooklog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 03:15:17.000000 notebooklog-0.0.1/notebooklog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 03:15:17.000000 notebooklog-0.0.1/notebooklog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-12 03:15:17.000000 notebooklog-0.0.1/notebooklog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-12 03:15:17.480222 notebooklog-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-12 03:14:43.000000 notebooklog-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 03:15:17.480222 notebooklog-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 03:14:43.000000 notebooklog-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-12 03:14:43.000000 notebooklog-0.0.1/tests/test_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:09:22.338135 notebooklog-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-15 01:08:47.000000 notebooklog-0.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-15 01:08:47.000000 notebooklog-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-15 01:08:47.000000 notebooklog-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-15 01:09:22.338135 notebooklog-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-15 01:08:47.000000 notebooklog-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:09:22.338135 notebooklog-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-15 01:08:47.000000 notebooklog-0.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-15 01:08:47.000000 notebooklog-0.0.2/docs/changelog.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7079 2023-07-15 01:08:47.000000 notebooklog-0.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-15 01:08:47.000000 notebooklog-0.0.2/docs/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-15 01:08:47.000000 notebooklog-0.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-15 01:08:47.000000 notebooklog-0.0.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-15 01:08:47.000000 notebooklog-0.0.2/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-15 01:08:47.000000 notebooklog-0.0.2/docs/notebooklog.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:09:22.338135 notebooklog-0.0.2/notebooklog/
+-rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-07-15 01:08:47.000000 notebooklog-0.0.2/notebooklog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:09:22.338135 notebooklog-0.0.2/notebooklog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-15 01:09:22.000000 notebooklog-0.0.2/notebooklog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-15 01:09:22.000000 notebooklog-0.0.2/notebooklog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 01:09:22.000000 notebooklog-0.0.2/notebooklog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 01:09:22.000000 notebooklog-0.0.2/notebooklog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-15 01:09:22.000000 notebooklog-0.0.2/notebooklog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 01:09:22.000000 notebooklog-0.0.2/notebooklog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-15 01:09:22.342135 notebooklog-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-15 01:08:47.000000 notebooklog-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:09:22.338135 notebooklog-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 01:08:47.000000 notebooklog-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-15 01:08:47.000000 notebooklog-0.0.2/tests/test_package.py
```

### Comparing `notebooklog-0.0.1/LICENSE` & `notebooklog-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `notebooklog-0.0.1/PKG-INFO` & `notebooklog-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebooklog
-Version: 0.0.1
+Version: 0.0.2
 Summary: notebooklog
 Home-page: https://github.com/maximz/notebooklog
 Author: Maxim Zaslavsky
 Author-email: maxim@maximz.com
 License: MIT license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `notebooklog-0.0.1/README.md` & `notebooklog-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `notebooklog-0.0.1/docs/Makefile` & `notebooklog-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `notebooklog-0.0.1/docs/conf.py` & `notebooklog-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `notebooklog-0.0.1/docs/index.md` & `notebooklog-0.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `notebooklog-0.0.1/docs/make.bat` & `notebooklog-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `notebooklog-0.0.1/notebooklog/__init__.py` & `notebooklog-0.0.2/notebooklog/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Create a logger for main application (e.g. current notebook) and configure writing to file as well.
 
 This will capture any direct stdout/stderr writes that didn't come from a logger, too.
 """
 
 __author__ = """Maxim Zaslavsky"""
 __email__ = "maxim@maximz.com"
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 
 import datetime
 import logging
 import os
 import sys
 from pathlib import Path
@@ -140,14 +140,17 @@
 
         self.file_object.flush()
 
         if self.pass_through is not None:
             # Flush the pass-through stream.
             self.pass_through.flush()
 
+    def close(self) -> None:
+        self.flush()
+
     def isatty(self):
         # pytest checks file.isatty()
         # see https://github.com/pytest-dev/pytest/issues/1447#issuecomment-194676124
         if self.pass_through is not None:
             return self.pass_through.isatty()
         return self.file_object.isatty()
```

### Comparing `notebooklog-0.0.1/notebooklog.egg-info/PKG-INFO` & `notebooklog-0.0.2/notebooklog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebooklog
-Version: 0.0.1
+Version: 0.0.2
 Summary: notebooklog
 Home-page: https://github.com/maximz/notebooklog
 Author: Maxim Zaslavsky
 Author-email: maxim@maximz.com
 License: MIT license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `notebooklog-0.0.1/setup.py` & `notebooklog-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 setup(
     author="Maxim Zaslavsky",
     author_email="maxim@maximz.com",
     name="notebooklog",
     description="notebooklog",
     packages=find_packages(include=["notebooklog", "notebooklog.*"]),
     python_requires=">=3.8",
-    version="0.0.1",
+    version="0.0.2",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
```

### Comparing `notebooklog-0.0.1/tests/test_package.py` & `notebooklog-0.0.2/tests/test_package.py`

 * *Files identical despite different names*

