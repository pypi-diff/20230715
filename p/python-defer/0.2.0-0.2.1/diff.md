# Comparing `tmp/python_defer-0.2.0.tar.gz` & `tmp/python_defer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_defer-0.2.0.tar", max compression
+gzip compressed data, was "python_defer-0.2.1.tar", max compression
```

## Comparing `python_defer-0.2.0.tar` & `python_defer-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0       34 2023-07-04 01:47:36.133244 python_defer-0.2.0/defer/__init__.py
--rw-r--r--   0        0        0      935 2023-07-04 01:22:30.431593 python_defer-0.2.0/defer/_defer.py
--rw-r--r--   0        0        0      646 2023-07-04 04:14:17.127049 python_defer-0.2.0/defer/defer.py
--rw-r--r--   0        0        0      333 2023-07-04 01:24:59.603625 python_defer-0.2.0/defer/errors.py
--rw-r--r--   0        0        0      232 2023-07-04 02:09:25.630570 python_defer-0.2.0/defer/sugar/__init__.py
--rw-r--r--   0        0        0     2047 2023-07-04 02:04:55.636063 python_defer-0.2.0/defer/sugar/_parse.py
--rw-r--r--   0        0        0     1879 2023-07-04 01:28:43.755218 python_defer-0.2.0/defer/sugar/transformer.py
--rw-r--r--   0        0        0      229 2023-07-04 04:13:20.784775 python_defer-0.2.0/defer/sugarfree/__init__.py
--rw-r--r--   0        0        0      462 2023-07-04 04:50:12.269413 python_defer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 python_defer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1498 2023-07-04 04:49:46.304195 python_defer-0.2.1/README.md
+-rw-r--r--   0        0        0       34 2023-07-04 01:47:36.133244 python_defer-0.2.1/defer/__init__.py
+-rw-r--r--   0        0        0      935 2023-07-04 01:22:30.431593 python_defer-0.2.1/defer/_defer.py
+-rw-r--r--   0        0        0      646 2023-07-04 04:14:17.127049 python_defer-0.2.1/defer/defer.py
+-rw-r--r--   0        0        0      333 2023-07-04 01:24:59.603625 python_defer-0.2.1/defer/errors.py
+-rw-r--r--   0        0        0      232 2023-07-04 02:09:25.630570 python_defer-0.2.1/defer/sugar/__init__.py
+-rw-r--r--   0        0        0     2047 2023-07-04 02:04:55.636063 python_defer-0.2.1/defer/sugar/_parse.py
+-rw-r--r--   0        0        0     1879 2023-07-04 01:28:43.755218 python_defer-0.2.1/defer/sugar/transformer.py
+-rw-r--r--   0        0        0      229 2023-07-04 04:13:20.784775 python_defer-0.2.1/defer/sugarfree/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-15 06:52:26.341627 python_defer-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 python_defer-0.2.1/PKG-INFO
```

### Comparing `python_defer-0.2.0/defer/_defer.py` & `python_defer-0.2.1/defer/_defer.py`

 * *Files identical despite different names*

### Comparing `python_defer-0.2.0/defer/defer.py` & `python_defer-0.2.1/defer/defer.py`

 * *Files identical despite different names*

### Comparing `python_defer-0.2.0/defer/sugar/_parse.py` & `python_defer-0.2.1/defer/sugar/_parse.py`

 * *Files identical despite different names*

### Comparing `python_defer-0.2.0/defer/sugar/transformer.py` & `python_defer-0.2.1/defer/sugar/transformer.py`

 * *Files identical despite different names*

