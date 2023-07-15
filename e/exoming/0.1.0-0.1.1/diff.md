# Comparing `tmp/exoming-0.1.0.tar.gz` & `tmp/exoming-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exoming-0.1.0.tar", max compression
+gzip compressed data, was "exoming-0.1.1.tar", max compression
```

## Comparing `exoming-0.1.0.tar` & `exoming-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-07-14 12:19:56.917811 exoming-0.1.0/exoming/__init__.py
--rw-r--r--   0        0        0     1185 2023-07-15 03:39:28.797463 exoming-0.1.0/exoming/command.py
--rw-r--r--   0        0        0     3830 2023-07-14 13:01:11.683211 exoming-0.1.0/exoming/exomIO.py
--rw-r--r--   0        0        0      269 2023-07-15 03:36:43.658498 exoming-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      320 1970-01-01 00:00:00.000000 exoming-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-14 12:19:56.917811 exoming-0.1.1/exoming/__init__.py
+-rw-r--r--   0        0        0     1185 2023-07-15 03:39:28.797463 exoming-0.1.1/exoming/command.py
+-rw-r--r--   0        0        0     3830 2023-07-14 13:01:11.683211 exoming-0.1.1/exoming/exomIO.py
+-rw-r--r--   0        0        0      269 2023-07-15 03:40:05.097401 exoming-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      320 1970-01-01 00:00:00.000000 exoming-0.1.1/PKG-INFO
```

### Comparing `exoming-0.1.0/exoming/command.py` & `exoming-0.1.1/exoming/command.py`

 * *Files identical despite different names*

### Comparing `exoming-0.1.0/exoming/exomIO.py` & `exoming-0.1.1/exoming/exomIO.py`

 * *Files identical despite different names*

