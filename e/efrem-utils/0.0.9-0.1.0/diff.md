# Comparing `tmp/efrem_utils-0.0.9.tar.gz` & `tmp/efrem_utils-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efrem_utils-0.0.9.tar", max compression
+gzip compressed data, was "efrem_utils-0.1.0.tar", max compression
```

## Comparing `efrem_utils-0.0.9.tar` & `efrem_utils-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2189 2023-07-13 15:07:11.403793 efrem_utils-0.0.9/efrem_utils.py
--rw-r--r--   0        0        0     1087 2023-07-13 00:02:18.108824 efrem_utils-0.0.9/LICENSE
--rw-r--r--   0        0        0      361 2023-07-13 15:08:13.495597 efrem_utils-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      192 2023-07-13 15:06:47.791531 efrem_utils-0.0.9/README.md
--rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 efrem_utils-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     2189 2023-07-14 09:31:24.930214 efrem_utils-0.1.0/efrem_utils.py
+-rw-r--r--   0        0        0     1087 2023-07-13 00:02:18.108824 efrem_utils-0.1.0/LICENSE
+-rw-r--r--   0        0        0      361 2023-07-15 19:42:35.485880 efrem_utils-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2560 2023-07-15 19:46:30.761405 efrem_utils-0.1.0/README.md
+-rw-r--r--   0        0        0     2943 1970-01-01 00:00:00.000000 efrem_utils-0.1.0/PKG-INFO
```

### Comparing `efrem_utils-0.0.9/efrem_utils.py` & `efrem_utils-0.1.0/efrem_utils.py`

 * *Files identical despite different names*

### Comparing `efrem_utils-0.0.9/LICENSE` & `efrem_utils-0.1.0/LICENSE`

 * *Files identical despite different names*

