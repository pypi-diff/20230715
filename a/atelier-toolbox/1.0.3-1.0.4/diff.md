# Comparing `tmp/atelier_toolbox-1.0.3.tar.gz` & `tmp/atelier_toolbox-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atelier_toolbox-1.0.3.tar", max compression
+gzip compressed data, was "atelier_toolbox-1.0.4.tar", max compression
```

## Comparing `atelier_toolbox-1.0.3.tar` & `atelier_toolbox-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1070 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/LICENSE
--rw-r--r--   0        0        0     5170 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/README.md
--rw-r--r--   0        0        0      766 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/src/toolbox/__init__.py
--rw-r--r--   0        0        0      547 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/src/toolbox/cli.py
--rw-r--r--   0        0        0      829 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/src/toolbox/common/calendar.py
--rw-r--r--   0        0        0      461 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/src/toolbox/common/exceptions.py
--rw-r--r--   0        0        0      410 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/src/toolbox/common/file.py
--rw-r--r--   0        0        0      868 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/src/toolbox/common/output.py
--rw-r--r--   0        0        0      836 2023-06-08 08:41:28.085724 atelier_toolbox-1.0.3/src/toolbox/common/work.py
--rw-r--r--   0        0        0      263 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/scripts.py
--rw-r--r--   0        0        0      112 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/business/__init__.py
--rw-r--r--   0        0        0       64 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/business/__version__.py
--rw-r--r--   0        0        0     1721 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/business/cli.py
--rw-r--r--   0        0        0       94 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/dw/__init__.py
--rw-r--r--   0        0        0       64 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/dw/__version__.py
--rw-r--r--   0        0        0     2058 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/dw/cli.py
--rw-r--r--   0        0        0    12979 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/dw/download.py
--rw-r--r--   0        0        0       96 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/hash/__init__.py
--rw-r--r--   0        0        0       64 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/hash/__version__.py
--rw-r--r--   0        0        0     1730 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/hash/cli.py
--rw-r--r--   0        0        0      334 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/hash/hash_algoritms_enum.py
--rw-r--r--   0        0        0       99 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/pdf/__init__.py
--rw-r--r--   0        0        0       64 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/pdf/__version__.py
--rw-r--r--   0        0        0     1605 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/pdf/cli.py
--rw-r--r--   0        0        0     1431 2023-06-08 08:41:28.089724 atelier_toolbox-1.0.3/src/toolbox/sets/pdf/converter.py
--rw-r--r--   0        0        0     6053 1970-01-01 00:00:00.000000 atelier_toolbox-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-15 09:35:53.722250 atelier_toolbox-1.0.4/LICENSE
+-rw-r--r--   0        0        0     5170 2023-07-15 09:35:53.722250 atelier_toolbox-1.0.4/README.md
+-rw-r--r--   0        0        0      766 2023-07-15 09:35:53.722250 atelier_toolbox-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-15 09:35:53.722250 atelier_toolbox-1.0.4/src/toolbox/__init__.py
+-rw-r--r--   0        0        0      547 2023-07-15 09:35:53.722250 atelier_toolbox-1.0.4/src/toolbox/cli.py
+-rw-r--r--   0        0        0      829 2023-07-15 09:35:53.722250 atelier_toolbox-1.0.4/src/toolbox/common/calendar.py
+-rw-r--r--   0        0        0      461 2023-07-15 09:35:53.722250 atelier_toolbox-1.0.4/src/toolbox/common/exceptions.py
+-rw-r--r--   0        0        0      410 2023-07-15 09:35:53.722250 atelier_toolbox-1.0.4/src/toolbox/common/file.py
+-rw-r--r--   0        0        0      868 2023-07-15 09:35:53.722250 atelier_toolbox-1.0.4/src/toolbox/common/output.py
+-rw-r--r--   0        0        0      836 2023-07-15 09:35:53.722250 atelier_toolbox-1.0.4/src/toolbox/common/work.py
+-rw-r--r--   0        0        0      263 2023-07-15 09:35:53.722250 atelier_toolbox-1.0.4/src/toolbox/scripts.py
+-rw-r--r--   0        0        0      112 2023-07-15 09:35:53.722250 atelier_toolbox-1.0.4/src/toolbox/sets/business/__init__.py
+-rw-r--r--   0        0        0       64 2023-07-15 09:35:53.726250 atelier_toolbox-1.0.4/src/toolbox/sets/business/__version__.py
+-rw-r--r--   0        0        0     1721 2023-07-15 09:35:53.726250 atelier_toolbox-1.0.4/src/toolbox/sets/business/cli.py
+-rw-r--r--   0        0        0       94 2023-07-15 09:35:53.726250 atelier_toolbox-1.0.4/src/toolbox/sets/dw/__init__.py
+-rw-r--r--   0        0        0       64 2023-07-15 09:35:53.726250 atelier_toolbox-1.0.4/src/toolbox/sets/dw/__version__.py
+-rw-r--r--   0        0        0     2058 2023-07-15 09:35:53.726250 atelier_toolbox-1.0.4/src/toolbox/sets/dw/cli.py
+-rw-r--r--   0        0        0    12979 2023-07-15 09:35:53.726250 atelier_toolbox-1.0.4/src/toolbox/sets/dw/download.py
+-rw-r--r--   0        0        0       96 2023-07-15 09:35:53.726250 atelier_toolbox-1.0.4/src/toolbox/sets/hash/__init__.py
+-rw-r--r--   0        0        0       64 2023-07-15 09:35:53.726250 atelier_toolbox-1.0.4/src/toolbox/sets/hash/__version__.py
+-rw-r--r--   0        0        0     1730 2023-07-15 09:35:53.726250 atelier_toolbox-1.0.4/src/toolbox/sets/hash/cli.py
+-rw-r--r--   0        0        0      334 2023-07-15 09:35:53.726250 atelier_toolbox-1.0.4/src/toolbox/sets/hash/hash_algoritms_enum.py
+-rw-r--r--   0        0        0       99 2023-07-15 09:35:53.726250 atelier_toolbox-1.0.4/src/toolbox/sets/pdf/__init__.py
+-rw-r--r--   0        0        0       64 2023-07-15 09:35:53.726250 atelier_toolbox-1.0.4/src/toolbox/sets/pdf/__version__.py
+-rw-r--r--   0        0        0     1605 2023-07-15 09:35:53.726250 atelier_toolbox-1.0.4/src/toolbox/sets/pdf/cli.py
+-rw-r--r--   0        0        0     1431 2023-07-15 09:35:53.726250 atelier_toolbox-1.0.4/src/toolbox/sets/pdf/converter.py
+-rw-r--r--   0        0        0     6053 1970-01-01 00:00:00.000000 atelier_toolbox-1.0.4/PKG-INFO
```

### Comparing `atelier_toolbox-1.0.3/LICENSE` & `atelier_toolbox-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.3/README.md` & `atelier_toolbox-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.3/pyproject.toml` & `atelier_toolbox-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atelier-toolbox"
-version = "1.0.3"
+version = "1.0.4"
 description = "Tools for various automations 🧰"
 authors = ["Mihai"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/mihaichris/atelier-toolbox"
 keywords = ["toolbox", "automation", "poetry"]
 packages = [{ include = "toolbox", from="src"}]
```

### Comparing `atelier_toolbox-1.0.3/src/toolbox/cli.py` & `atelier_toolbox-1.0.4/src/toolbox/cli.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.3/src/toolbox/common/calendar.py` & `atelier_toolbox-1.0.4/src/toolbox/common/calendar.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.3/src/toolbox/common/output.py` & `atelier_toolbox-1.0.4/src/toolbox/common/output.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.3/src/toolbox/common/work.py` & `atelier_toolbox-1.0.4/src/toolbox/common/work.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.3/src/toolbox/sets/business/cli.py` & `atelier_toolbox-1.0.4/src/toolbox/sets/business/cli.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.3/src/toolbox/sets/dw/cli.py` & `atelier_toolbox-1.0.4/src/toolbox/sets/dw/cli.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.3/src/toolbox/sets/dw/download.py` & `atelier_toolbox-1.0.4/src/toolbox/sets/dw/download.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.3/src/toolbox/sets/hash/cli.py` & `atelier_toolbox-1.0.4/src/toolbox/sets/hash/cli.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.3/src/toolbox/sets/pdf/cli.py` & `atelier_toolbox-1.0.4/src/toolbox/sets/pdf/cli.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.3/src/toolbox/sets/pdf/converter.py` & `atelier_toolbox-1.0.4/src/toolbox/sets/pdf/converter.py`

 * *Files identical despite different names*

### Comparing `atelier_toolbox-1.0.3/PKG-INFO` & `atelier_toolbox-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atelier-toolbox
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tools for various automations 🧰
 Home-page: https://github.com/mihaichris/atelier-toolbox
 License: MIT
 Keywords: toolbox,automation,poetry
 Author: Mihai
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

