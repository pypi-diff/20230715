# Comparing `tmp/sgd_dstc8_data_model-0.1.3.tar.gz` & `tmp/sgd_dstc8_data_model-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgd_dstc8_data_model-0.1.3.tar", max compression
+gzip compressed data, was "sgd_dstc8_data_model-0.1.4.tar", max compression
```

## Comparing `sgd_dstc8_data_model-0.1.3.tar` & `sgd_dstc8_data_model-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2023-04-14 06:22:51.949605 sgd_dstc8_data_model-0.1.3/LICENSE
--rw-r--r--   0        0        0      194 2023-03-26 18:28:50.772270 sgd_dstc8_data_model-0.1.3/README.md
--rw-r--r--   0        0        0     1033 2023-04-14 06:23:54.990259 sgd_dstc8_data_model-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-26 17:53:27.185714 sgd_dstc8_data_model-0.1.3/sgd_dstc8_data_model/__init__.py
--rw-r--r--   0        0        0     1362 2023-04-14 06:18:23.366819 sgd_dstc8_data_model-0.1.3/sgd_dstc8_data_model/dstc_constants.py
--rw-r--r--   0        0        0     7259 2023-04-14 06:18:08.046660 sgd_dstc8_data_model-0.1.3/sgd_dstc8_data_model/dstc_dataclasses.py
--rw-r--r--   0        0        0      754 2023-04-14 06:18:19.518779 sgd_dstc8_data_model-0.1.3/sgd_dstc8_data_model/dstc_utils.py
--rw-r--r--   0        0        0       80 2023-03-25 21:38:17.000000 sgd_dstc8_data_model-0.1.3/sgd_dstc8_data_model/example.py
--rw-r--r--   0        0        0     1305 1970-01-01 00:00:00.000000 sgd_dstc8_data_model-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-14 06:22:51.949605 sgd_dstc8_data_model-0.1.4/LICENSE
+-rw-r--r--   0        0        0      194 2023-03-26 18:28:50.772270 sgd_dstc8_data_model-0.1.4/README.md
+-rw-r--r--   0        0        0     1033 2023-07-15 06:27:19.516782 sgd_dstc8_data_model-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-26 17:53:27.185714 sgd_dstc8_data_model-0.1.4/sgd_dstc8_data_model/__init__.py
+-rw-r--r--   0        0        0     1362 2023-04-14 06:18:23.366819 sgd_dstc8_data_model-0.1.4/sgd_dstc8_data_model/dstc_constants.py
+-rw-r--r--   0        0        0     7259 2023-04-14 06:18:08.046660 sgd_dstc8_data_model-0.1.4/sgd_dstc8_data_model/dstc_dataclasses.py
+-rw-r--r--   0        0        0      829 2023-07-15 06:26:14.932101 sgd_dstc8_data_model-0.1.4/sgd_dstc8_data_model/dstc_utils.py
+-rw-r--r--   0        0        0       80 2023-03-25 21:38:17.000000 sgd_dstc8_data_model-0.1.4/sgd_dstc8_data_model/example.py
+-rw-r--r--   0        0        0     1305 1970-01-01 00:00:00.000000 sgd_dstc8_data_model-0.1.4/PKG-INFO
```

### Comparing `sgd_dstc8_data_model-0.1.3/LICENSE` & `sgd_dstc8_data_model-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sgd_dstc8_data_model-0.1.3/pyproject.toml` & `sgd_dstc8_data_model-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sgd-dstc8-data-model"
-version = "0.1.3"
+version = "0.1.4"
 description = "Model Classes for the SGD DSTC8 dataset"
 authors = ["Adib Mosharrof <adib.mosharrof@gmail.com>"]
 repository = "https://github.com/adibMosharrof/sgd_dstc8_data_model"
 readme = "README.md"
 packages = [{include = "sgd_dstc8_data_model"}]
 keywords = ["sgd", "dstc8", "data", "model", "classes"]
 classifiers = [
```

### Comparing `sgd_dstc8_data_model-0.1.3/sgd_dstc8_data_model/dstc_constants.py` & `sgd_dstc8_data_model-0.1.4/sgd_dstc8_data_model/dstc_constants.py`

 * *Files identical despite different names*

### Comparing `sgd_dstc8_data_model-0.1.3/sgd_dstc8_data_model/dstc_dataclasses.py` & `sgd_dstc8_data_model-0.1.4/sgd_dstc8_data_model/dstc_dataclasses.py`

 * *Files identical despite different names*

### Comparing `sgd_dstc8_data_model-0.1.3/sgd_dstc8_data_model/dstc_utils.py` & `sgd_dstc8_data_model-0.1.4/sgd_dstc8_data_model/dstc_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import json
 
 import yaml
 
 
 def get_dstc_service_name(service_name: str) -> str:
+    i = service_name.find("_")
+    if i == -1:
+        return service_name
     return service_name[: service_name.find("_")]
 
 
 def read_json(path: str):
     with open(path, "r") as f:
         data = json.load(f)
     return data
```

### Comparing `sgd_dstc8_data_model-0.1.3/PKG-INFO` & `sgd_dstc8_data_model-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgd-dstc8-data-model
-Version: 0.1.3
+Version: 0.1.4
 Summary: Model Classes for the SGD DSTC8 dataset
 Home-page: https://github.com/adibMosharrof/sgd_dstc8_data_model
 Keywords: sgd,dstc8,data,model,classes
 Author: Adib Mosharrof
 Author-email: adib.mosharrof@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

