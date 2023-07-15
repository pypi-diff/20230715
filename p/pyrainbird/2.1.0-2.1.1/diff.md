# Comparing `tmp/pyrainbird-2.1.0.tar.gz` & `tmp/pyrainbird-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrainbird-2.1.0.tar", last modified: Thu Jul  6 06:06:08 2023, max compression
+gzip compressed data, was "pyrainbird-2.1.1.tar", last modified: Sat Jul 15 02:43:30 2023, max compression
```

## Comparing `pyrainbird-2.1.0.tar` & `pyrainbird-2.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:06:08.457235 pyrainbird-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-06 06:06:08.457235 pyrainbird-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:06:08.453235 pyrainbird-2.1.0/pyrainbird/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    21075 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/rainbird.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:06:08.453235 pyrainbird-2.1.0/pyrainbird/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/resources/models.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/resources/sipcommands.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/pyrainbird/timeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:06:08.453235 pyrainbird-2.1.0/pyrainbird.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-06 06:06:08.000000 pyrainbird-2.1.0/pyrainbird.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-06 06:06:08.000000 pyrainbird-2.1.0/pyrainbird.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 06:06:08.000000 pyrainbird-2.1.0/pyrainbird.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-06 06:06:08.000000 pyrainbird-2.1.0/pyrainbird.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 06:06:08.000000 pyrainbird-2.1.0/pyrainbird.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-06 06:06:08.457235 pyrainbird-2.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 06:06:08.457235 pyrainbird-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    46176 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/tests/test_async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-06 06:05:53.000000 pyrainbird-2.1.0/tests/test_rainbird.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:30.275490 pyrainbird-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-15 02:43:30.275490 pyrainbird-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:30.271490 pyrainbird-2.1.1/pyrainbird/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21075 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/rainbird.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:30.271490 pyrainbird-2.1.1/pyrainbird/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/resources/models.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/resources/sipcommands.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:30.275490 pyrainbird-2.1.1/pyrainbird.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-15 02:43:30.000000 pyrainbird-2.1.1/pyrainbird.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-15 02:43:30.000000 pyrainbird-2.1.1/pyrainbird.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 02:43:30.000000 pyrainbird-2.1.1/pyrainbird.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-15 02:43:30.000000 pyrainbird-2.1.1/pyrainbird.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-15 02:43:30.000000 pyrainbird-2.1.1/pyrainbird.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-15 02:43:30.275490 pyrainbird-2.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:30.275490 pyrainbird-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    46176 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/tests/test_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/tests/test_rainbird.py
```

### Comparing `pyrainbird-2.1.0/LICENSE` & `pyrainbird-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.0/PKG-INFO` & `pyrainbird-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrainbird
-Version: 2.1.0
+Version: 2.1.1
 Summary: Rain Bird Controller
 Home-page: https://github.com/allenporter/pyrainbird
 Author: J.J.Barrancos
 Author-email: jordy@fusion-ict.nl
 License: MIT
 Keywords: Rain Bird
 Description-Content-Type: text/markdown
```

### Comparing `pyrainbird-2.1.0/README.md` & `pyrainbird-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.0/pyrainbird/async_client.py` & `pyrainbird-2.1.1/pyrainbird/async_client.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.0/pyrainbird/const.py` & `pyrainbird-2.1.1/pyrainbird/const.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.0/pyrainbird/data.py` & `pyrainbird-2.1.1/pyrainbird/data.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.0/pyrainbird/encryption.py` & `pyrainbird-2.1.1/pyrainbird/encryption.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.0/pyrainbird/rainbird.py` & `pyrainbird-2.1.1/pyrainbird/rainbird.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.0/pyrainbird/resources/__init__.py` & `pyrainbird-2.1.1/pyrainbird/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.0/pyrainbird/resources/models.yaml` & `pyrainbird-2.1.1/pyrainbird/resources/models.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ---
 - device_id: "0003"
   code: ESP_RZXe
   name: ESP-RZXe
   supports_water_budget: false
   max_programs: 0
   max_run_times: 6
+  retries: true
 
 - device_id: "0007"
   code: ESP_ME
   name: ESP-Me
   supports_water_budget: true
   max_programs: 4
   max_run_times: 6
```

### Comparing `pyrainbird-2.1.0/pyrainbird/resources/sipcommands.yaml` & `pyrainbird-2.1.1/pyrainbird/resources/sipcommands.yaml`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.0/pyrainbird/timeline.py` & `pyrainbird-2.1.1/pyrainbird/timeline.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.0/pyrainbird.egg-info/PKG-INFO` & `pyrainbird-2.1.1/pyrainbird.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrainbird
-Version: 2.1.0
+Version: 2.1.1
 Summary: Rain Bird Controller
 Home-page: https://github.com/allenporter/pyrainbird
 Author: J.J.Barrancos
 Author-email: jordy@fusion-ict.nl
 License: MIT
 Keywords: Rain Bird
 Description-Content-Type: text/markdown
```

### Comparing `pyrainbird-2.1.0/pyrainbird.egg-info/SOURCES.txt` & `pyrainbird-2.1.1/pyrainbird.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.0/setup.cfg` & `pyrainbird-2.1.1/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyrainbird
-version = 2.1.0
+version = 2.1.1
 description = Rain Bird Controller
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/pyrainbird
 author = J.J.Barrancos
 author_email = jordy@fusion-ict.nl
 license = MIT
```

### Comparing `pyrainbird-2.1.0/tests/test_async_client.py` & `pyrainbird-2.1.1/tests/test_async_client.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.0/tests/test_data.py` & `pyrainbird-2.1.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.0/tests/test_rainbird.py` & `pyrainbird-2.1.1/tests/test_rainbird.py`

 * *Files identical despite different names*

