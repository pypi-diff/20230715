# Comparing `tmp/omgpt-0.0.2.tar.gz` & `tmp/omgpt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omgpt-0.0.2.tar", max compression
+gzip compressed data, was "omgpt-0.0.3.tar", max compression
```

## Comparing `omgpt-0.0.2.tar` & `omgpt-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-07-12 15:32:14.072394 omgpt-0.0.2/LICENSE
--rw-r--r--   0        0        0    10972 2023-07-14 08:42:38.371494 omgpt-0.0.2/README.md
--rw-r--r--   0        0        0     2778 2023-07-15 02:06:09.514634 omgpt-0.0.2/omgpt.py
--rw-r--r--   0        0        0      590 2023-07-15 02:35:37.783250 omgpt-0.0.2/pyproject.toml
--rw-r--r--   0        0        0    11642 1970-01-01 00:00:00.000000 omgpt-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-12 15:32:14.072394 omgpt-0.0.3/LICENSE
+-rw-r--r--   0        0        0    10972 2023-07-14 08:42:38.371494 omgpt-0.0.3/README.md
+-rw-r--r--   0        0        0     2778 2023-07-15 02:06:09.514634 omgpt-0.0.3/omgpt.py
+-rw-r--r--   0        0        0      598 2023-07-15 02:47:46.706415 omgpt-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0    11640 1970-01-01 00:00:00.000000 omgpt-0.0.3/PKG-INFO
```

### Comparing `omgpt-0.0.2/LICENSE` & `omgpt-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `omgpt-0.0.2/README.md` & `omgpt-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `omgpt-0.0.2/omgpt.py` & `omgpt-0.0.3/omgpt.py`

 * *Files identical despite different names*

### Comparing `omgpt-0.0.2/pyproject.toml` & `omgpt-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "omgpt"
-version = "0.0.2"
+version = "0.0.3"
 description = "An AI-powered command-line interface"
 authors = ["Youngwook Kim <youngwook.kim@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/ywkim/omgpt"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-langchain = "^0.0.205"
+langchain = ">=0.0.205,<0.1.0"
 prompt-toolkit = "^3.0.39"
 openai = "^0.27.8"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
 isort = "^5.12.0"
 pyright = "^1.1.316"
```

### Comparing `omgpt-0.0.2/PKG-INFO` & `omgpt-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: omgpt
-Version: 0.0.2
+Version: 0.0.3
 Summary: An AI-powered command-line interface
 Home-page: https://github.com/ywkim/omgpt
 License: MIT
 Author: Youngwook Kim
 Author-email: youngwook.kim@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: langchain (>=0.0.205,<0.0.206)
+Requires-Dist: langchain (>=0.0.205,<0.1.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: prompt-toolkit (>=3.0.39,<4.0.0)
 Description-Content-Type: text/markdown
 
 # 🐚 OMGpt Shell
 
 ![🎬 Demo](omgpt.gif)
```

