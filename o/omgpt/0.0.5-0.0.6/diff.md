# Comparing `tmp/omgpt-0.0.5.tar.gz` & `tmp/omgpt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omgpt-0.0.5.tar", max compression
+gzip compressed data, was "omgpt-0.0.6.tar", max compression
```

## Comparing `omgpt-0.0.5.tar` & `omgpt-0.0.6.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1069 2023-07-12 15:32:14.072394 omgpt-0.0.5/LICENSE
--rw-r--r--   0        0        0    10972 2023-07-14 08:42:38.371494 omgpt-0.0.5/README.md
--rw-r--r--   0        0        0     2778 2023-07-15 02:06:09.514634 omgpt-0.0.5/omgpt.py
--rw-r--r--   0        0        0      677 2023-07-15 03:33:02.538529 omgpt-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    11674 1970-01-01 00:00:00.000000 omgpt-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-12 15:32:14.072394 omgpt-0.0.6/LICENSE
+-rw-r--r--   0        0        0    10972 2023-07-14 08:42:38.371494 omgpt-0.0.6/README.md
+-rw-r--r--   0        0        0     2784 2023-07-15 03:46:46.552764 omgpt-0.0.6/omgpt/__init__.py
+-rw-r--r--   0        0        0     2009 2023-07-15 02:06:06.594390 omgpt-0.0.6/omgpt/shtool.py
+-rw-r--r--   0        0        0      677 2023-07-15 03:49:17.360540 omgpt-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    11674 1970-01-01 00:00:00.000000 omgpt-0.0.6/PKG-INFO
```

### Comparing `omgpt-0.0.5/LICENSE` & `omgpt-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `omgpt-0.0.5/README.md` & `omgpt-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `omgpt-0.0.5/omgpt.py` & `omgpt-0.0.6/omgpt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from langchain.memory import ConversationBufferMemory
 from langchain.prompts import MessagesPlaceholder
 from langchain.schema import SystemMessage
 from langchain.tools import Tool
 from prompt_toolkit import PromptSession, prompt
 from prompt_toolkit.history import FileHistory
 
-from shtool import ShellTool, ShellToolSchema
+from omgpt.shtool import ShellTool, ShellToolSchema
 
 DEFAULT_CONFIG = {
     "settings": {
         "chat_model": "gpt-3.5-turbo-0613",
         "system_prompt": "You are a shell. Your name is OMGpt.",
         "temperature": "0",
     },
```

### Comparing `omgpt-0.0.5/pyproject.toml` & `omgpt-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omgpt"
-version = "0.0.5"
+version = "0.0.6"
 description = "Simplify and enhance your command-line experience with the power of AI"
 authors = ["Youngwook Kim <youngwook.kim@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/ywkim/omgpt"
 license = "MIT"
 
 [tool.poetry.dependencies]
```

### Comparing `omgpt-0.0.5/PKG-INFO` & `omgpt-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omgpt
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simplify and enhance your command-line experience with the power of AI
 Home-page: https://github.com/ywkim/omgpt
 License: MIT
 Author: Youngwook Kim
 Author-email: youngwook.kim@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

