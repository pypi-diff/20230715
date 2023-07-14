# Comparing `tmp/gridappsd_python-2023.7.1a1.tar.gz` & `tmp/gridappsd_python-2023.7.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridappsd_python-2023.7.1a1.tar", max compression
+gzip compressed data, was "gridappsd_python-2023.7.1a2.tar", max compression
```

## Comparing `gridappsd_python-2023.7.1a1.tar` & `gridappsd_python-2023.7.1a2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    10500 2023-07-12 21:49:11.289059 gridappsd_python-2023.7.1a1/README.md
--rw-r--r--   0        0        0     3756 2023-07-12 21:49:11.289059 gridappsd_python-2023.7.1a1/gridappsd/__init__.py
--rw-r--r--   0        0        0     4620 2023-07-12 21:49:11.289059 gridappsd_python-2023.7.1a1/gridappsd/__main__.py
--rw-r--r--   0        0        0     7189 2023-07-12 21:49:11.289059 gridappsd_python-2023.7.1a1/gridappsd/app_registration.py
--rw-r--r--   0        0        0     4689 2023-07-12 21:49:11.289059 gridappsd_python-2023.7.1a1/gridappsd/difference_builder.py
--rw-r--r--   0        0        0    30366 2023-07-12 21:49:11.289059 gridappsd_python-2023.7.1a1/gridappsd/docker_handler.py
--rw-r--r--   0        0        0    17130 2023-07-12 21:49:11.289059 gridappsd_python-2023.7.1a1/gridappsd/goss.py
--rw-r--r--   0        0        0    12684 2023-07-12 21:49:11.289059 gridappsd_python-2023.7.1a1/gridappsd/gridappsd.py
--rw-r--r--   0        0        0     3318 2023-07-12 21:49:11.289059 gridappsd_python-2023.7.1a1/gridappsd/houses.py
--rw-r--r--   0        0        0     2723 2023-07-12 21:49:11.289059 gridappsd_python-2023.7.1a1/gridappsd/loghandler.py
--rw-r--r--   0        0        0     2449 2023-07-12 21:49:11.289059 gridappsd_python-2023.7.1a1/gridappsd/register_app.py
--rw-r--r--   0        0        0    12220 2023-07-12 21:49:11.289059 gridappsd_python-2023.7.1a1/gridappsd/simulation.py
--rw-r--r--   0        0        0     3234 2023-07-12 21:49:11.289059 gridappsd_python-2023.7.1a1/gridappsd/timeseries.py
--rw-r--r--   0        0        0    12052 2023-07-12 21:49:11.289059 gridappsd_python-2023.7.1a1/gridappsd/topics.py
--rw-r--r--   0        0        0     3177 2023-07-12 21:49:11.289059 gridappsd_python-2023.7.1a1/gridappsd/utils.py
--rw-r--r--   0        0        0     1155 2023-07-12 21:50:31.818033 gridappsd_python-2023.7.1a1/pyproject.toml
--rw-r--r--   0        0        0    11433 1970-01-01 00:00:00.000000 gridappsd_python-2023.7.1a1/PKG-INFO
+-rw-r--r--   0        0        0    10500 2023-07-14 23:35:23.267939 gridappsd_python-2023.7.1a2/README.md
+-rw-r--r--   0        0        0     3756 2023-07-14 23:35:23.271939 gridappsd_python-2023.7.1a2/gridappsd/__init__.py
+-rw-r--r--   0        0        0     4620 2023-07-14 23:35:23.271939 gridappsd_python-2023.7.1a2/gridappsd/__main__.py
+-rw-r--r--   0        0        0     7189 2023-07-14 23:35:23.271939 gridappsd_python-2023.7.1a2/gridappsd/app_registration.py
+-rw-r--r--   0        0        0     4689 2023-07-14 23:35:23.271939 gridappsd_python-2023.7.1a2/gridappsd/difference_builder.py
+-rw-r--r--   0        0        0    30366 2023-07-14 23:35:23.271939 gridappsd_python-2023.7.1a2/gridappsd/docker_handler.py
+-rw-r--r--   0        0        0    17130 2023-07-14 23:35:23.271939 gridappsd_python-2023.7.1a2/gridappsd/goss.py
+-rw-r--r--   0        0        0    12684 2023-07-14 23:35:23.271939 gridappsd_python-2023.7.1a2/gridappsd/gridappsd.py
+-rw-r--r--   0        0        0     3318 2023-07-14 23:35:23.271939 gridappsd_python-2023.7.1a2/gridappsd/houses.py
+-rw-r--r--   0        0        0     2723 2023-07-14 23:35:23.271939 gridappsd_python-2023.7.1a2/gridappsd/loghandler.py
+-rw-r--r--   0        0        0     2449 2023-07-14 23:35:23.271939 gridappsd_python-2023.7.1a2/gridappsd/register_app.py
+-rw-r--r--   0        0        0    12220 2023-07-14 23:35:23.271939 gridappsd_python-2023.7.1a2/gridappsd/simulation.py
+-rw-r--r--   0        0        0     3234 2023-07-14 23:35:23.271939 gridappsd_python-2023.7.1a2/gridappsd/timeseries.py
+-rw-r--r--   0        0        0    12052 2023-07-14 23:35:23.271939 gridappsd_python-2023.7.1a2/gridappsd/topics.py
+-rw-r--r--   0        0        0     3177 2023-07-14 23:35:23.271939 gridappsd_python-2023.7.1a2/gridappsd/utils.py
+-rw-r--r--   0        0        0     1155 2023-07-14 23:36:44.953497 gridappsd_python-2023.7.1a2/pyproject.toml
+-rw-r--r--   0        0        0    11433 1970-01-01 00:00:00.000000 gridappsd_python-2023.7.1a2/PKG-INFO
```

### Comparing `gridappsd_python-2023.7.1a1/README.md` & `gridappsd_python-2023.7.1a2/README.md`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.7.1a1/gridappsd/__init__.py` & `gridappsd_python-2023.7.1a2/gridappsd/__init__.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.7.1a1/gridappsd/__main__.py` & `gridappsd_python-2023.7.1a2/gridappsd/__main__.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.7.1a1/gridappsd/app_registration.py` & `gridappsd_python-2023.7.1a2/gridappsd/app_registration.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.7.1a1/gridappsd/difference_builder.py` & `gridappsd_python-2023.7.1a2/gridappsd/difference_builder.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.7.1a1/gridappsd/docker_handler.py` & `gridappsd_python-2023.7.1a2/gridappsd/docker_handler.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.7.1a1/gridappsd/goss.py` & `gridappsd_python-2023.7.1a2/gridappsd/goss.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.7.1a1/gridappsd/gridappsd.py` & `gridappsd_python-2023.7.1a2/gridappsd/gridappsd.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.7.1a1/gridappsd/houses.py` & `gridappsd_python-2023.7.1a2/gridappsd/houses.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.7.1a1/gridappsd/loghandler.py` & `gridappsd_python-2023.7.1a2/gridappsd/loghandler.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.7.1a1/gridappsd/register_app.py` & `gridappsd_python-2023.7.1a2/gridappsd/register_app.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.7.1a1/gridappsd/simulation.py` & `gridappsd_python-2023.7.1a2/gridappsd/simulation.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.7.1a1/gridappsd/timeseries.py` & `gridappsd_python-2023.7.1a2/gridappsd/timeseries.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.7.1a1/gridappsd/topics.py` & `gridappsd_python-2023.7.1a2/gridappsd/topics.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.7.1a1/gridappsd/utils.py` & `gridappsd_python-2023.7.1a2/gridappsd/utils.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2023.7.1a1/pyproject.toml` & `gridappsd_python-2023.7.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridappsd-python"
-version = "2023.7.1a1"
+version = "2023.7.1a2"
 description = "A GridAPPS-D Python Adapter"
 authors = [
     "C. Allwardt <3979063+craig8@users.noreply.github.com>",
     "P. Sharma <poorva.sharma@pnnl.gov",
     "A. Fisher <andrew.fisher@pnnl.gov"
 ]
 license = "BSD-3-Clause"
```

### Comparing `gridappsd_python-2023.7.1a1/PKG-INFO` & `gridappsd_python-2023.7.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridappsd-python
-Version: 2023.7.1a1
+Version: 2023.7.1a2
 Summary: A GridAPPS-D Python Adapter
 Home-page: https://gridappsd.readthedocs.io
 License: BSD-3-Clause
 Keywords: gridappsd,grid,activmq,powergrid,simulation,library
 Author: C. Allwardt
 Author-email: 3979063+craig8@users.noreply.github.com
 Requires-Python: >=3.7.9,<4.0
```

