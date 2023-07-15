# Comparing `tmp/lkmlfmt-0.0.8.tar.gz` & `tmp/lkmlfmt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lkmlfmt-0.0.8.tar", max compression
+gzip compressed data, was "lkmlfmt-0.0.9.tar", max compression
```

## Comparing `lkmlfmt-0.0.8.tar` & `lkmlfmt-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/LICENSE
--rw-r--r--   0        0        0     2582 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/README.md
--rw-r--r--   0        0        0       53 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/__init__.py
--rw-r--r--   0        0        0       70 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/__main__.py
--rw-r--r--   0        0        0     2738 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/command.py
--rw-r--r--   0        0        0      100 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/exception.py
--rw-r--r--   0        0        0    11592 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/formatter.py
--rw-r--r--   0        0        0      757 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/lkml.lark
--rw-r--r--   0        0        0       64 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/logger.py
--rw-r--r--   0        0        0     2292 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/parser.py
--rw-r--r--   0        0        0        0 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/py.typed
--rw-r--r--   0        0        0     4251 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/template.py
--rw-r--r--   0        0        0      534 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2987 1970-01-01 00:00:00.000000 lkmlfmt-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-15 13:18:12.639182 lkmlfmt-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2582 2023-07-15 13:18:12.639182 lkmlfmt-0.0.9/README.md
+-rw-r--r--   0        0        0       53 2023-07-15 13:18:12.639182 lkmlfmt-0.0.9/lkmlfmt/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-15 13:18:12.639182 lkmlfmt-0.0.9/lkmlfmt/__main__.py
+-rw-r--r--   0        0        0     2738 2023-07-15 13:18:12.639182 lkmlfmt-0.0.9/lkmlfmt/command.py
+-rw-r--r--   0        0        0      100 2023-07-15 13:18:12.639182 lkmlfmt-0.0.9/lkmlfmt/exception.py
+-rw-r--r--   0        0        0    11592 2023-07-15 13:18:12.639182 lkmlfmt-0.0.9/lkmlfmt/formatter.py
+-rw-r--r--   0        0        0      757 2023-07-15 13:18:12.639182 lkmlfmt-0.0.9/lkmlfmt/lkml.lark
+-rw-r--r--   0        0        0       64 2023-07-15 13:18:12.639182 lkmlfmt-0.0.9/lkmlfmt/logger.py
+-rw-r--r--   0        0        0     2292 2023-07-15 13:18:12.639182 lkmlfmt-0.0.9/lkmlfmt/parser.py
+-rw-r--r--   0        0        0        0 2023-07-15 13:18:12.639182 lkmlfmt-0.0.9/lkmlfmt/py.typed
+-rw-r--r--   0        0        0     4251 2023-07-15 13:18:12.639182 lkmlfmt-0.0.9/lkmlfmt/template.py
+-rw-r--r--   0        0        0      534 2023-07-15 13:18:12.639182 lkmlfmt-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2987 1970-01-01 00:00:00.000000 lkmlfmt-0.0.9/PKG-INFO
```

### Comparing `lkmlfmt-0.0.8/LICENSE` & `lkmlfmt-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.8/README.md` & `lkmlfmt-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.8/lkmlfmt/command.py` & `lkmlfmt-0.0.9/lkmlfmt/command.py`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.8/lkmlfmt/formatter.py` & `lkmlfmt-0.0.9/lkmlfmt/formatter.py`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.8/lkmlfmt/lkml.lark` & `lkmlfmt-0.0.9/lkmlfmt/lkml.lark`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.8/lkmlfmt/parser.py` & `lkmlfmt-0.0.9/lkmlfmt/parser.py`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.8/lkmlfmt/template.py` & `lkmlfmt-0.0.9/lkmlfmt/template.py`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.8/pyproject.toml` & `lkmlfmt-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "lkmlfmt"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["dr666m1 <skndr666m1@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 lkmlfmt = "lkmlfmt.command:run"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 lark = "^1.1.5"
 click = "^8.1.3"
-shandy-sqlfmt = "^0.18.1"
+shandy-sqlfmt = "^0.19.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.1"
 isort = "^5.12.0"
```

### Comparing `lkmlfmt-0.0.8/PKG-INFO` & `lkmlfmt-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: lkmlfmt
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: dr666m1
 Author-email: skndr666m1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: lark (>=1.1.5,<2.0.0)
-Requires-Dist: shandy-sqlfmt (>=0.18.1,<0.19.0)
+Requires-Dist: shandy-sqlfmt (>=0.19.1,<0.20.0)
 Description-Content-Type: text/markdown
 
 # lkmlfmt
 lkmlfmt formats your LookML files including embedded SQL and HTML.
 
 ## Installation
 ```sh
```

