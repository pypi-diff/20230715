# Comparing `tmp/openai2-1.5.10.tar.gz` & `tmp/openai2-1.5.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai2-1.5.10.tar", last modified: Fri Jul 14 17:41:20 2023, max compression
+gzip compressed data, was "openai2-1.5.11.tar", last modified: Sat Jul 15 15:54:08 2023, max compression
```

## Comparing `openai2-1.5.10.tar` & `openai2-1.5.11.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11038 2023-07-14 17:01:09.603744 openai2-1.5.10/LICENSE
--rw-r--r--   0        0        0     2919 2023-07-14 14:42:06.502368 openai2-1.5.10/README.md
--rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.10/openai2/Dependent Packages/openai/LICENSE
--rw-r--r--   0        0        0       23 2023-05-28 06:12:32.856591 openai2-1.5.10/openai2/__init__.py
--rw-r--r--   0        0        0     2629 2023-07-14 17:14:22.791779 openai2-1.5.10/openai2/_core.py
--rw-r--r--   0        0        0      613 2023-07-14 17:41:20.470812 openai2-1.5.10/pyproject.toml
--rw-r--r--   0        0        0     3263 1970-01-01 00:00:00.000000 openai2-1.5.10/PKG-INFO
+-rw-r--r--   0        0        0    11038 2023-07-14 17:01:09.603744 openai2-1.5.11/LICENSE
+-rw-r--r--   0        0        0     8664 2023-07-15 15:35:15.008513 openai2-1.5.11/README.md
+-rw-r--r--   0        0        0     1083 2020-12-22 18:45:03.000000 openai2-1.5.11/openai2/Dependent Packages/openai/LICENSE
+-rw-r--r--   0        0        0       56 2023-07-15 11:05:31.162471 openai2-1.5.11/openai2/__init__.py
+-rw-r--r--   0        0        0     5434 2023-07-15 14:06:17.992651 openai2-1.5.11/openai2/_core.py
+-rw-r--r--   0        0        0      648 2023-07-15 15:36:52.162685 openai2-1.5.11/pyproject.toml
+-rw-r--r--   0        0        0     8899 1970-01-01 00:00:00.000000 openai2-1.5.11/PKG-INFO
```

### Comparing `openai2-1.5.10/LICENSE` & `openai2-1.5.11/LICENSE`

 * *Files identical despite different names*

### Comparing `openai2-1.5.10/openai2/Dependent Packages/openai/LICENSE` & `openai2-1.5.11/openai2/Dependent Packages/openai/LICENSE`

 * *Files identical despite different names*

