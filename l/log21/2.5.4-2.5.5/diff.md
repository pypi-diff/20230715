# Comparing `tmp/log21-2.5.4.tar.gz` & `tmp/log21-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log21-2.5.4.tar", last modified: Wed Jul 12 15:56:22 2023, max compression
+gzip compressed data, was "log21-2.5.5.tar", last modified: Sat Jul 15 14:55:51 2023, max compression
```

## Comparing `log21-2.5.4.tar` & `log21-2.5.5.tar`

### file list

```diff
@@ -1,30 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:56:22.150226 log21-2.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-12 15:56:05.000000 log21-2.5.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-07-12 15:56:22.150226 log21-2.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9550 2023-07-12 15:56:05.000000 log21-2.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:56:22.150226 log21-2.5.4/log21/
--rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-07-12 15:56:05.000000 log21-2.5.4/log21/Argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-07-12 15:56:05.000000 log21-2.5.4/log21/Colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:56:22.150226 log21-2.5.4/log21/CrashReporter/
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-12 15:56:05.000000 log21-2.5.4/log21/CrashReporter/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13999 2023-07-12 15:56:05.000000 log21-2.5.4/log21/CrashReporter/Reporters.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-12 15:56:05.000000 log21-2.5.4/log21/CrashReporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-12 15:56:05.000000 log21-2.5.4/log21/FileHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-07-12 15:56:05.000000 log21-2.5.4/log21/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-12 15:56:05.000000 log21-2.5.4/log21/Levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-12 15:56:05.000000 log21-2.5.4/log21/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-07-12 15:56:05.000000 log21-2.5.4/log21/LoggingWindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-12 15:56:05.000000 log21-2.5.4/log21/Manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    25520 2023-07-12 15:56:05.000000 log21-2.5.4/log21/PPrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-07-12 15:56:05.000000 log21-2.5.4/log21/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-12 15:56:05.000000 log21-2.5.4/log21/StreamHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-07-12 15:56:05.000000 log21-2.5.4/log21/TreePrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-07-12 15:56:05.000000 log21-2.5.4/log21/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:56:22.150226 log21-2.5.4/log21.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-07-12 15:56:22.000000 log21-2.5.4/log21.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-12 15:56:22.000000 log21-2.5.4/log21.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:56:22.000000 log21-2.5.4/log21.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-12 15:56:22.000000 log21-2.5.4/log21.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 15:56:22.000000 log21-2.5.4/log21.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-12 15:56:05.000000 log21-2.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 15:56:22.150226 log21-2.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:55:51.096461 log21-2.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-07-15 14:55:36.000000 log21-2.5.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-07-15 14:55:51.092461 log21-2.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-07-15 14:55:36.000000 log21-2.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:55:51.092461 log21-2.5.5/log21/
+-rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-07-15 14:55:36.000000 log21-2.5.5/log21/Argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11804 2023-07-15 14:55:36.000000 log21-2.5.5/log21/Colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-15 14:55:36.000000 log21-2.5.5/log21/FileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-07-15 14:55:36.000000 log21-2.5.5/log21/Formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-15 14:55:36.000000 log21-2.5.5/log21/Levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-15 14:55:36.000000 log21-2.5.5/log21/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31105 2023-07-15 14:55:36.000000 log21-2.5.5/log21/LoggingWindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-15 14:55:36.000000 log21-2.5.5/log21/Manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25520 2023-07-15 14:55:36.000000 log21-2.5.5/log21/PPrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-07-15 14:55:36.000000 log21-2.5.5/log21/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-15 14:55:36.000000 log21-2.5.5/log21/StreamHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-15 14:55:36.000000 log21-2.5.5/log21/TreePrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22036 2023-07-15 14:55:36.000000 log21-2.5.5/log21/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:55:51.092461 log21-2.5.5/log21.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-07-15 14:55:51.000000 log21-2.5.5/log21.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-15 14:55:51.000000 log21-2.5.5/log21.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 14:55:51.000000 log21-2.5.5/log21.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-15 14:55:51.000000 log21-2.5.5/log21.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-15 14:55:51.000000 log21-2.5.5/log21.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-15 14:55:36.000000 log21-2.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 14:55:51.096461 log21-2.5.5/setup.cfg
```

### Comparing `log21-2.5.4/LICENSE.txt` & `log21-2.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/PKG-INFO` & `log21-2.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.5.4
+Version: 2.5.5
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Author-email: "CodeWriter21(Mehrad Pooryoussof)" <CodeWriter21@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/MPCodeWriter21/log21
 Project-URL: Donations, https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md
 Project-URL: Source, https://github.com/MPCodeWriter21/log21
 Keywords: python,log,colorize,color,logging,Python3,CodeWriter21
@@ -71,23 +71,17 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.5.4
+### 2.5.5
 
-Added constant colors directly to the Colors module. Now you can do this:
-```python
-from log21 import print
-from log21.colors import GREEN, WHITE, RED
-
-print(GREEN + 'This' + WHITE + ' is' + RED + ' Red')
-```
+Fixed a bug in the `TreePrint` class.
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.5.4/README.md` & `log21-2.5.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -49,23 +49,17 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.5.4
+### 2.5.5
 
-Added constant colors directly to the Colors module. Now you can do this:
-```python
-from log21 import print
-from log21.colors import GREEN, WHITE, RED
-
-print(GREEN + 'This' + WHITE + ' is' + RED + ' Red')
-```
+Fixed a bug in the `TreePrint` class.
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.5.4/log21/Argparse.py` & `log21-2.5.5/log21/Argparse.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/Colors.py` & `log21-2.5.5/log21/Colors.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/FileHandler.py` & `log21-2.5.5/log21/FileHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/Formatters.py` & `log21-2.5.5/log21/Formatters.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/Logger.py` & `log21-2.5.5/log21/Logger.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/LoggingWindow.py` & `log21-2.5.5/log21/LoggingWindow.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/Manager.py` & `log21-2.5.5/log21/Manager.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/PPrint.py` & `log21-2.5.5/log21/PPrint.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/ProgressBar.py` & `log21-2.5.5/log21/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/StreamHandler.py` & `log21-2.5.5/log21/StreamHandler.py`

 * *Files identical despite different names*

### Comparing `log21-2.5.4/log21/TreePrint.py` & `log21-2.5.5/log21/TreePrint.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 # log21.TreePrint.py
 # CodeWriter21
 
 from __future__ import annotations
 
-from typing import Union as _Union, Mapping as _Mapping, Sequence as _Sequence, Optional as _Optional, List as _List
+from typing import (
+    List as _List, Union as _Union, Mapping as _Mapping, Optional as _Optional, Sequence
+    as _Sequence
+)
 
 from log21.Colors import get_colors as _gc
 
 
 class TreePrint:
+
     class Node:
-        def __init__(self, value: _Union[str, int], children: _Optional[_List[TreePrint.Node]] = None, indent: int = 4,
-                     colors: _Optional[_Mapping[str, str]] = None, mode: str='-'):
+
+        def __init__(
+            self,
+            value: _Union[str, int],
+            children: _Optional[_List[TreePrint.Node]] = None,
+            indent: int = 4,
+            colors: _Optional[_Mapping[str, str]] = None,
+            mode: str = '-'
+        ):
             self.value = str(value)
             if children:
                 self._children = children
             else:
                 self._children = []
             self.indent = indent
             self.colors = {
@@ -78,15 +89,16 @@
                         prefix_ += prefix[j]
 
                 if i + 1 == len(self._children):
                     prefix_ += chars[6]  # └ OR ╚
                 else:
                     prefix_ += chars[5]  # ├ OR ╠
                 prefix_ += chars[0] * (self.indent - 1)  # ─ OR ═
-                prefix_ = prefix_[:len(prefix)] + _gc(self.colors['branches']) + prefix_[len(prefix):]
+                prefix_ = prefix_[:len(prefix)] + _gc(self.colors['branches']
+                                                      ) + prefix_[len(prefix):]
                 text += child.__str__(level=level + 1, prefix=prefix_, mode=mode)
 
             return text
 
         def has_child(self):
             return len(self._children) > 0
 
@@ -103,67 +115,109 @@
             if value:
                 for child in self._children:
                     if child.value == value:
                         return child
             if index:
                 return self._children[index]
 
-        @staticmethod
-        def add_to(node: TreePrint.Node, data: _Union[_Mapping, _Sequence, str, int], indent: int = 4,
-                   colors: _Optional[_Mapping[str, str]] = None, mode='-'):
+        def add_to(
+            self: TreePrint.Node,
+            data: _Union[_Mapping, _Sequence, str, int],
+            indent: int = 4,
+            colors: _Optional[_Mapping[str, str]] = None,
+            mode='-'
+        ):
             if isinstance(data, _Mapping):
                 if len(data) == 1:
-                    child = TreePrint.Node(list(data.keys())[0], indent=indent, colors=colors, mode=mode)
-                    TreePrint.Node.add_to(child, list(data.values())[0], indent=indent, colors=colors, mode=mode)
-                    node.add_child(child)
+                    child = TreePrint.Node(
+                        list(data.keys())[0], indent=indent, colors=colors, mode=mode
+                    )
+                    child.add_to(
+                        list(data.values())[0], indent=indent, colors=colors, mode=mode
+                    )
+                    self.add_child(child)
                 else:
                     for key, value in data.items():
-                        child = TreePrint.Node(key, indent=indent, colors=colors, mode=mode)
-                        TreePrint.Node.add_to(child, value, indent=indent, colors=colors, mode=mode)
-                        node.add_child(child)
-            elif isinstance(data, _Sequence):
-                for value in data:
-                    if isinstance(value, _Mapping):
-                        for key, dict_value in value.items():
-                            child = TreePrint.Node(key, indent=indent, colors=colors, mode=mode)
-                            TreePrint.Node.add_to(child, dict_value, indent=indent, colors=colors, mode=mode)
-                            node.add_child(child)
-                    elif isinstance(value, _Sequence):
-                        child = TreePrint.Node('>', indent=indent, colors=colors, mode=mode)
-                        TreePrint.Node.add_to(child, value, indent=indent, colors=colors, mode=mode)
-                        node.add_child(child)
-                    else:
-                        child = TreePrint.Node(str(value), indent=indent, colors=colors, mode=mode)
-                        node.add_child(child)
+                        child = TreePrint.Node(
+                            key, indent=indent, colors=colors, mode=mode
+                        )
+                        child.add_to(value, indent=indent, colors=colors, mode=mode)
+                        self.add_child(child)
+            elif isinstance(data, _Sequence) and not isinstance(data, str):
+                if len(data) == 1:
+                    self.add_child(
+                        TreePrint.Node(
+                            data[0], indent=indent, colors=colors, mode=mode
+                        )
+                    )
+                else:
+                    for value in data:
+                        if isinstance(value, _Mapping):
+                            for key, dict_value in value.items():
+                                child = TreePrint.Node(
+                                    key, indent=indent, colors=colors, mode=mode
+                                )
+                                child.add_to(
+                                    dict_value, indent=indent, colors=colors, mode=mode
+                                )
+                                self.add_child(child)
+                        elif isinstance(value, _Sequence):
+                            child = TreePrint.Node(
+                                '>', indent=indent, colors=colors, mode=mode
+                            )
+                            child.add_to(value, indent=indent, colors=colors, mode=mode)
+                            self.add_child(child)
+                        else:
+                            child = TreePrint.Node(
+                                str(value), indent=indent, colors=colors, mode=mode
+                            )
+                            self.add_child(child)
             else:
-                child = TreePrint.Node(str(data), indent=indent, colors=colors, mode=mode)
-                node.add_child(child)
-
-    def __init__(self, data: _Union[_Mapping, _Sequence, str, int], indent: int = 4, 
-                 colors: _Optional[_Mapping[str, str]] = None, mode='-'):
+                child = TreePrint.Node(
+                    str(data), indent=indent, colors=colors, mode=mode
+                )
+                self.add_child(child)
+
+    def __init__(
+        self,
+        data: _Union[_Mapping, _Sequence, str, int],
+        indent: int = 4,
+        colors: _Optional[_Mapping[str, str]] = None,
+        mode='-'
+    ):
         self.indent = indent
         self.mode = mode
         if isinstance(data, _Mapping):
             if len(data) == 1:
-                self.root = self.Node(list(data.keys())[0], indent=indent, colors=colors)
+                self.root = self.Node(
+                    list(data.keys())[0], indent=indent, colors=colors
+                )
                 self.add_to_root(list(data.values()), colors=colors)
             else:
                 self.root = self.Node('root', indent=indent, colors=colors)
                 self.add_to_root(data, colors=colors)
         elif isinstance(data, _Sequence):
             self.root = self.Node('root', indent=indent, colors=colors)
             self.add_to_root(data, colors=colors)
         else:
             self.root = self.Node(str(data), indent=indent, colors=colors)
 
-    def add_to_root(self, data: _Union[_Mapping, _Sequence, str, int], colors: _Optional[_Mapping[str, str]] = None):
-        self.Node.add_to(self.root, data, indent=self.indent, colors=colors, mode=self.mode)
+    def add_to_root(
+        self,
+        data: _Union[_Mapping, _Sequence, str, int],
+        colors: _Optional[_Mapping[str, str]] = None
+    ):
+        self.root.add_to(data, indent=self.indent, colors=colors, mode=self.mode)
 
     def __str__(self, mode=None):
         if not mode:
             mode = self.mode
         return self.root.__str__(mode=mode)
 
 
-def tree_format(data: _Union[_Mapping, _Sequence, str, int], indent: int = 4, mode='-',
-                colors: _Optional[_Mapping[str, str]] = None):
+def tree_format(
+    data: _Union[_Mapping, _Sequence, str, int],
+    indent: int = 4,
+    mode='-',
+    colors: _Optional[_Mapping[str, str]] = None
+):
     return str(TreePrint(data, indent=indent, colors=colors, mode=mode))
```

### Comparing `log21-2.5.4/log21/__init__.py` & `log21-2.5.5/log21/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,71 +18,97 @@
 from log21.Argparse import ColorizingArgumentParser
 from log21.FileHandler import DecolorizingFileHandler
 from log21.LoggingWindow import LoggingWindow, LoggingWindowHandler
 from log21.StreamHandler import ColorizingStreamHandler, StreamHandler
 from log21.Formatters import ColorizingFormatter, DecolorizingFormatter
 from log21.Colors import Colors, get_color, get_colors, ansi_escape, get_color_name, closest_color
 
-__version__ = "2.5.4"
+__version__ = "2.5.5"
 __author__ = "CodeWriter21 (Mehrad Pooryoussof)"
 __github__ = "Https://GitHub.com/MPCodeWriter21/log21"
-__all__ = ['ColorizingStreamHandler', 'DecolorizingFileHandler', 'ColorizingFormatter', 'DecolorizingFormatter',
-           'get_logger', 'Logger', 'Colors', 'get_color', 'get_colors', 'CRITICAL', 'FATAL', 'ERROR', 'WARNING', 'WARN',
-           'INFO', 'DEBUG', 'NOTSET', 'INPUT', 'StreamHandler', 'ColorizingArgumentParser', 'PrettyPrinter', 'pformat',
-           'pprint', 'pretty_print', 'tree_format', 'TreePrint', 'Manager', 'get_color_name', 'closest_color',
-           'ansi_escape', '__version__', '__author__', '__github__', 'debug', 'info', 'warning', 'warn', 'error',
-           'critical', 'fatal', 'exception', 'log', 'basic_config', 'basicConfig', 'ProgressBar', 'progress_bar',
-           'LoggingWindow', 'LoggingWindowHandler', 'get_logging_window', 'CrashReporter', 'console_reporter',
-           'file_reporter']
+__all__ = [
+    'ColorizingStreamHandler', 'DecolorizingFileHandler', 'ColorizingFormatter',
+    'DecolorizingFormatter', 'get_logger', 'Logger', 'Colors', 'get_color',
+    'get_colors', 'CRITICAL', 'FATAL', 'ERROR', 'WARNING', 'WARN', 'INFO', 'DEBUG',
+    'NOTSET', 'INPUT', 'StreamHandler', 'ColorizingArgumentParser', 'PrettyPrinter',
+    'pformat', 'pprint', 'pretty_print', 'tree_format', 'TreePrint', 'Manager',
+    'get_color_name', 'closest_color', 'ansi_escape', '__version__', '__author__',
+    '__github__', 'debug', 'info', 'warning', 'warn', 'error', 'critical', 'fatal',
+    'exception', 'log', 'basic_config', 'basicConfig', 'ProgressBar', 'progress_bar',
+    'LoggingWindow', 'LoggingWindowHandler', 'get_logging_window', 'CrashReporter',
+    'console_reporter', 'file_reporter'
+]
 
 _manager = Manager()
 _logging.setLoggerClass(Logger)
 
 
-def _prepare_formatter(fmt: _Optional[str] = None, style: str = '%', datefmt: str = "%H:%M:%S",
-                       show_level: bool = True, show_time: bool = True, colorize_time_and_level: bool = True,
-                       level_names: _Optional[_Mapping[int, str]] = None,
-                       level_colors: _Optional[_Mapping[int, _Tuple[str, ...]]] = None,
-                       formatter_class: _Type[_logging.Formatter] = ColorizingFormatter):
+def _prepare_formatter(
+    fmt: _Optional[str] = None,
+    style: str = '%',
+    datefmt: str = "%H:%M:%S",
+    show_level: bool = True,
+    show_time: bool = True,
+    colorize_time_and_level: bool = True,
+    level_names: _Optional[_Mapping[int, str]] = None,
+    level_colors: _Optional[_Mapping[int, _Tuple[str, ...]]] = None,
+    formatter_class: _Type[_logging.Formatter] = ColorizingFormatter
+):
     # Prepares a formatting if the fmt was None
     if not fmt:
         style = '%'
         fmt = "%(message)s"
         if show_level:
             fmt = "[%(levelname)s] " + fmt
         if show_time:
             fmt = "[%(asctime)s] " + fmt
         fmt = '\r' + fmt
 
     if level_colors and not issubclass(formatter_class, ColorizingFormatter):
-        warning('`formatter_class` should be a subclass of ColorizingFormatter when used with level_colors.')
-        warning(f'Using `{formatter_class.__name__}` might lead to unexpected behaviour!')
+        warning(
+            '`formatter_class` should be a subclass of ColorizingFormatter when used with level_colors.'
+        )
+        warning(
+            f'Using `{formatter_class.__name__}` might lead to unexpected behaviour!'
+        )
 
     # Defines the formatter
     if level_colors:
-        formatter = formatter_class(fmt, datefmt, style=style, level_colors=level_colors)
+        formatter = formatter_class(
+            fmt, datefmt, style=style, level_colors=level_colors
+        )
     else:
         formatter = formatter_class(fmt, datefmt, style=style)
-    
+
     if isinstance(formatter, Formatters._Formatter) and level_names:
         formatter.level_names = level_names
     if not colorize_time_and_level and isinstance(formatter, ColorizingFormatter):
         for key in formatter.level_colors:
             formatter.level_colors[key] = tuple()
         formatter.time_color = tuple()
 
     return formatter
 
 
-def get_logger(name: str = '', level: _Union[int, str] = NOTSET, show_time: bool = True,
-               show_level: bool = True, colorize_time_and_level: bool = True, fmt: _Optional[str] = None,
-               datefmt: str = "%H:%M:%S", style: str = '%', handle_carriage_return: bool = True,
-               handle_new_line: bool = True, override=False, level_names: _Optional[_Mapping[int, str]] = None,
-               level_colors: _Optional[_Mapping[int, _Tuple[str, ...]]] = None,
-               file: _Optional[_Union[_os.PathLike, str]] = None) -> _Union[Logger, _logging.Logger]:
+def get_logger(
+    name: str = '',
+    level: _Union[int, str] = NOTSET,
+    show_time: bool = True,
+    show_level: bool = True,
+    colorize_time_and_level: bool = True,
+    fmt: _Optional[str] = None,
+    datefmt: str = "%H:%M:%S",
+    style: str = '%',
+    handle_carriage_return: bool = True,
+    handle_new_line: bool = True,
+    override=False,
+    level_names: _Optional[_Mapping[int, str]] = None,
+    level_colors: _Optional[_Mapping[int, _Tuple[str, ...]]] = None,
+    file: _Optional[_Union[_os.PathLike, str]] = None
+) -> _Union[Logger, _logging.Logger]:
     """
     Returns a logging.Logger with colorizing support.
     >>>
     >>> import log21
     >>>
     >>> l = log21.get_logger()
     >>> l.warning('Pretty basic, huh?')
@@ -144,39 +170,63 @@
     if not isinstance(name, str):
         raise TypeError('A logger name must be a string')
     logger = None
     if name:
         logger = _manager.getLogger(name)
     if (not logger) or override:
         logger = Logger(name, level)
-        formatter = _prepare_formatter(fmt, style, datefmt, show_level, show_time, colorize_time_and_level,
-                                       level_names, level_colors)
+        formatter = _prepare_formatter(
+            fmt, style, datefmt, show_level, show_time, colorize_time_and_level,
+            level_names, level_colors
+        )
 
         # Defines the handler
-        handler = ColorizingStreamHandler(handle_carriage_return=handle_carriage_return,
-                                          handle_new_line=handle_new_line)
+        handler = ColorizingStreamHandler(
+            handle_carriage_return=handle_carriage_return,
+            handle_new_line=handle_new_line
+        )
         handler.setFormatter(formatter)
         logger.addHandler(handler)
         _manager.addLogger(name, logger)
 
         if file:
             file_handler = FileHandler.FileHandler(file)
-            file_formatter = _prepare_formatter(fmt, style, datefmt, show_level, show_time, False, level_names,
-                                                formatter_class=Formatters.DecolorizingFormatter)
+            file_formatter = _prepare_formatter(
+                fmt,
+                style,
+                datefmt,
+                show_level,
+                show_time,
+                False,
+                level_names,
+                formatter_class=Formatters.DecolorizingFormatter
+            )
             file_handler.setFormatter(file_formatter)
             logger.addHandler(file_handler)
 
     return logger
 
 
-def get_logging_window(name: str = '', level: _Union[int, str] = NOTSET, show_time: bool = True,
-                       show_level: bool = True, colorize_time_and_level: bool = True, fmt: _Optional[str] = None,
-                       datefmt: str = "%H:%M:%S", style: str = '%', handle_carriage_return: bool = True,
-                       handle_new_line: bool = True, override=False, level_names: _Optional[_Mapping[int, str]] = None,
-                       width: int = 80, height: int = 20, allow_shell: bool = False) -> LoggingWindow:
+def get_logging_window(
+    name: str = '',
+    level: _Union[int, str] = NOTSET,
+    show_time: bool = True,
+    show_level: bool = True,
+    colorize_time_and_level: bool = True,
+    fmt: _Optional[str] = None,
+    datefmt: str = "%H:%M:%S",
+    style: str = '%',
+    handle_carriage_return: bool = True,
+    handle_new_line: bool = True,
+    override=False,
+    level_names: _Optional[_Mapping[int, str]] = None,
+    width: int = 80,
+    height: int = 20,
+    allow_shell: bool = False
+) -> LoggingWindow:
     """
     Returns a logging window.
 
     >>> # Let's see how it works
     >>> # Imports log21 and time modules
     >>> import log21, time
     >>> # Creates a new LoggingWindow object
@@ -228,20 +278,28 @@
     """
     if not isinstance(name, str):
         raise TypeError('A logger name must be a string')
     logging_window = None
     if name:
         logging_window = _manager.getLogger(name)
     if (not logging_window) or override:
-        logging_window = LoggingWindow(name, level=level, width=width, height=height, allow_shell=allow_shell)
-        formatter = _prepare_formatter(fmt, style, datefmt, show_level, show_time, colorize_time_and_level, level_names)
+        logging_window = LoggingWindow(
+            name, level=level, width=width, height=height, allow_shell=allow_shell
+        )
+        formatter = _prepare_formatter(
+            fmt, style, datefmt, show_level, show_time, colorize_time_and_level,
+            level_names
+        )
 
         # Defines the handler
-        handler = LoggingWindowHandler(logging_window, handle_carriage_return=handle_carriage_return,
-                                       handle_new_line=handle_new_line)
+        handler = LoggingWindowHandler(
+            logging_window,
+            handle_carriage_return=handle_carriage_return,
+            handle_new_line=handle_new_line
+        )
         handler.setFormatter(formatter)
         logging_window.addHandler(handler)
         _manager.addLogger(name, logging_window)
     return logging_window
 
 
 getLogger = get_logger
@@ -258,37 +316,81 @@
 
 
 def getpass(*msg, args: tuple = (), end='', **kwargs):
     logger = get_logger('log21.getpass', level=DEBUG, show_time=False, show_level=False)
     return logger.getpass(*msg, args=args, end=end, **kwargs)
 
 
-def pprint(obj, indent=1, width=80, depth=None, signs_colors: _Optional[_Mapping[str, str]] = None, *, sort_dicts=True,
-           underscore_numbers=False, compact=False, end='\033[0m\n', **kwargs):
+def pprint(
+    obj,
+    indent=1,
+    width=80,
+    depth=None,
+    signs_colors: _Optional[_Mapping[str, str]] = None,
+    *,
+    sort_dicts=True,
+    underscore_numbers=False,
+    compact=False,
+    end='\033[0m\n',
+    **kwargs
+):
     logger = get_logger('log21.pprint', level=DEBUG, show_time=False, show_level=False)
-    logger.print(pformat(obj=obj, indent=indent, width=width, depth=depth, signs_colors=signs_colors, compact=compact,
-                         sort_dicts=sort_dicts, underscore_numbers=underscore_numbers), end=end, **kwargs)
+    logger.print(
+        pformat(
+            obj=obj,
+            indent=indent,
+            width=width,
+            depth=depth,
+            signs_colors=signs_colors,
+            compact=compact,
+            sort_dicts=sort_dicts,
+            underscore_numbers=underscore_numbers
+        ),
+        end=end,
+        **kwargs
+    )
 
 
 pretty_print = pprint
 
 
-def tree_print(obj, indent: int = 4, mode='-', colors: _Mapping[str, str] = None, end='\033[0m\n', **kwargs):
-    logger = get_logger('log21.tree_print', level=DEBUG, show_time=False, show_level=False)
-    logger.print(tree_format(obj, indent=indent, mode=mode, colors=colors), end=end, **kwargs)
+def tree_print(
+    obj,
+    indent: int = 4,
+    mode='-',
+    colors: _Mapping[str, str] = None,
+    end='\033[0m\n',
+    **kwargs
+):
+    logger = get_logger(
+        'log21.tree_print', level=DEBUG, show_time=False, show_level=False
+    )
+    logger.print(
+        tree_format(obj, indent=indent, mode=mode, colors=colors), end=end, **kwargs
+    )
 
 
 tprint = tree_print
 
 root = Logger('root-logger', INFO)
 
 
-def basic_config(force: bool = False, encoding: str = None, errors: _Optional[str] = 'backslashreplace', handlers=None,
-                 stream=None, filename=None, filemode: str = 'a', date_format: str = "%H:%M:%S", style: str = '%',
-                 format_: str = None, level: _Union[int, str] = None):
+def basic_config(
+    force: bool = False,
+    encoding: str = None,
+    errors: _Optional[str] = 'backslashreplace',
+    handlers=None,
+    stream=None,
+    filename=None,
+    filemode: str = 'a',
+    date_format: str = "%H:%M:%S",
+    style: str = '%',
+    format_: str = None,
+    level: _Union[int, str] = None
+):
     """
     Do basic configuration for the logging system.
 
     This function does nothing if the root logger already has handlers
     configured, unless the keyword argument *force* is set to ``True``.
     It is a convenience method intended for use by simple scripts
     to do one-shot configuration of the logging package.
@@ -339,34 +441,42 @@
     if force:
         for handler in root.handlers[:]:
             root.removeHandler(handler)
             handler.close()
     if len(root.handlers) == 0:
         if handlers is None:
             if stream and filename:
-                raise ValueError("'stream' and 'filename' should not be specified together")
+                raise ValueError(
+                    "'stream' and 'filename' should not be specified together"
+                )
         else:
             if stream or filename:
-                raise ValueError("'stream' or 'filename' should not be specified together with 'handlers'")
+                raise ValueError(
+                    "'stream' or 'filename' should not be specified together with 'handlers'"
+                )
         if handlers is None:
             if filename:
                 if 'b' in filemode:
                     errors = None
                 else:
                     encoding = _io.text_encoding(encoding)
-                handler = DecolorizingFileHandler(filename, filemode, encoding=encoding, errors=errors)
+                handler = DecolorizingFileHandler(
+                    filename, filemode, encoding=encoding, errors=errors
+                )
             else:
                 handler = ColorizingStreamHandler(stream=stream)
             handlers = [handler]
         if style not in '%{$':
             raise ValueError('Style must be one of: %, {, $')
         if not format_:
-            format_ = {'%': '[%(asctime)s] [%(levelname)s] %(message)s',
-                       '{': '[{asctime}] [{levelname}] {message}',
-                       '$': '[${asctime}] [${levelname}] ${message}'}[style]
+            format_ = {
+                '%': '[%(asctime)s] [%(levelname)s] %(message)s',
+                '{': '[{asctime}] [{levelname}] {message}',
+                '$': '[${asctime}] [${levelname}] ${message}'
+            }[style]
         else:
             format_ = format_
         formatter = ColorizingFormatter(format_, date_format, style=style)
         for handler in handlers:
             if handler.formatter is None:
                 handler.setFormatter(formatter)
             root.addHandler(handler)
@@ -452,21 +562,29 @@
     basicConfig() to add a console handler with a pre-defined format.
     """
     if len(root.handlers) == 0:
         basic_config()
     root.log(level, *msg, args=args, **kwargs)
 
 
-def progress_bar(progress: float, total: float, width: _Optional[int] = None, prefix: str = '|', suffix: str = '|',
-                 show_percentage: bool = True):
+def progress_bar(
+    progress: float,
+    total: float,
+    width: _Optional[int] = None,
+    prefix: str = '|',
+    suffix: str = '|',
+    show_percentage: bool = True
+):
     """
     Print a progress bar to the console.
     """
 
-    bar = ProgressBar(width=width, prefix=prefix, suffix=suffix, show_percentage=show_percentage)
+    bar = ProgressBar(
+        width=width, prefix=prefix, suffix=suffix, show_percentage=show_percentage
+    )
 
     print(bar.get_bar(progress, total))
 
 
 console_reporter = CrashReporter.ConsoleReporter()
 
 file_reporter = CrashReporter.FileReporter(file='crash_report.log')
```

### Comparing `log21-2.5.4/log21.egg-info/PKG-INFO` & `log21-2.5.5/log21.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log21
-Version: 2.5.4
+Version: 2.5.5
 Summary: A simple logging package that helps you log colorized messages in Windows console.
 Author-email: "CodeWriter21(Mehrad Pooryoussof)" <CodeWriter21@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/MPCodeWriter21/log21
 Project-URL: Donations, https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md
 Project-URL: Source, https://github.com/MPCodeWriter21/log21
 Keywords: python,log,colorize,color,logging,Python3,CodeWriter21
@@ -71,23 +71,17 @@
 ```shell
 python setup.py install
 ```
 
 Changes
 -------
 
-### 2.5.4
+### 2.5.5
 
-Added constant colors directly to the Colors module. Now you can do this:
-```python
-from log21 import print
-from log21.colors import GREEN, WHITE, RED
-
-print(GREEN + 'This' + WHITE + ' is' + RED + ' Red')
-```
+Fixed a bug in the `TreePrint` class.
 
 [Full CHANGELOG](https://github.com/MPCodeWriter21/log21/blob/master/CHANGELOG.md)
 
 
 Usage Examples:
 ---------------
```

### Comparing `log21-2.5.4/pyproject.toml` & `log21-2.5.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -21,13 +21,16 @@
   "Operating System :: Unix",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS :: MacOS X"
 ]
 dependencies = [
   "webcolors"
 ]
-version = "2.5.4"
+version = "2.5.5"
+
+[tool.setuptools]
+packages = ["log21"]
 
 [project.urls]
 Homepage = "https://github.com/MPCodeWriter21/log21"
 Donations = "https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md"
 Source = "https://github.com/MPCodeWriter21/log21"
```

