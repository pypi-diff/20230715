# Comparing `tmp/bovine_pubsub-0.2.6.tar.gz` & `tmp/bovine_pubsub-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine_pubsub-0.2.6.tar", max compression
+gzip compressed data, was "bovine_pubsub-0.3.0.tar", max compression
```

## Comparing `bovine_pubsub-0.2.6.tar` & `bovine_pubsub-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       68 2023-06-04 18:36:16.378481 bovine_pubsub-0.2.6/README.md
--rw-r--r--   0        0        0      279 2023-06-04 18:36:16.378481 bovine_pubsub-0.2.6/bovine_pubsub/__init__.py
--rw-r--r--   0        0        0      868 2023-06-04 18:36:16.378481 bovine_pubsub-0.2.6/bovine_pubsub/queue.py
--rw-r--r--   0        0        0     1091 2023-06-04 18:36:16.378481 bovine_pubsub-0.2.6/bovine_pubsub/redis.py
--rw-r--r--   0        0        0      258 2023-06-04 18:36:16.378481 bovine_pubsub-0.2.6/bovine_pubsub/test_app.py
--rw-r--r--   0        0        0      632 2023-06-04 18:36:16.378481 bovine_pubsub-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      776 1970-01-01 00:00:00.000000 bovine_pubsub-0.2.6/setup.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 bovine_pubsub-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1390 2023-07-15 11:45:43.763733 bovine_pubsub-0.3.0/README.md
+-rw-r--r--   0        0        0      583 2023-07-15 11:45:43.763733 bovine_pubsub-0.3.0/bovine_pubsub/__init__.py
+-rw-r--r--   0        0        0      868 2023-07-15 11:45:43.763733 bovine_pubsub-0.3.0/bovine_pubsub/queue.py
+-rw-r--r--   0        0        0     1091 2023-07-15 11:45:43.763733 bovine_pubsub-0.3.0/bovine_pubsub/redis.py
+-rw-r--r--   0        0        0     1048 2023-07-15 11:45:43.763733 bovine_pubsub-0.3.0/bovine_pubsub/test_app.py
+-rw-r--r--   0        0        0      690 2023-07-15 11:45:43.763733 bovine_pubsub-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2140 1970-01-01 00:00:00.000000 bovine_pubsub-0.3.0/setup.py
+-rw-r--r--   0        0        0     2017 1970-01-01 00:00:00.000000 bovine_pubsub-0.3.0/PKG-INFO
```

### Comparing `bovine_pubsub-0.2.6/bovine_pubsub/queue.py` & `bovine_pubsub-0.3.0/bovine_pubsub/queue.py`

 * *Files identical despite different names*

### Comparing `bovine_pubsub-0.2.6/bovine_pubsub/redis.py` & `bovine_pubsub-0.3.0/bovine_pubsub/redis.py`

 * *Files identical despite different names*

### Comparing `bovine_pubsub-0.2.6/pyproject.toml` & `bovine_pubsub-0.3.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bovine-pubsub"
-version = "0.2.6"
+version = "0.3.0"
 description = "A Quart Redis thing to handle pubsub tasks in particular the event source"
 authors = ["Helge <helge.krueger@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://codeberg.org/bovine/bovine"
 packages = [{include = "bovine_pubsub"}]
 
@@ -21,7 +21,11 @@
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 ruff = "^0.0.261"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pytest.ini_options]
+asyncio_mode="auto"
+log_cli= 1
```

