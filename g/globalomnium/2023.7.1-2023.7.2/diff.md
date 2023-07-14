# Comparing `tmp/globalomnium-2023.7.1.tar.gz` & `tmp/globalomnium-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globalomnium-2023.7.1.tar", last modified: Fri Jul 14 23:37:52 2023, max compression
+gzip compressed data, was "globalomnium-2023.7.2.tar", last modified: Fri Jul 14 23:46:39 2023, max compression
```

## Comparing `globalomnium-2023.7.1.tar` & `globalomnium-2023.7.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:37:52.684210 globalomnium-2023.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-14 23:37:43.000000 globalomnium-2023.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-14 23:37:52.684210 globalomnium-2023.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-14 23:37:43.000000 globalomnium-2023.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:37:52.680210 globalomnium-2023.7.1/globalomnium/
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-14 23:37:43.000000 globalomnium-2023.7.1/globalomnium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-14 23:37:43.000000 globalomnium-2023.7.1/globalomnium/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-14 23:37:43.000000 globalomnium-2023.7.1/globalomnium/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    15001 2023-07-14 23:37:43.000000 globalomnium-2023.7.1/globalomnium/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-14 23:37:43.000000 globalomnium-2023.7.1/globalomnium/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-14 23:37:43.000000 globalomnium-2023.7.1/globalomnium/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-14 23:37:43.000000 globalomnium-2023.7.1/globalomnium/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:37:52.684210 globalomnium-2023.7.1/globalomnium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-14 23:37:52.000000 globalomnium-2023.7.1/globalomnium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-14 23:37:52.000000 globalomnium-2023.7.1/globalomnium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:37:52.000000 globalomnium-2023.7.1/globalomnium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-14 23:37:52.000000 globalomnium-2023.7.1/globalomnium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-14 23:37:52.000000 globalomnium-2023.7.1/globalomnium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 23:37:52.000000 globalomnium-2023.7.1/globalomnium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-14 23:37:43.000000 globalomnium-2023.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-14 23:37:52.684210 globalomnium-2023.7.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:37:52.684210 globalomnium-2023.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-14 23:37:43.000000 globalomnium-2023.7.1/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:46:39.942671 globalomnium-2023.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-14 23:46:29.000000 globalomnium-2023.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-14 23:46:39.942671 globalomnium-2023.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-14 23:46:29.000000 globalomnium-2023.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:46:39.942671 globalomnium-2023.7.2/globalomnium/
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-14 23:46:29.000000 globalomnium-2023.7.2/globalomnium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-14 23:46:29.000000 globalomnium-2023.7.2/globalomnium/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-14 23:46:29.000000 globalomnium-2023.7.2/globalomnium/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15001 2023-07-14 23:46:29.000000 globalomnium-2023.7.2/globalomnium/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-14 23:46:29.000000 globalomnium-2023.7.2/globalomnium/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-14 23:46:29.000000 globalomnium-2023.7.2/globalomnium/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-14 23:46:29.000000 globalomnium-2023.7.2/globalomnium/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:46:39.942671 globalomnium-2023.7.2/globalomnium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-14 23:46:39.000000 globalomnium-2023.7.2/globalomnium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-14 23:46:39.000000 globalomnium-2023.7.2/globalomnium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:46:39.000000 globalomnium-2023.7.2/globalomnium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-14 23:46:39.000000 globalomnium-2023.7.2/globalomnium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-14 23:46:39.000000 globalomnium-2023.7.2/globalomnium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 23:46:39.000000 globalomnium-2023.7.2/globalomnium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-14 23:46:29.000000 globalomnium-2023.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-14 23:46:39.942671 globalomnium-2023.7.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:46:39.942671 globalomnium-2023.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-14 23:46:29.000000 globalomnium-2023.7.2/tests/test_client.py
```

### Comparing `globalomnium-2023.7.1/LICENSE` & `globalomnium-2023.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `globalomnium-2023.7.1/PKG-INFO` & `globalomnium-2023.7.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalomnium
-Version: 2023.7.1
+Version: 2023.7.2
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
-Metadata-Version: 2.1 Name: globalomnium Version: 2023.7.1 Summary: Interface
+Metadata-Version: 2.1 Name: globalomnium Version: 2023.7.2 Summary: Interface
 to globalomnium.com water data Home-page: https://github.com/carlos-48/
 globalomnium Author: carlos-48 (forked from Luis LÃ³pez) Author-email:
 karloselmaster@gmail.com Project-URL: Bug Tracker, https://github.com/carlos-
 48/globalomnium/issues Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown Provides-Extra: mqtt License-File: LICENSE # I'M SORRY BUT ALL
```

### Comparing `globalomnium-2023.7.1/README.md` & `globalomnium-2023.7.2/README.md`

 * *Files identical despite different names*

### Comparing `globalomnium-2023.7.1/globalomnium/__init__.py` & `globalomnium-2023.7.2/globalomnium/__init__.py`

 * *Files identical despite different names*

### Comparing `globalomnium-2023.7.1/globalomnium/__main__.py` & `globalomnium-2023.7.2/globalomnium/__main__.py`

 * *Files identical despite different names*

### Comparing `globalomnium-2023.7.1/globalomnium/cli.py` & `globalomnium-2023.7.2/globalomnium/cli.py`

 * *Files identical despite different names*

### Comparing `globalomnium-2023.7.1/globalomnium/client.py` & `globalomnium-2023.7.2/globalomnium/client.py`

 * *Files identical despite different names*

### Comparing `globalomnium-2023.7.1/globalomnium/mqtt.py` & `globalomnium-2023.7.2/globalomnium/mqtt.py`

 * *Files identical despite different names*

### Comparing `globalomnium-2023.7.1/globalomnium/parsers.py` & `globalomnium-2023.7.2/globalomnium/parsers.py`

 * *Files identical despite different names*

### Comparing `globalomnium-2023.7.1/globalomnium.egg-info/PKG-INFO` & `globalomnium-2023.7.2/globalomnium.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globalomnium
-Version: 2023.7.1
+Version: 2023.7.2
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
-Metadata-Version: 2.1 Name: globalomnium Version: 2023.7.1 Summary: Interface
+Metadata-Version: 2.1 Name: globalomnium Version: 2023.7.2 Summary: Interface
 to globalomnium.com water data Home-page: https://github.com/carlos-48/
 globalomnium Author: carlos-48 (forked from Luis LÃ³pez) Author-email:
 karloselmaster@gmail.com Project-URL: Bug Tracker, https://github.com/carlos-
 48/globalomnium/issues Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown Provides-Extra: mqtt License-File: LICENSE # I'M SORRY BUT ALL
```

### Comparing `globalomnium-2023.7.1/setup.cfg` & `globalomnium-2023.7.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = globalomnium
-version = 2023.7.1
+version = 2023.07.2
 author = carlos-48 (forked from Luis López)
 author_email = karloselmaster@gmail.com
 description = Interface to globalomnium.com water data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/carlos-48/globalomnium
 project_urls =
```

### Comparing `globalomnium-2023.7.1/tests/test_client.py` & `globalomnium-2023.7.2/tests/test_client.py`

 * *Files identical despite different names*

