# Comparing `tmp/baseblock-0.2.23.tar.gz` & `tmp/baseblock-0.2.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseblock-0.2.23.tar", max compression
+gzip compressed data, was "baseblock-0.2.24.tar", max compression
```

## Comparing `baseblock-0.2.23.tar` & `baseblock-0.2.24.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      509 2022-11-01 19:40:10.480205 baseblock-0.2.23/baseblock/__init__.py
--rw-r--r--   0        0        0     1665 2023-03-31 18:06:04.643612 baseblock-0.2.23/baseblock/base_object.py
--rw-r--r--   0        0        0     2206 2022-11-01 19:40:21.549334 baseblock-0.2.23/baseblock/common_utils.py
--rw-r--r--   0        0        0     3400 2022-11-01 19:40:24.233178 baseblock-0.2.23/baseblock/crypto_base.py
--rw-r--r--   0        0        0    17519 2023-05-16 05:48:05.464931 baseblock-0.2.23/baseblock/enforce_type.py
--rw-r--r--   0        0        0     6749 2023-01-10 20:33:14.114247 baseblock-0.2.23/baseblock/env_io.py
--rw-r--r--   0        0        0    25397 2023-02-07 00:55:29.559730 baseblock-0.2.23/baseblock/file_io.py
--rw-r--r--   0        0        0     1918 2022-11-01 19:40:37.387998 baseblock-0.2.23/baseblock/service_event_generator.py
--rw-r--r--   0        0        0     2320 2022-11-01 19:40:10.479705 baseblock-0.2.23/baseblock/stopwatch.py
--rw-r--r--   0        0        0     5147 2023-01-27 20:32:24.092475 baseblock-0.2.23/baseblock/text_matcher.py
--rw-r--r--   0        0        0    29945 2023-01-26 05:18:13.221964 baseblock-0.2.23/baseblock/text_utils.py
--rw-r--r--   0        0        0     1364 2022-11-01 19:40:49.507564 baseblock-0.2.23/baseblock/time_helper.py
--rw-r--r--   0        0        0     1344 2023-05-16 03:21:11.641161 baseblock-0.2.23/pyproject.toml
--rw-r--r--   0        0        0      506 2022-10-20 17:03:08.598380 baseblock-0.2.23/README.md
--rw-r--r--   0        0        0     1237 2023-05-16 05:49:06.863304 baseblock-0.2.23/setup.py
--rw-r--r--   0        0        0     1364 2023-05-16 05:49:06.863804 baseblock-0.2.23/PKG-INFO
+-rw-r--r--   0        0        0      509 2022-11-01 19:40:10.480205 baseblock-0.2.24/baseblock/__init__.py
+-rw-r--r--   0        0        0     1665 2023-03-31 18:06:04.643612 baseblock-0.2.24/baseblock/base_object.py
+-rw-r--r--   0        0        0     2206 2022-11-01 19:40:21.549334 baseblock-0.2.24/baseblock/common_utils.py
+-rw-r--r--   0        0        0     3400 2022-11-01 19:40:24.233178 baseblock-0.2.24/baseblock/crypto_base.py
+-rw-r--r--   0        0        0    17519 2023-05-16 05:48:05.464931 baseblock-0.2.24/baseblock/enforce_type.py
+-rw-r--r--   0        0        0     6749 2023-01-10 20:33:14.114247 baseblock-0.2.24/baseblock/env_io.py
+-rw-r--r--   0        0        0    25790 2023-07-15 16:47:51.402254 baseblock-0.2.24/baseblock/file_io.py
+-rw-r--r--   0        0        0     1918 2022-11-01 19:40:37.387998 baseblock-0.2.24/baseblock/service_event_generator.py
+-rw-r--r--   0        0        0     2320 2022-11-01 19:40:10.479705 baseblock-0.2.24/baseblock/stopwatch.py
+-rw-r--r--   0        0        0     5147 2023-01-27 20:32:24.092475 baseblock-0.2.24/baseblock/text_matcher.py
+-rw-r--r--   0        0        0    29945 2023-01-26 05:18:13.221964 baseblock-0.2.24/baseblock/text_utils.py
+-rw-r--r--   0        0        0     1364 2022-11-01 19:40:49.507564 baseblock-0.2.24/baseblock/time_helper.py
+-rw-r--r--   0        0        0     1344 2023-07-15 16:47:31.363255 baseblock-0.2.24/pyproject.toml
+-rw-r--r--   0        0        0      506 2022-10-20 17:03:08.598380 baseblock-0.2.24/README.md
+-rw-r--r--   0        0        0     1237 1970-01-01 00:00:00.000000 baseblock-0.2.24/setup.py
+-rw-r--r--   0        0        0     1415 1970-01-01 00:00:00.000000 baseblock-0.2.24/PKG-INFO
```

### Comparing `baseblock-0.2.23/baseblock/base_object.py` & `baseblock-0.2.24/baseblock/base_object.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.23/baseblock/common_utils.py` & `baseblock-0.2.24/baseblock/common_utils.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.23/baseblock/crypto_base.py` & `baseblock-0.2.24/baseblock/crypto_base.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.23/baseblock/enforce_type.py` & `baseblock-0.2.24/baseblock/enforce_type.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.23/baseblock/env_io.py` & `baseblock-0.2.24/baseblock/env_io.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.23/baseblock/file_io.py` & `baseblock-0.2.24/baseblock/file_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """ File Input/Output Utility Methods """
 
 
 import os
+import traceback
 from datetime import datetime
 
 from io import StringIO
 from io import open as io_open
 
 from csv import reader as csv_reader
 from typing import List
@@ -27,16 +28,19 @@
 from yaml import dump as yaml_dump
 from yaml import load as yaml_load
 
 
 class FileIO(object):
     """ File Input/Output Utility Methods """
 
+    
+
     @staticmethod
     def is_empty_folder(folder_name: str) -> bool:
+        
         """ Check if a Folder is Empty of Contents
 
         Args:
             folder_name (str): a fully qualified path to a folder
 
         Returns:
             bool: True if the folder has no contents
@@ -392,19 +396,30 @@
             ValueError: the file is not valid YAML
 
         Returns:
             dict: a py YAML dictionary
         """
         FileIO.exists_or_error(file_path)
 
-        with open(file_path, 'r') as stream:
+        with open(file_path, 'r', encoding='utf-8') as stream:
             try:
-                return yaml_load(stream, Loader)
+
+                return yaml_load(stream, Loader=Loader)
+
             except YAMLError:
-                raise ValueError(f'Invalid YAML File: {file_path}')
+                traceback.format_exc()
+                raise ValueError('\n'.join([
+                    'Invalid File',
+                    '\t{0}'.format(file_path)]))
+
+            except UnicodeDecodeError:
+                print(traceback.format_exc())
+                raise ValueError('\n'.join([
+                    'Encoding Error',
+                    '\t{0}'.format(file_path)]))
 
     @staticmethod
     def read_lines(file_path: str,
                    file_encoding: str = 'utf-8') -> list:
         """ Read Lines of a File into a List
 
         Args:
```

### Comparing `baseblock-0.2.23/baseblock/service_event_generator.py` & `baseblock-0.2.24/baseblock/service_event_generator.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.23/baseblock/stopwatch.py` & `baseblock-0.2.24/baseblock/stopwatch.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.23/baseblock/text_matcher.py` & `baseblock-0.2.24/baseblock/text_matcher.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.23/baseblock/text_utils.py` & `baseblock-0.2.24/baseblock/text_utils.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.23/baseblock/time_helper.py` & `baseblock-0.2.24/baseblock/time_helper.py`

 * *Files identical despite different names*

### Comparing `baseblock-0.2.23/pyproject.toml` & `baseblock-0.2.24/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "Craig Trim <craigtrim@gmail.com>",
 ]
 
 description = "Base Block of Common Enterprise Python Utilities"
 license = "MIT"
 name = "baseblock"
 readme = "README.md"
-version = "0.2.23"
+version = "0.2.24"
 
 keywords = ["utility", "helper", "text", "matching"]
 repository = "https://github.com/craigtrim/climate-bot"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `baseblock-0.2.23/setup.py` & `baseblock-0.2.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['PyYAML==6.0', 'cryptography==38.0.1', 'unicodedata2']
 
 setup_kwargs = {
     'name': 'baseblock',
-    'version': '0.2.23',
+    'version': '0.2.24',
     'description': 'Base Block of Common Enterprise Python Utilities',
     'long_description': '# Base Block (baseblock)\n\nBase Block of Common Enterprise Python Utilities\n\n\n## Crypto Base\nUsage\n```python\nfrom baseblock import CryptoBase\n\nkey = CryptoBase.generate_private_key()\n```\n\nThe `key` is used to both encrypt and decrypt text, like this:\n```python\ninput_text = "Hello, World!"\n\ncrypt = CryptoBase(key)\n\nx = crypt.encrypt_str(input_text)\ny = crypt.decrypt_str(x)\n\nassert input_text == y\n```\n\nThe key can also be stored in the environment under **BASEBLOCK_CRYPTO_KEY**.\n',
     'author': 'Craig Trim',
     'author_email': 'craigtrim@gmail.com',
     'maintainer': 'Craig Trim',
     'maintainer_email': 'craigtrim@gmail.com',
     'url': 'https://github.com/craigtrim/climate-bot',
```

### Comparing `baseblock-0.2.23/PKG-INFO` & `baseblock-0.2.24/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: baseblock
-Version: 0.2.23
+Version: 0.2.24
 Summary: Base Block of Common Enterprise Python Utilities
 Home-page: https://github.com/craigtrim/climate-bot
 License: MIT
 Keywords: utility,helper,text,matching
 Author: Craig Trim
 Author-email: craigtrim@gmail.com
 Maintainer: Craig Trim
 Maintainer-email: craigtrim@gmail.com
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyYAML (==6.0)
 Requires-Dist: cryptography (==38.0.1)
 Requires-Dist: unicodedata2
 Project-URL: Repository, https://github.com/craigtrim/climate-bot
 Description-Content-Type: text/markdown
```

