# Comparing `tmp/open_interpreter-0.0.221.tar.gz` & `tmp/open_interpreter-0.0.222.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.221.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.222.tar", max compression
```

## Comparing `open_interpreter-0.0.221.tar` & `open_interpreter-0.0.222.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.221/LICENSE
--rw-r--r--   0        0        0      246 2023-07-14 08:56:06.552917 open_interpreter-0.0.221/README.md
--rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.221/interpreter/__init__.py
--rw-r--r--   0        0        0     5239 2023-07-14 17:35:57.437462 open_interpreter-0.0.221/interpreter/exec.py
--rw-r--r--   0        0        0     6241 2023-07-14 08:45:19.160956 open_interpreter-0.0.221/interpreter/interpreter.py
--rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.221/interpreter/json_utils.py
--rw-r--r--   0        0        0     3810 2023-07-14 07:24:41.161431 open_interpreter-0.0.221/interpreter/openai_utils.py
--rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.221/interpreter/view.py
--rw-r--r--   0        0        0      490 2023-07-14 17:36:30.520548 open_interpreter-0.0.221/pyproject.toml
--rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 open_interpreter-0.0.221/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.222/LICENSE
+-rw-r--r--   0        0        0      246 2023-07-14 08:56:06.552917 open_interpreter-0.0.222/README.md
+-rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.222/interpreter/__init__.py
+-rw-r--r--   0        0        0     5389 2023-07-14 21:59:19.287606 open_interpreter-0.0.222/interpreter/exec.py
+-rw-r--r--   0        0        0     6309 2023-07-14 17:50:24.410330 open_interpreter-0.0.222/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.222/interpreter/json_utils.py
+-rw-r--r--   0        0        0     3810 2023-07-14 07:24:41.161431 open_interpreter-0.0.222/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.222/interpreter/view.py
+-rw-r--r--   0        0        0      490 2023-07-14 21:59:44.149453 open_interpreter-0.0.222/pyproject.toml
+-rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 open_interpreter-0.0.222/PKG-INFO
```

### Comparing `open_interpreter-0.0.221/LICENSE` & `open_interpreter-0.0.222/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.221/interpreter/exec.py` & `open_interpreter-0.0.222/interpreter/exec.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,18 @@
       
         # Clean ANSI escape sequences
         ansi_escape = re.compile(r'\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])')
         self.data = ansi_escape.sub('', self.data)
 
         # Truncate and prepend a message if truncated
         self.data = truncate_output(self.data)
+
+        # None outputs should be removed, they happen with things like plt.show()
+        if self.data.strip() == "None":
+            self.data = ""
         
         panel = Panel(self.data.strip(), box=MINIMAL, style="#FFFFFF on #3b3b37")
         self.live.update(panel, refresh=True)
 
     def flush(self):
         pass
```

### Comparing `open_interpreter-0.0.221/interpreter/interpreter.py` & `open_interpreter-0.0.222/interpreter/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 system_message = """
 Only use the function you have been provided with, which has one keyword argument: code.
 Remember to write your messages to the user in Markdown.
 You can access the internet. Run whatever code you'd like to achieve the goal, and if at first you don't succeed, try again and again.
 If you run_code and it fails, write a normal message explaining what happened, theorizing why, and planning a new way forward.
 You can install new packages with !pip.
-While you can generate and display static plots (like those from Matplotlib), interactive and dynamic visualizations (like those from Plotly) won't be displayed correctly, so if you need to do something like that, save it as an image and display it.
+While you can generate and display static plots (like those from Matplotlib), you will not be able to see the output-- only the user will see it. Interactive and dynamic visualizations (like those from Plotly) won't be displayed correctly, so if you need to do something like that, save it as an image and display it.
 """.strip()
 
 class Interpreter:
     def __init__(self):
         self.messages = []
         self._logs = []
         self.system_message = system_message
```

### Comparing `open_interpreter-0.0.221/interpreter/json_utils.py` & `open_interpreter-0.0.222/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.221/interpreter/openai_utils.py` & `open_interpreter-0.0.222/interpreter/openai_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.221/interpreter/view.py` & `open_interpreter-0.0.222/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.221/PKG-INFO` & `open_interpreter-0.0.222/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.221
+Version: 0.0.222
 Summary: Ask GPT-4 to run code locally
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

