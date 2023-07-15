# Comparing `tmp/lbstanza-wrappers-0.2.0.tar.gz` & `tmp/lbstanza-wrappers-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbstanza-wrappers-0.2.0.tar", last modified: Sat Jul 15 04:36:09 2023, max compression
+gzip compressed data, was "lbstanza-wrappers-0.2.1.tar", last modified: Sat Jul 15 04:45:56 2023, max compression
```

## Comparing `lbstanza-wrappers-0.2.0.tar` & `lbstanza-wrappers-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 callendorph  (1000) callendorph  (1000)        0 2023-07-15 04:36:09.374735 lbstanza-wrappers-0.2.0/
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)    35149 2023-07-15 04:12:23.000000 lbstanza-wrappers-0.2.0/LICENSE
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)     2586 2023-07-15 04:36:09.374735 lbstanza-wrappers-0.2.0/PKG-INFO
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)     2232 2023-07-15 03:41:35.000000 lbstanza-wrappers-0.2.0/README.md
--rwxrwxr-x   0 callendorph  (1000) callendorph  (1000)    30527 2023-07-15 04:35:10.000000 lbstanza-wrappers-0.2.0/convert2stanza.py
--rwxrw-r--   0 callendorph  (1000) callendorph  (1000)      760 2023-07-15 03:43:15.000000 lbstanza-wrappers-0.2.0/dump-c-header.py
-drwxrwxr-x   0 callendorph  (1000) callendorph  (1000)        0 2023-07-15 04:36:09.374735 lbstanza-wrappers-0.2.0/lbstanza_wrappers.egg-info/
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)     2586 2023-07-15 04:36:09.000000 lbstanza-wrappers-0.2.0/lbstanza_wrappers.egg-info/PKG-INFO
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)      265 2023-07-15 04:36:09.000000 lbstanza-wrappers-0.2.0/lbstanza_wrappers.egg-info/SOURCES.txt
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)        1 2023-07-15 04:36:09.000000 lbstanza-wrappers-0.2.0/lbstanza_wrappers.egg-info/dependency_links.txt
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)       40 2023-07-15 04:36:09.000000 lbstanza-wrappers-0.2.0/lbstanza_wrappers.egg-info/requires.txt
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)        1 2023-07-15 04:36:09.000000 lbstanza-wrappers-0.2.0/lbstanza_wrappers.egg-info/top_level.txt
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)       38 2023-07-15 04:36:09.374735 lbstanza-wrappers-0.2.0/setup.cfg
--rw-rw-r--   0 callendorph  (1000) callendorph  (1000)      707 2023-07-15 04:35:06.000000 lbstanza-wrappers-0.2.0/setup.py
+drwxrwxr-x   0 callendorph  (1000) callendorph  (1000)        0 2023-07-15 04:45:56.290342 lbstanza-wrappers-0.2.1/
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)    35149 2023-07-15 04:37:49.000000 lbstanza-wrappers-0.2.1/LICENSE
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)     2586 2023-07-15 04:45:56.290342 lbstanza-wrappers-0.2.1/PKG-INFO
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)     2232 2023-07-15 04:37:49.000000 lbstanza-wrappers-0.2.1/README.md
+-rwxrwxr-x   0 callendorph  (1000) callendorph  (1000)    30594 2023-07-15 04:45:38.000000 lbstanza-wrappers-0.2.1/convert2stanza.py
+-rwxrwxr-x   0 callendorph  (1000) callendorph  (1000)      760 2023-07-15 04:37:49.000000 lbstanza-wrappers-0.2.1/dump-c-header.py
+drwxrwxr-x   0 callendorph  (1000) callendorph  (1000)        0 2023-07-15 04:45:56.290342 lbstanza-wrappers-0.2.1/lbstanza_wrappers.egg-info/
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)     2586 2023-07-15 04:45:56.000000 lbstanza-wrappers-0.2.1/lbstanza_wrappers.egg-info/PKG-INFO
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)      265 2023-07-15 04:45:56.000000 lbstanza-wrappers-0.2.1/lbstanza_wrappers.egg-info/SOURCES.txt
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)        1 2023-07-15 04:45:56.000000 lbstanza-wrappers-0.2.1/lbstanza_wrappers.egg-info/dependency_links.txt
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)       40 2023-07-15 04:45:56.000000 lbstanza-wrappers-0.2.1/lbstanza_wrappers.egg-info/requires.txt
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)        1 2023-07-15 04:45:56.000000 lbstanza-wrappers-0.2.1/lbstanza_wrappers.egg-info/top_level.txt
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)       38 2023-07-15 04:45:56.290342 lbstanza-wrappers-0.2.1/setup.cfg
+-rw-rw-r--   0 callendorph  (1000) callendorph  (1000)      690 2023-07-15 04:45:38.000000 lbstanza-wrappers-0.2.1/setup.py
```

### Comparing `lbstanza-wrappers-0.2.0/LICENSE` & `lbstanza-wrappers-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lbstanza-wrappers-0.2.0/PKG-INFO` & `lbstanza-wrappers-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbstanza-wrappers
-Version: 0.2.0
+Version: 0.2.1
 Summary: Utility to create lbstanza wrappers from C headers
 Home-page: https://github.com/callendorph/lbstanza-wrappers
 Author: Carl Allendorph
 License: GPLv3
 Keywords: lbstanza wrappers utility
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lbstanza-wrappers-0.2.0/README.md` & `lbstanza-wrappers-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lbstanza-wrappers-0.2.0/convert2stanza.py` & `lbstanza-wrappers-0.2.1/convert2stanza.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #!/usr/bin/env python3
 import argparse
 import os
 import os.path
 import sys
 import logging
+import pkg_resources
 from collections import OrderedDict
 from contextlib import contextmanager
 
 from pycparser import c_parser, c_ast, parse_file
 import pycparser_fake_libc
 
-__version__ = "0.2.0"
+__version__ = pkg_resources.require("lbstanza-wrappers")[0].version
 
 class Exporter(object):
 
   INDENT_STR = "  "
 
   def __init__(self, fout):
     self._fout = fout
```

### Comparing `lbstanza-wrappers-0.2.0/dump-c-header.py` & `lbstanza-wrappers-0.2.1/dump-c-header.py`

 * *Files identical despite different names*

### Comparing `lbstanza-wrappers-0.2.0/lbstanza_wrappers.egg-info/PKG-INFO` & `lbstanza-wrappers-0.2.1/lbstanza_wrappers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lbstanza-wrappers
-Version: 0.2.0
+Version: 0.2.1
 Summary: Utility to create lbstanza wrappers from C headers
 Home-page: https://github.com/callendorph/lbstanza-wrappers
 Author: Carl Allendorph
 License: GPLv3
 Keywords: lbstanza wrappers utility
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

