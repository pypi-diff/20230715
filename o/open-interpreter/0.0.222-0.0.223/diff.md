# Comparing `tmp/open_interpreter-0.0.222.tar.gz` & `tmp/open_interpreter-0.0.223.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.222.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.223.tar", max compression
```

## Comparing `open_interpreter-0.0.222.tar` & `open_interpreter-0.0.223.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.222/LICENSE
--rw-r--r--   0        0        0      246 2023-07-14 08:56:06.552917 open_interpreter-0.0.222/README.md
--rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.222/interpreter/__init__.py
--rw-r--r--   0        0        0     5389 2023-07-14 21:59:19.287606 open_interpreter-0.0.222/interpreter/exec.py
--rw-r--r--   0        0        0     6309 2023-07-14 17:50:24.410330 open_interpreter-0.0.222/interpreter/interpreter.py
--rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.222/interpreter/json_utils.py
--rw-r--r--   0        0        0     3810 2023-07-14 07:24:41.161431 open_interpreter-0.0.222/interpreter/openai_utils.py
--rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.222/interpreter/view.py
--rw-r--r--   0        0        0      490 2023-07-14 21:59:44.149453 open_interpreter-0.0.222/pyproject.toml
--rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 open_interpreter-0.0.222/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.223/LICENSE
+-rw-r--r--   0        0        0      246 2023-07-14 08:56:06.552917 open_interpreter-0.0.223/README.md
+-rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.223/interpreter/__init__.py
+-rw-r--r--   0        0        0     5462 2023-07-15 04:40:20.248931 open_interpreter-0.0.223/interpreter/exec.py
+-rw-r--r--   0        0        0     5611 2023-07-15 04:41:44.032938 open_interpreter-0.0.223/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.223/interpreter/json_utils.py
+-rw-r--r--   0        0        0     3810 2023-07-14 07:24:41.161431 open_interpreter-0.0.223/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     1283 2023-07-14 23:14:50.878970 open_interpreter-0.0.223/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.223/interpreter/view.py
+-rw-r--r--   0        0        0      485 2023-07-15 04:44:35.841357 open_interpreter-0.0.223/pyproject.toml
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 open_interpreter-0.0.223/PKG-INFO
```

### Comparing `open_interpreter-0.0.222/LICENSE` & `open_interpreter-0.0.223/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.222/interpreter/exec.py` & `open_interpreter-0.0.223/interpreter/exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import ast
-import astunparse
+import astor
 from IPython.core.interactiveshell import InteractiveShell
 from IPython.core.ultratb import AutoFormattedTB
 from contextlib import redirect_stdout, redirect_stderr
 import sys
 import re
 from rich.console import Console
 from rich.panel import Panel
@@ -16,28 +16,26 @@
 def check_for_syntax_errors(code):
     # Needs to happen before we execute.
     lines = code.split('\n')
     filtered_lines = [line for line in lines if not re.match(r'^[!%]', line.strip())]
     cleaned_code = '\n'.join(filtered_lines)
     compile(cleaned_code, '<string>', 'exec')
 
-
 def truncate_output(data):
     max_length = 7000
     message = f'Output truncated. Showing the last {max_length} characters:\n\n'
 
     # Remove previous truncation message if it exists
     if data.startswith(message):
         data = data[len(message):]
 
     # If data exceeds max length, truncate it and add message
     if len(data) > max_length:
         data = message + data[-max_length:]
     return data
-  
 
 class RichOutStream:
 
     def __init__(self, live):
         self.live = live
         self.data = ""
 
@@ -50,20 +48,21 @@
         # Clean ANSI escape sequences
         ansi_escape = re.compile(r'\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])')
         self.data = ansi_escape.sub('', self.data)
 
         # Truncate and prepend a message if truncated
         self.data = truncate_output(self.data)
 
-        # None outputs should be removed, they happen with things like plt.show()
-        if self.data.strip() == "None":
+        # None outputs should be empty, they happen with things like plt.show()
+        if self.data.strip() == "None" or self.data.strip() == "":
             self.data = ""
-        
-        panel = Panel(self.data.strip(), box=MINIMAL, style="#FFFFFF on #3b3b37")
-        self.live.update(panel, refresh=True)
+            self.live.update("", refresh=True)
+        else:
+            panel = Panel(self.data.strip(), box=MINIMAL, style="#FFFFFF on #3b3b37")
+            self.live.update(panel, refresh=True)
 
     def flush(self):
         pass
 
 def exec_and_capture_output(code):
     # Store the original stdout and stderr
     old_stdout = sys.stdout
@@ -150,15 +149,15 @@
 
     # Replace last statement with print if needed
     last_statement = tree.body[-1]
     if isinstance(last_statement, ast.Expr) and not (isinstance(last_statement.value, ast.Call) and isinstance(last_statement.value.func, ast.Name) and last_statement.value.func.id == 'print'):
         tree.body[-1] = ast.Expr(ast.Call(func=ast.Name(id='print', ctx=ast.Load()), args=[last_statement.value], keywords=[]))
 
     # Convert modified AST back into source code
-    new_code_lines = astunparse.unparse(tree).split('\n')
+    new_code_lines = astor.to_source(tree).split('\n')
 
     # Reinsert magic commands in their original places
     for i, line in magic_commands.items():
         new_code_lines.insert(i, line)
 
     # Join the code lines back together into a single string
     new_code = '\n'.join(new_code_lines)
```

### Comparing `open_interpreter-0.0.222/interpreter/interpreter.py` & `open_interpreter-0.0.223/interpreter/interpreter.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,36 +2,30 @@
 from .exec import exec_and_capture_output
 from .view import View
 from .json_utils import JsonDeltaCalculator
 from .openai_utils import openai_streaming_response
 
 functions = [{
     "name": "run_code",
-    "description": "Executes given code in an IPython shell, capturing prints, return values, terminal outputs, and tracebacks.",
+    "description": "Executes code in a stateful IPython shell, capturing prints, return values, terminal outputs, and tracebacks.",
     "parameters": {
         "type": "object",
         "properties": {
             "code": {
                 "type": "string",
                 "description": "The code to execute as a JSON decodable string. Can include standard Python and IPython commands."
             }
         },
         "required": ["code"],
     },
     "function": exec_and_capture_output
 }]
 
-system_message = """
-Only use the function you have been provided with, which has one keyword argument: code.
-Remember to write your messages to the user in Markdown.
-You can access the internet. Run whatever code you'd like to achieve the goal, and if at first you don't succeed, try again and again.
-If you run_code and it fails, write a normal message explaining what happened, theorizing why, and planning a new way forward.
-You can install new packages with !pip.
-While you can generate and display static plots (like those from Matplotlib), you will not be able to see the output-- only the user will see it. Interactive and dynamic visualizations (like those from Plotly) won't be displayed correctly, so if you need to do something like that, save it as an image and display it.
-""".strip()
+with open('interpreter/system_message.txt', 'r') as file:
+    system_message = file.read().strip()
 
 class Interpreter:
     def __init__(self):
         self.messages = []
         self._logs = []
         self.system_message = system_message
         self.api_key = None
```

### Comparing `open_interpreter-0.0.222/interpreter/json_utils.py` & `open_interpreter-0.0.223/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.222/interpreter/openai_utils.py` & `open_interpreter-0.0.223/interpreter/openai_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.222/interpreter/view.py` & `open_interpreter-0.0.223/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.222/PKG-INFO` & `open_interpreter-0.0.223/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.222
+Version: 0.0.223
 Summary: Ask GPT-4 to run code locally
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: astunparse (>=1.6.3,<2.0.0)
+Requires-Dist: astor (>=0.8.1,<0.9.0)
 Requires-Dist: ipython (>=8.14.0,<9.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
 
 # Open Interpreter
```

