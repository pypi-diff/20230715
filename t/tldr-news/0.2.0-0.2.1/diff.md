# Comparing `tmp/tldr_news-0.2.0.tar.gz` & `tmp/tldr_news-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldr_news-0.2.0.tar", max compression
+gzip compressed data, was "tldr_news-0.2.1.tar", max compression
```

## Comparing `tldr_news-0.2.0.tar` & `tldr_news-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1046 2023-04-01 11:35:47.426329 tldr_news-0.2.0/README.md
--rw-r--r--   0        0        0     1195 2023-04-01 11:36:19.278324 tldr_news-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-01 11:36:19.278324 tldr_news-0.2.0/tldr_news/__init__.py
--rw-r--r--   0        0        0     1081 2023-04-01 11:35:47.434329 tldr_news-0.2.0/tldr_news/cli.py
--rw-r--r--   0        0        0      204 2023-04-01 11:35:47.434329 tldr_news-0.2.0/tldr_news/main.css
--rw-r--r--   0        0        0      698 2023-04-01 11:35:47.434329 tldr_news-0.2.0/tldr_news/ui.py
--rw-r--r--   0        0        0     1873 2023-04-01 11:35:47.434329 tldr_news-0.2.0/tldr_news/utils.py
--rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 tldr_news-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1046 2023-07-15 05:01:12.864621 tldr_news-0.2.1/README.md
+-rw-r--r--   0        0        0     1195 2023-07-15 05:01:39.537379 tldr_news-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-15 05:01:39.537379 tldr_news-0.2.1/tldr_news/__init__.py
+-rw-r--r--   0        0        0     1081 2023-07-15 05:01:12.868622 tldr_news-0.2.1/tldr_news/cli.py
+-rw-r--r--   0        0        0      204 2023-07-15 05:01:12.872622 tldr_news-0.2.1/tldr_news/main.css
+-rw-r--r--   0        0        0      698 2023-07-15 05:01:12.872622 tldr_news-0.2.1/tldr_news/ui.py
+-rw-r--r--   0        0        0     1873 2023-07-15 05:01:12.872622 tldr_news-0.2.1/tldr_news/utils.py
+-rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 tldr_news-0.2.1/PKG-INFO
```

### Comparing `tldr_news-0.2.0/README.md` & `tldr_news-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tldr_news-0.2.0/pyproject.toml` & `tldr_news-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tldr-news"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Harry Tran <huytran.quang080199@gmail.com>"]
 readme = "README.md"
 packages = [{include = "tldr_news"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `tldr_news-0.2.0/tldr_news/cli.py` & `tldr_news-0.2.1/tldr_news/cli.py`

 * *Files identical despite different names*

### Comparing `tldr_news-0.2.0/tldr_news/ui.py` & `tldr_news-0.2.1/tldr_news/ui.py`

 * *Files identical despite different names*

### Comparing `tldr_news-0.2.0/tldr_news/utils.py` & `tldr_news-0.2.1/tldr_news/utils.py`

 * *Files identical despite different names*

### Comparing `tldr_news-0.2.0/PKG-INFO` & `tldr_news-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldr-news
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Harry Tran
 Author-email: huytran.quang080199@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

