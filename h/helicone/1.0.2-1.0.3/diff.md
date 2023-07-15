# Comparing `tmp/helicone-1.0.2.tar.gz` & `tmp/helicone-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helicone-1.0.2.tar", max compression
+gzip compressed data, was "helicone-1.0.3.tar", max compression
```

## Comparing `helicone-1.0.2.tar` & `helicone-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    11341 2023-07-03 21:17:48.000658 helicone-1.0.2/LICENSE
--rw-r--r--   0        0        0        1 2023-07-10 04:44:07.860264 helicone-1.0.2/helicone/async_logger/__init__.py
--rw-r--r--   0        0        0     3165 2023-07-10 04:44:07.860522 helicone-1.0.2/helicone/async_logger/async_logger.py
--rw-r--r--   0        0        0       52 2023-07-10 04:44:07.860863 helicone-1.0.2/helicone/globals/__init__.py
--rw-r--r--   0        0        0     1347 2023-07-10 17:47:57.079414 helicone-1.0.2/helicone/globals/helicone.py
--rw-r--r--   0        0        0      102 2023-07-10 04:44:07.861504 helicone-1.0.2/helicone/openai_async/__init__.py
--rw-r--r--   0        0        0     8835 2023-07-10 04:44:07.861726 helicone-1.0.2/helicone/openai_async/openai_injector.py
--rw-r--r--   0        0        0     9942 2023-07-10 04:44:07.861894 helicone-1.0.2/helicone/openai_proxy/__init__.py
--rw-r--r--   0        0        0       20 2023-07-03 21:17:48.000891 helicone-1.0.2/helicone/requirements.txt
--rw-r--r--   0        0        0    11545 2023-07-10 04:44:07.862095 helicone-1.0.2/helicone/test.py
--rw-r--r--   0        0        0      380 2023-07-10 17:47:57.079878 helicone-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 helicone-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-07-03 21:17:48.000658 helicone-1.0.3/LICENSE
+-rw-r--r--   0        0        0        1 2023-07-10 04:44:07.860264 helicone-1.0.3/helicone/async_logger/__init__.py
+-rw-r--r--   0        0        0     3165 2023-07-10 04:44:07.860522 helicone-1.0.3/helicone/async_logger/async_logger.py
+-rw-r--r--   0        0        0       52 2023-07-10 04:44:07.860863 helicone-1.0.3/helicone/globals/__init__.py
+-rw-r--r--   0        0        0     1347 2023-07-10 17:47:57.079414 helicone-1.0.3/helicone/globals/helicone.py
+-rw-r--r--   0        0        0     1574 2023-07-15 05:36:31.345474 helicone-1.0.3/helicone/lock/__init__.py
+-rw-r--r--   0        0        0      102 2023-07-10 04:44:07.861504 helicone-1.0.3/helicone/openai_async/__init__.py
+-rw-r--r--   0        0        0     8835 2023-07-10 04:44:07.861726 helicone-1.0.3/helicone/openai_async/openai_injector.py
+-rw-r--r--   0        0        0     9942 2023-07-10 04:44:07.861894 helicone-1.0.3/helicone/openai_proxy/__init__.py
+-rw-r--r--   0        0        0       29 2023-07-15 05:37:02.735045 helicone-1.0.3/helicone/requirements.txt
+-rw-r--r--   0        0        0    11545 2023-07-10 04:44:07.862095 helicone-1.0.3/helicone/test.py
+-rw-r--r--   0        0        0      380 2023-07-15 05:37:46.978071 helicone-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 helicone-1.0.3/PKG-INFO
```

### Comparing `helicone-1.0.2/LICENSE` & `helicone-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `helicone-1.0.2/helicone/async_logger/async_logger.py` & `helicone-1.0.3/helicone/async_logger/async_logger.py`

 * *Files identical despite different names*

### Comparing `helicone-1.0.2/helicone/globals/helicone.py` & `helicone-1.0.3/helicone/globals/helicone.py`

 * *Files identical despite different names*

### Comparing `helicone-1.0.2/helicone/openai_async/openai_injector.py` & `helicone-1.0.3/helicone/openai_async/openai_injector.py`

 * *Files identical despite different names*

### Comparing `helicone-1.0.2/helicone/openai_proxy/__init__.py` & `helicone-1.0.3/helicone/openai_proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `helicone-1.0.2/helicone/test.py` & `helicone-1.0.3/helicone/test.py`

 * *Files identical despite different names*

### Comparing `helicone-1.0.2/PKG-INFO` & `helicone-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helicone
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python wrapper for the OpenAI API that logs all requests to Helicone.
 Home-page: https://www.helicone.ai
 License: Apache-2.0
 Author: Helicone, Inc.
 Author-email: help@helicone.ai
 Requires-Python: >=3.8.1
 Classifier: License :: OSI Approved :: Apache Software License
```

