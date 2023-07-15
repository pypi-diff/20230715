# Comparing `tmp/plover_regenpfeifer-1.1.0.tar.gz` & `tmp/plover_regenpfeifer-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plover_regenpfeifer-1.1.0.tar", last modified: Sat Mar  4 07:20:49 2023, max compression
+gzip compressed data, was "plover_regenpfeifer-1.1.1.tar", last modified: Sat Jul 15 10:42:40 2023, max compression
```

## Comparing `plover_regenpfeifer-1.1.0.tar` & `plover_regenpfeifer-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 07:20:49.486082 plover_regenpfeifer-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-04 07:20:39.000000 plover_regenpfeifer-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-04 07:20:39.000000 plover_regenpfeifer-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-04 07:20:49.486082 plover_regenpfeifer-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-04 07:20:39.000000 plover_regenpfeifer-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 07:20:49.474082 plover_regenpfeifer-1.1.0/plover_regenpfeifer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 07:20:39.000000 plover_regenpfeifer-1.1.0/plover_regenpfeifer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 07:20:49.478082 plover_regenpfeifer-1.1.0/plover_regenpfeifer/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (123)  8217533 2023-03-04 07:20:39.000000 plover_regenpfeifer-1.1.0/plover_regenpfeifer/dictionaries/regenpfeifer_main.json
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-03-04 07:20:39.000000 plover_regenpfeifer-1.1.0/plover_regenpfeifer/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 07:20:49.478082 plover_regenpfeifer-1.1.0/plover_regenpfeifer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-04 07:20:49.000000 plover_regenpfeifer-1.1.0/plover_regenpfeifer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-04 07:20:49.000000 plover_regenpfeifer-1.1.0/plover_regenpfeifer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 07:20:49.000000 plover_regenpfeifer-1.1.0/plover_regenpfeifer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-04 07:20:49.000000 plover_regenpfeifer-1.1.0/plover_regenpfeifer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-04 07:20:49.000000 plover_regenpfeifer-1.1.0/plover_regenpfeifer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-04 07:20:49.000000 plover_regenpfeifer-1.1.0/plover_regenpfeifer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 07:20:49.000000 plover_regenpfeifer-1.1.0/plover_regenpfeifer.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-04 07:20:49.486082 plover_regenpfeifer-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-04 07:20:39.000000 plover_regenpfeifer-1.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-04 07:20:39.000000 plover_regenpfeifer-1.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:42:40.197531 plover_regenpfeifer-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-15 10:42:28.000000 plover_regenpfeifer-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-15 10:42:28.000000 plover_regenpfeifer-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-15 10:42:40.197531 plover_regenpfeifer-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-15 10:42:28.000000 plover_regenpfeifer-1.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:42:40.185531 plover_regenpfeifer-1.1.1/plover_regenpfeifer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:42:28.000000 plover_regenpfeifer-1.1.1/plover_regenpfeifer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:42:40.189531 plover_regenpfeifer-1.1.1/plover_regenpfeifer/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (123)  8217533 2023-07-15 10:42:28.000000 plover_regenpfeifer-1.1.1/plover_regenpfeifer/dictionaries/regenpfeifer_main.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-15 10:42:28.000000 plover_regenpfeifer-1.1.1/plover_regenpfeifer/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:42:40.189531 plover_regenpfeifer-1.1.1/plover_regenpfeifer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-15 10:42:40.000000 plover_regenpfeifer-1.1.1/plover_regenpfeifer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-15 10:42:40.000000 plover_regenpfeifer-1.1.1/plover_regenpfeifer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 10:42:40.000000 plover_regenpfeifer-1.1.1/plover_regenpfeifer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-15 10:42:40.000000 plover_regenpfeifer-1.1.1/plover_regenpfeifer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-15 10:42:40.000000 plover_regenpfeifer-1.1.1/plover_regenpfeifer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-15 10:42:40.000000 plover_regenpfeifer-1.1.1/plover_regenpfeifer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 10:42:40.000000 plover_regenpfeifer-1.1.1/plover_regenpfeifer.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-15 10:42:40.197531 plover_regenpfeifer-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-15 10:42:28.000000 plover_regenpfeifer-1.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-15 10:42:28.000000 plover_regenpfeifer-1.1.1/tox.ini
```

### Comparing `plover_regenpfeifer-1.1.0/LICENSE` & `plover_regenpfeifer-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plover_regenpfeifer-1.1.0/PKG-INFO` & `plover_regenpfeifer-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plover_regenpfeifer
-Version: 1.1.0
+Version: 1.1.1
 Summary: German realtime system for Plover
 Home-page: https://github.com/mkrnr/plover_regenpfeifer
 Author: Martin Koerner
 Author-email: info@mkoerner.de
 License: GNU General Public License v3 or later (GPLv3+)
 Keywords: plover plover_plugin
 Classifier: Development Status :: 4 - Beta
```

### Comparing `plover_regenpfeifer-1.1.0/README.rst` & `plover_regenpfeifer-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `plover_regenpfeifer-1.1.0/plover_regenpfeifer/dictionaries/regenpfeifer_main.json` & `plover_regenpfeifer-1.1.1/plover_regenpfeifer/dictionaries/regenpfeifer_main.json`

 * *Files identical despite different names*

### Comparing `plover_regenpfeifer-1.1.0/plover_regenpfeifer/system.py` & `plover_regenpfeifer-1.1.1/plover_regenpfeifer/system.py`

 * *Files identical despite different names*

### Comparing `plover_regenpfeifer-1.1.0/plover_regenpfeifer.egg-info/PKG-INFO` & `plover_regenpfeifer-1.1.1/plover_regenpfeifer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plover-regenpfeifer
-Version: 1.1.0
+Version: 1.1.1
 Summary: German realtime system for Plover
 Home-page: https://github.com/mkrnr/plover_regenpfeifer
 Author: Martin Koerner
 Author-email: info@mkoerner.de
 License: GNU General Public License v3 or later (GPLv3+)
 Keywords: plover plover_plugin
 Classifier: Development Status :: 4 - Beta
```

### Comparing `plover_regenpfeifer-1.1.0/setup.cfg` & `plover_regenpfeifer-1.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = plover_regenpfeifer
-version = 1.1.0
+version = 1.1.1
 description = German realtime system for Plover
 long_description = file: README.rst
 author = Martin Koerner
 author_email = info@mkoerner.de
 license = GNU General Public License v3 or later (GPLv3+)
 url = https://github.com/mkrnr/plover_regenpfeifer
 classifiers = 
@@ -16,15 +16,15 @@
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 keywords = plover plover_plugin
 
 [options]
 zip_safe = True
 install_requires = 
-	plover>=4.0.0.dev1
+	plover>=5.0.0.dev1
 include_package_data = True
 packages = 
 	plover_regenpfeifer
 
 [options.entry_points]
 plover.system = 
 	Regenpfeifer = plover_regenpfeifer.system
```

