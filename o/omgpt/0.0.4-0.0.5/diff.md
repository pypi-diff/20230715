# Comparing `tmp/omgpt-0.0.4.tar.gz` & `tmp/omgpt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omgpt-0.0.4.tar", max compression
+gzip compressed data, was "omgpt-0.0.5.tar", max compression
```

## Comparing `omgpt-0.0.4.tar` & `omgpt-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-07-12 15:32:14.072394 omgpt-0.0.4/LICENSE
--rw-r--r--   0        0        0    10972 2023-07-14 08:42:38.371494 omgpt-0.0.4/README.md
--rw-r--r--   0        0        0     2778 2023-07-15 02:06:09.514634 omgpt-0.0.4/omgpt.py
--rw-r--r--   0        0        0      692 2023-07-15 03:21:45.586134 omgpt-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    11674 1970-01-01 00:00:00.000000 omgpt-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-12 15:32:14.072394 omgpt-0.0.5/LICENSE
+-rw-r--r--   0        0        0    10972 2023-07-14 08:42:38.371494 omgpt-0.0.5/README.md
+-rw-r--r--   0        0        0     2778 2023-07-15 02:06:09.514634 omgpt-0.0.5/omgpt.py
+-rw-r--r--   0        0        0      677 2023-07-15 03:33:02.538529 omgpt-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    11674 1970-01-01 00:00:00.000000 omgpt-0.0.5/PKG-INFO
```

### Comparing `omgpt-0.0.4/LICENSE` & `omgpt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `omgpt-0.0.4/README.md` & `omgpt-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `omgpt-0.0.4/omgpt.py` & `omgpt-0.0.5/omgpt.py`

 * *Files identical despite different names*

### Comparing `omgpt-0.0.4/pyproject.toml` & `omgpt-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omgpt"
-version = "0.0.4"
+version = "0.0.5"
 description = "Simplify and enhance your command-line experience with the power of AI"
 authors = ["Youngwook Kim <youngwook.kim@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/ywkim/omgpt"
 license = "MIT"
 
 [tool.poetry.dependencies]
@@ -23,8 +23,8 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 omgpt = "omgpt:main"
-test = "pytest"
+
```

### Comparing `omgpt-0.0.4/PKG-INFO` & `omgpt-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omgpt
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simplify and enhance your command-line experience with the power of AI
 Home-page: https://github.com/ywkim/omgpt
 License: MIT
 Author: Youngwook Kim
 Author-email: youngwook.kim@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

