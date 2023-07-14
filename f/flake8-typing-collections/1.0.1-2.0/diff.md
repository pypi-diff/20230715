# Comparing `tmp/flake8-typing-collections-1.0.1.tar.gz` & `tmp/flake8-typing-collections-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flake8-typing-collections-1.0.1.tar", last modified: Sun Aug 23 12:02:51 2020, max compression
+gzip compressed data, was "flake8-typing-collections-2.0.tar", last modified: Fri Jul 14 23:32:32 2023, max compression
```

## Comparing `flake8-typing-collections-1.0.1.tar` & `flake8-typing-collections-2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-23 12:02:51.143737 flake8-typing-collections-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1063 2020-08-23 12:02:44.000000 flake8-typing-collections-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     7830 2020-08-23 12:02:51.143737 flake8-typing-collections-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5089 2020-08-23 12:02:44.000000 flake8-typing-collections-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-23 12:02:51.143737 flake8-typing-collections-1.0.1/flake8_typing_collections/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-08-23 12:02:44.000000 flake8-typing-collections-1.0.1/flake8_typing_collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7314 2020-08-23 12:02:44.000000 flake8-typing-collections-1.0.1/flake8_typing_collections/ast_import_decode.py
--rw-r--r--   0 runner    (1001) docker     (116)     9656 2020-08-23 12:02:44.000000 flake8-typing-collections-1.0.1/flake8_typing_collections/checker.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-23 12:02:51.143737 flake8-typing-collections-1.0.1/flake8_typing_collections.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7830 2020-08-23 12:02:50.000000 flake8-typing-collections-1.0.1/flake8_typing_collections.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      454 2020-08-23 12:02:51.000000 flake8-typing-collections-1.0.1/flake8_typing_collections.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-23 12:02:50.000000 flake8-typing-collections-1.0.1/flake8_typing_collections.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       69 2020-08-23 12:02:50.000000 flake8-typing-collections-1.0.1/flake8_typing_collections.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-23 12:02:50.000000 flake8-typing-collections-1.0.1/flake8_typing_collections.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       26 2020-08-23 12:02:50.000000 flake8-typing-collections-1.0.1/flake8_typing_collections.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1021 2020-08-23 12:02:51.143737 flake8-typing-collections-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-08-23 12:02:44.000000 flake8-typing-collections-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:32.633916 flake8-typing-collections-2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-14 23:32:23.000000 flake8-typing-collections-2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-14 23:32:32.633916 flake8-typing-collections-2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-14 23:32:23.000000 flake8-typing-collections-2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:32.633916 flake8-typing-collections-2.0/flake8_typing_collections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:23.000000 flake8-typing-collections-2.0/flake8_typing_collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-07-14 23:32:23.000000 flake8-typing-collections-2.0/flake8_typing_collections/ast_import_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9649 2023-07-14 23:32:23.000000 flake8-typing-collections-2.0/flake8_typing_collections/checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:32.633916 flake8-typing-collections-2.0/flake8_typing_collections.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-14 23:32:32.000000 flake8-typing-collections-2.0/flake8_typing_collections.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-14 23:32:32.000000 flake8-typing-collections-2.0/flake8_typing_collections.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:32:32.000000 flake8-typing-collections-2.0/flake8_typing_collections.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-14 23:32:32.000000 flake8-typing-collections-2.0/flake8_typing_collections.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:32:32.000000 flake8-typing-collections-2.0/flake8_typing_collections.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-14 23:32:32.000000 flake8-typing-collections-2.0/flake8_typing_collections.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-14 23:32:32.633916 flake8-typing-collections-2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 23:32:23.000000 flake8-typing-collections-2.0/setup.py
```

### Comparing `flake8-typing-collections-1.0.1/LICENSE` & `flake8-typing-collections-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-typing-collections-1.0.1/README.md` & `flake8-typing-collections-2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 the `collections` module.
 
 ## Options
 
 The plugin offers the following flags to select which errors to enable.
 All errors that are not explicitly enabled, are not reported.
 
-* `--tyco_generic_alt`: Enables `TYCO101`, `TYCO102`, `TYCO103`, `TYCO106`, 
-`TYCO107`, `TYCO108`, `TYCO109`, `TYCO110`, `TYCO111`, `TYCO112`, `TYCO114`, 
-`TYCO115`, `TYCO116`, `TYCO117`, `TYCO118`, `TYCO119`, `TYCO120`, `TYCO121`, 
-`TYCO122`, `TYCO123`, `TYCO124`, `TYCO125`, `TYCO126`, `TYCO127`, `TYCO128`,
-`TYCO129`, `TYCO130`, `TYCO131`, and `TYCO132`. 
-* `--tyco_alias_alt`: Enables `TYCO104`, `TYCO105`, and `TYCO113`.
-* `--tyco_general_args`: Enables `TYCO200`, `TYCO201`, and `TYCO202`.
+* `--tyc_generic_alt`: Enables `TYC101`, `TYC102`, `TYC103`, `TYC106`, 
+`TYC107`, `TYC108`, `TYC109`, `TYC110`, `TYC111`, `TYC112`, `TYC114`, 
+`TYC115`, `TYC116`, `TYC117`, `TYC118`, `TYC119`, `TYC120`, `TYC121`, 
+`TYC122`, `TYC123`, `TYC124`, `TYC125`, `TYC126`, `TYC127`, `TYC128`,
+`TYC129`, `TYC130`, `TYC131`, and `TYC132`. 
+* `--tyc_alias_alt`: Enables `TYC104`, `TYC105`, and `TYC113`.
+* `--tyc_general_args`: Enables `TYC200`, `TYC201`, and `TYC202`.
 
 If none of these flags is given, the default selection is used instead,
-which is `--tyco_generic_alt` and `--tyco_general_args`.
+which is `--tyc_generic_alt` and `--tyc_general_args`.
 
 ## Error Codes
 
-## TYCO1xx class
+## TYC1xx class
 
 The `typing` module defines several generic versions of built-in
 classes, such as `typing.List[T]` instead of `list`. Their usage
 is preferred.
 
 ```python
 # Good
@@ -33,184 +33,184 @@
     ...
 
 # Bad
 def sum_list(x: list) -> float:
     ...
 ```
 
-### TYCO100
+### TYC100
 
 Use `typing.Iterable` instead of `collections.abc.Iterable` for type annotations.
 
 
-### TYCO101
+### TYC101
 
 Use `typing.Iterator` instead of `collections.abc.Iterator` for type annotations.
 
 
-### TYCO102
+### TYC102
 
 Use `typing.Reversible` instead of `collections.abc.Reversible` for type annotations.
 
 
-### TYCO103
+### TYC103
 
 Use `typing.Container` instead of `collections.abc.Container` for type annotations.
 
 
-### TYCO104
+### TYC104
 
 Use `typing.Hashable` instead of `collections.abc.Hashable` for type annotations.
 
 
-### TYCO105
+### TYC105
 
 Use `typing.Sized` instead of `collections.abc.Sized` for type annotations.
 
 
-### TYCO106
+### TYC106
 
 Use `typing.Collection` instead of `collections.abc.Collection` for type annotations.
 
 
-### TYCO107
+### TYC107
 
 Use `typing.AbstractSet` instead of `collections.abc.Set` for type annotations.
 
 
-### TYCO108
+### TYC108
 
 Use `typing.MutableSet` instead of `collections.abc.MutableSet` for type annotations.
 
 
-### TYCO109
+### TYC109
 
 Use `typing.Mapping` instead of `collections.abc.Mapping` for type annotations.
 
 
-### TYCO110
+### TYC110
 
 Use `typing.MutableMapping` instead of `collections.abc.MutableMapping` for type annotations.
 
 
-### TYCO111
+### TYC111
 
 Use `typing.Sequence` instead of `collections.abc.Sequence` for type annotations.
 
 
-### TYCO112
+### TYC112
 
 Use `typing.MutableSequence` instead of `collections.abc.MutableSequence` for type annotations.
 
 
-### TYCO113
+### TYC113
 
 Use `typing.ByteString` instead of `bytes` for type annotations.
 
 
-### TYCO114
+### TYC114
 
 Use `typing.Deque` instead of `collections.Deque` for type annotations.
 
 
-### TYCO115
+### TYC115
 
 Use `typing.List` instead of `list` for type annotations.
 
 
-### TYCO116
+### TYC116
 
 Use `typing.Set` instead of `set` for type annotations.
 
 
-### TYCO117
+### TYC117
 
 Use `typing.FrozenSet` instead of `frozenset` for type annotations.
 
 
-### TYCO118
+### TYC118
 
 Use `typing.MappingView` instead of `collections.abc.MappingView` for type annotations.
 
 
-### TYCO119
+### TYC119
 
 Use `typing.KeysView` instead of `collections.abc.KeysView` for type annotations.
 
 
-### TYCO120
+### TYC120
 
 Use `typing.ItemsView` instead of `collections.abc.ItemsView` for type annotations.
 
 
-### TYCO121
+### TYC121
 
 Use `typing.ValuesView` instead of `collections.abc.ValuesView` for type annotations.
 
 
-### TYCO122
+### TYC122
 
 Use `typing.Awaitable` instead of `collections.abc.Awaitable` for type annotations.
 
 
-### TYCO123
+### TYC123
 
 Use `typing.Coroutine` instead of `collections.abc.Coroutine` for type annotations.
 
 
-### TYCO124
+### TYC124
 
 Use `typing.AsyncIterable` instead of `collections.abc.AsyncIterable` for type annotations.
 
 
-### TYCO125
+### TYC125
 
 Use `typing.AsyncIterator` instead of `collections.abc.AsyncIterator` for type annotations.
 
 
-### TYCO126
+### TYC126
 
 Use `typing.ContextManager` instead of `contextlib.AbstractContextManager` for type annotations.
 
 
-### TYCO127
+### TYC127
 
 Use `typing.AsyncContextManager` instead of `contextlib.AbstractAsyncContextManager` for type annotations.
 
 
-### TYCO128
+### TYC128
 
 Use `typing.Dict` instead of `dict` for type annotations.
 
 
-### TYCO129
+### TYC129
 
 Use `typing.DefaultDict` instead of `collections.defaultdict` for type annotations.
 
 
-### TYCO130
+### TYC130
 
 Use `typing.OrderedDict` instead of `collections.OrderedDict` for type annotations.
 
 
-### TYCO131
+### TYC131
 
 Use `typing.Counter` instead of `collections.Counter` for type annotations.
 
 
-### TYCO132
+### TYC132
 
 Use `typing.ChainMap` instead of `collections.ChainMap` for type annotations.
 
 
 
 
 
 
-## TYCO2xx class
+## TYC2xx class
 
 The documentation of the `typing` module recommends to use
 more general types such as `typing.Sequence` over specialized
 types such as `typing.List` in function parameters.
 
 ```python
 # Good
@@ -218,21 +218,21 @@
     ...
 
 # Bad
 def sum_list(x: List[int]) -> int:
     ...
 ```
 
-### TYCO200
+### TYC200
 
 Use `typing.Sequence` or `typing.MutableSequence`
 instead of `typing.List` in function arguments.
 
-### TYCO201
+### TYC201
 
 Use `typing.AbstractSet` or `typing.MutableSet`
 instead of `typing.Set` in function arguments.
 
-### TYCO201
+### TYC201
 
 Use `typing.Mapping` or `typing.MutableMapping`
 instead of `typing.Dict` in function arguments.
```

### Comparing `flake8-typing-collections-1.0.1/flake8_typing_collections/ast_import_decode.py` & `flake8-typing-collections-2.0/flake8_typing_collections/ast_import_decode.py`

 * *Files identical despite different names*

### Comparing `flake8-typing-collections-1.0.1/flake8_typing_collections/checker.py` & `flake8-typing-collections-2.0/flake8_typing_collections/checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,39 +112,39 @@
 
     def __init__(self, tree: ast.AST):
         self.tree = tree
 
     @staticmethod
     def add_options(option_manager: flake8.options.manager.OptionManager):
         option_manager.add_option(
-            "--tyco_generic_alt",
+            "--tyc_generic_alt",
             action="store_true",
             help="Activate errors about generic type versions. See README.md for details.",
         )
         option_manager.add_option(
-            "--tyco_alias_alt",
+            "--tyc_alias_alt",
             action="store_true",
             help="Activate errors about alias type versions. See README.md for details.",
         )
         option_manager.add_option(
-            "--tyco_general_args",
+            "--tyc_general_args",
             action="store_true",
             help="Activate errors about more general types in function parameters. See README.md for details.",
         )
 
     @classmethod
     def parse_options(
         cls,
         option_manager: flake8.options.manager.OptionManager,
         options: argparse.Namespace,
         extra_args,
     ):
-        cls.flags.generic_alt = options.tyco_generic_alt
-        cls.flags.alias_alt = options.tyco_alias_alt
-        cls.flags.general_args = options.tyco_general_args
+        cls.flags.generic_alt = options.tyc_generic_alt
+        cls.flags.alias_alt = options.tyc_alias_alt
+        cls.flags.general_args = options.tyc_general_args
         if not any(dataclasses.asdict(cls.flags).values()):
             cls.flags = DEFAULT_FLAGS
 
     def run(self) -> Iterable[Tuple[int, int, str, type]]:
         for node in ast.walk(self.tree):
             if isinstance(node, ast.AnnAssign):
                 yield from self._check_1xx(node.annotation)
@@ -202,15 +202,15 @@
             if (
                 ast_import_decode.decode(self.tree, type_hint)
                 in BETTER_ALTERNATIVES[error_code]
             ):
                 yield (
                     type_hint.lineno,
                     type_hint.col_offset,
-                    f"TYCO{error_code} " + ERROR_MESSAGES[error_code],
+                    f"TYC{error_code} " + ERROR_MESSAGES[error_code],
                     Checker,
                 )
 
 
 ERROR_MESSAGES = {
     100: "Use typing.Iterable instead of collections.abc.Iterable in type annotations.",
     101: "Use typing.Iterator instead of collections.abc.Iterator in type annotations.",
```

### Comparing `flake8-typing-collections-1.0.1/setup.cfg` & `flake8-typing-collections-2.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flake8-typing-collections
-version = 1.0.1
+version = 2.0
 description = A flake8 plugin that checks the use of type alternatives from the typing module over actual run time types, especially from the collections module.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Andreas Tollkötter
 url = https://github.com/atollk/flake8-typing-collections
 license = MIT
 license_file = LICENSE
@@ -14,23 +14,25 @@
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 packages = 
 	flake8_typing_collections
 include_package_data = True
 python_requires = >=3.8
 zip_safe = False
 
 [options.entry_points]
 flake8.extension = 
-	TYCO = flake8_typing_collections.checker:Checker
+	TYC = flake8_typing_collections.checker:Checker
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

