# Comparing `tmp/dbt_loom-0.1.0.tar.gz` & `tmp/dbt_loom-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_loom-0.1.0.tar", max compression
+gzip compressed data, was "dbt_loom-0.1.1.tar", max compression
```

## Comparing `dbt_loom-0.1.0.tar` & `dbt_loom-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     1843 2023-07-14 20:56:46.447890 dbt_loom-0.1.0/README.md
--rw-r--r--   0        0        0     4797 2023-07-14 01:44:39.452701 dbt_loom-0.1.0/dbt_loom/__init__.py
--rw-r--r--   0        0        0      412 2023-07-13 01:12:03.957975 dbt_loom-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2348 1970-01-01 00:00:00.000000 dbt_loom-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-15 15:02:27.527145 dbt_loom-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1843 2023-07-15 15:02:27.527145 dbt_loom-0.1.1/README.md
+-rw-r--r--   0        0        0     5343 2023-07-15 15:02:27.527145 dbt_loom-0.1.1/dbt_loom/__init__.py
+-rw-r--r--   0        0        0      716 2023-07-15 15:02:27.527145 dbt_loom-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2344 1970-01-01 00:00:00.000000 dbt_loom-0.1.1/PKG-INFO
```

### Comparing `dbt_loom-0.1.0/README.md` & `dbt_loom-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.1.0/PKG-INFO` & `dbt_loom-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: dbt-loom
-Version: 0.1.0
+Version: 0.1.1
 Summary: A dbt-core plugin to import public nodes in multi-project deployments.
 Author: Nicholas Yager
 Author-email: yager@nicholasyager.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dbt-postgres (==1.6.0-b8)
+Requires-Dist: dbt-core (==1.6.0-b8)
 Description-Content-Type: text/markdown
 
 # dbt-loom
 A dbt-core plugin to support multi-project deployments.
 
 :warning: **This package depends on dbt-core's plugin functionality, which is still in beta. Please note that this may 
 break in the future as dbt Labs solidifies the dbt plugin API.**
```

