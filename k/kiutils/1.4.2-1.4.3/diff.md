# Comparing `tmp/kiutils-1.4.2.tar.gz` & `tmp/kiutils-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiutils-1.4.2.tar", last modified: Fri Jun  9 19:17:39 2023, max compression
+gzip compressed data, was "kiutils-1.4.3.tar", last modified: Sat Jul 15 19:57:27 2023, max compression
```

## Comparing `kiutils-1.4.2.tar` & `kiutils-1.4.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:17:39.747579 kiutils-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-09 19:17:12.000000 kiutils-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-09 19:17:39.747579 kiutils-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-09 19:17:12.000000 kiutils-1.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-09 19:17:12.000000 kiutils-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-09 19:17:39.747579 kiutils-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-09 19:17:12.000000 kiutils-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:17:39.739578 kiutils-1.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:17:39.743578 kiutils-1.4.2/src/kiutils/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/board.py
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/dru.py
--rw-r--r--   0 runner    (1001) docker     (123)    46972 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/footprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:17:39.743578 kiutils-1.4.2/src/kiutils/items/
--rw-r--r--   0 runner    (1001) docker     (123)    47460 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/items/brditems.py
--rw-r--r--   0 runner    (1001) docker     (123)    42864 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/items/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/items/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/items/fpitems.py
--rw-r--r--   0 runner    (1001) docker     (123)    31527 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/items/gritems.py
--rw-r--r--   0 runner    (1001) docker     (123)    75394 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/items/schitems.py
--rw-r--r--   0 runner    (1001) docker     (123)    21590 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/items/syitems.py
--rw-r--r--   0 runner    (1001) docker     (123)    27998 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/items/zones.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/libraries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:17:39.743578 kiutils-1.4.2/src/kiutils/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/misc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14716 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/schematic.py
--rw-r--r--   0 runner    (1001) docker     (123)    25567 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/symbol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:17:39.743578 kiutils-1.4.2/src/kiutils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/utils/sexpr.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/utils/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)    38203 2023-06-09 19:17:12.000000 kiutils-1.4.2/src/kiutils/wks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:17:39.743578 kiutils-1.4.2/src/kiutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-09 19:17:39.000000 kiutils-1.4.2/src/kiutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-09 19:17:39.000000 kiutils-1.4.2/src/kiutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 19:17:39.000000 kiutils-1.4.2/src/kiutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 19:17:39.000000 kiutils-1.4.2/src/kiutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:17:39.747579 kiutils-1.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-06-09 19:17:12.000000 kiutils-1.4.2/tests/test_board.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-09 19:17:12.000000 kiutils-1.4.2/tests/test_designrules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-09 19:17:12.000000 kiutils-1.4.2/tests/test_footprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-09 19:17:12.000000 kiutils-1.4.2/tests/test_libtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-09 19:17:12.000000 kiutils-1.4.2/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-06-09 19:17:12.000000 kiutils-1.4.2/tests/test_schematic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-06-09 19:17:12.000000 kiutils-1.4.2/tests/test_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-09 19:17:12.000000 kiutils-1.4.2/tests/test_worksheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-09 19:17:12.000000 kiutils-1.4.2/tests/testfunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:57:27.166137 kiutils-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-15 19:57:01.000000 kiutils-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-15 19:57:27.166137 kiutils-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-15 19:57:01.000000 kiutils-1.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-15 19:57:01.000000 kiutils-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-15 19:57:27.166137 kiutils-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-15 19:57:01.000000 kiutils-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:57:27.154137 kiutils-1.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:57:27.158137 kiutils-1.4.3/src/kiutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/dru.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47417 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/footprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:57:27.162137 kiutils-1.4.3/src/kiutils/items/
+-rw-r--r--   0 runner    (1001) docker     (123)    47460 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/items/brditems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42864 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/items/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/items/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34336 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/items/fpitems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31527 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/items/gritems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75394 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/items/schitems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21590 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/items/syitems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27998 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/items/zones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/libraries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:57:27.162137 kiutils-1.4.3/src/kiutils/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/misc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14716 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/schematic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25567 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/symbol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:57:27.162137 kiutils-1.4.3/src/kiutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/utils/sexpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/utils/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38203 2023-07-15 19:57:01.000000 kiutils-1.4.3/src/kiutils/wks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:57:27.158137 kiutils-1.4.3/src/kiutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-15 19:57:27.000000 kiutils-1.4.3/src/kiutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-15 19:57:27.000000 kiutils-1.4.3/src/kiutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 19:57:27.000000 kiutils-1.4.3/src/kiutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 19:57:27.000000 kiutils-1.4.3/src/kiutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:57:27.166137 kiutils-1.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-07-15 19:57:01.000000 kiutils-1.4.3/tests/test_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-15 19:57:01.000000 kiutils-1.4.3/tests/test_designrules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-15 19:57:01.000000 kiutils-1.4.3/tests/test_footprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-15 19:57:01.000000 kiutils-1.4.3/tests/test_libtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-15 19:57:01.000000 kiutils-1.4.3/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-07-15 19:57:01.000000 kiutils-1.4.3/tests/test_schematic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-07-15 19:57:01.000000 kiutils-1.4.3/tests/test_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-15 19:57:01.000000 kiutils-1.4.3/tests/test_worksheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-07-15 19:57:01.000000 kiutils-1.4.3/tests/testfunctions.py
```

### Comparing `kiutils-1.4.2/LICENSE` & `kiutils-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/PKG-INFO` & `kiutils-1.4.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: kiutils
-Version: 1.4.2
+Version: 1.4.3
 Summary: Simple and SCM-friendly KiCad file parser for KiCad 6.0 and up
 Home-page: https://github.com/mvnmgrx/kiutils
 Author: Marvin Mager
 Author-email: 99667992+mvnmgrx@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/mvnmgrx/kiutils/issues
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # KiUtils
 
 [![PyPI version](https://img.shields.io/pypi/v/kiutils)](https://pypi.org/project/kiutils)
+[![PyPI downloads](https://img.shields.io/pypi/dm/kiutils.svg)](https://pypistats.org/packages/kiutils)
 ![Python version](https://img.shields.io/pypi/pyversions/kiutils)
 [![License](https://img.shields.io/github/license/mvnmgrx/kiutils)](https://github.com/mvnmgrx/kiutils/blob/master/LICENSE)
 ![Last commit](https://img.shields.io/github/last-commit/mvnmgrx/kiutils)
 [![Documentation Status](https://readthedocs.org/projects/kiutils/badge/?version=latest)](https://kiutils.readthedocs.io/en/latest/?badge=latest)
 
 Simple and SCM-friendly KiCad file parser based on Python dataclasses for KiCad 6.0
 and up. The following KiCad-related files are currently supported:
```

### Comparing `kiutils-1.4.2/README.md` & `kiutils-1.4.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # KiUtils
 
 [![PyPI version](https://img.shields.io/pypi/v/kiutils)](https://pypi.org/project/kiutils)
+[![PyPI downloads](https://img.shields.io/pypi/dm/kiutils.svg)](https://pypistats.org/packages/kiutils)
 ![Python version](https://img.shields.io/pypi/pyversions/kiutils)
 [![License](https://img.shields.io/github/license/mvnmgrx/kiutils)](https://github.com/mvnmgrx/kiutils/blob/master/LICENSE)
 ![Last commit](https://img.shields.io/github/last-commit/mvnmgrx/kiutils)
 [![Documentation Status](https://readthedocs.org/projects/kiutils/badge/?version=latest)](https://kiutils.readthedocs.io/en/latest/?badge=latest)
 
 Simple and SCM-friendly KiCad file parser based on Python dataclasses for KiCad 6.0
 and up. The following KiCad-related files are currently supported:
@@ -42,8 +43,8 @@
 
 ## Documentation
 Visit the [kiutils documentation](https://kiutils.readthedocs.io/) for more information on how to 
 install, use and develop `kiutils`, as well as examples and general module documentation.
 
 ## Donate
 If you found this module helpful for your project consider donating via
-[PayPal](https://paypal.me/mrvnmgr). Thanks!
+[PayPal](https://paypal.me/mrvnmgr). Thanks!
```

### Comparing `kiutils-1.4.2/setup.cfg` & `kiutils-1.4.3/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 [metadata]
 name = kiutils
-version = 1.4.2
+version = 1.4.3
 author = Marvin Mager
 author_email = 99667992+mvnmgrx@users.noreply.github.com
 description = Simple and SCM-friendly KiCad file parser for KiCad 6.0 and up
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mvnmgrx/kiutils
 project_urls = 
 	Bug Tracker = https://github.com/mvnmgrx/kiutils/issues
 classifiers = 
 	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 	Operating System :: OS Independent
 	Development Status :: 5 - Production/Stable
 	Natural Language :: English
 	Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 
 [options]
```

### Comparing `kiutils-1.4.2/src/kiutils/board.py` & `kiutils-1.4.3/src/kiutils/board.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/src/kiutils/dru.py` & `kiutils-1.4.3/src/kiutils/dru.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/src/kiutils/footprint.py` & `kiutils-1.4.3/src/kiutils/footprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,54 +143,66 @@
 
     scale: Coordinate = field(default_factory=lambda: Coordinate(1.0, 1.0, 1.0))
     """The ``scale`` token specifies the model scale factor for each 3D axis"""
 
     rotate: Coordinate = field(default_factory=lambda: Coordinate(0.0, 0.0, 0.0))
     """The ``rotate`` token specifies the model rotation for each 3D axis relative to the footprint"""
 
+    hide: bool = False
+    """The `hide` token specifies if the 3d model is visible or not"""
+
     @classmethod
     def from_sexpr(cls, exp: list) -> Model:
         """Convert the given S-Expresstion into a Model object
 
         Args:
             - exp (list): Part of parsed S-Expression ``(model ...)``
 
         Raises:
             - Exception: When given parameter's type is not a list or the list is not 5 long
             - Exception: When the first item of the list is not model
 
         Returns:
             - Model: Object of the class initialized with the given S-Expression
         """
-        if not isinstance(exp, list) or len(exp) != 5:
+        if not isinstance(exp, list) or len(exp) < 5 or len(exp) > 6:
             raise Exception("Expression does not have the correct type")
 
         if exp[0] != 'model':
             raise Exception("Expression does not have the correct type")
 
         object = cls()
         object.path = exp[1]
-        object.pos = Coordinate.from_sexpr(exp[2][1])
-        object.scale = Coordinate.from_sexpr(exp[3][1])
-        object.rotate = Coordinate.from_sexpr(exp[4][1])
+        if len(exp) == 6 and exp[2] == 'hide':
+            object.hide = True
+            object.pos = Coordinate.from_sexpr(exp[3][1])
+            object.scale = Coordinate.from_sexpr(exp[4][1])
+            object.rotate = Coordinate.from_sexpr(exp[5][1])
+        else:
+            object.pos = Coordinate.from_sexpr(exp[2][1])
+            object.scale = Coordinate.from_sexpr(exp[3][1])
+            object.rotate = Coordinate.from_sexpr(exp[4][1])
+
         return object
 
     def to_sexpr(self, indent=2, newline=True) -> str:
         """Generate the S-Expression representing this object
 
         Args:
             - indent (int): Number of whitespaces used to indent the output. Defaults to 2.
             - newline (bool): Adds a newline to the end of the output. Defaults to True.
 
         Returns:
             - str: S-Expression of this object
         """
         indents = ' '*indent
         endline = '\n' if newline else ''
-        expression =  f'{indents}(model "{dequote(self.path)}"\n'
+        hide = " hide" if self.hide else ""
+
+        expression =  f'{indents}(model "{dequote(self.path)}"{hide}\n'
         expression += f'{indents}  (offset {self.pos.to_sexpr()})\n'
         expression += f'{indents}  (scale {self.scale.to_sexpr()})\n'
         expression += f'{indents}  (rotate {self.rotate.to_sexpr()})\n'
         expression += f'{indents}){endline}'
         return expression
 
 @dataclass
```

### Comparing `kiutils-1.4.2/src/kiutils/items/brditems.py` & `kiutils-1.4.3/src/kiutils/items/brditems.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/src/kiutils/items/common.py` & `kiutils-1.4.3/src/kiutils/items/common.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/src/kiutils/items/dimensions.py` & `kiutils-1.4.3/src/kiutils/items/dimensions.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/src/kiutils/items/fpitems.py` & `kiutils-1.4.3/src/kiutils/items/fpitems.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/src/kiutils/items/gritems.py` & `kiutils-1.4.3/src/kiutils/items/gritems.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/src/kiutils/items/schitems.py` & `kiutils-1.4.3/src/kiutils/items/schitems.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/src/kiutils/items/syitems.py` & `kiutils-1.4.3/src/kiutils/items/syitems.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/src/kiutils/items/zones.py` & `kiutils-1.4.3/src/kiutils/items/zones.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/src/kiutils/libraries.py` & `kiutils-1.4.3/src/kiutils/libraries.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/src/kiutils/schematic.py` & `kiutils-1.4.3/src/kiutils/schematic.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/src/kiutils/symbol.py` & `kiutils-1.4.3/src/kiutils/symbol.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/src/kiutils/utils/sexpr.py` & `kiutils-1.4.3/src/kiutils/utils/sexpr.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/src/kiutils/utils/strings.py` & `kiutils-1.4.3/src/kiutils/utils/strings.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/src/kiutils/wks.py` & `kiutils-1.4.3/src/kiutils/wks.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/src/kiutils.egg-info/PKG-INFO` & `kiutils-1.4.3/src/kiutils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 Metadata-Version: 2.1
 Name: kiutils
-Version: 1.4.2
+Version: 1.4.3
 Summary: Simple and SCM-friendly KiCad file parser for KiCad 6.0 and up
 Home-page: https://github.com/mvnmgrx/kiutils
 Author: Marvin Mager
 Author-email: 99667992+mvnmgrx@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/mvnmgrx/kiutils/issues
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # KiUtils
 
 [![PyPI version](https://img.shields.io/pypi/v/kiutils)](https://pypi.org/project/kiutils)
+[![PyPI downloads](https://img.shields.io/pypi/dm/kiutils.svg)](https://pypistats.org/packages/kiutils)
 ![Python version](https://img.shields.io/pypi/pyversions/kiutils)
 [![License](https://img.shields.io/github/license/mvnmgrx/kiutils)](https://github.com/mvnmgrx/kiutils/blob/master/LICENSE)
 ![Last commit](https://img.shields.io/github/last-commit/mvnmgrx/kiutils)
 [![Documentation Status](https://readthedocs.org/projects/kiutils/badge/?version=latest)](https://kiutils.readthedocs.io/en/latest/?badge=latest)
 
 Simple and SCM-friendly KiCad file parser based on Python dataclasses for KiCad 6.0
 and up. The following KiCad-related files are currently supported:
```

### Comparing `kiutils-1.4.2/src/kiutils.egg-info/SOURCES.txt` & `kiutils-1.4.3/src/kiutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/tests/test_board.py` & `kiutils-1.4.3/tests/test_board.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/tests/test_designrules.py` & `kiutils-1.4.3/tests/test_designrules.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/tests/test_footprint.py` & `kiutils-1.4.3/tests/test_footprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,21 @@
             library_id = 'empty-footprint-other',
             value = 'empty-footprint-other'
         )
         # Set timestamps to be the same as in the expected test output
         footprint.tedit = '6328916A'
 
         self.assertTrue(to_file_and_compare(footprint, self.testData))
+    
+    def test_3dModelHideProperty(self):
+        """Tests the 3d model hide property (see issue #96)"""
+        self.testData.compareToTestFile = True
+        self.testData.pathToTestFile = path.join(FOOTPRINT_BASE, 'test_3dModelHideProperty')
+        footprint = Footprint().from_file(self.testData.pathToTestFile)
+        self.assertTrue(to_file_and_compare(footprint, self.testData))
 
 class Tests_Footprint_Since_V7(unittest.TestCase):
     """Test cases for Footprints since KiCad 7"""
 
     def setUp(self) -> None:
         prepare_test(self)
         return super().setUp()
```

### Comparing `kiutils-1.4.2/tests/test_libtable.py` & `kiutils-1.4.3/tests/test_libtable.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/tests/test_misc.py` & `kiutils-1.4.3/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/tests/test_schematic.py` & `kiutils-1.4.3/tests/test_schematic.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/tests/test_symbol.py` & `kiutils-1.4.3/tests/test_symbol.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/tests/test_worksheets.py` & `kiutils-1.4.3/tests/test_worksheets.py`

 * *Files identical despite different names*

### Comparing `kiutils-1.4.2/tests/testfunctions.py` & `kiutils-1.4.3/tests/testfunctions.py`

 * *Files identical despite different names*

