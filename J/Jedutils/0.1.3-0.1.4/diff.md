# Comparing `tmp/Jedutils-0.1.3.tar.gz` & `tmp/Jedutils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jedutils-0.1.3.tar", last modified: Mon Jul 10 15:01:24 2023, max compression
+gzip compressed data, was "Jedutils-0.1.4.tar", last modified: Fri Jul 14 22:26:50 2023, max compression
```

## Comparing `Jedutils-0.1.3.tar` & `Jedutils-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:01:24.729741 Jedutils-0.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:01:24.729741 Jedutils-0.1.3/Jedutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-10 15:01:24.000000 Jedutils-0.1.3/Jedutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-10 15:01:24.000000 Jedutils-0.1.3/Jedutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 15:01:24.000000 Jedutils-0.1.3/Jedutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 15:01:24.000000 Jedutils-0.1.3/Jedutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-10 15:01:17.000000 Jedutils-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 15:01:17.000000 Jedutils-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-10 15:01:24.729741 Jedutils-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-10 15:01:17.000000 Jedutils-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:01:24.729741 Jedutils-0.1.3/jedutils/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-10 15:01:17.000000 Jedutils-0.1.3/jedutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:01:24.729741 Jedutils-0.1.3/jedutils/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-10 15:01:17.000000 Jedutils-0.1.3/jedutils/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-10 15:01:17.000000 Jedutils-0.1.3/jedutils/asyncio/_async_redis_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-10 15:01:17.000000 Jedutils-0.1.3/jedutils/asyncio/_run_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 15:01:24.729741 Jedutils-0.1.3/jedutils/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-10 15:01:17.000000 Jedutils-0.1.3/jedutils/strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-10 15:01:17.000000 Jedutils-0.1.3/jedutils/strings/_random_string.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 15:01:24.729741 Jedutils-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-10 15:01:17.000000 Jedutils-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:26:50.165222 Jedutils-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:26:50.165222 Jedutils-0.1.4/Jedutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-14 22:26:50.000000 Jedutils-0.1.4/Jedutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-14 22:26:50.000000 Jedutils-0.1.4/Jedutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:26:50.000000 Jedutils-0.1.4/Jedutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 22:26:50.000000 Jedutils-0.1.4/Jedutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 22:26:48.000000 Jedutils-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 22:26:48.000000 Jedutils-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-14 22:26:50.165222 Jedutils-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-14 22:26:48.000000 Jedutils-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:26:50.165222 Jedutils-0.1.4/jedutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-14 22:26:48.000000 Jedutils-0.1.4/jedutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:26:50.165222 Jedutils-0.1.4/jedutils/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-14 22:26:48.000000 Jedutils-0.1.4/jedutils/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-14 22:26:48.000000 Jedutils-0.1.4/jedutils/asyncio/_async_redis_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-14 22:26:48.000000 Jedutils-0.1.4/jedutils/asyncio/_run_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:26:50.165222 Jedutils-0.1.4/jedutils/asyncio/network/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 22:26:48.000000 Jedutils-0.1.4/jedutils/asyncio/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-14 22:26:48.000000 Jedutils-0.1.4/jedutils/asyncio/network/_dl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:26:50.165222 Jedutils-0.1.4/jedutils/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-14 22:26:48.000000 Jedutils-0.1.4/jedutils/strings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-14 22:26:48.000000 Jedutils-0.1.4/jedutils/strings/_random_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 22:26:50.165222 Jedutils-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-14 22:26:48.000000 Jedutils-0.1.4/setup.py
```

### Comparing `Jedutils-0.1.3/Jedutils.egg-info/PKG-INFO` & `Jedutils-0.1.4/Jedutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jedutils
-Version: 0.1.3
+Version: 0.1.4
 Summary: Jedutils is a Python utilities package that provides a collection of useful helper functions.
 Home-page: https://github.com/AYMENJD/jedutils
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AYMENJD/jedutils
 Project-URL: Tracker, https://github.com/AYMENJD/jedutils/issues
```

### Comparing `Jedutils-0.1.3/LICENSE` & `Jedutils-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Jedutils-0.1.3/PKG-INFO` & `Jedutils-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jedutils
-Version: 0.1.3
+Version: 0.1.4
 Summary: Jedutils is a Python utilities package that provides a collection of useful helper functions.
 Home-page: https://github.com/AYMENJD/jedutils
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AYMENJD/jedutils
 Project-URL: Tracker, https://github.com/AYMENJD/jedutils/issues
```

### Comparing `Jedutils-0.1.3/README.md` & `Jedutils-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `Jedutils-0.1.3/jedutils/asyncio/_async_redis_pipe.py` & `Jedutils-0.1.4/jedutils/asyncio/_async_redis_pipe.py`

 * *Files identical despite different names*

### Comparing `Jedutils-0.1.3/jedutils/strings/_random_string.py` & `Jedutils-0.1.4/jedutils/strings/_random_string.py`

 * *Files identical despite different names*

### Comparing `Jedutils-0.1.3/setup.py` & `Jedutils-0.1.4/setup.py`

 * *Files identical despite different names*

