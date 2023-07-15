# Comparing `tmp/examon_core-1.0.0.tar.gz` & `tmp/examon_core-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon_core-1.0.0.tar", max compression
+gzip compressed data, was "examon_core-1.0.1.tar", max compression
```

## Comparing `examon_core-1.0.0.tar` & `examon_core-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      199 2023-05-28 20:39:21.972747 examon_core-1.0.0/examon_core/__init__.py
--rw-r--r--   0        0        0     1124 2023-06-23 14:33:10.060860 examon_core-1.0.0/examon_core/code_metrics.py
--rwxr-xr-x   0        0        0      705 2023-05-28 20:45:23.567671 examon_core-1.0.0/examon_core/examon_item.py
--rwxr-xr-x   0        0        0      478 2023-06-23 14:39:27.007604 examon_core-1.0.0/examon_core/examon_item_registry.py
--rwxr-xr-x   0        0        0     1761 2023-06-23 14:39:27.015545 examon_core-1.0.0/examon_core/function_raw_code.py
--rw-r--r--   0        0        0      389 2023-06-23 14:39:26.999135 examon_core-1.0.0/examon_core/multi_choice_factory.py
--rw-r--r--   0        0        0      751 2023-05-28 16:34:39.065018 examon_core-1.0.0/examon_core/print_ext.py
--rwxr-xr-x   0        0        0      621 2023-05-23 09:37:48.400052 examon_core-1.0.0/examon_core/question.py
--rw-r--r--   0        0        0     2525 2023-06-23 14:33:10.050623 examon_core-1.0.0/examon_core/question_factory.py
--rwxr-xr-x   0        0        0      190 2023-05-08 16:43:26.032452 examon_core-1.0.0/examon_core/question_response.py
--rw-r--r--   0        0        0      107 2023-06-23 14:39:27.010739 examon_core-1.0.0/examon_core/todo.md
--rw-r--r--   0        0        0      480 2023-07-07 13:27:32.172211 examon_core-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 examon_core-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      199 2023-05-28 20:39:21.972747 examon_core-1.0.1/examon_core/__init__.py
+-rw-r--r--   0        0        0     1124 2023-06-23 14:33:10.060860 examon_core-1.0.1/examon_core/code_metrics.py
+-rwxr-xr-x   0        0        0      705 2023-05-28 20:45:23.567671 examon_core-1.0.1/examon_core/examon_item.py
+-rwxr-xr-x   0        0        0      478 2023-06-23 14:39:27.007604 examon_core-1.0.1/examon_core/examon_item_registry.py
+-rwxr-xr-x   0        0        0     1761 2023-06-23 14:39:27.015545 examon_core-1.0.1/examon_core/function_raw_code.py
+-rw-r--r--   0        0        0      389 2023-06-23 14:39:26.999135 examon_core-1.0.1/examon_core/multi_choice_factory.py
+-rw-r--r--   0        0        0      751 2023-05-28 16:34:39.065018 examon_core-1.0.1/examon_core/print_ext.py
+-rwxr-xr-x   0        0        0      621 2023-05-23 09:37:48.400052 examon_core-1.0.1/examon_core/question.py
+-rw-r--r--   0        0        0     2525 2023-06-23 14:33:10.050623 examon_core-1.0.1/examon_core/question_factory.py
+-rwxr-xr-x   0        0        0      201 2023-07-15 15:48:50.722464 examon_core-1.0.1/examon_core/question_response.py
+-rw-r--r--   0        0        0      107 2023-06-23 14:39:27.010739 examon_core-1.0.1/examon_core/todo.md
+-rw-r--r--   0        0        0      517 2023-07-15 19:31:39.430003 examon_core-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 examon_core-1.0.1/PKG-INFO
```

### Comparing `examon_core-1.0.0/examon_core/code_metrics.py` & `examon_core-1.0.1/examon_core/code_metrics.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.0/examon_core/examon_item.py` & `examon_core-1.0.1/examon_core/examon_item.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.0/examon_core/function_raw_code.py` & `examon_core-1.0.1/examon_core/function_raw_code.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.0/examon_core/print_ext.py` & `examon_core-1.0.1/examon_core/print_ext.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.0/examon_core/question.py` & `examon_core-1.0.1/examon_core/question.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.0.0/examon_core/question_factory.py` & `examon_core-1.0.1/examon_core/question_factory.py`

 * *Files identical despite different names*

