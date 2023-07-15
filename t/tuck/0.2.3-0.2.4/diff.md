# Comparing `tmp/tuck-0.2.3.tar.gz` & `tmp/tuck-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuck-0.2.3.tar", last modified: Sun Jun 25 13:08:05 2023, max compression
+gzip compressed data, was "tuck-0.2.4.tar", last modified: Sat Jul 15 21:31:43 2023, max compression
```

## Comparing `tuck-0.2.3.tar` & `tuck-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 13:08:05.082511 tuck-0.2.3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11344 2023-06-25 13:07:56.000000 tuck-0.2.3/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2064 2023-06-25 13:08:05.082511 tuck-0.2.3/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1115 2023-06-25 13:07:56.000000 tuck-0.2.3/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      981 2023-06-25 13:08:05.086511 tuck-0.2.3/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2023-06-25 13:07:56.000000 tuck-0.2.3/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 13:08:05.082511 tuck-0.2.3/tuck/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2023-06-25 13:07:56.000000 tuck-0.2.3/tuck/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       30 2023-06-25 13:07:56.000000 tuck-0.2.3/tuck/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9057 2023-06-25 13:07:56.000000 tuck-0.2.3/tuck/ast.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3584 2023-06-25 13:07:56.000000 tuck-0.2.3/tuck/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4631 2023-06-25 13:07:56.000000 tuck-0.2.3/tuck/editing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-06-25 13:07:56.000000 tuck-0.2.3/tuck/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5655 2023-06-25 13:07:56.000000 tuck-0.2.3/tuck/main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-25 13:07:56.000000 tuck-0.2.3/tuck/py.typed
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14949 2023-06-25 13:07:56.000000 tuck-0.2.3/tuck/wrappers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 13:08:05.082511 tuck-0.2.3/tuck.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2064 2023-06-25 13:08:05.000000 tuck-0.2.3/tuck.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      312 2023-06-25 13:08:05.000000 tuck-0.2.3/tuck.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-25 13:08:05.000000 tuck-0.2.3/tuck.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-06-25 13:08:05.000000 tuck-0.2.3/tuck.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-06-25 13:08:05.000000 tuck-0.2.3/tuck.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-15 21:31:43.504325 tuck-0.2.4/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11344 2023-07-15 21:31:33.000000 tuck-0.2.4/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2064 2023-07-15 21:31:43.504325 tuck-0.2.4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1115 2023-07-15 21:31:33.000000 tuck-0.2.4/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2023-07-15 21:31:43.504325 tuck-0.2.4/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1345 2023-07-15 21:31:33.000000 tuck-0.2.4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-15 21:31:43.504325 tuck-0.2.4/tuck/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      463 2023-07-15 21:31:33.000000 tuck-0.2.4/tuck/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       30 2023-07-15 21:31:33.000000 tuck-0.2.4/tuck/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9057 2023-07-15 21:31:33.000000 tuck-0.2.4/tuck/ast.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3584 2023-07-15 21:31:33.000000 tuck-0.2.4/tuck/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4631 2023-07-15 21:31:33.000000 tuck-0.2.4/tuck/editing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-07-15 21:31:33.000000 tuck-0.2.4/tuck/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5836 2023-07-15 21:31:33.000000 tuck-0.2.4/tuck/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-15 21:31:33.000000 tuck-0.2.4/tuck/py.typed
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14949 2023-07-15 21:31:33.000000 tuck-0.2.4/tuck/wrappers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-15 21:31:43.504325 tuck-0.2.4/tuck.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2064 2023-07-15 21:31:43.000000 tuck-0.2.4/tuck.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      312 2023-07-15 21:31:43.000000 tuck-0.2.4/tuck.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-15 21:31:43.000000 tuck-0.2.4/tuck.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-07-15 21:31:43.000000 tuck-0.2.4/tuck.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-07-15 21:31:43.000000 tuck-0.2.4/tuck.egg-info/top_level.txt
```

### Comparing `tuck-0.2.3/LICENSE` & `tuck-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tuck-0.2.3/PKG-INFO` & `tuck-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuck
-Version: 0.2.3
+Version: 0.2.4
 Summary: Semi-automated Python formatting.
 Home-page: https://github.com/PeterJCLaw/tuck
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: Apache 2.0
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/tuck/issues
 Platform: UNKNOWN
```

### Comparing `tuck-0.2.3/README.md` & `tuck-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `tuck-0.2.3/setup.cfg` & `tuck-0.2.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 	.git,
 	.pybuild,
 	__pycache__,
 	build,
 	debian,
 	script
 ignore = 
+	C401
 	W503
 max_line_length = 95
 noqa-require-code = true
 
 [isort]
 atomic = True
 balanced_wrapping = True
```

### Comparing `tuck-0.2.3/setup.py` & `tuck-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages  # type: ignore[import]
 
 long_description = (Path(__file__).parent / 'README.md').read_text()
 
 setup(
     name='tuck',
-    version='0.2.3',
+    version='0.2.4',
     url='https://github.com/PeterJCLaw/tuck',
     project_urls={
         'Issue tracker': 'https://github.com/PeterJCLaw/tuck/issues',
     },
     description="Semi-automated Python formatting.",
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `tuck-0.2.3/tuck/ast.py` & `tuck-0.2.4/tuck/ast.py`

 * *Files identical despite different names*

### Comparing `tuck-0.2.3/tuck/cli.py` & `tuck-0.2.4/tuck/cli.py`

 * *Files identical despite different names*

### Comparing `tuck-0.2.3/tuck/editing.py` & `tuck-0.2.4/tuck/editing.py`

 * *Files identical despite different names*

### Comparing `tuck-0.2.3/tuck/main.py` & `tuck-0.2.4/tuck/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -119,21 +119,22 @@
         for prev, current in zip([None, *wrapping_summary], wrapping_summary)
         if should_keep(*current, prev)
     ]
 
     return wrapping_summary
 
 
-def determine_insertions(asttokens: ASTTokens, position: Position) -> list[Insertion]:
+def determine_node(asttokens: ASTTokens, position: Position) -> ast.AST:
     finder = NodeFinder(position, WRAPPABLE_NODE_TYPES)
     assert asttokens.tree is not None
     finder.visit(asttokens.tree)
+    return finder.get_found_node(asttokens)
 
-    node = finder.get_found_node(asttokens)
 
+def determine_insertions(asttokens: ASTTokens, node: ast.AST) -> list[Insertion]:
     # Note: insertions are actually applied in reverse, though we'll generate
     # them forwards.
 
     current_indent = get_current_indent(asttokens, node)
 
     mutations = {
         MutationType.WRAP: "\n" + " " * current_indent,
@@ -174,13 +175,20 @@
     try:
         asttokens = ASTTokens(content, parse=True, filename=filename)
     except SyntaxError as e:
         # Catch syntax errors within the file we were asked to parse. We trust
         # that the error is not within asttokens itself.
         raise TargetSyntaxError(e) from e
 
-    insertions = merge_insertions(
-        determine_insertions(asttokens, position)
+    nodes = set(
+        determine_node(asttokens, position)
         for position in positions
     )
 
+    insertions = merge_insertions(
+        determine_insertions(asttokens, node)
+        for node in nodes
+    )
+
+    insertions.sort()
+
     return insertions
```

### Comparing `tuck-0.2.3/tuck/wrappers.py` & `tuck-0.2.4/tuck/wrappers.py`

 * *Files identical despite different names*

### Comparing `tuck-0.2.3/tuck.egg-info/PKG-INFO` & `tuck-0.2.4/tuck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuck
-Version: 0.2.3
+Version: 0.2.4
 Summary: Semi-automated Python formatting.
 Home-page: https://github.com/PeterJCLaw/tuck
 Author: Peter Law
 Author-email: PeterJCLaw@gmail.com
 License: Apache 2.0
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/tuck/issues
 Platform: UNKNOWN
```

