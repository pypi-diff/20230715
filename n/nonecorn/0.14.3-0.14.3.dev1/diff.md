# Comparing `tmp/nonecorn-0.14.3.tar.gz` & `tmp/nonecorn-0.14.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonecorn-0.14.3.tar", last modified: Sat Jul 15 13:12:40 2023, max compression
+gzip compressed data, was "nonecorn-0.14.3.dev1.tar", last modified: Wed May 24 10:08:42 2023, max compression
```

## Comparing `nonecorn-0.14.3.tar` & `nonecorn-0.14.3.dev1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 13:12:40.672516 nonecorn-0.14.3/
--rw-rw-rw-   0        0        0     1072 2023-03-10 03:15:15.000000 nonecorn-0.14.3/LICENSE
--rw-rw-rw-   0        0        0       30 2023-05-24 06:47:35.000000 nonecorn-0.14.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4926 2023-07-15 13:12:40.672516 nonecorn-0.14.3/PKG-INFO
--rw-rw-rw-   0        0        0     3798 2023-05-24 06:47:35.000000 nonecorn-0.14.3/README.rst
--rw-rw-rw-   0        0        0     3073 2023-07-15 13:11:07.000000 nonecorn-0.14.3/pyproject.toml
--rw-rw-rw-   0        0        0      156 2023-07-15 13:12:40.673517 nonecorn-0.14.3/setup.cfg
--rw-rw-rw-   0        0        0     2195 2023-07-15 13:12:20.000000 nonecorn-0.14.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:12:40.633493 nonecorn-0.14.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-15 13:12:40.647496 nonecorn-0.14.3/src/hypercorn/
--rw-rw-rw-   0        0        0       91 2023-03-10 03:15:15.000000 nonecorn-0.14.3/src/hypercorn/__init__.py
--rw-rw-rw-   0        0        0    10631 2023-03-10 03:15:15.000000 nonecorn-0.14.3/src/hypercorn/__main__.py
--rw-rw-rw-   0        0        0     5159 2023-07-08 14:46:18.000000 nonecorn-0.14.3/src/hypercorn/app_wrappers.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:12:40.653496 nonecorn-0.14.3/src/hypercorn/asyncio/
--rw-rw-rw-   0        0        0     1607 2023-03-10 03:15:15.000000 nonecorn-0.14.3/src/hypercorn/asyncio/__init__.py
--rw-rw-rw-   0        0        0     4069 2023-05-24 05:53:19.000000 nonecorn-0.14.3/src/hypercorn/asyncio/lifespan.py
--rw-rw-rw-   0        0        0     9160 2023-05-24 05:53:19.000000 nonecorn-0.14.3/src/hypercorn/asyncio/run.py
--rw-rw-rw-   0        0        0      795 2023-03-10 03:15:15.000000 nonecorn-0.14.3/src/hypercorn/asyncio/statsd.py
--rw-rw-rw-   0        0        0     2636 2023-03-10 03:15:15.000000 nonecorn-0.14.3/src/hypercorn/asyncio/task_group.py
--rw-rw-rw-   0        0        0     6378 2023-07-08 16:37:15.000000 nonecorn-0.14.3/src/hypercorn/asyncio/tcp_server.py
--rw-rw-rw-   0        0        0     3139 2023-05-24 06:47:35.000000 nonecorn-0.14.3/src/hypercorn/asyncio/udp_server.py
--rw-rw-rw-   0        0        0      849 2023-03-10 03:15:15.000000 nonecorn-0.14.3/src/hypercorn/asyncio/worker_context.py
--rw-rw-rw-   0        0        0    14132 2023-07-15 13:10:12.000000 nonecorn-0.14.3/src/hypercorn/config.py
--rw-rw-rw-   0        0        0      557 2023-05-24 06:47:35.000000 nonecorn-0.14.3/src/hypercorn/events.py
--rw-rw-rw-   0        0        0     7397 2023-03-10 03:15:16.000000 nonecorn-0.14.3/src/hypercorn/logging.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:12:40.656497 nonecorn-0.14.3/src/hypercorn/middleware/
--rw-rw-rw-   0        0        0      345 2023-03-10 03:15:16.000000 nonecorn-0.14.3/src/hypercorn/middleware/__init__.py
--rw-rw-rw-   0        0        0     4414 2023-03-10 03:15:16.000000 nonecorn-0.14.3/src/hypercorn/middleware/dispatcher.py
--rw-rw-rw-   0        0        0     2686 2023-03-10 03:15:16.000000 nonecorn-0.14.3/src/hypercorn/middleware/http_to_https.py
--rw-rw-rw-   0        0        0     1538 2023-03-10 03:15:16.000000 nonecorn-0.14.3/src/hypercorn/middleware/wsgi.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:12:40.661514 nonecorn-0.14.3/src/hypercorn/protocol/
--rw-rw-rw-   0        0        0     3235 2023-05-24 06:47:35.000000 nonecorn-0.14.3/src/hypercorn/protocol/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-05-24 06:47:35.000000 nonecorn-0.14.3/src/hypercorn/protocol/events.py
--rw-rw-rw-   0        0        0    13477 2023-07-15 13:10:12.000000 nonecorn-0.14.3/src/hypercorn/protocol/h11.py
--rw-rw-rw-   0        0        0    16826 2023-05-24 06:47:35.000000 nonecorn-0.14.3/src/hypercorn/protocol/h2.py
--rw-rw-rw-   0        0        0     6082 2023-05-24 06:47:35.000000 nonecorn-0.14.3/src/hypercorn/protocol/h3.py
--rw-rw-rw-   0        0        0    12426 2023-07-08 16:37:15.000000 nonecorn-0.14.3/src/hypercorn/protocol/http_stream.py
--rw-rw-rw-   0        0        0     5346 2023-05-24 05:53:19.000000 nonecorn-0.14.3/src/hypercorn/protocol/quic.py
--rw-rw-rw-   0        0        0    16021 2023-07-08 14:46:18.000000 nonecorn-0.14.3/src/hypercorn/protocol/ws_stream.py
--rw-rw-rw-   0        0        0        8 2023-03-10 03:15:16.000000 nonecorn-0.14.3/src/hypercorn/py.typed
--rw-rw-rw-   0        0        0     3454 2023-05-24 06:47:35.000000 nonecorn-0.14.3/src/hypercorn/run.py
--rw-rw-rw-   0        0        0     3927 2023-03-10 03:15:16.000000 nonecorn-0.14.3/src/hypercorn/statsd.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:12:40.667515 nonecorn-0.14.3/src/hypercorn/trio/
--rw-rw-rw-   0        0        0     1722 2023-03-10 03:15:16.000000 nonecorn-0.14.3/src/hypercorn/trio/__init__.py
--rw-rw-rw-   0        0        0     3726 2023-05-24 05:53:19.000000 nonecorn-0.14.3/src/hypercorn/trio/lifespan.py
--rw-rw-rw-   0        0        0     4834 2023-07-08 16:37:15.000000 nonecorn-0.14.3/src/hypercorn/trio/run.py
--rw-rw-rw-   0        0        0      509 2023-03-10 03:15:16.000000 nonecorn-0.14.3/src/hypercorn/trio/statsd.py
--rw-rw-rw-   0        0        0     2503 2023-07-08 16:37:15.000000 nonecorn-0.14.3/src/hypercorn/trio/task_group.py
--rw-rw-rw-   0        0        0     5326 2023-07-15 13:10:12.000000 nonecorn-0.14.3/src/hypercorn/trio/tcp_server.py
--rw-rw-rw-   0        0        0     1678 2023-05-24 05:53:19.000000 nonecorn-0.14.3/src/hypercorn/trio/udp_server.py
--rw-rw-rw-   0        0        0      837 2023-03-10 03:15:16.000000 nonecorn-0.14.3/src/hypercorn/trio/worker_context.py
--rw-rw-rw-   0        0        0     8138 2023-05-24 06:47:35.000000 nonecorn-0.14.3/src/hypercorn/typing.py
--rw-rw-rw-   0        0        0     9813 2023-05-24 06:47:35.000000 nonecorn-0.14.3/src/hypercorn/utils.py
--rw-rw-rw-   0        0        0     6305 2023-05-24 06:47:35.000000 nonecorn-0.14.3/src/hypercorn/workers.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:12:40.671516 nonecorn-0.14.3/src/nonecorn.egg-info/
--rw-rw-rw-   0        0        0     4926 2023-07-15 13:12:40.000000 nonecorn-0.14.3/src/nonecorn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1519 2023-07-15 13:12:40.000000 nonecorn-0.14.3/src/nonecorn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 13:12:40.000000 nonecorn-0.14.3/src/nonecorn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-07-15 13:12:40.000000 nonecorn-0.14.3/src/nonecorn.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      235 2023-07-15 13:12:40.000000 nonecorn-0.14.3/src/nonecorn.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-15 13:12:40.000000 nonecorn-0.14.3/src/nonecorn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 10:08:42.313403 nonecorn-0.14.3.dev1/
+-rw-rw-rw-   0        0        0     1072 2023-03-10 03:15:15.000000 nonecorn-0.14.3.dev1/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4879 2023-05-24 10:08:42.313914 nonecorn-0.14.3.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     3798 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/README.rst
+-rw-rw-rw-   0        0        0     2934 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/pyproject.toml
+-rw-rw-rw-   0        0        0      156 2023-05-24 10:08:42.314293 nonecorn-0.14.3.dev1/setup.cfg
+-rw-rw-rw-   0        0        0     2148 2023-05-24 10:08:28.000000 nonecorn-0.14.3.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:08:42.264329 nonecorn-0.14.3.dev1/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 10:08:42.280967 nonecorn-0.14.3.dev1/src/hypercorn/
+-rw-rw-rw-   0        0        0       91 2023-03-10 03:15:15.000000 nonecorn-0.14.3.dev1/src/hypercorn/__init__.py
+-rw-rw-rw-   0        0        0    10631 2023-03-10 03:15:15.000000 nonecorn-0.14.3.dev1/src/hypercorn/__main__.py
+-rw-rw-rw-   0        0        0     5262 2023-03-10 03:15:15.000000 nonecorn-0.14.3.dev1/src/hypercorn/app_wrappers.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:08:42.288621 nonecorn-0.14.3.dev1/src/hypercorn/asyncio/
+-rw-rw-rw-   0        0        0     1607 2023-03-10 03:15:15.000000 nonecorn-0.14.3.dev1/src/hypercorn/asyncio/__init__.py
+-rw-rw-rw-   0        0        0     4069 2023-05-24 05:53:19.000000 nonecorn-0.14.3.dev1/src/hypercorn/asyncio/lifespan.py
+-rw-rw-rw-   0        0        0     9160 2023-05-24 05:53:19.000000 nonecorn-0.14.3.dev1/src/hypercorn/asyncio/run.py
+-rw-rw-rw-   0        0        0      795 2023-03-10 03:15:15.000000 nonecorn-0.14.3.dev1/src/hypercorn/asyncio/statsd.py
+-rw-rw-rw-   0        0        0     2636 2023-03-10 03:15:15.000000 nonecorn-0.14.3.dev1/src/hypercorn/asyncio/task_group.py
+-rw-rw-rw-   0        0        0     6360 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/asyncio/tcp_server.py
+-rw-rw-rw-   0        0        0     3139 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/asyncio/udp_server.py
+-rw-rw-rw-   0        0        0      849 2023-03-10 03:15:15.000000 nonecorn-0.14.3.dev1/src/hypercorn/asyncio/worker_context.py
+-rw-rw-rw-   0        0        0    14098 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/config.py
+-rw-rw-rw-   0        0        0      557 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/events.py
+-rw-rw-rw-   0        0        0     7397 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/logging.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:08:42.292166 nonecorn-0.14.3.dev1/src/hypercorn/middleware/
+-rw-rw-rw-   0        0        0      345 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/middleware/__init__.py
+-rw-rw-rw-   0        0        0     4414 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/middleware/dispatcher.py
+-rw-rw-rw-   0        0        0     2686 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/middleware/http_to_https.py
+-rw-rw-rw-   0        0        0     1538 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/middleware/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:08:42.299716 nonecorn-0.14.3.dev1/src/hypercorn/protocol/
+-rw-rw-rw-   0        0        0     3235 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/protocol/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/protocol/events.py
+-rw-rw-rw-   0        0        0    13330 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/protocol/h11.py
+-rw-rw-rw-   0        0        0    16826 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/protocol/h2.py
+-rw-rw-rw-   0        0        0     6082 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/protocol/h3.py
+-rw-rw-rw-   0        0        0    12487 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/protocol/http_stream.py
+-rw-rw-rw-   0        0        0     5346 2023-05-24 05:53:19.000000 nonecorn-0.14.3.dev1/src/hypercorn/protocol/quic.py
+-rw-rw-rw-   0        0        0    16039 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/protocol/ws_stream.py
+-rw-rw-rw-   0        0        0        8 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/py.typed
+-rw-rw-rw-   0        0        0     3454 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/run.py
+-rw-rw-rw-   0        0        0     3927 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/statsd.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:08:42.306961 nonecorn-0.14.3.dev1/src/hypercorn/trio/
+-rw-rw-rw-   0        0        0     1722 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/trio/__init__.py
+-rw-rw-rw-   0        0        0     3726 2023-05-24 05:53:19.000000 nonecorn-0.14.3.dev1/src/hypercorn/trio/lifespan.py
+-rw-rw-rw-   0        0        0     4569 2023-05-24 06:47:42.000000 nonecorn-0.14.3.dev1/src/hypercorn/trio/run.py
+-rw-rw-rw-   0        0        0      509 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/trio/statsd.py
+-rw-rw-rw-   0        0        0     2485 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/trio/task_group.py
+-rw-rw-rw-   0        0        0     5267 2023-05-24 05:53:19.000000 nonecorn-0.14.3.dev1/src/hypercorn/trio/tcp_server.py
+-rw-rw-rw-   0        0        0     1678 2023-05-24 05:53:19.000000 nonecorn-0.14.3.dev1/src/hypercorn/trio/udp_server.py
+-rw-rw-rw-   0        0        0      837 2023-03-10 03:15:16.000000 nonecorn-0.14.3.dev1/src/hypercorn/trio/worker_context.py
+-rw-rw-rw-   0        0        0     8138 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/typing.py
+-rw-rw-rw-   0        0        0     9813 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/utils.py
+-rw-rw-rw-   0        0        0     6305 2023-05-24 06:47:35.000000 nonecorn-0.14.3.dev1/src/hypercorn/workers.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:08:42.312510 nonecorn-0.14.3.dev1/src/nonecorn.egg-info/
+-rw-rw-rw-   0        0        0     4879 2023-05-24 10:08:42.000000 nonecorn-0.14.3.dev1/src/nonecorn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1519 2023-05-24 10:08:42.000000 nonecorn-0.14.3.dev1/src/nonecorn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 10:08:42.000000 nonecorn-0.14.3.dev1/src/nonecorn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-24 10:08:42.000000 nonecorn-0.14.3.dev1/src/nonecorn.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      235 2023-05-24 10:08:42.000000 nonecorn-0.14.3.dev1/src/nonecorn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-24 10:08:42.000000 nonecorn-0.14.3.dev1/src/nonecorn.egg-info/top_level.txt
```

### Comparing `nonecorn-0.14.3/LICENSE` & `nonecorn-0.14.3.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/PKG-INFO` & `nonecorn-0.14.3.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonecorn
-Version: 0.14.3
+Version: 0.14.3.dev1
 Summary: A ASGI Server forked from hypercorn with more extra feature beyond ASGI
 Home-page: https://gitlab.com/pgjones/hypercorn/
 Author: P G Jones
 Author-email: philip.graham.jones@googlemail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -13,15 +13,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Provides-Extra: h3
 Provides-Extra: tests
 Provides-Extra: trio
 Provides-Extra: uvloop
```

### Comparing `nonecorn-0.14.3/README.rst` & `nonecorn-0.14.3.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/pyproject.toml` & `nonecorn-0.14.3.dev1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 [tool.poetry]
 name = "nonecorn"
-version = "0.14.3"
+version = "0.14.3dev1"
 description = "A ASGI Server based on Hyper libraries and inspired by Gunicorn"
 authors = ["pgjones <philip.graham.jones@googlemail.com>"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = ["src/hypercorn/py.typed"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/pgjones/hypercorn/"
 documentation = "https://hypercorn.readthedocs.io"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 aioquic = { version = ">= 0.9.0, < 1.0", optional = true }
-exceptiongroup = { version = ">= 1.1.0", python = "<3.11", optional = true }
 h11 = "*"
 h2 = ">=3.1.0"
 priority = "*"
 pydata_sphinx_theme = { version = "*", optional = true }
 tomli = { version = "*", python = "<3.11" }
-trio = { version = ">=0.22.0", optional = true }
+trio = { version = ">=0.11.0", optional = true }
 typing_extensions = { version = ">=3.7.4", python = "<3.8" }
 uvloop = { version = "*", markers = "platform_system != 'Windows'", optional = true }
 wsproto = ">=0.14.0"
 
 [tool.poetry.dev-dependencies]
 hypothesis = "*"
 mock = "*"
@@ -49,15 +47,15 @@
 
 [tool.poetry.scripts]
 hypercorn = "hypercorn.__main__:main"
 
 [tool.poetry.extras]
 docs = ["pydata_sphinx_theme"]
 h3 = ["aioquic"]
-trio = ["exceptiongroup", "trio"]
+trio = ["trio"]
 uvloop = ["uvloop"]
 
 [tool.black]
 line-length = 100
 target-version = ["py37"]
 
 [tool.isort]
```

### Comparing `nonecorn-0.14.3/setup.py` & `nonecorn-0.14.3.dev1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "pytest-cov",
     "pytest-trio",
     "trio",
 ]
 
 setup(
     name="nonecorn",
-    version="0.14.3",
+    version="0.14.3dev1",
     python_requires=">=3.7",
     description="A ASGI Server forked from hypercorn with more extra feature beyond ASGI",
     long_description=long_description,
     url="https://gitlab.com/pgjones/hypercorn/",
     author="P G Jones",
     author_email="philip.graham.jones@googlemail.com",
     license="MIT",
@@ -48,15 +48,14 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
         "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     packages=find_packages("src"),
     package_dir={"": "src"},
     py_modules=["hypercorn"],
     install_requires=INSTALL_REQUIRES,
```

### Comparing `nonecorn-0.14.3/src/hypercorn/__main__.py` & `nonecorn-0.14.3.dev1/src/hypercorn/__main__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/app_wrappers.py` & `nonecorn-0.14.3.dev1/src/hypercorn/app_wrappers.py`

 * *Files 15% similar despite different names*

```diff
@@ -64,27 +64,27 @@
         call_soon: Callable,
     ) -> None:
         body = bytearray()
         while True:
             message = await receive()
             body.extend(message.get("body", b""))  # type: ignore
             if len(body) > self.max_body_size:
-                await send({"type": "http.response.start", "status": 400, "headers": []})
-                await send({"type": "http.response.body", "body": b"", "more_body": False})
+                await send({"type": "http.response.start", "status": 400, "headers": []})  # type: ignore # noqa: E501
+                await send({"type": "http.response.body", "body": b"", "more_body": False})  # type: ignore # noqa: E501
                 return
             if not message.get("more_body"):
                 break
 
         try:
             environ = _build_environ(scope, body)
         except InvalidPathError:
-            await send({"type": "http.response.start", "status": 404, "headers": []})
+            await send({"type": "http.response.start", "status": 404, "headers": []})  # type: ignore # noqa: E501
         else:
             await sync_spawn(self.run_app, environ, partial(call_soon, send))
-        await send({"type": "http.response.body", "body": b"", "more_body": False})
+        await send({"type": "http.response.body", "body": b"", "more_body": False})  # type: ignore
 
     def run_app(self, environ: dict, send: Callable) -> None:
         headers: List[Tuple[bytes, bytes]]
         status_code: Optional[int] = None
 
         def start_response(
             status: str,
```

### Comparing `nonecorn-0.14.3/src/hypercorn/asyncio/__init__.py` & `nonecorn-0.14.3.dev1/src/hypercorn/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/asyncio/lifespan.py` & `nonecorn-0.14.3.dev1/src/hypercorn/asyncio/lifespan.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/asyncio/run.py` & `nonecorn-0.14.3.dev1/src/hypercorn/asyncio/run.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/asyncio/statsd.py` & `nonecorn-0.14.3.dev1/src/hypercorn/asyncio/statsd.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/asyncio/task_group.py` & `nonecorn-0.14.3.dev1/src/hypercorn/asyncio/task_group.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/asyncio/tcp_server.py` & `nonecorn-0.14.3.dev1/src/hypercorn/asyncio/tcp_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,30 +130,29 @@
             except (
                 ConnectionError,
                 OSError,
                 asyncio.TimeoutError,
                 TimeoutError,
                 SSLError,
             ):
+                await self.protocol.handle(Closed())
                 break
             else:
                 await self.protocol.handle(RawData(data))
 
-        await self.protocol.handle(Closed())
-
     async def _close(self) -> None:
         try:
             self.writer.write_eof()
         except (NotImplementedError, OSError, RuntimeError):
             pass  # Likely SSL connection
 
         try:
             self.writer.close()
             await self.writer.wait_closed()
-        except (BrokenPipeError, ConnectionAbortedError, ConnectionResetError, RuntimeError):
+        except (BrokenPipeError, ConnectionResetError, RuntimeError):
             pass  # Already closed
 
         await self._stop_idle()
 
     async def _initiate_server_close(self) -> None:
         await self.protocol.handle(Closed())
         self.writer.close()
```

### Comparing `nonecorn-0.14.3/src/hypercorn/asyncio/udp_server.py` & `nonecorn-0.14.3.dev1/src/hypercorn/asyncio/udp_server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/asyncio/worker_context.py` & `nonecorn-0.14.3.dev1/src/hypercorn/asyncio/worker_context.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/config.py` & `nonecorn-0.14.3.dev1/src/hypercorn/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,14 @@
     debug = False
     dogstatsd_tags = ""
     errorlog: Union[logging.Logger, str, None] = "-"
     graceful_timeout: float = 3 * SECONDS
     read_timeout: Optional[int] = None
     group: Optional[int] = None
     h11_max_incomplete_size = 16 * 1024 * BYTES
-    h11_pass_raw_headers = False
     h2_max_concurrent_streams = 100
     h2_max_header_list_size = 2**16
     h2_max_inbound_frame_size = 2**14 * OCTETS
     include_date_header = True
     include_server_header = True
     keep_alive_timeout = 5 * SECONDS
     keyfile: Optional[str] = None
```

### Comparing `nonecorn-0.14.3/src/hypercorn/events.py` & `nonecorn-0.14.3.dev1/src/hypercorn/events.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/logging.py` & `nonecorn-0.14.3.dev1/src/hypercorn/logging.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/middleware/dispatcher.py` & `nonecorn-0.14.3.dev1/src/hypercorn/middleware/dispatcher.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/middleware/http_to_https.py` & `nonecorn-0.14.3.dev1/src/hypercorn/middleware/http_to_https.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/middleware/wsgi.py` & `nonecorn-0.14.3.dev1/src/hypercorn/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/protocol/__init__.py` & `nonecorn-0.14.3.dev1/src/hypercorn/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/protocol/events.py` & `nonecorn-0.14.3.dev1/src/hypercorn/protocol/events.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/protocol/h11.py` & `nonecorn-0.14.3.dev1/src/hypercorn/protocol/h11.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,24 +256,18 @@
                 self.client,
                 self.server,
                 self.stream_send,
                 STREAM_ID,
                 self.tls,
                 self.app_state
             )
-
-        if self.config.h11_pass_raw_headers:
-            headers = request.headers.raw_items()
-        else:
-            headers = list(request.headers)
-
         await self.stream.handle(
             Request(
                 stream_id=STREAM_ID,
-                headers=headers,
+                headers=list(request.headers),
                 http_version=request.http_version.decode(),
                 method=request.method.decode("ascii").upper(),
                 raw_path=request.target,
             )
         )
 
     async def _send_h11_event(self, event: H11SendableEvent) -> None:
```

### Comparing `nonecorn-0.14.3/src/hypercorn/protocol/h2.py` & `nonecorn-0.14.3.dev1/src/hypercorn/protocol/h2.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/protocol/h3.py` & `nonecorn-0.14.3.dev1/src/hypercorn/protocol/h3.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/protocol/http_stream.py` & `nonecorn-0.14.3.dev1/src/hypercorn/protocol/http_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,23 +133,26 @@
                 {"type": "http.request", "body": bytes(event.data), "more_body": True}
             )
         elif isinstance(event, EndBody):
             await self.app_put({"type": "http.request", "body": b"", "more_body": False})
         elif isinstance(event, StreamClosed):
             self.closed = True
             if self.app_put is not None:
-                await self.app_put({"type": "http.disconnect"})
+                await self.app_put({"type": "http.disconnect"})  # type: ignore
 
     async def app_send(self, message: Optional[ASGISendEvent]) -> None:
+        if self.closed:
+            # Allow app to finish after close
+            return
+
         if message is None:  # ASGI App has finished sending messages
-            if not self.closed:
-                # Cleanup if required
-                if self.state == ASGIHTTPState.REQUEST:
-                    await self._send_error_response(500)
-                await self.send(StreamClosed(stream_id=self.stream_id))
+            # Cleanup if required
+            if self.state == ASGIHTTPState.REQUEST:
+                await self._send_error_response(500)
+            await self.send(StreamClosed(stream_id=self.stream_id))
         else:
             if message["type"] == "http.response.start" and self.state == ASGIHTTPState.REQUEST:
                 self.response = message
                 self.trailers_expected = message.get("trailers", False)
             elif (
                 message["type"] == "http.response.push"
                 and self.scope["http_version"] in PUSH_VERSIONS
```

### Comparing `nonecorn-0.14.3/src/hypercorn/protocol/quic.py` & `nonecorn-0.14.3.dev1/src/hypercorn/protocol/quic.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/protocol/ws_stream.py` & `nonecorn-0.14.3.dev1/src/hypercorn/protocol/ws_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
             elif not self.handshake.is_valid():
                 await self._send_error_response(400)
                 self.closed = True
             else:
                 self.app_put = await self.task_group.spawn_app(
                     self.app, self.config, self.scope, self.app_send
                 )
-                await self.app_put({"type": "websocket.connect"})
+                await self.app_put({"type": "websocket.connect"})  # type: ignore
         elif isinstance(event, (Body, Data)):
             self.connection.receive_data(event.data)
             await self._handle_events()
         elif isinstance(event, StreamClosed):
             self.closed = True
             if self.app_put is not None:
                 if self.state in {ASGIWebsocketState.HTTPCLOSED, ASGIWebsocketState.CLOSED}:
@@ -260,15 +260,15 @@
             # Cleanup if required
             if self.state == ASGIWebsocketState.HANDSHAKE:
                 await self._send_error_response(500)
                 await self.config.log.access(
                     self.scope, {"status": 500, "headers": []}, time() - self.start_time
                 )
             elif self.state == ASGIWebsocketState.CONNECTED:
-                await self._send_wsproto_event(CloseConnection(code=CloseReason.INTERNAL_ERROR))
+                await self._send_wsproto_event(CloseConnection(code=CloseReason.ABNORMAL_CLOSURE))
             await self.send(StreamClosed(stream_id=self.stream_id))
         else:
             if message["type"] == "websocket.accept" and self.state == ASGIWebsocketState.HANDSHAKE:
                 await self._accept(message)
             elif (
                 message["type"] == "websocket.http.response.start"
                 and self.state == ASGIWebsocketState.HANDSHAKE
```

### Comparing `nonecorn-0.14.3/src/hypercorn/run.py` & `nonecorn-0.14.3.dev1/src/hypercorn/run.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/statsd.py` & `nonecorn-0.14.3.dev1/src/hypercorn/statsd.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/trio/__init__.py` & `nonecorn-0.14.3.dev1/src/hypercorn/trio/__init__.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/trio/lifespan.py` & `nonecorn-0.14.3.dev1/src/hypercorn/trio/lifespan.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/trio/run.py` & `nonecorn-0.14.3.dev1/src/hypercorn/trio/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import sys
 from functools import partial
 from multiprocessing.synchronize import Event as EventType
 from typing import Awaitable, Callable, Optional
 
 import trio
 
 from .lifespan import Lifespan
@@ -18,17 +17,14 @@
     check_multiprocess_shutdown_event,
     load_application,
     raise_shutdown,
     repr_socket_addr,
     ShutdownError,
 )
 
-if sys.version_info < (3, 11):
-    from exceptiongroup import BaseExceptionGroup
-
 
 async def worker_serve(
     app: AppWrapper,
     config: Config,
     *,
     sockets: Optional[Sockets] = None,
     shutdown_trigger: Optional[Callable[..., Awaitable[None]]] = None,
@@ -75,32 +71,30 @@
             for sock in sockets.quic_sockets:
                 await server_nursery.start(UDPServer(app, config, context, sock, lifespan.state.copy()).run)
                 bind = repr_socket_addr(sock.family, sock.getsockname())
                 await config.log.info(f"Running on https://{bind} (QUIC) (CTRL + C to quit)")
 
             task_status.started(binds)
             try:
-                async with trio.open_nursery(strict_exception_groups=True) as nursery:
+                async with trio.open_nursery() as nursery:
                     if shutdown_trigger is not None:
                         nursery.start_soon(raise_shutdown, shutdown_trigger)
 
                     nursery.start_soon(
                         partial(
                             trio.serve_listeners,
                             partial(TCPServer, app, config, context, app_state=lifespan.state.copy()),
                             listeners,
                             handler_nursery=server_nursery,
                         ),
                     )
 
                     await trio.sleep_forever()
-            except BaseExceptionGroup as error:
-                _, other_errors = error.split((ShutdownError, KeyboardInterrupt))
-                if other_errors is not None:
-                    raise other_errors
+            except (ShutdownError, KeyboardInterrupt):
+                pass
             finally:
                 await context.terminated.set()
                 server_nursery.cancel_scope.deadline = trio.current_time() + config.graceful_timeout
 
         await lifespan.wait_for_shutdown()
         lifespan_nursery.cancel_scope.cancel()
```

### Comparing `nonecorn-0.14.3/src/hypercorn/trio/task_group.py` & `nonecorn-0.14.3.dev1/src/hypercorn/trio/task_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 from __future__ import annotations
 
-import sys
 from types import TracebackType
 from typing import Any, Awaitable, Callable, Optional
 
 import trio
 
 from ..config import Config
 from ..typing import AppWrapper, ASGIReceiveCallable, ASGIReceiveEvent, ASGISendEvent, Scope
 
-if sys.version_info < (3, 11):
-    from exceptiongroup import BaseExceptionGroup
-
 
 async def _handle(
     app: AppWrapper,
     config: Config,
     scope: Scope,
     receive: ASGIReceiveCallable,
     send: Callable[[Optional[ASGISendEvent]], Awaitable[None]],
     sync_spawn: Callable,
     call_soon: Callable,
 ) -> None:
     try:
         await app(scope, receive, send, sync_spawn, call_soon)
     except trio.Cancelled:
         raise
-    except BaseExceptionGroup as error:
-        _, other_errors = error.split(trio.Cancelled)
-        if other_errors is not None:
+    except trio.MultiError as error:
+        errors = trio.MultiError.filter(
+            lambda exc: None if isinstance(exc, trio.Cancelled) else exc, root_exc=error
+        )
+        if errors is not None:
             await config.log.exception("Error in ASGI Framework")
             await send(None)
         else:
             raise
     except Exception:
         await config.log.exception("Error in ASGI Framework")
     finally:
```

### Comparing `nonecorn-0.14.3/src/hypercorn/trio/tcp_server.py` & `nonecorn-0.14.3.dev1/src/hypercorn/trio/tcp_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
                     self.protocol_send,
                     alpn_protocol,
                     self.app_state
                 )
                 await self.protocol.initiate()
                 await self._start_idle()
                 await self._read_data()
-        except OSError:
+        except (trio.MultiError, OSError):
             pass
         finally:
             await self._close()
 
     async def protocol_send(self, event: Event) -> None:
         if isinstance(event, RawData):
             async with self.send_lock:
@@ -94,25 +94,21 @@
                 await self._stop_idle()
 
     async def _read_data(self) -> None:
         while True:
             try:
                 with trio.fail_after(self.config.read_timeout or inf):
                     data = await self.stream.receive_some(MAX_RECV)
-            except (
-                trio.ClosedResourceError,
-                trio.BrokenResourceError,
-                trio.TooSlowError,
-            ):
+            except (trio.ClosedResourceError, trio.BrokenResourceError):
+                await self.protocol.handle(Closed())
                 break
             else:
                 await self.protocol.handle(RawData(data))
                 if data == b"":
                     break
-        await self.protocol.handle(Closed())
 
     async def _close(self) -> None:
         try:
             await self.stream.send_eof()
         except (
             trio.BrokenResourceError,
             AttributeError,
```

### Comparing `nonecorn-0.14.3/src/hypercorn/trio/udp_server.py` & `nonecorn-0.14.3.dev1/src/hypercorn/trio/udp_server.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/trio/worker_context.py` & `nonecorn-0.14.3.dev1/src/hypercorn/trio/worker_context.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/typing.py` & `nonecorn-0.14.3.dev1/src/hypercorn/typing.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/utils.py` & `nonecorn-0.14.3.dev1/src/hypercorn/utils.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/hypercorn/workers.py` & `nonecorn-0.14.3.dev1/src/hypercorn/workers.py`

 * *Files identical despite different names*

### Comparing `nonecorn-0.14.3/src/nonecorn.egg-info/PKG-INFO` & `nonecorn-0.14.3.dev1/src/nonecorn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonecorn
-Version: 0.14.3
+Version: 0.14.3.dev1
 Summary: A ASGI Server forked from hypercorn with more extra feature beyond ASGI
 Home-page: https://gitlab.com/pgjones/hypercorn/
 Author: P G Jones
 Author-email: philip.graham.jones@googlemail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -13,15 +13,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Provides-Extra: h3
 Provides-Extra: tests
 Provides-Extra: trio
 Provides-Extra: uvloop
```

### Comparing `nonecorn-0.14.3/src/nonecorn.egg-info/SOURCES.txt` & `nonecorn-0.14.3.dev1/src/nonecorn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

