# Comparing `tmp/flake8-import-restrictions-1.1.1.tar.gz` & `tmp/flake8-import-restrictions-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flake8-import-restrictions-1.1.1.tar", last modified: Thu Aug 13 08:42:59 2020, max compression
+gzip compressed data, was "flake8-import-restrictions-2.0.tar", last modified: Fri Jul 14 23:38:01 2023, max compression
```

## Comparing `flake8-import-restrictions-1.1.1.tar` & `flake8-import-restrictions-2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-13 08:42:59.591344 flake8-import-restrictions-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1063 2020-08-13 08:42:52.000000 flake8-import-restrictions-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     5682 2020-08-13 08:42:59.591344 flake8-import-restrictions-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3531 2020-08-13 08:42:52.000000 flake8-import-restrictions-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-13 08:42:59.591344 flake8-import-restrictions-1.1.1/flake8_import_restrictions/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-08-13 08:42:52.000000 flake8-import-restrictions-1.1.1/flake8_import_restrictions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10646 2020-08-13 08:42:52.000000 flake8-import-restrictions-1.1.1/flake8_import_restrictions/checker.py
--rw-r--r--   0 runner    (1001) docker     (116)     2133 2020-08-13 08:42:52.000000 flake8-import-restrictions-1.1.1/flake8_import_restrictions/imports_submodule.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-13 08:42:59.591344 flake8-import-restrictions-1.1.1/flake8_import_restrictions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5682 2020-08-13 08:42:59.000000 flake8-import-restrictions-1.1.1/flake8_import_restrictions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      463 2020-08-13 08:42:59.000000 flake8-import-restrictions-1.1.1/flake8_import_restrictions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-13 08:42:59.000000 flake8-import-restrictions-1.1.1/flake8_import_restrictions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       75 2020-08-13 08:42:59.000000 flake8-import-restrictions-1.1.1/flake8_import_restrictions.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-13 08:42:59.000000 flake8-import-restrictions-1.1.1/flake8_import_restrictions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       27 2020-08-13 08:42:59.000000 flake8-import-restrictions-1.1.1/flake8_import_restrictions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      962 2020-08-13 08:42:59.591344 flake8-import-restrictions-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-08-13 08:42:52.000000 flake8-import-restrictions-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:38:01.705492 flake8-import-restrictions-2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-14 23:37:52.000000 flake8-import-restrictions-2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-14 23:38:01.705492 flake8-import-restrictions-2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-14 23:37:52.000000 flake8-import-restrictions-2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:38:01.705492 flake8-import-restrictions-2.0/flake8_import_restrictions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 23:37:52.000000 flake8-import-restrictions-2.0/flake8_import_restrictions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-07-14 23:37:52.000000 flake8-import-restrictions-2.0/flake8_import_restrictions/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-14 23:37:52.000000 flake8-import-restrictions-2.0/flake8_import_restrictions/imports_submodule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:38:01.705492 flake8-import-restrictions-2.0/flake8_import_restrictions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-14 23:38:01.000000 flake8-import-restrictions-2.0/flake8_import_restrictions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-14 23:38:01.000000 flake8-import-restrictions-2.0/flake8_import_restrictions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:38:01.000000 flake8-import-restrictions-2.0/flake8_import_restrictions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-14 23:38:01.000000 flake8-import-restrictions-2.0/flake8_import_restrictions.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:38:01.000000 flake8-import-restrictions-2.0/flake8_import_restrictions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-14 23:38:01.000000 flake8-import-restrictions-2.0/flake8_import_restrictions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-14 23:38:01.705492 flake8-import-restrictions-2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 23:37:52.000000 flake8-import-restrictions-2.0/setup.py
```

### Comparing `flake8-import-restrictions-1.1.1/LICENSE` & `flake8-import-restrictions-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-import-restrictions-1.1.1/README.md` & `flake8-import-restrictions-2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,95 +8,95 @@
 
 This plugin talks about the `import` syntax (`import X.Y.Z [as foo]`)
 and the `from` syntax (`from X.Y import Z [as foo]`). It talks about
 `import` segments (`import X`), `from` segments (`from Y`), and `as`
 segments (`as Z`).
 
 ## Options
-For every error `I20xx` listed below, there are options `--i20xx_include` and `--i20xx_exclude` 
+For every error `IMR2xx` listed below, there are options `--imr2xx_include` and `--imr2xx_exclude` 
 which are passed a comma separated list of UNIX wildcard patterns each. The error
 will then only be reported on imports of modules that match a include pattern but no exclude 
 pattern.
 
-By default, I2000, I2001, I2002, I2021, I2023, I2041, and I2043 include all (`*`) modules. Only I2041 excludes the
+By default, IMR200, IMR201, IMR202, IMR221, IMR223, IMR241, and IMR243 include all (`*`) modules. Only IMR241 excludes the
 `typing` module from checks, the other errors have no excludes by default.
 
 ## General Import Errors
 
-### I2000
+### IMR200
 Imports should only happen on module level, not locally.
 
 ```python
 # Bad
 def f():
     import os.path
     return os.path.join("a", "b")
 
 # Good
 import os.path
 def f():
     return os.path.join("a", "b")
 ```
 
-### I2001
+### IMR201
 Alias identifiers defined from `as` segments should be at
 least two characters long.
 
 ```python
 # Bad
 import os.path as p
 
 # Good
 import os.path as path
 ```
 
-### I2002
+### IMR202
 Alias identifiers should not have the same name as the imported object.
 
 ```python
 # Bad
 import sys as sys
 
 # Good
 import sys
 ```
 
 ## `import` Syntax Errors
 
-### I2020
+### IMR220
 When using the `import` syntax, if the imported module is a submodule,
 i.e. not a top level module, an `as` segment should be present.
 
 ```python
 # Bad
 import os.path
 
 # Good
 import sys
 import os.path as path
 ```
 
-### I2021
+### IMR221
 When using the `import` syntax, each import statement should
 only import one module.
 
 ```python
 # Bad
 import sys, os
 
 # Good
 import sys
 import os
 ```
 
-### I2022
+### IMR222
 The `import` syntax should not be used.
 
 
-### I2023
+### IMR223
 When using the `import` syntax, do not duplicate module names in the `as`
 segment.
 
 ```python
 # Bad
 import os.path as path
 
@@ -104,68 +104,68 @@
 from os import path
 import os.path as ospath
 ```
 
 
 ## `from` Syntax Errors
 
-### I2040
+### IMR240
 When using the `from` syntax, the `import` segment only contains one
 import.
 
 ```python
 # Bad
 from os import path, environ
 
 # Good
 from os import path
 from os import environ
 ```
 
-### I2041
+### IMR241
 When using the `from` syntax, only submodules are imported, not
 module elements.
 
 ```python
 # Bad
 from os.path import join
 
 # Good
 from os import path
 ```
 
-### I2042
+### IMR242
 When using the `from` syntax, only module elements are imported,
 not submodules.
 
 ```python
 # Bad
 from os import path
 
 # Good
 from os.path import join
 ```
 
-### I2043
+### IMR243
 When using the `from` syntax, `import *` should not be used.
 
 ```python
 # Bad
 from os.path import *
 
 # Good
 from os.path import join
 ```
 
-### I2044
+### IMR244
 Relative imports should not be used.
 
 ```python
 # Bad
 from . import foo
 
 # Good
 from flake8_import_restrictions import foo
 ```
 
-### I2045
+### IMR245
 The `from` syntax should not be used.
```

### Comparing `flake8-import-restrictions-1.1.1/flake8_import_restrictions/imports_submodule.py` & `flake8-import-restrictions-2.0/flake8_import_restrictions/imports_submodule.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             return None
         package = ".".join(filename.split(os.path.sep))
     else:
         package = None
 
     try:
         parent = importlib.import_module("." * level + from_, package)
-    except ImportError:
+    except (ImportError, TypeError):
         return None
     if not hasattr(parent, import_):
         try:
             importlib.import_module(
                 "." * level + from_ + "." + import_, package
             )
         except ImportError:
```

### Comparing `flake8-import-restrictions-1.1.1/setup.cfg` & `flake8-import-restrictions-2.0/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flake8-import-restrictions
-version = 1.1.1
+version = 2.0
 description = A flake8 plugin used to disallow certain forms of imports.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Andreas Tollkötter
 url = https://github.com/atollk/flake8-import-restrictions
 license = MIT
 license_file = LICENSE
@@ -12,26 +12,27 @@
 classifiers = 
 	Framework :: Flake8
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 packages = 
 	flake8_import_restrictions
 include_package_data = True
-python_requires = >=3.7
+python_requires = >=3.8
 zip_safe = False
 
 [options.entry_points]
 flake8.extension = 
-	I20 = flake8_import_restrictions.checker:ImportChecker
+	IMR2 = flake8_import_restrictions.checker:ImportChecker
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

