# Comparing `tmp/open_interpreter-0.0.225.tar.gz` & `tmp/open_interpreter-0.0.226.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.225.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.226.tar", max compression
```

## Comparing `open_interpreter-0.0.225.tar` & `open_interpreter-0.0.226.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.225/LICENSE
--rw-r--r--   0        0        0      246 2023-07-14 08:56:06.552917 open_interpreter-0.0.225/README.md
--rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.225/interpreter/__init__.py
--rw-r--r--   0        0        0     5462 2023-07-15 04:40:20.248931 open_interpreter-0.0.225/interpreter/exec.py
--rw-r--r--   0        0        0     5782 2023-07-15 05:03:34.126136 open_interpreter-0.0.225/interpreter/interpreter.py
--rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.225/interpreter/json_utils.py
--rw-r--r--   0        0        0     3810 2023-07-14 07:24:41.161431 open_interpreter-0.0.225/interpreter/openai_utils.py
--rw-r--r--   0        0        0     1283 2023-07-14 23:14:50.878970 open_interpreter-0.0.225/interpreter/system_message.txt
--rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.225/interpreter/view.py
--rw-r--r--   0        0        0      485 2023-07-15 05:04:16.946229 open_interpreter-0.0.225/pyproject.toml
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 open_interpreter-0.0.225/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.226/LICENSE
+-rw-r--r--   0        0        0      246 2023-07-14 08:56:06.552917 open_interpreter-0.0.226/README.md
+-rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.226/interpreter/__init__.py
+-rw-r--r--   0        0        0     5462 2023-07-15 04:40:20.248931 open_interpreter-0.0.226/interpreter/exec.py
+-rw-r--r--   0        0        0     5847 2023-07-15 17:55:30.625029 open_interpreter-0.0.226/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.226/interpreter/json_utils.py
+-rw-r--r--   0        0        0     3857 2023-07-15 17:54:55.373624 open_interpreter-0.0.226/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     1283 2023-07-14 23:14:50.878970 open_interpreter-0.0.226/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.226/interpreter/view.py
+-rw-r--r--   0        0        0      541 2023-07-15 17:56:37.307470 open_interpreter-0.0.226/pyproject.toml
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 open_interpreter-0.0.226/PKG-INFO
```

### Comparing `open_interpreter-0.0.225/LICENSE` & `open_interpreter-0.0.226/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.225/interpreter/exec.py` & `open_interpreter-0.0.226/interpreter/exec.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.225/interpreter/interpreter.py` & `open_interpreter-0.0.226/interpreter/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     system_message = f.read().strip()
 
 class Interpreter:
     def __init__(self):
         self.messages = []
         self._logs = []
         self.system_message = system_message
+        self.temperature = 0.2
         self.api_key = None
 
     def reset(self):
         self.messages = []
         self._logs = []
 
     def load(self, messages):
@@ -86,14 +87,15 @@
             # make openai call
             gpt_functions = [{k: v for k, v in d.items() if k != 'function'} for d in functions]
             response = openai_streaming_response(
                 self.messages,
                 gpt_functions,
                 self.system_message,
                 "gpt-4-0613",
+                self.temperature,
                 self.api_key
             )
 
             base_event = {
                 "role": "assistant",
                 "content": ""
             }
```

### Comparing `open_interpreter-0.0.225/interpreter/json_utils.py` & `open_interpreter-0.0.226/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.225/interpreter/openai_utils.py` & `open_interpreter-0.0.226/interpreter/openai_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
               # This isn't great but functions doesn't work with this! So I do this:
               value = json.dumps(value)
               num_tokens += len(encoding.encode(value))
 
     num_tokens += 3  # every reply is primed with <|start|>assistant<|message|>
     return num_tokens
 
-def openai_streaming_response(messages, functions, system_message, model, api_key):
+def openai_streaming_response(messages, functions, system_message, model, temperature, api_key):
 
     if api_key == None:
         if 'OPENAI_API_KEY' in os.environ:
             api_key = os.environ['OPENAI_API_KEY']
         else:
             raise Exception("Please provide an OpenAI API key via interpreter.openai_api_key or as an environment variable ('OPENAI_API_KEY').")
     else:
@@ -102,9 +102,10 @@
 
     final_messages.insert(0, system_message_event)
 
     yield from openai.ChatCompletion.create(
         model=model,
         messages=final_messages,
         functions=functions,
-        stream=True
+        stream=True,
+        temperature=temperature,
     )
```

### Comparing `open_interpreter-0.0.225/interpreter/system_message.txt` & `open_interpreter-0.0.226/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.225/interpreter/view.py` & `open_interpreter-0.0.226/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.225/PKG-INFO` & `open_interpreter-0.0.226/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.225
+Version: 0.0.226
 Summary: Ask GPT-4 to run code locally
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

