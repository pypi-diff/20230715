# Comparing `tmp/shil-2023.7.15.10.43.tar.gz` & `tmp/shil-2023.7.15.12.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shil-2023.7.15.10.43.tar", last modified: Sat Jul 15 10:43:43 2023, max compression
+gzip compressed data, was "shil-2023.7.15.12.33.tar", last modified: Sat Jul 15 12:33:45 2023, max compression
```

## Comparing `shil-2023.7.15.10.43.tar` & `shil-2023.7.15.12.33.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:43:43.402336 shil-2023.7.15.10.43/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-15 10:43:43.402336 shil-2023.7.15.10.43/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-15 10:42:08.000000 shil-2023.7.15.10.43/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-15 10:43:43.402336 shil-2023.7.15.10.43/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-15 10:42:08.000000 shil-2023.7.15.10.43/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:43:43.382336 shil-2023.7.15.10.43/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:43:43.390336 shil-2023.7.15.10.43/src/shil/
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-15 10:42:47.000000 shil-2023.7.15.10.43/src/shil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-15 10:42:08.000000 shil-2023.7.15.10.43/src/shil/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-15 10:43:39.000000 shil-2023.7.15.10.43/src/shil/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-15 10:42:08.000000 shil-2023.7.15.10.43/src/shil/bin.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-15 10:42:08.000000 shil-2023.7.15.10.43/src/shil/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:43:43.402336 shil-2023.7.15.10.43/src/shil/format/
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-15 10:42:08.000000 shil-2023.7.15.10.43/src/shil/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-15 10:42:46.000000 shil-2023.7.15.10.43/src/shil/format/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-07-15 10:42:08.000000 shil-2023.7.15.10.43/src/shil/format/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-15 10:42:08.000000 shil-2023.7.15.10.43/src/shil/grammar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:43:43.402336 shil-2023.7.15.10.43/src/shil/models/
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-15 10:42:47.000000 shil-2023.7.15.10.43/src/shil/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-15 10:42:08.000000 shil-2023.7.15.10.43/src/shil/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:43:43.394336 shil-2023.7.15.10.43/src/shil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-15 10:43:43.000000 shil-2023.7.15.10.43/src/shil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-15 10:43:43.000000 shil-2023.7.15.10.43/src/shil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 10:43:43.000000 shil-2023.7.15.10.43/src/shil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 10:43:43.000000 shil-2023.7.15.10.43/src/shil.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-15 10:43:43.000000 shil-2023.7.15.10.43/src/shil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-15 10:43:43.000000 shil-2023.7.15.10.43/src/shil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:33:45.888633 shil-2023.7.15.12.33/
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-15 12:33:45.888633 shil-2023.7.15.12.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-15 12:33:45.888633 shil-2023.7.15.12.33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:33:45.884633 shil-2023.7.15.12.33/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:33:45.888633 shil-2023.7.15.12.33/src/shil/
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-15 12:32:51.000000 shil-2023.7.15.12.33/src/shil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/src/shil/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-15 12:33:41.000000 shil-2023.7.15.12.33/src/shil/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/src/shil/bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/src/shil/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:33:45.888633 shil-2023.7.15.12.33/src/shil/format/
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/src/shil/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/src/shil/format/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/src/shil/format/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/src/shil/grammar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:33:45.888633 shil-2023.7.15.12.33/src/shil/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-15 12:32:51.000000 shil-2023.7.15.12.33/src/shil/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-15 12:32:12.000000 shil-2023.7.15.12.33/src/shil/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:33:45.888633 shil-2023.7.15.12.33/src/shil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-15 12:33:45.000000 shil-2023.7.15.12.33/src/shil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-15 12:33:45.000000 shil-2023.7.15.12.33/src/shil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:33:45.000000 shil-2023.7.15.12.33/src/shil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:33:45.000000 shil-2023.7.15.12.33/src/shil.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-15 12:33:45.000000 shil-2023.7.15.12.33/src/shil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-15 12:33:45.000000 shil-2023.7.15.12.33/src/shil.egg-info/top_level.txt
```

### Comparing `shil-2023.7.15.10.43/setup.cfg` & `shil-2023.7.15.12.33/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [metadata]
 name = shil
 description = Shell helper utilities for python
 author = elo
 platforms = any
 license = MIT
 license_files = LICENSE.txt
-long_description = See the project README
-long_description_content_type = text/x-rst; charset=UTF-8
+long_description = file: README.md
+long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://github.com/elo-enterprises/shil/
 project_urls = 
 	Documentation = https://github.com/elo-enterprises/shil/
 	Source = https://github.com/elo-enterprises/shil/
 	Download = https://github.com/elo-enterprises/shil/#files
 classifiers = 
 	Programming Language :: Python
```

### Comparing `shil-2023.7.15.10.43/setup.py` & `shil-2023.7.15.12.33/setup.py`

 * *Files identical despite different names*

### Comparing `shil-2023.7.15.10.43/src/shil/__init__.py` & `shil-2023.7.15.12.33/src/shil/__init__.py`

 * *Files identical despite different names*

### Comparing `shil-2023.7.15.10.43/src/shil/__main__.py` & `shil-2023.7.15.12.33/src/shil/__main__.py`

 * *Files identical despite different names*

### Comparing `shil-2023.7.15.10.43/src/shil/format/__init__.py` & `shil-2023.7.15.12.33/src/shil/format/__init__.py`

 * *Files identical despite different names*

### Comparing `shil-2023.7.15.10.43/src/shil/format/__main__.py` & `shil-2023.7.15.12.33/src/shil/format/__main__.py`

 * *Files identical despite different names*

### Comparing `shil-2023.7.15.10.43/src/shil/format/grammar.py` & `shil-2023.7.15.12.33/src/shil/format/grammar.py`

 * *Files identical despite different names*

### Comparing `shil-2023.7.15.10.43/src/shil/grammar.py` & `shil-2023.7.15.12.33/src/shil/grammar.py`

 * *Files identical despite different names*

### Comparing `shil-2023.7.15.10.43/src/shil/models/__init__.py` & `shil-2023.7.15.12.33/src/shil/models/__init__.py`

 * *Files identical despite different names*

### Comparing `shil-2023.7.15.10.43/src/shil/util.py` & `shil-2023.7.15.12.33/src/shil/util.py`

 * *Files identical despite different names*

