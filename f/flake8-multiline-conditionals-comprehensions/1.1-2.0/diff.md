# Comparing `tmp/flake8-multiline-conditionals-comprehensions-1.1.tar.gz` & `tmp/flake8-multiline-conditionals-comprehensions-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flake8-multiline-conditionals-comprehensions-1.1.tar", last modified: Wed Jun 24 06:10:27 2020, max compression
+gzip compressed data, was "flake8-multiline-conditionals-comprehensions-2.0.tar", last modified: Fri Jul 14 23:32:46 2023, max compression
```

## Comparing `flake8-multiline-conditionals-comprehensions-1.1.tar` & `flake8-multiline-conditionals-comprehensions-2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 06:10:27.612835 flake8-multiline-conditionals-comprehensions-1.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1063 2020-06-24 06:10:21.000000 flake8-multiline-conditionals-comprehensions-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     5673 2020-06-24 06:10:27.612835 flake8-multiline-conditionals-comprehensions-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3278 2020-06-24 06:10:21.000000 flake8-multiline-conditionals-comprehensions-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 06:10:27.612835 flake8-multiline-conditionals-comprehensions-1.1/flake8_multiline_conditionals_comprehensions/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-06-24 06:10:21.000000 flake8-multiline-conditionals-comprehensions-1.1/flake8_multiline_conditionals_comprehensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10119 2020-06-24 06:10:21.000000 flake8-multiline-conditionals-comprehensions-1.1/flake8_multiline_conditionals_comprehensions/mcc_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-06-24 06:10:27.612835 flake8-multiline-conditionals-comprehensions-1.1/flake8_multiline_conditionals_comprehensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5673 2020-06-24 06:10:27.000000 flake8-multiline-conditionals-comprehensions-1.1/flake8_multiline_conditionals_comprehensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      563 2020-06-24 06:10:27.000000 flake8-multiline-conditionals-comprehensions-1.1/flake8_multiline_conditionals_comprehensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-24 06:10:27.000000 flake8-multiline-conditionals-comprehensions-1.1/flake8_multiline_conditionals_comprehensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       94 2020-06-24 06:10:27.000000 flake8-multiline-conditionals-comprehensions-1.1/flake8_multiline_conditionals_comprehensions.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-06-24 06:10:27.000000 flake8-multiline-conditionals-comprehensions-1.1/flake8_multiline_conditionals_comprehensions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       45 2020-06-24 06:10:27.000000 flake8-multiline-conditionals-comprehensions-1.1/flake8_multiline_conditionals_comprehensions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1116 2020-06-24 06:10:27.612835 flake8-multiline-conditionals-comprehensions-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-06-24 06:10:21.000000 flake8-multiline-conditionals-comprehensions-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:46.924631 flake8-multiline-conditionals-comprehensions-2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-14 23:32:33.000000 flake8-multiline-conditionals-comprehensions-2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-14 23:32:46.924631 flake8-multiline-conditionals-comprehensions-2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-14 23:32:33.000000 flake8-multiline-conditionals-comprehensions-2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:46.920631 flake8-multiline-conditionals-comprehensions-2.0/flake8_multiline_conditionals_comprehensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:33.000000 flake8-multiline-conditionals-comprehensions-2.0/flake8_multiline_conditionals_comprehensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-07-14 23:32:33.000000 flake8-multiline-conditionals-comprehensions-2.0/flake8_multiline_conditionals_comprehensions/mcc_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:32:46.924631 flake8-multiline-conditionals-comprehensions-2.0/flake8_multiline_conditionals_comprehensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-14 23:32:46.000000 flake8-multiline-conditionals-comprehensions-2.0/flake8_multiline_conditionals_comprehensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-14 23:32:46.000000 flake8-multiline-conditionals-comprehensions-2.0/flake8_multiline_conditionals_comprehensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:32:46.000000 flake8-multiline-conditionals-comprehensions-2.0/flake8_multiline_conditionals_comprehensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 23:32:46.000000 flake8-multiline-conditionals-comprehensions-2.0/flake8_multiline_conditionals_comprehensions.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:32:46.000000 flake8-multiline-conditionals-comprehensions-2.0/flake8_multiline_conditionals_comprehensions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 23:32:46.000000 flake8-multiline-conditionals-comprehensions-2.0/flake8_multiline_conditionals_comprehensions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-14 23:32:46.924631 flake8-multiline-conditionals-comprehensions-2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 23:32:33.000000 flake8-multiline-conditionals-comprehensions-2.0/setup.py
```

### Comparing `flake8-multiline-conditionals-comprehensions-1.1/LICENSE` & `flake8-multiline-conditionals-comprehensions-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-multiline-conditionals-comprehensions-1.1/README.md` & `flake8-multiline-conditionals-comprehensions-2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 ## Contents
   * [Options](#options)
   * [Comprehension Errors](#comprehension-errors)
   * [Condition Errors](#condition-errors)
 
 ## Options
-The flag `--select_c20` can be used to select the set of errors
-to include. By default, the active errors are C2000, C2001, C2002,
-C2020, C2021, C2023.
+The flag `--select_mcc2` can be used to select the set of errors
+to include. By default, the active errors are MCC200, MCC201, MCC202,
+MCC220, MCC221, MCC223.
 
 
 ## Comprehension Errors
 
-### C2000
+### MCC200
 
 A comprehension expression should place each of its generators on a 
 separate line.
 
 ```python
 # Bad
 [x+y for x in range(10) for y in range(10)]
@@ -36,15 +36,15 @@
     x + y
     for x in range(10)
     for y in range(10)
 ]
 ```
 
 
-### C2001
+### MCC201
 
 A multiline comprehension expression should place each of its segments
 (map, generator, filter) on a separate line.
 
 ```python
 # Bad
 [x+y for x in range(10) 
@@ -56,40 +56,40 @@
     for x in range(10)
     for y in range(10)
     if x + y > 5
 ]
 ```
 
 
-### C2002
+### MCC202
 
 A comprehension expression should not contain multiple filters.
 
 ```python
 # Bad
 [x for x in range(10) if x % 2 == 0 if x % 3 == 0]
 
 # Good
 [x for x in range(10) if x % 2 == x % 3 == 0]
 ```
 
-### C2003
+### MCC203
 
 A comprehension expression should not span over multiple lines.
 
 ```python
 # Bad
 [x + y 
 for x in range(10) ]
 
 # Good
 [x+y for x in range(10)]
 ```
 
-### C2004
+### MCC204
 
 A comprehension expression should span over multiple lines.
 
 ```python
 # Bad
 [x for x in range(10)]
 
@@ -98,15 +98,15 @@
 for x in range(10)]
 ```
 
 
 
 ## Condition Errors
 
-### C2020
+### MCC220
 
 A multiline conditional expression should place each of its segments
 on a separate line.
 
 ```python
 # Bad
 1 
@@ -115,29 +115,29 @@
 # Good
 1
 if something()
 else 0
 ```
 
 
-### C2021
+### MCC221
 
 A conditional expression used for assignment should be surrounded by
 parantheses.
 
 ```python
 # Bad
 a = 1 if something() else 0
 
 # Good
 a = (1 if something() else 0)
 ```
 
 
-### C2022
+### MCC222
 
 A conditional expression should not contain further conditional
 expressions.
 
 ```python
 # Bad
 1 if x > 0 else -1 if x < 0 else 0
@@ -148,40 +148,40 @@
 elif x < 0:
     return -1
 else:
     return 0
 ```
 
 
-### C2023
+### MCC223
 
 A conditional expression should not span over multiple lines.
 
 ```python
 # Bad
 1
 if something()
 else 0
 
 # Good
 1 if something() else 0
 ```
 
 
-### C2024
+### MCC224
 
 A conditional expression should span over multiple lines.
 
 ```python
 # Bad
 1 if something() else 0
 
 # Good
 1
 if something()
 else 0
 ```
 
 
-### C2025
+### MCC225
 
 Conditional expressions should not be used.
```

### Comparing `flake8-multiline-conditionals-comprehensions-1.1/flake8_multiline_conditionals_comprehensions/mcc_checker.py` & `flake8-multiline-conditionals-comprehensions-2.0/flake8_multiline_conditionals_comprehensions/mcc_checker.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 import flake8.options.manager
 
 ComprehensionType = Union[
     ast.ListComp, ast.SetComp, ast.DictComp, ast.GeneratorExp
 ]
 
 DEFAULT_SELECT = [
-    "C2000",
-    "C2001",
-    "C2002",
-    "C2020",
-    "C2021",
-    "C2023",
+    "MCC200",
+    "MCC201",
+    "MCC202",
+    "MCC220",
+    "MCC221",
+    "MCC223",
 ]
 
 PYTHON_36 = sys.version_info >= (3, 6)
 PYTHON_37 = sys.version_info >= (3, 7)
 PYTHON_38 = sys.version_info >= (3, 8)
 PYTHON_39 = sys.version_info >= (3, 9)
 
@@ -39,30 +39,30 @@
     def __init__(self, tree: ast.AST, file_tokens: List[tokenize.TokenInfo]):
         self.tree = tree
         self.tokens = file_tokens
 
     @staticmethod
     def add_options(option_manager: flake8.options.manager.OptionManager):
         option_manager.add_option(
-            "--select_c20",
+            "--select_mcc2",
             type=str,
             comma_separated_list=True,
             default=DEFAULT_SELECT,
             parse_from_config=True,
             help="Error types to use. Default: %(default)s",
         )
 
     @staticmethod
     def parse_options(
         option_manager: flake8.options.manager.OptionManager,
         options: argparse.Namespace,
         extra_args,
     ):
         MCCChecker.enabled_errors = [
-            int(option[1:]) for option in options.select_c20
+            int(option[3:]) for option in options.select_mcc2
         ]
 
     def _get_tokens_with_surrounding(
         self, node: ast.AST, margin: int
     ) -> Iterable[tokenize.TokenInfo]:
         start_index, end_index = None, None
         for i, token in enumerate(self.tokens):
@@ -94,59 +94,59 @@
                 for comp in [
                     ast.ListComp,
                     ast.SetComp,
                     ast.DictComp,
                     ast.GeneratorExp,
                 ]
             ):
-                if 2000 in MCCChecker.enabled_errors:
-                    yield from _c2000(cast(ComprehensionType, node))
-                if 2001 in MCCChecker.enabled_errors:
-                    yield from _c2001(cast(ComprehensionType, node))
-                if 2002 in MCCChecker.enabled_errors:
-                    yield from _c2002(cast(ComprehensionType, node))
-                if 2003 in MCCChecker.enabled_errors:
-                    yield from _c2003(cast(ComprehensionType, node))
-                if 2004 in MCCChecker.enabled_errors:
-                    yield from _c2004(cast(ComprehensionType, node))
+                if 200 in MCCChecker.enabled_errors:
+                    yield from _mcc200(cast(ComprehensionType, node))
+                if 201 in MCCChecker.enabled_errors:
+                    yield from _mcc201(cast(ComprehensionType, node))
+                if 202 in MCCChecker.enabled_errors:
+                    yield from _mcc202(cast(ComprehensionType, node))
+                if 203 in MCCChecker.enabled_errors:
+                    yield from _mcc203(cast(ComprehensionType, node))
+                if 204 in MCCChecker.enabled_errors:
+                    yield from _mcc204(cast(ComprehensionType, node))
 
             if isinstance(node, ast.Assign) and isinstance(
                 node.value, ast.IfExp
             ):
-                if 2021 in MCCChecker.enabled_errors:
-                    yield from _c2021(
+                if 221 in MCCChecker.enabled_errors:
+                    yield from _mcc221(
                         node,
                         list(self._get_tokens_with_surrounding(node.value, 1)),
                     )
 
             if isinstance(node, ast.IfExp):
-                if 2020 in MCCChecker.enabled_errors:
-                    yield from _c2020(node)
-                if 2022 in MCCChecker.enabled_errors:
-                    yield from _c2022(node)
-                if 2023 in MCCChecker.enabled_errors:
-                    yield from _c2023(node)
-                if 2024 in MCCChecker.enabled_errors:
-                    yield from _c2024(node)
-                if 2025 in MCCChecker.enabled_errors:
-                    yield from _c2025(node)
+                if 220 in MCCChecker.enabled_errors:
+                    yield from _mcc220(node)
+                if 222 in MCCChecker.enabled_errors:
+                    yield from _mcc222(node)
+                if 223 in MCCChecker.enabled_errors:
+                    yield from _mcc223(node)
+                if 224 in MCCChecker.enabled_errors:
+                    yield from _mcc224(node)
+                if 225 in MCCChecker.enabled_errors:
+                    yield from _mcc225(node)
 
 
 ERROR_MESSAGES = {
-    2000: "Generators in comprehension expression are on the same line.",
-    2001: "Different segments of a comprehension expression share a line.",
-    2002: "Multiple filter segments within a single comprehension expression.",
-    2003: "Multiline comprehension expression are forbidden.",
-    2004: "Singleline comprehension expression are forbidden.",
-    2020: "Different segments of a conditional expression share a line.",
-    2021: "Conditional expression used for assignment not surrounded by parantheses.",
-    2022: "Nested conditional expressions are forbidden.",
-    2023: "Multiline conditional expression are forbidden.",
-    2024: "Singleline conditional expression are forbidden.",
-    2025: "Conditional expressions are forbidden.",
+    200: "Generators in comprehension expression are on the same line.",
+    201: "Different segments of a comprehension expression share a line.",
+    202: "Multiple filter segments within a single comprehension expression.",
+    203: "Multiline comprehension expression are forbidden.",
+    204: "Singleline comprehension expression are forbidden.",
+    220: "Different segments of a conditional expression share a line.",
+    221: "Conditional expression used for assignment not surrounded by parantheses.",
+    222: "Nested conditional expressions are forbidden.",
+    223: "Multiline conditional expression are forbidden.",
+    224: "Singleline conditional expression are forbidden.",
+    225: "Conditional expressions are forbidden.",
 }
 
 
 def lineno(node: ast.AST):
     return node.lineno
 
 
@@ -176,137 +176,137 @@
         )
 
 
 def _error_tuple(error_code: int, node: ast.AST) -> Tuple[int, int, str, type]:
     return (
         lineno(node),
         col_offset(node),
-        f"C{error_code} {ERROR_MESSAGES[error_code]}",
+        f"MCC{error_code} {ERROR_MESSAGES[error_code]}",
         MCCChecker,
     )
 
 
-def _c2000(node: ComprehensionType) -> Iterable[Tuple[int, int, str, type]]:
+def _mcc200(node: ComprehensionType) -> Iterable[Tuple[int, int, str, type]]:
     """
     A comprehension expression should place each of its generators on a separate line.
     """
     for generator1, generator2 in itertools.combinations(node.generators, 2):
         if lineno(generator1.target) <= lineno(generator2.target) <= end_lineno(
             generator1.iter
         ) or lineno(generator2.target) <= lineno(
             generator1.target
         ) <= end_lineno(
             generator2.iter
         ):
-            yield _error_tuple(2000, node)
+            yield _error_tuple(200, node)
 
 
-def _c2001(node: ComprehensionType) -> Iterable[Tuple[int, int, str, type]]:
+def _mcc201(node: ComprehensionType) -> Iterable[Tuple[int, int, str, type]]:
     """
     A multiline comprehension expression should place each of its segments (map, generator, filter) on a separate line.
     """
     if lineno(node) == end_lineno(node):
         return ()  # single line comprehension
 
     seen_line_nos = set()
 
     for generator in node.generators:
         if lineno(generator.target) in seen_line_nos:
-            yield _error_tuple(2001, generator.target)
+            yield _error_tuple(201, generator.target)
         seen_line_nos.add(lineno(generator.target))
 
         for if_clause in generator.ifs:
             if lineno(if_clause) in seen_line_nos:
-                yield _error_tuple(2001, if_clause)
+                yield _error_tuple(201, if_clause)
             seen_line_nos.add(lineno(if_clause))
 
     if isinstance(node, ast.DictComp):
         if lineno(node.value) in seen_line_nos:
-            yield _error_tuple(2001, node.key)
+            yield _error_tuple(201, node.key)
         seen_line_nos.add(lineno(node.value))
     else:
         if lineno(node.elt) in seen_line_nos:
-            yield _error_tuple(2001, node.elt)
+            yield _error_tuple(201, node.elt)
         seen_line_nos.add(lineno(node.elt))
 
 
-def _c2002(node: ComprehensionType) -> Iterable[Tuple[int, int, str, type]]:
+def _mcc202(node: ComprehensionType) -> Iterable[Tuple[int, int, str, type]]:
     """
     A comprehension expression should not contain multiple filters.
     """
     ifs_seen = 0
     for generator in node.generators:
         for if_clause in generator.ifs:
             ifs_seen += 1
             if ifs_seen > 1:
-                yield _error_tuple(2002, if_clause)
+                yield _error_tuple(202, if_clause)
 
 
-def _c2003(node: ComprehensionType) -> Iterable[Tuple[int, int, str, type]]:
+def _mcc203(node: ComprehensionType) -> Iterable[Tuple[int, int, str, type]]:
     """
     A comprehension expression should not span over multiple lines.
     """
     if lineno(node) != end_lineno(node):
-        yield _error_tuple(2003, node)
+        yield _error_tuple(203, node)
 
 
-def _c2004(node: ComprehensionType) -> Iterable[Tuple[int, int, str, type]]:
+def _mcc204(node: ComprehensionType) -> Iterable[Tuple[int, int, str, type]]:
     """
     A comprehension expression should span over multiple lines.
     """
     if lineno(node) == end_lineno(node):
-        yield _error_tuple(2004, node)
+        yield _error_tuple(204, node)
 
 
-def _c2020(node: ast.IfExp) -> Iterable[Tuple[int, int, str, type]]:
+def _mcc220(node: ast.IfExp) -> Iterable[Tuple[int, int, str, type]]:
     """
     A multiline conditional expression should place each of its segments on a separate line.
     """
     if lineno(node) == end_lineno(node):
         return ()  # single line expression
 
     if len({lineno(node.body), lineno(node.test), lineno(node.orelse)}) < 3:
-        yield _error_tuple(2020, node)
+        yield _error_tuple(220, node)
 
 
-def _c2021(
+def _mcc221(
     node: ast.Assign, tokens: List[tokenize.TokenInfo]
 ) -> Iterable[Tuple[int, int, str, type]]:
     """
-    A conditional expression used for assignment must be surrounded by parantheses.
+    A conditional expression used for assignment must be surrounded by parentheses.
     """
     if tokens[0].type != tokenize.OP or "(" not in tokens[0].string:
-        yield _error_tuple(2021, node)
+        yield _error_tuple(221, node)
 
 
-def _c2022(node: ast.IfExp) -> Iterable[Tuple[int, int, str, type]]:
+def _mcc222(node: ast.IfExp) -> Iterable[Tuple[int, int, str, type]]:
     """
     A conditional expression should not contain further conditional expressions.
     """
     for ancestor in itertools.chain(
         ast.walk(node.body), ast.walk(node.test), ast.walk(node.orelse)
     ):
         if isinstance(ancestor, ast.IfExp):
-            yield _error_tuple(2022, ancestor)
+            yield _error_tuple(222, ancestor)
 
 
-def _c2023(node: ast.IfExp) -> Iterable[Tuple[int, int, str, type]]:
+def _mcc223(node: ast.IfExp) -> Iterable[Tuple[int, int, str, type]]:
     """
     A conditional expression should not span over multiple lines.
     """
     if lineno(node) != end_lineno(node):
-        yield _error_tuple(2023, node)
+        yield _error_tuple(223, node)
 
 
-def _c2024(node: ast.IfExp) -> Iterable[Tuple[int, int, str, type]]:
+def _mcc224(node: ast.IfExp) -> Iterable[Tuple[int, int, str, type]]:
     """
     A conditional expression should span over multiple lines.
     """
     if lineno(node) == end_lineno(node):
-        yield _error_tuple(2024, node)
+        yield _error_tuple(224, node)
 
 
-def _c2025(node: ast.IfExp) -> Iterable[Tuple[int, int, str, type]]:
+def _mcc225(node: ast.IfExp) -> Iterable[Tuple[int, int, str, type]]:
     """
     Conditional expressions should not be used.
     """
-    yield _error_tuple(2025, node)
+    yield _error_tuple(225, node)
```

### Comparing `flake8-multiline-conditionals-comprehensions-1.1/flake8_multiline_conditionals_comprehensions.egg-info/SOURCES.txt` & `flake8-multiline-conditionals-comprehensions-2.0/flake8_multiline_conditionals_comprehensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flake8-multiline-conditionals-comprehensions-1.1/setup.cfg` & `flake8-multiline-conditionals-comprehensions-2.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flake8-multiline-conditionals-comprehensions
-version = 1.1
+version = 2.0
 description = A flake8 plugin to make sure complex conditional expressions and comprehension expressions are split over several lines.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Andreas Tollkötter
 url = https://github.com/atollk/flake8-multiline-conditionals-comprehensions
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
 	flake8_multiline_conditionals_comprehensions
 include_package_data = True
-python_requires = >=3.7
+python_requires = >=3.8
 zip_safe = False
 
 [options.entry_points]
 flake8.extension = 
-	C20 = flake8_multiline_conditionals_comprehensions.mcc_checker:MCCChecker
+	MCC2 = flake8_multiline_conditionals_comprehensions.mcc_checker:MCCChecker
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

