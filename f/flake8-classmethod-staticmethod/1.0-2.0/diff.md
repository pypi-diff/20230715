# Comparing `tmp/flake8-classmethod-staticmethod-1.0.tar.gz` & `tmp/flake8-classmethod-staticmethod-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flake8-classmethod-staticmethod-1.0.tar", last modified: Fri Jul 17 19:56:00 2020, max compression
+gzip compressed data, was "flake8-classmethod-staticmethod-2.0.tar", last modified: Fri Jul 14 23:32:20 2023, max compression
```

## Comparing `flake8-classmethod-staticmethod-1.0.tar` & `flake8-classmethod-staticmethod-2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 19:56:00.985241 flake8-classmethod-staticmethod-1.0/
--rw-r--r--   0 runner    (1001) docker     (116)     1063 2020-07-17 19:55:53.000000 flake8-classmethod-staticmethod-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     3438 2020-07-17 19:56:00.989241 flake8-classmethod-staticmethod-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1769 2020-07-17 19:55:53.000000 flake8-classmethod-staticmethod-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 19:56:00.985241 flake8-classmethod-staticmethod-1.0/flake8_classmethod_staticmethod/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-17 19:55:53.000000 flake8-classmethod-staticmethod-1.0/flake8_classmethod_staticmethod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4288 2020-07-17 19:55:53.000000 flake8-classmethod-staticmethod-1.0/flake8_classmethod_staticmethod/checker.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 19:56:00.985241 flake8-classmethod-staticmethod-1.0/flake8_classmethod_staticmethod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3438 2020-07-17 19:56:00.000000 flake8-classmethod-staticmethod-1.0/flake8_classmethod_staticmethod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      455 2020-07-17 19:56:00.000000 flake8-classmethod-staticmethod-1.0/flake8_classmethod_staticmethod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-17 19:56:00.000000 flake8-classmethod-staticmethod-1.0/flake8_classmethod_staticmethod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       76 2020-07-17 19:56:00.000000 flake8-classmethod-staticmethod-1.0/flake8_classmethod_staticmethod.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-17 19:56:00.000000 flake8-classmethod-staticmethod-1.0/flake8_classmethod_staticmethod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       32 2020-07-17 19:56:00.000000 flake8-classmethod-staticmethod-1.0/flake8_classmethod_staticmethod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1023 2020-07-17 19:56:00.989241 flake8-classmethod-staticmethod-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-07-17 19:55:53.000000 flake8-classmethod-staticmethod-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:20.933146 flake8-classmethod-staticmethod-2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-14 23:32:12.000000 flake8-classmethod-staticmethod-2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-14 23:32:20.933146 flake8-classmethod-staticmethod-2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-14 23:32:12.000000 flake8-classmethod-staticmethod-2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:20.933146 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:12.000000 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-14 23:32:12.000000 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod/checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:20.933146 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-14 23:32:20.000000 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-14 23:32:20.000000 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:32:20.000000 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-14 23:32:20.000000 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:32:20.000000 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-14 23:32:20.000000 flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-14 23:32:20.933146 flake8-classmethod-staticmethod-2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 23:32:12.000000 flake8-classmethod-staticmethod-2.0/setup.py
```

### Comparing `flake8-classmethod-staticmethod-1.0/LICENSE` & `flake8-classmethod-staticmethod-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-classmethod-staticmethod-1.0/README.md` & `flake8-classmethod-staticmethod-2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # flake8-classmethod-staticmethod
+[![Build Status](https://github.com/atollk/flake8-classmethod-staticmethod/workflows/tox/badge.svg)](https://github.com/atollk/flake8-classmethod-staticmethod/actions)
+[![Build Status](https://github.com/atollk/flake8-classmethod-staticmethod/workflows/black/badge.svg)](https://github.com/atollk/flake8-classmethod-staticmethod/actions)
+
+
 flake8 plugin that checks rules regarding the staticmethod and classmethod decorators.
 
 ## Options
 
-The plugin offers one flag, `--select_clst1`, accepting a list of error
+The plugin offers one flag, `--select_csm1`, accepting a list of error
 codes (see below) to be enabled. By default, the enabled errors
-are `CLST101` and `CLST131`.
+are `CSM101` and `CSM131`.
 
 ## Error Codes
 
-### CLST100
+### CSM100
 
 `@staticmethod` should not be used.
 
-### CLST101
+### CSM101
 
 A method marked as `@staticmethod` should not reference the class it
 is defined in. Use `@classmethod` otherwise.
 
 **Bad** 
 ```python
 class MyClass:
@@ -30,15 +34,15 @@
 ```python
 class MyClass:
     @classmethod
     def my_name(cls):
         return cls.__name__
 ```
 
-### CLST102
+### CSM102
 
 Do not inherit and override a method marked as `@staticmethod`.
 
 **Bad** 
 ```python
 class MyClass:
     @staticmethod
@@ -55,19 +59,19 @@
 ```python
 class MyClass:
     @classmethod
     def my_name(cls):
         return cls.__name__
 ```
 
-### CLST130
+### CSM130
 
 `@classmethod` should not be used.
 
-### CLST131
+### CSM131
 
 A method marked as `@classmethod` should access the parameter `cls`.
 Use `@staticmethod` otherwise.
 
 **Bad** 
 ```python
 class MyClass:
@@ -80,15 +84,15 @@
 ```python
 class MyClass:
     @staticmethod
     def my_name():
         return "MyClass"
 ```
 
-### CLST132
+### CSM132
 A method marked as `@classmethod` should not reference the class it
 is defined in. Use the `cls` parameter.
 
 ```python
 class MyClass:
     @classmethod
     def my_name(cls):
```

### Comparing `flake8-classmethod-staticmethod-1.0/flake8_classmethod_staticmethod/checker.py` & `flake8-classmethod-staticmethod-2.0/flake8_classmethod_staticmethod/checker.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 import ast
 import sys
 from typing import Iterable, Tuple
 
 import flake8.options.manager
 
 DEFAULT_SELECT = [
-    "CLST101",
-    "CLST131",
+    "CSM101",
+    "CSM131",
 ]
 
-PYTHON_38 = sys.version_info >= (3, 8)
-
 
 class Checker:
     """
     flake8 plugin that checks rules regarding the staticmethod and classmethod decorators.
     """
 
     name = "flake8-classmethod-staticmethod"
@@ -24,32 +22,30 @@
 
     def __init__(self, tree: ast.AST):
         self.tree = tree
 
     @staticmethod
     def add_options(option_manager: flake8.options.manager.OptionManager):
         option_manager.add_option(
-            "--select_clst1",
+            "--select_csm1",
             type=str,
             comma_separated_list=True,
             default=DEFAULT_SELECT,
             parse_from_config=True,
             help="Error types to use. Default: %(default)s",
         )
 
     @classmethod
     def parse_options(
         cls,
         option_manager: flake8.options.manager.OptionManager,
         options: argparse.Namespace,
         extra_args,
     ):
-        cls.enabled_errors = [
-            int(option[4:]) for option in options.select_clst1
-        ]
+        cls.enabled_errors = [int(option[3:]) for option in options.select_csm1]
 
     def run(self) -> Iterable[Tuple[int, int, str, type]]:
         for cls_node in ast.walk(self.tree):
             if isinstance(cls_node, ast.ClassDef):
                 classname = cls_node.name
                 for fn_node in ast.walk(cls_node):
                     if isinstance(fn_node, ast.FunctionDef):
@@ -62,24 +58,24 @@
         )
         is_classmethod = any(
             isinstance(deco, ast.Name) and deco.id == "classmethod"
             for deco in fn_node.decorator_list
         )
         if is_staticmethod:
             if 100 in self.enabled_errors:
-                yield from _clst100(fn_node)
+                yield from _csm100(fn_node)
             if 101 in self.enabled_errors:
-                yield from _clst101(fn_node, classname)
+                yield from _csm101(fn_node, classname)
         if is_classmethod:
             if 130 in self.enabled_errors:
-                yield from _clst130(fn_node)
+                yield from _csm130(fn_node)
             if 131 in self.enabled_errors:
-                yield from _clst131(fn_node)
+                yield from _csm131(fn_node)
             if 132 in self.enabled_errors:
-                yield from _clst132(fn_node, classname)
+                yield from _csm132(fn_node, classname)
 
 
 ERROR_MESSAGES = {
     100: "@staticmethod is used. (hint: try @classmethod or a normal method instead)",
     101: "@staticmethod references its containing class. (hint: use @classmethod instead)",
     130: "@classmethod is used. (hint: try @staticmethod or a normal method instead)",
     131: "@classmethod does not use the cls parameter. (hint: use @staticmethod instead)",
@@ -94,43 +90,43 @@
     )
 
 
 def _error_tuple(error_code: int, node: ast.AST) -> Tuple[int, int, str, type]:
     return (
         node.lineno,
         node.col_offset,
-        f"CLST{error_code} {ERROR_MESSAGES[error_code]}",
+        f"CSM{error_code} {ERROR_MESSAGES[error_code]}",
         Checker,
     )
 
 
-def _clst100(node: ast.FunctionDef) -> Iterable[Tuple[int, int, str, type]]:
+def _csm100(node: ast.FunctionDef) -> Iterable[Tuple[int, int, str, type]]:
     yield _error_tuple(100, node)
 
 
-def _clst101(
+def _csm101(
     node: ast.FunctionDef, classname: str
 ) -> Iterable[Tuple[int, int, str, type]]:
     references_class = any(
         isinstance(child, ast.Name) and child.id == classname
         for child in ast.walk(node)
     )
     if references_class:
         yield _error_tuple(101, node)
 
 
-def _clst130(node: ast.FunctionDef) -> Iterable[Tuple[int, int, str, type]]:
+def _csm130(node: ast.FunctionDef) -> Iterable[Tuple[int, int, str, type]]:
     yield _error_tuple(130, node)
 
 
-def _clst131(node: ast.FunctionDef) -> Iterable[Tuple[int, int, str, type]]:
+def _csm131(node: ast.FunctionDef) -> Iterable[Tuple[int, int, str, type]]:
     if node.args.args:
         cls_param = node.args.args[0].arg
         if not _function_uses_identifier(node, cls_param):
             yield _error_tuple(131, node)
 
 
-def _clst132(
+def _csm132(
     node: ast.FunctionDef, classname: str
 ) -> Iterable[Tuple[int, int, str, type]]:
     if _function_uses_identifier(node, classname):
         yield _error_tuple(132, node)
```

### Comparing `flake8-classmethod-staticmethod-1.0/setup.cfg` & `flake8-classmethod-staticmethod-2.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flake8-classmethod-staticmethod
-version = 1.0
+version = 2.0
 description = flake8 plugin that checks rules regarding the staticmethod and classmethod decorators.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Andreas Tollkötter
 url = https://github.com/atollk/flake8-classmethod-staticmethod
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
 	flake8_classmethod_staticmethod
 include_package_data = True
-python_requires = >=3.7
+python_requires = >=3.8
 zip_safe = False
 
 [options.entry_points]
 flake8.extension = 
-	CLST1 = flake8_classmethod_staticmethod.checker:Checker
+	CSM1 = flake8_classmethod_staticmethod.checker:Checker
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

