# Comparing `tmp/helicone-1.0.5.tar.gz` & `tmp/helicone-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helicone-1.0.5.tar", max compression
+gzip compressed data, was "helicone-1.0.6.tar", max compression
```

## Comparing `helicone-1.0.5.tar` & `helicone-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11341 2023-07-03 21:17:48.000658 helicone-1.0.5/LICENSE
--rw-r--r--   0        0        0        1 2023-07-10 04:44:07.860264 helicone-1.0.5/helicone/async_logger/__init__.py
--rw-r--r--   0        0        0     3165 2023-07-10 04:44:07.860522 helicone-1.0.5/helicone/async_logger/async_logger.py
--rw-r--r--   0        0        0       52 2023-07-10 04:44:07.860863 helicone-1.0.5/helicone/globals/__init__.py
--rw-r--r--   0        0        0     1347 2023-07-10 17:47:57.079414 helicone-1.0.5/helicone/globals/helicone.py
--rw-r--r--   0        0        0     1574 2023-07-15 05:36:31.345474 helicone-1.0.5/helicone/lock/__init__.py
--rw-r--r--   0        0        0      102 2023-07-10 04:44:07.861504 helicone-1.0.5/helicone/openai_async/__init__.py
--rw-r--r--   0        0        0     8835 2023-07-10 04:44:07.861726 helicone-1.0.5/helicone/openai_async/openai_injector.py
--rw-r--r--   0        0        0     9942 2023-07-10 04:44:07.861894 helicone-1.0.5/helicone/openai_proxy/__init__.py
--rw-r--r--   0        0        0       29 2023-07-15 05:44:38.023402 helicone-1.0.5/helicone/requirements.txt
--rw-r--r--   0        0        0    11545 2023-07-10 04:44:07.862095 helicone-1.0.5/helicone/test.py
--rw-r--r--   0        0        0      401 2023-07-15 05:46:50.154724 helicone-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 helicone-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-07-03 21:17:48.000658 helicone-1.0.6/LICENSE
+-rw-r--r--   0        0        0        1 2023-07-10 04:44:07.860264 helicone-1.0.6/helicone/async_logger/__init__.py
+-rw-r--r--   0        0        0     3165 2023-07-10 04:44:07.860522 helicone-1.0.6/helicone/async_logger/async_logger.py
+-rw-r--r--   0        0        0       52 2023-07-10 04:44:07.860863 helicone-1.0.6/helicone/globals/__init__.py
+-rw-r--r--   0        0        0     1347 2023-07-10 17:47:57.079414 helicone-1.0.6/helicone/globals/helicone.py
+-rw-r--r--   0        0        0     1836 2023-07-15 05:50:37.896824 helicone-1.0.6/helicone/lock/__init__.py
+-rw-r--r--   0        0        0      102 2023-07-10 04:44:07.861504 helicone-1.0.6/helicone/openai_async/__init__.py
+-rw-r--r--   0        0        0     8835 2023-07-10 04:44:07.861726 helicone-1.0.6/helicone/openai_async/openai_injector.py
+-rw-r--r--   0        0        0     9942 2023-07-10 04:44:07.861894 helicone-1.0.6/helicone/openai_proxy/__init__.py
+-rw-r--r--   0        0        0       29 2023-07-15 05:44:38.023402 helicone-1.0.6/helicone/requirements.txt
+-rw-r--r--   0        0        0    11545 2023-07-10 04:44:07.862095 helicone-1.0.6/helicone/test.py
+-rw-r--r--   0        0        0      401 2023-07-15 05:50:52.252483 helicone-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 helicone-1.0.6/PKG-INFO
```

### Comparing `helicone-1.0.5/LICENSE` & `helicone-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `helicone-1.0.5/helicone/async_logger/async_logger.py` & `helicone-1.0.6/helicone/async_logger/async_logger.py`

 * *Files identical despite different names*

### Comparing `helicone-1.0.5/helicone/globals/helicone.py` & `helicone-1.0.6/helicone/globals/helicone.py`

 * *Files identical despite different names*

### Comparing `helicone-1.0.5/helicone/lock/__init__.py` & `helicone-1.0.6/helicone/lock/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 import json
 import os
 import lockfile
 
 
 class HeliconeLockManager:
-    LOCKFILE_PATH = os.path.expanduser(
-        "~/.helicone/custom_properties.json.lock")
-    JSON_PATH = os.path.expanduser("~/.helicone/custom_properties.json")
+    DIR_PATH = os.path.expanduser("~/.helicone")
+    LOCKFILE_PATH = os.path.join(DIR_PATH, "custom_properties.json.lock")
+    JSON_PATH = os.path.join(DIR_PATH, "custom_properties.json")
+
+    @staticmethod
+    def check_files():
+        os.makedirs(HeliconeLockManager.DIR_PATH, exist_ok=True)
+        if not os.path.exists(HeliconeLockManager.JSON_PATH):
+            with open(HeliconeLockManager.JSON_PATH, 'w') as json_file:
+                json.dump({}, json_file)
 
     @staticmethod
     def write_custom_property(property_name, value):
+        HeliconeLockManager.check_files()
         with lockfile.LockFile(HeliconeLockManager.LOCKFILE_PATH):
-            if os.path.exists(HeliconeLockManager.JSON_PATH):
-                with open(HeliconeLockManager.JSON_PATH, "r") as json_file:
-                    properties = json.load(json_file)
-            else:
-                properties = {}
+            with open(HeliconeLockManager.JSON_PATH, "r") as json_file:
+                properties = json.load(json_file)
 
             properties[property_name] = value
 
             with open(HeliconeLockManager.JSON_PATH, "w") as json_file:
                 json.dump(properties, json_file)
 
     @staticmethod
     def clear_all_properties():
+        HeliconeLockManager.check_files()
         with lockfile.LockFile(HeliconeLockManager.LOCKFILE_PATH):
             with open(HeliconeLockManager.JSON_PATH, "w") as json_file:
                 json.dump({}, json_file)
 
     @staticmethod
     def remove_custom_property(property_name):
+        HeliconeLockManager.check_files()
         with lockfile.LockFile(HeliconeLockManager.LOCKFILE_PATH):
-            if os.path.exists(HeliconeLockManager.JSON_PATH):
-                with open(HeliconeLockManager.JSON_PATH, "r") as json_file:
-                    properties = json.load(json_file)
+            with open(HeliconeLockManager.JSON_PATH, "r") as json_file:
+                properties = json.load(json_file)
+
+            if property_name in properties:
+                del properties[property_name]
+
+                with open(HeliconeLockManager.JSON_PATH, "w") as json_file:
+                    json.dump(properties, json_file)
 
-                if property_name in properties:
-                    del properties[property_name]
 
-                    with open(HeliconeLockManager.JSON_PATH, "w") as json_file:
-                        json.dump(properties, json_file)
+HeliconeLockManager.check_files()
```

### Comparing `helicone-1.0.5/helicone/openai_async/openai_injector.py` & `helicone-1.0.6/helicone/openai_async/openai_injector.py`

 * *Files identical despite different names*

### Comparing `helicone-1.0.5/helicone/openai_proxy/__init__.py` & `helicone-1.0.6/helicone/openai_proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `helicone-1.0.5/helicone/test.py` & `helicone-1.0.6/helicone/test.py`

 * *Files identical despite different names*

### Comparing `helicone-1.0.5/PKG-INFO` & `helicone-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helicone
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python wrapper for the OpenAI API that logs all requests to Helicone.
 Home-page: https://www.helicone.ai
 License: Apache-2.0
 Author: Helicone, Inc.
 Author-email: help@helicone.ai
 Requires-Python: >=3.8.1
 Classifier: License :: OSI Approved :: Apache Software License
```

