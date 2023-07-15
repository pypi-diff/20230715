# Comparing `tmp/omgpt-0.0.3.tar.gz` & `tmp/omgpt-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omgpt-0.0.3.tar", max compression
+gzip compressed data, was "omgpt-0.0.4.tar", max compression
```

## Comparing `omgpt-0.0.3.tar` & `omgpt-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-07-12 15:32:14.072394 omgpt-0.0.3/LICENSE
--rw-r--r--   0        0        0    10972 2023-07-14 08:42:38.371494 omgpt-0.0.3/README.md
--rw-r--r--   0        0        0     2778 2023-07-15 02:06:09.514634 omgpt-0.0.3/omgpt.py
--rw-r--r--   0        0        0      598 2023-07-15 02:47:46.706415 omgpt-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    11640 1970-01-01 00:00:00.000000 omgpt-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-12 15:32:14.072394 omgpt-0.0.4/LICENSE
+-rw-r--r--   0        0        0    10972 2023-07-14 08:42:38.371494 omgpt-0.0.4/README.md
+-rw-r--r--   0        0        0     2778 2023-07-15 02:06:09.514634 omgpt-0.0.4/omgpt.py
+-rw-r--r--   0        0        0      692 2023-07-15 03:21:45.586134 omgpt-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    11674 1970-01-01 00:00:00.000000 omgpt-0.0.4/PKG-INFO
```

### Comparing `omgpt-0.0.3/LICENSE` & `omgpt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `omgpt-0.0.3/README.md` & `omgpt-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `omgpt-0.0.3/omgpt.py` & `omgpt-0.0.4/omgpt.py`

 * *Files identical despite different names*

### Comparing `omgpt-0.0.3/PKG-INFO` & `omgpt-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: omgpt
-Version: 0.0.3
-Summary: An AI-powered command-line interface
+Version: 0.0.4
+Summary: Simplify and enhance your command-line experience with the power of AI
 Home-page: https://github.com/ywkim/omgpt
 License: MIT
 Author: Youngwook Kim
 Author-email: youngwook.kim@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

