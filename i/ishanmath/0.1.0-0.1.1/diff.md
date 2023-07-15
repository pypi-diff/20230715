# Comparing `tmp/ishanmath-0.1.0.tar.gz` & `tmp/ishanmath-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ishanmath-0.1.0.tar", max compression
+gzip compressed data, was "ishanmath-0.1.1.tar", max compression
```

## Comparing `ishanmath-0.1.0.tar` & `ishanmath-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      344 2023-07-15 06:51:29.017881 ishanmath-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       13 2023-07-15 07:04:20.194171 ishanmath-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-15 06:51:29.011869 ishanmath-0.1.0/src/ishanmath/__init__.py
--rw-r--r--   0        0        0      193 2023-07-15 05:23:06.357054 ishanmath-0.1.0/src/ishanmath/exceptions.py
--rw-r--r--   0        0        0     5523 2023-07-15 06:47:43.309442 ishanmath-0.1.0/src/ishanmath/physics.py
--rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 ishanmath-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      344 2023-07-15 07:27:16.664431 ishanmath-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-07-15 07:04:20.194171 ishanmath-0.1.1/README.md
+-rw-r--r--   0        0        0       40 2023-07-15 07:27:09.014990 ishanmath-0.1.1/src/ishanmath/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-15 05:23:06.357054 ishanmath-0.1.1/src/ishanmath/exceptions.py
+-rw-r--r--   0        0        0     5523 2023-07-15 06:47:43.309442 ishanmath-0.1.1/src/ishanmath/physics.py
+-rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 ishanmath-0.1.1/PKG-INFO
```

### Comparing `ishanmath-0.1.0/src/ishanmath/physics.py` & `ishanmath-0.1.1/src/ishanmath/physics.py`

 * *Files identical despite different names*

