# Comparing `tmp/open_interpreter-0.0.223.tar.gz` & `tmp/open_interpreter-0.0.224.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.223.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.224.tar", max compression
```

## Comparing `open_interpreter-0.0.223.tar` & `open_interpreter-0.0.224.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.223/LICENSE
--rw-r--r--   0        0        0      246 2023-07-14 08:56:06.552917 open_interpreter-0.0.223/README.md
--rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.223/interpreter/__init__.py
--rw-r--r--   0        0        0     5462 2023-07-15 04:40:20.248931 open_interpreter-0.0.223/interpreter/exec.py
--rw-r--r--   0        0        0     5611 2023-07-15 04:41:44.032938 open_interpreter-0.0.223/interpreter/interpreter.py
--rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.223/interpreter/json_utils.py
--rw-r--r--   0        0        0     3810 2023-07-14 07:24:41.161431 open_interpreter-0.0.223/interpreter/openai_utils.py
--rw-r--r--   0        0        0     1283 2023-07-14 23:14:50.878970 open_interpreter-0.0.223/interpreter/system_message.txt
--rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.223/interpreter/view.py
--rw-r--r--   0        0        0      485 2023-07-15 04:44:35.841357 open_interpreter-0.0.223/pyproject.toml
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 open_interpreter-0.0.223/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.224/LICENSE
+-rw-r--r--   0        0        0      246 2023-07-14 08:56:06.552917 open_interpreter-0.0.224/README.md
+-rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.224/interpreter/__init__.py
+-rw-r--r--   0        0        0     5462 2023-07-15 04:40:20.248931 open_interpreter-0.0.224/interpreter/exec.py
+-rw-r--r--   0        0        0     5785 2023-07-15 05:01:34.498705 open_interpreter-0.0.224/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.224/interpreter/json_utils.py
+-rw-r--r--   0        0        0     3810 2023-07-14 07:24:41.161431 open_interpreter-0.0.224/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     1283 2023-07-14 23:14:50.878970 open_interpreter-0.0.224/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.224/interpreter/view.py
+-rw-r--r--   0        0        0      485 2023-07-15 05:02:15.990670 open_interpreter-0.0.224/pyproject.toml
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 open_interpreter-0.0.224/PKG-INFO
```

### Comparing `open_interpreter-0.0.223/LICENSE` & `open_interpreter-0.0.224/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.223/interpreter/exec.py` & `open_interpreter-0.0.224/interpreter/exec.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.223/interpreter/interpreter.py` & `open_interpreter-0.0.224/interpreter/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from .exec import exec_and_capture_output
 from .view import View
 from .json_utils import JsonDeltaCalculator
 from .openai_utils import openai_streaming_response
+import os
 
 functions = [{
     "name": "run_code",
     "description": "Executes code in a stateful IPython shell, capturing prints, return values, terminal outputs, and tracebacks.",
     "parameters": {
         "type": "object",
         "properties": {
@@ -16,15 +17,18 @@
             }
         },
         "required": ["code"],
     },
     "function": exec_and_capture_output
 }]
 
-with open('interpreter/system_message.txt', 'r') as file:
+# Locate system_message.txt using the absolute path
+# for the directory where this file is located ("here"):
+here = os.path.abspath(os.path.dirname(__file__))
+with open(os.path.join(here, 'system_message.txt'), 'r') as f:
     system_message = file.read().strip()
 
 class Interpreter:
     def __init__(self):
         self.messages = []
         self._logs = []
         self.system_message = system_message
```

### Comparing `open_interpreter-0.0.223/interpreter/json_utils.py` & `open_interpreter-0.0.224/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.223/interpreter/openai_utils.py` & `open_interpreter-0.0.224/interpreter/openai_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.223/interpreter/system_message.txt` & `open_interpreter-0.0.224/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.223/interpreter/view.py` & `open_interpreter-0.0.224/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.223/PKG-INFO` & `open_interpreter-0.0.224/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.223
+Version: 0.0.224
 Summary: Ask GPT-4 to run code locally
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

