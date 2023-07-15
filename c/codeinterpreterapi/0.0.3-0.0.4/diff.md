# Comparing `tmp/codeinterpreterapi-0.0.3.tar.gz` & `tmp/codeinterpreterapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeinterpreterapi-0.0.3.tar", max compression
+gzip compressed data, was "codeinterpreterapi-0.0.4.tar", max compression
```

## Comparing `codeinterpreterapi-0.0.3.tar` & `codeinterpreterapi-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1064 2023-07-13 22:00:10.218142 codeinterpreterapi-0.0.3/LICENSE
--rw-r--r--   0        0        0     2134 2023-07-14 23:43:23.004409 codeinterpreterapi-0.0.3/README.md
--rw-r--r--   0        0        0       62 2023-07-14 11:46:56.280365 codeinterpreterapi-0.0.3/codeinterpreterapi/__init__.py
--rw-r--r--   0        0        0      929 2023-07-14 17:11:05.935330 codeinterpreterapi-0.0.3/codeinterpreterapi/callbacks.py
--rw-r--r--   0        0        0        0 2023-07-14 11:28:44.348803 codeinterpreterapi-0.0.3/codeinterpreterapi/chains/__init__.py
--rw-r--r--   0        0        0     9989 2023-07-14 17:11:06.026589 codeinterpreterapi-0.0.3/codeinterpreterapi/chains/functions_agent.py
--rw-r--r--   0        0        0     3054 2023-07-14 17:11:05.973711 codeinterpreterapi-0.0.3/codeinterpreterapi/chains/modifications_check.py
--rw-r--r--   0        0        0     1836 2023-07-14 17:11:05.948871 codeinterpreterapi-0.0.3/codeinterpreterapi/chains/remove_download_link.py
--rw-r--r--   0        0        0      336 2023-07-14 17:11:05.942603 codeinterpreterapi-0.0.3/codeinterpreterapi/config.py
--rw-r--r--   0        0        0       78 2023-07-14 17:11:05.936317 codeinterpreterapi-0.0.3/codeinterpreterapi/prompts/__init__.py
--rw-r--r--   0        0        0     1600 2023-07-14 17:11:05.938058 codeinterpreterapi-0.0.3/codeinterpreterapi/prompts/system_message.py
--rw-r--r--   0        0        0      122 2023-07-14 14:25:57.660993 codeinterpreterapi-0.0.3/codeinterpreterapi/schema/__init__.py
--rw-r--r--   0        0        0     1578 2023-07-14 17:11:05.961530 codeinterpreterapi-0.0.3/codeinterpreterapi/schema/file.py
--rw-r--r--   0        0        0      123 2023-07-14 17:11:05.943821 codeinterpreterapi-0.0.3/codeinterpreterapi/schema/input.py
--rw-r--r--   0        0        0      629 2023-07-14 17:11:05.960810 codeinterpreterapi-0.0.3/codeinterpreterapi/schema/response.py
--rw-r--r--   0        0        0     7960 2023-07-14 17:36:03.828238 codeinterpreterapi-0.0.3/codeinterpreterapi/session.py
--rw-r--r--   0        0        0      629 2023-07-14 23:39:07.982737 codeinterpreterapi-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2909 1970-01-01 00:00:00.000000 codeinterpreterapi-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-13 22:00:10.218142 codeinterpreterapi-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2142 2023-07-15 08:38:12.853808 codeinterpreterapi-0.0.4/README.md
+-rw-r--r--   0        0        0       62 2023-07-14 11:46:56.280365 codeinterpreterapi-0.0.4/codeinterpreterapi/__init__.py
+-rw-r--r--   0        0        0      929 2023-07-14 17:11:05.935330 codeinterpreterapi-0.0.4/codeinterpreterapi/callbacks.py
+-rw-r--r--   0        0        0        0 2023-07-14 11:28:44.348803 codeinterpreterapi-0.0.4/codeinterpreterapi/chains/__init__.py
+-rw-r--r--   0        0        0     9989 2023-07-14 17:11:06.026589 codeinterpreterapi-0.0.4/codeinterpreterapi/chains/functions_agent.py
+-rw-r--r--   0        0        0     3054 2023-07-14 17:11:05.973711 codeinterpreterapi-0.0.4/codeinterpreterapi/chains/modifications_check.py
+-rw-r--r--   0        0        0     1836 2023-07-14 17:11:05.948871 codeinterpreterapi-0.0.4/codeinterpreterapi/chains/remove_download_link.py
+-rw-r--r--   0        0        0      336 2023-07-14 17:11:05.942603 codeinterpreterapi-0.0.4/codeinterpreterapi/config.py
+-rw-r--r--   0        0        0       78 2023-07-14 17:11:05.936317 codeinterpreterapi-0.0.4/codeinterpreterapi/prompts/__init__.py
+-rw-r--r--   0        0        0     1600 2023-07-14 17:11:05.938058 codeinterpreterapi-0.0.4/codeinterpreterapi/prompts/system_message.py
+-rw-r--r--   0        0        0      122 2023-07-14 14:25:57.660993 codeinterpreterapi-0.0.4/codeinterpreterapi/schema/__init__.py
+-rw-r--r--   0        0        0     2285 2023-07-15 11:55:28.309715 codeinterpreterapi-0.0.4/codeinterpreterapi/schema/file.py
+-rw-r--r--   0        0        0      123 2023-07-14 17:11:05.943821 codeinterpreterapi-0.0.4/codeinterpreterapi/schema/input.py
+-rw-r--r--   0        0        0      629 2023-07-14 17:11:05.960810 codeinterpreterapi-0.0.4/codeinterpreterapi/schema/response.py
+-rw-r--r--   0        0        0     7960 2023-07-14 17:36:03.828238 codeinterpreterapi-0.0.4/codeinterpreterapi/session.py
+-rw-r--r--   0        0        0      629 2023-07-15 12:04:32.328557 codeinterpreterapi-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2917 1970-01-01 00:00:00.000000 codeinterpreterapi-0.0.4/PKG-INFO
```

### Comparing `codeinterpreterapi-0.0.3/LICENSE` & `codeinterpreterapi-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.3/README.md` & `codeinterpreterapi-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 ```
 
 ## Usage
 
 ```python
 from codeinterpreterapi import CodeInterpreterSession
 
-# start a session
-session = CodeInterpreterSession()
 
 async def main():
+    # start a session
+    session = CodeInterpreterSession()
     await session.astart()
 
     # generate a response based on user input
     output = await session.generate_response(
         "Plot the bitcoin chart of 2023 YTD"
     )
     # show output image in default image viewer
```

### Comparing `codeinterpreterapi-0.0.3/codeinterpreterapi/callbacks.py` & `codeinterpreterapi-0.0.4/codeinterpreterapi/callbacks.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.3/codeinterpreterapi/chains/functions_agent.py` & `codeinterpreterapi-0.0.4/codeinterpreterapi/chains/functions_agent.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.3/codeinterpreterapi/chains/modifications_check.py` & `codeinterpreterapi-0.0.4/codeinterpreterapi/chains/modifications_check.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.3/codeinterpreterapi/chains/remove_download_link.py` & `codeinterpreterapi-0.0.4/codeinterpreterapi/chains/remove_download_link.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.3/codeinterpreterapi/prompts/system_message.py` & `codeinterpreterapi-0.0.4/codeinterpreterapi/prompts/system_message.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.3/codeinterpreterapi/schema/file.py` & `codeinterpreterapi-0.0.4/codeinterpreterapi/schema/file.py`

 * *Files 24% similar despite different names*

```diff
@@ -48,15 +48,34 @@
             exit(1)
 
         from io import BytesIO
 
         img_io = BytesIO(self.content)
         img = Image.open(img_io)
 
+        # Convert image to RGB if it's not
+        if img.mode not in ('RGB', 'L'):  # L is for greyscale images
+            img = img.convert('RGB')
+
         # Display the image
-        img.show()
+        try:
+            # Try to get the IPython shell if available.
+            shell = get_ipython().__class__.__name__
+
+            # If the shell is ZMQInteractiveShell, it means we're in a Jupyter notebook or similar.
+            if shell == 'ZMQInteractiveShell':
+                from IPython.display import display
+                display(img)
+            else:
+                # We're not in a Jupyter notebook.
+                img.show()
+        except NameError:
+            # We're probably not in an IPython environment, use PIL's show.
+            img.show()
+
+
 
     def __str__(self):
         return self.name
 
     def __repr__(self):
         return f"File(name={self.name})"
```

### Comparing `codeinterpreterapi-0.0.3/codeinterpreterapi/schema/response.py` & `codeinterpreterapi-0.0.4/codeinterpreterapi/schema/response.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.3/codeinterpreterapi/session.py` & `codeinterpreterapi-0.0.4/codeinterpreterapi/session.py`

 * *Files identical despite different names*

### Comparing `codeinterpreterapi-0.0.3/pyproject.toml` & `codeinterpreterapi-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "codeinterpreterapi"
-version = "0.0.3"
+version = "0.0.4"
 description = "CodeInterpreterAPI is an unofficial and open source python interface for the ChatGPT CodeInterpreter."
 authors = ["Shroominic <pleurae-berets.0u@icloud.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^1.0.0"
 openai = "^0.27.8"
 langchain = "^0.0.232"
-codeboxapi = "^0.0.6"
+codeboxapi = "^0.0.7"
 
 [tool.poetry.extras]
 image_support = ["Pillow"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.0"
 mypy = "^1.4.1"
```

### Comparing `codeinterpreterapi-0.0.3/PKG-INFO` & `codeinterpreterapi-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: codeinterpreterapi
-Version: 0.0.3
+Version: 0.0.4
 Summary: CodeInterpreterAPI is an unofficial and open source python interface for the ChatGPT CodeInterpreter.
 License: MIT
 Author: Shroominic
 Author-email: pleurae-berets.0u@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: image-support
-Requires-Dist: codeboxapi (>=0.0.6,<0.0.7)
+Requires-Dist: codeboxapi (>=0.0.7,<0.0.8)
 Requires-Dist: langchain (>=0.0.232,<0.0.233)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Code Interpreter API
 
@@ -32,18 +32,18 @@
 ```
 
 ## Usage
 
 ```python
 from codeinterpreterapi import CodeInterpreterSession
 
-# start a session
-session = CodeInterpreterSession()
 
 async def main():
+    # start a session
+    session = CodeInterpreterSession()
     await session.astart()
 
     # generate a response based on user input
     output = await session.generate_response(
         "Plot the bitcoin chart of 2023 YTD"
     )
     # show output image in default image viewer
```

