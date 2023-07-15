# Comparing `tmp/globalomnium-2023.7.3.tar.gz` & `tmp/globalomnium-2023.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globalomnium-2023.7.3.tar", last modified: Fri Jul 14 23:58:33 2023, max compression
+gzip compressed data, was "globalomnium-2023.7.4.tar", last modified: Sat Jul 15 00:07:02 2023, max compression
```

## Comparing `globalomnium-2023.7.3.tar` & `globalomnium-2023.7.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:58:33.980594 globalomnium-2023.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-14 23:58:23.000000 globalomnium-2023.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-14 23:58:33.980594 globalomnium-2023.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-14 23:58:23.000000 globalomnium-2023.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:58:33.980594 globalomnium-2023.7.3/globalomnium/
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-14 23:58:23.000000 globalomnium-2023.7.3/globalomnium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-14 23:58:23.000000 globalomnium-2023.7.3/globalomnium/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-14 23:58:23.000000 globalomnium-2023.7.3/globalomnium/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15003 2023-07-14 23:58:23.000000 globalomnium-2023.7.3/globalomnium/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-14 23:58:23.000000 globalomnium-2023.7.3/globalomnium/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-14 23:58:23.000000 globalomnium-2023.7.3/globalomnium/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-14 23:58:23.000000 globalomnium-2023.7.3/globalomnium/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:58:33.980594 globalomnium-2023.7.3/globalomnium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-14 23:58:33.000000 globalomnium-2023.7.3/globalomnium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-14 23:58:33.000000 globalomnium-2023.7.3/globalomnium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:58:33.000000 globalomnium-2023.7.3/globalomnium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-14 23:58:33.000000 globalomnium-2023.7.3/globalomnium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-14 23:58:33.000000 globalomnium-2023.7.3/globalomnium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 23:58:33.000000 globalomnium-2023.7.3/globalomnium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-14 23:58:23.000000 globalomnium-2023.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-14 23:58:33.984595 globalomnium-2023.7.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:58:33.980594 globalomnium-2023.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-14 23:58:23.000000 globalomnium-2023.7.3/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:07:02.939720 globalomnium-2023.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-15 00:07:02.939720 globalomnium-2023.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:07:02.939720 globalomnium-2023.7.4/globalomnium/
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/globalomnium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/globalomnium/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/globalomnium/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/globalomnium/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/globalomnium/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/globalomnium/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/globalomnium/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:07:02.939720 globalomnium-2023.7.4/globalomnium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-15 00:07:02.000000 globalomnium-2023.7.4/globalomnium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-15 00:07:02.000000 globalomnium-2023.7.4/globalomnium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 00:07:02.000000 globalomnium-2023.7.4/globalomnium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-15 00:07:02.000000 globalomnium-2023.7.4/globalomnium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-15 00:07:02.000000 globalomnium-2023.7.4/globalomnium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-15 00:07:02.000000 globalomnium-2023.7.4/globalomnium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-15 00:07:02.939720 globalomnium-2023.7.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:07:02.939720 globalomnium-2023.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-15 00:06:53.000000 globalomnium-2023.7.4/tests/test_client.py
```

### Comparing `globalomnium-2023.7.3/LICENSE` & `globalomnium-2023.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `globalomnium-2023.7.3/PKG-INFO` & `globalomnium-2023.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalomnium
-Version: 2023.7.3
+Version: 2023.7.4
 Summary: Interface to globalomnium.com water data
 Home-page: https://github.com/carlos-48/globalomnium
 Author: carlos-48 (forked from Luis López)
 Author-email: karloselmaster@gmail.com
 Project-URL: Bug Tracker, https://github.com/carlos-48/globalomnium/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: globalomnium Version: 2023.7.3 Summary: Interface
+Metadata-Version: 2.1 Name: globalomnium Version: 2023.7.4 Summary: Interface
 to globalomnium.com water data Home-page: https://github.com/carlos-48/
 globalomnium Author: carlos-48 (forked from Luis LÃ³pez) Author-email:
 karloselmaster@gmail.com Project-URL: Bug Tracker, https://github.com/carlos-
 48/globalomnium/issues Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown Provides-Extra: mqtt License-File: LICENSE # I'M SORRY BUT ALL
```

### Comparing `globalomnium-2023.7.3/README.md` & `globalomnium-2023.7.4/README.md`

 * *Files identical despite different names*

### Comparing `globalomnium-2023.7.3/globalomnium/__init__.py` & `globalomnium-2023.7.4/globalomnium/__init__.py`

 * *Files identical despite different names*

### Comparing `globalomnium-2023.7.3/globalomnium/__main__.py` & `globalomnium-2023.7.4/globalomnium/__main__.py`

 * *Files identical despite different names*

### Comparing `globalomnium-2023.7.3/globalomnium/cli.py` & `globalomnium-2023.7.4/globalomnium/cli.py`

 * *Files identical despite different names*

### Comparing `globalomnium-2023.7.3/globalomnium/client.py` & `globalomnium-2023.7.4/globalomnium/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,16 +100,17 @@
         # "esVersionNueva": "1",
         # "idioma": "es",
         # "movilAPP": "si",
         # "tipoAPP": "ios",
         # "User-Agent": (
         #     "Mozilla/5.0 (iPhone; CPU iPhone OS 11_4_1 like Mac OS X) "
         #     "AppleWebKit/605.1.15 (KHTML, like Gecko) Mobile/15G77"
+        # ),
         "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
-        ),
+        
     }
 
     def __init__(
         self,
         session: aiohttp.ClientSession,
         user: str,
         passw: str,
```

### Comparing `globalomnium-2023.7.3/globalomnium/mqtt.py` & `globalomnium-2023.7.4/globalomnium/mqtt.py`

 * *Files identical despite different names*

### Comparing `globalomnium-2023.7.3/globalomnium/parsers.py` & `globalomnium-2023.7.4/globalomnium/parsers.py`

 * *Files identical despite different names*

### Comparing `globalomnium-2023.7.3/globalomnium.egg-info/PKG-INFO` & `globalomnium-2023.7.4/globalomnium.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalomnium
-Version: 2023.7.3
+Version: 2023.7.4
 Summary: Interface to globalomnium.com water data
 Home-page: https://github.com/carlos-48/globalomnium
 Author: carlos-48 (forked from Luis López)
 Author-email: karloselmaster@gmail.com
 Project-URL: Bug Tracker, https://github.com/carlos-48/globalomnium/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: globalomnium Version: 2023.7.3 Summary: Interface
+Metadata-Version: 2.1 Name: globalomnium Version: 2023.7.4 Summary: Interface
 to globalomnium.com water data Home-page: https://github.com/carlos-48/
 globalomnium Author: carlos-48 (forked from Luis LÃ³pez) Author-email:
 karloselmaster@gmail.com Project-URL: Bug Tracker, https://github.com/carlos-
 48/globalomnium/issues Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown Provides-Extra: mqtt License-File: LICENSE # I'M SORRY BUT ALL
```

### Comparing `globalomnium-2023.7.3/setup.cfg` & `globalomnium-2023.7.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = globalomnium
-version = 2023.07.3
+version = 2023.07.4
 author = carlos-48 (forked from Luis López)
 author_email = karloselmaster@gmail.com
 description = Interface to globalomnium.com water data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/carlos-48/globalomnium
 project_urls =
```

### Comparing `globalomnium-2023.7.3/tests/test_client.py` & `globalomnium-2023.7.4/tests/test_client.py`

 * *Files identical despite different names*

