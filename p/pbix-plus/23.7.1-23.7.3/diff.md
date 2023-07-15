# Comparing `tmp/pbix_plus-23.7.1.tar.gz` & `tmp/pbix_plus-23.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbix_plus-23.7.1.tar", last modified: Sat Jul 15 06:34:05 2023, max compression
+gzip compressed data, was "pbix_plus-23.7.3.tar", last modified: Sat Jul 15 07:32:45 2023, max compression
```

## Comparing `pbix_plus-23.7.1.tar` & `pbix_plus-23.7.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 06:34:05.912562 pbix_plus-23.7.1/
--rw-rw-rw-   0        0        0       69 2023-07-15 06:34:05.911561 pbix_plus-23.7.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-15 06:34:05.891591 pbix_plus-23.7.1/pbix_plus/
--rw-rw-rw-   0        0        0       48 2023-07-15 05:57:54.000000 pbix_plus-23.7.1/pbix_plus/__init__.py
--rw-rw-rw-   0        0        0     2054 2023-07-15 06:01:07.000000 pbix_plus-23.7.1/pbix_plus/pbix_refresher.py
-drwxrwxrwx   0        0        0        0 2023-07-15 06:34:05.906566 pbix_plus-23.7.1/pbix_plus.egg-info/
--rw-rw-rw-   0        0        0       69 2023-07-15 06:34:05.000000 pbix_plus-23.7.1/pbix_plus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-07-15 06:34:05.000000 pbix_plus-23.7.1/pbix_plus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 06:34:05.000000 pbix_plus-23.7.1/pbix_plus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-15 06:34:05.000000 pbix_plus-23.7.1/pbix_plus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 06:34:05.913567 pbix_plus-23.7.1/setup.cfg
--rw-rw-rw-   0        0        0      215 2023-07-15 06:32:52.000000 pbix_plus-23.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 07:32:45.067423 pbix_plus-23.7.3/
+-rw-rw-rw-   0        0        0       96 2023-07-15 07:32:45.066412 pbix_plus-23.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2023-07-15 07:22:48.000000 pbix_plus-23.7.3/license.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 07:32:45.049433 pbix_plus-23.7.3/pbix_plus/
+-rw-rw-rw-   0        0        0       48 2023-07-15 05:57:54.000000 pbix_plus-23.7.3/pbix_plus/__init__.py
+-rw-rw-rw-   0        0        0     2054 2023-07-15 06:01:07.000000 pbix_plus-23.7.3/pbix_plus/pbix_refresher.py
+drwxrwxrwx   0        0        0        0 2023-07-15 07:32:45.062426 pbix_plus-23.7.3/pbix_plus.egg-info/
+-rw-rw-rw-   0        0        0       96 2023-07-15 07:32:44.000000 pbix_plus-23.7.3/pbix_plus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-15 07:32:44.000000 pbix_plus-23.7.3/pbix_plus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 07:32:44.000000 pbix_plus-23.7.3/pbix_plus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-15 07:32:44.000000 pbix_plus-23.7.3/pbix_plus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 07:32:45.067423 pbix_plus-23.7.3/setup.cfg
+-rw-rw-rw-   0        0        0      215 2023-07-15 07:31:46.000000 pbix_plus-23.7.3/setup.py
```

### Comparing `pbix_plus-23.7.1/pbix_plus/pbix_refresher.py` & `pbix_plus-23.7.3/pbix_plus/pbix_refresher.py`

 * *Files identical despite different names*

