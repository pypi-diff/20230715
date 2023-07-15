# Comparing `tmp/Coquille-1.0.1.tar.gz` & `tmp/Coquille-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Coquille-1.0.1.tar", last modified: Fri Jul 14 11:17:39 2023, max compression
+gzip compressed data, was "Coquille-1.0.2.tar", last modified: Sat Jul 15 11:38:19 2023, max compression
```

## Comparing `Coquille-1.0.1.tar` & `Coquille-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 11:17:39.758945 Coquille-1.0.1/
--rw-r--r--   0 qexat     (1000) qexat     (1001)     1813 2023-07-14 10:50:09.000000 Coquille-1.0.1/.gitignore
--rw-r--r--   0 qexat     (1000) qexat     (1001)      551 2023-07-14 10:50:09.000000 Coquille-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 qexat     (1000) qexat     (1001)     1062 2023-07-14 10:50:09.000000 Coquille-1.0.1/LICENSE
--rw-r--r--   0 qexat     (1000) qexat     (1001)     4842 2023-07-14 11:17:39.758945 Coquille-1.0.1/PKG-INFO
--rw-r--r--   0 qexat     (1000) qexat     (1001)     3086 2023-07-14 10:50:09.000000 Coquille-1.0.1/README.md
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 11:17:39.748945 Coquille-1.0.1/examples/
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 11:17:39.752278 Coquille-1.0.1/examples/coquille_context/
--rw-r--r--   0 qexat     (1000) qexat     (1001)      437 2023-07-14 10:50:09.000000 Coquille-1.0.1/examples/coquille_context/__main__.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)    31985 2023-07-14 10:50:09.000000 Coquille-1.0.1/examples/coquille_context/screenshot.png
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 11:17:39.752278 Coquille-1.0.1/examples/coquille_write/
--rw-r--r--   0 qexat     (1000) qexat     (1001)      436 2023-07-14 10:50:09.000000 Coquille-1.0.1/examples/coquille_write/__main__.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)       45 2023-07-14 10:50:09.000000 Coquille-1.0.1/examples/coquille_write/output.txt
--rw-r--r--   0 qexat     (1000) qexat     (1001)    44980 2023-07-14 10:50:09.000000 Coquille-1.0.1/examples/coquille_write/screenshot.png
--rw-r--r--   0 qexat     (1000) qexat     (1001)      698 2023-07-14 11:17:20.000000 Coquille-1.0.1/pyproject.toml
--rw-r--r--   0 qexat     (1000) qexat     (1001)       38 2023-07-14 11:17:39.758945 Coquille-1.0.1/setup.cfg
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 11:17:39.748945 Coquille-1.0.1/src/
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 11:17:39.755612 Coquille-1.0.1/src/Coquille.egg-info/
--rw-r--r--   0 qexat     (1000) qexat     (1001)     4842 2023-07-14 11:17:39.000000 Coquille-1.0.1/src/Coquille.egg-info/PKG-INFO
--rw-r--r--   0 qexat     (1000) qexat     (1001)      601 2023-07-14 11:17:39.000000 Coquille-1.0.1/src/Coquille.egg-info/SOURCES.txt
--rw-r--r--   0 qexat     (1000) qexat     (1001)        1 2023-07-14 11:17:39.000000 Coquille-1.0.1/src/Coquille.egg-info/dependency_links.txt
--rw-r--r--   0 qexat     (1000) qexat     (1001)       35 2023-07-14 11:17:39.000000 Coquille-1.0.1/src/Coquille.egg-info/requires.txt
--rw-r--r--   0 qexat     (1000) qexat     (1001)        9 2023-07-14 11:17:39.000000 Coquille-1.0.1/src/Coquille.egg-info/top_level.txt
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 11:17:39.758945 Coquille-1.0.1/src/coquille/
--rw-r--r--   0 qexat     (1000) qexat     (1001)       32 2023-07-14 10:50:09.000000 Coquille-1.0.1/src/coquille/__init__.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)     6327 2023-07-14 10:57:15.000000 Coquille-1.0.1/src/coquille/coquille.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)    10596 2023-07-14 10:50:09.000000 Coquille-1.0.1/src/coquille/sequences.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)      340 2023-07-14 10:50:09.000000 Coquille-1.0.1/src/coquille/typeshed.py
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-14 11:17:39.758945 Coquille-1.0.1/tests/
--rw-r--r--   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:50:09.000000 Coquille-1.0.1/tests/__init__.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)     1081 2023-07-14 10:50:09.000000 Coquille-1.0.1/tests/coquille_test.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)     4219 2023-07-14 10:50:09.000000 Coquille-1.0.1/tests/sequences_test.py
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-15 11:38:19.067735 Coquille-1.0.2/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     1813 2023-07-14 10:50:09.000000 Coquille-1.0.2/.gitignore
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      551 2023-07-14 10:50:09.000000 Coquille-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     1062 2023-07-14 10:50:09.000000 Coquille-1.0.2/LICENSE
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     4842 2023-07-15 11:38:19.067735 Coquille-1.0.2/PKG-INFO
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     3086 2023-07-14 10:50:09.000000 Coquille-1.0.2/README.md
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-15 11:38:19.057735 Coquille-1.0.2/examples/
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-15 11:38:19.061068 Coquille-1.0.2/examples/coquille_context/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      437 2023-07-14 10:50:09.000000 Coquille-1.0.2/examples/coquille_context/__main__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)    31985 2023-07-14 10:50:09.000000 Coquille-1.0.2/examples/coquille_context/screenshot.png
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-15 11:38:19.064401 Coquille-1.0.2/examples/coquille_write/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      436 2023-07-14 10:50:09.000000 Coquille-1.0.2/examples/coquille_write/__main__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       45 2023-07-14 10:50:09.000000 Coquille-1.0.2/examples/coquille_write/output.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)    44980 2023-07-14 10:50:09.000000 Coquille-1.0.2/examples/coquille_write/screenshot.png
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      698 2023-07-15 11:32:25.000000 Coquille-1.0.2/pyproject.toml
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       38 2023-07-15 11:38:19.071068 Coquille-1.0.2/setup.cfg
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-15 11:38:19.057735 Coquille-1.0.2/src/
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-15 11:38:19.064401 Coquille-1.0.2/src/Coquille.egg-info/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     4842 2023-07-15 11:38:19.000000 Coquille-1.0.2/src/Coquille.egg-info/PKG-INFO
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      601 2023-07-15 11:38:19.000000 Coquille-1.0.2/src/Coquille.egg-info/SOURCES.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)        1 2023-07-15 11:38:19.000000 Coquille-1.0.2/src/Coquille.egg-info/dependency_links.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       35 2023-07-15 11:38:19.000000 Coquille-1.0.2/src/Coquille.egg-info/requires.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)        9 2023-07-15 11:38:19.000000 Coquille-1.0.2/src/Coquille.egg-info/top_level.txt
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-15 11:38:19.067735 Coquille-1.0.2/src/coquille/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       32 2023-07-14 10:50:09.000000 Coquille-1.0.2/src/coquille/__init__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     6335 2023-07-15 11:32:17.000000 Coquille-1.0.2/src/coquille/coquille.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)    10596 2023-07-14 10:50:09.000000 Coquille-1.0.2/src/coquille/sequences.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      340 2023-07-14 10:50:09.000000 Coquille-1.0.2/src/coquille/typeshed.py
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-15 11:38:19.067735 Coquille-1.0.2/tests/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:50:09.000000 Coquille-1.0.2/tests/__init__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     1081 2023-07-14 10:50:09.000000 Coquille-1.0.2/tests/coquille_test.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     4219 2023-07-14 10:50:09.000000 Coquille-1.0.2/tests/sequences_test.py
```

### Comparing `Coquille-1.0.1/.gitignore` & `Coquille-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.1/.pre-commit-config.yaml` & `Coquille-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.1/LICENSE` & `Coquille-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.1/PKG-INFO` & `Coquille-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Coquille
-Version: 1.0.1
+Version: 1.0.2
 Summary: Coquille is a library that wraps terminal escape sequences as convenient functions.
 Author: Qexat
 License: MIT License
         
         Copyright (c) 2023 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `Coquille-1.0.1/README.md` & `Coquille-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.1/examples/coquille_context/screenshot.png` & `Coquille-1.0.2/examples/coquille_context/screenshot.png`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.1/examples/coquille_write/screenshot.png` & `Coquille-1.0.2/examples/coquille_write/screenshot.png`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.1/pyproject.toml` & `Coquille-1.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Coquille"
-version = "1.0.1"
+version = "1.0.2"
 authors = [{ name = "Qexat" }]
 description = "Coquille is a library that wraps terminal escape sequences as convenient functions."
 readme = "README.md"
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `Coquille-1.0.1/src/Coquille.egg-info/PKG-INFO` & `Coquille-1.0.2/src/Coquille.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Coquille
-Version: 1.0.1
+Version: 1.0.2
 Summary: Coquille is a library that wraps terminal escape sequences as convenient functions.
 Author: Qexat
 License: MIT License
         
         Copyright (c) 2023 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `Coquille-1.0.1/src/Coquille.egg-info/SOURCES.txt` & `Coquille-1.0.2/src/Coquille.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.1/src/coquille/coquille.py` & `Coquille-1.0.2/src/coquille/coquille.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # pyright: reportUnusedCallResult = false
-
 from __future__ import annotations
 
 import sys
 from collections.abc import Callable
 from dataclasses import dataclass
 from typing import overload
 from typing import TYPE_CHECKING
 
 from coquille.sequences import EscapeSequence
 from coquille.sequences import soft_reset
 
-__all__ = ["apply", "Coquille", "EscapeSequence", "prepare"]
+__all__ = ["apply", "Coquille", "EscapeSequence", "prepare", "write"]
 
 # ... don't say anything.
 if TYPE_CHECKING:  # pragma: no cover
     if sys.version_info >= (3, 10):
         from typing import ParamSpec
 
         P = ParamSpec("P")
```

### Comparing `Coquille-1.0.1/src/coquille/sequences.py` & `Coquille-1.0.2/src/coquille/sequences.py`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.1/tests/coquille_test.py` & `Coquille-1.0.2/tests/coquille_test.py`

 * *Files identical despite different names*

### Comparing `Coquille-1.0.1/tests/sequences_test.py` & `Coquille-1.0.2/tests/sequences_test.py`

 * *Files identical despite different names*

