# Comparing `tmp/carica_dynamodb_tools-1.4.tar.gz` & `tmp/carica_dynamodb_tools-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carica_dynamodb_tools-1.4.tar", last modified: Sat Jan 29 02:21:29 2022, max compression
+gzip compressed data, was "carica_dynamodb_tools-1.5.tar", last modified: Sat Jul 15 19:32:20 2023, max compression
```

## Comparing `carica_dynamodb_tools-1.4.tar` & `carica_dynamodb_tools-1.5.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxr-x   0 sterwill  (1000) sterwill  (1000)        0 2022-01-29 02:21:29.100144 carica_dynamodb_tools-1.4/
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)    11358 2021-11-16 14:20:22.000000 carica_dynamodb_tools-1.4/LICENSE
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)     1254 2022-01-29 02:21:29.100144 carica_dynamodb_tools-1.4/PKG-INFO
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      651 2021-12-13 18:39:28.000000 carica_dynamodb_tools-1.4/README.rst
-drwxrwxr-x   0 sterwill  (1000) sterwill  (1000)        0 2022-01-29 02:21:29.100144 carica_dynamodb_tools-1.4/carica_dynamodb_tools/
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)        0 2021-11-16 14:20:22.000000 carica_dynamodb_tools-1.4/carica_dynamodb_tools/__init__.py
--rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)     2033 2022-01-29 02:20:51.000000 carica_dynamodb_tools-1.4/carica_dynamodb_tools/dump.py
--rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)     5931 2021-11-16 15:20:40.000000 carica_dynamodb_tools-1.4/carica_dynamodb_tools/load.py
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      593 2021-11-16 15:20:28.000000 carica_dynamodb_tools-1.4/carica_dynamodb_tools/session.py
--rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)       20 2022-01-29 02:21:00.000000 carica_dynamodb_tools-1.4/carica_dynamodb_tools/version.py
-drwxrwxr-x   0 sterwill  (1000) sterwill  (1000)        0 2022-01-29 02:21:29.100144 carica_dynamodb_tools-1.4/carica_dynamodb_tools.egg-info/
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)     1254 2022-01-29 02:21:29.000000 carica_dynamodb_tools-1.4/carica_dynamodb_tools.egg-info/PKG-INFO
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      484 2022-01-29 02:21:29.000000 carica_dynamodb_tools-1.4/carica_dynamodb_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)        1 2022-01-29 02:21:29.000000 carica_dynamodb_tools-1.4/carica_dynamodb_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      127 2022-01-29 02:21:29.000000 carica_dynamodb_tools-1.4/carica_dynamodb_tools.egg-info/entry_points.txt
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)       55 2022-01-29 02:21:29.000000 carica_dynamodb_tools-1.4/carica_dynamodb_tools.egg-info/requires.txt
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)       22 2022-01-29 02:21:29.000000 carica_dynamodb_tools-1.4/carica_dynamodb_tools.egg-info/top_level.txt
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)       45 2021-11-16 14:20:22.000000 carica_dynamodb_tools-1.4/pyproject.toml
--rw-rw-r--   0 sterwill  (1000) sterwill  (1000)       67 2022-01-29 02:21:29.100144 carica_dynamodb_tools-1.4/setup.cfg
--rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)     1620 2021-11-16 15:26:18.000000 carica_dynamodb_tools-1.4/setup.py
+drwxrwxr-x   0 sterwill  (1000) sterwill  (1000)        0 2023-07-15 19:32:20.399934 carica_dynamodb_tools-1.5/
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)    11358 2021-11-16 14:20:22.000000 carica_dynamodb_tools-1.5/LICENSE
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)     1395 2023-07-15 19:32:20.399934 carica_dynamodb_tools-1.5/PKG-INFO
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      651 2023-04-08 13:04:58.000000 carica_dynamodb_tools-1.5/README.rst
+drwxrwxr-x   0 sterwill  (1000) sterwill  (1000)        0 2023-07-15 19:32:20.399934 carica_dynamodb_tools-1.5/carica_dynamodb_tools/
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)        0 2021-11-16 14:20:22.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools/__init__.py
+-rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)      977 2023-07-15 18:48:48.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools/dump.py
+-rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)     6212 2023-07-15 19:24:30.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools/dump_s3_export.py
+-rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)     5931 2023-04-08 13:07:12.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools/load.py
+-rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)     2085 2023-07-15 19:22:19.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools/s3_export.py
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      593 2021-11-16 15:20:28.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools/session.py
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      262 2023-07-15 18:48:48.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools/utils.py
+-rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)       20 2023-07-15 19:31:33.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools/version.py
+drwxrwxr-x   0 sterwill  (1000) sterwill  (1000)        0 2023-07-15 19:32:20.399934 carica_dynamodb_tools-1.5/carica_dynamodb_tools.egg-info/
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)     1395 2023-07-15 19:32:20.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      590 2023-07-15 19:32:20.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)        1 2023-07-15 19:32:20.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)      265 2023-07-15 19:32:20.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)       55 2023-07-15 19:32:20.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools.egg-info/requires.txt
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)       22 2023-07-15 19:32:20.000000 carica_dynamodb_tools-1.5/carica_dynamodb_tools.egg-info/top_level.txt
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)       46 2023-03-02 19:05:06.000000 carica_dynamodb_tools-1.5/pyproject.toml
+-rw-rw-r--   0 sterwill  (1000) sterwill  (1000)       67 2023-07-15 19:32:20.399934 carica_dynamodb_tools-1.5/setup.cfg
+-rwxrwxr-x   0 sterwill  (1000) sterwill  (1000)     1784 2023-07-15 19:17:19.000000 carica_dynamodb_tools-1.5/setup.py
```

### Comparing `carica_dynamodb_tools-1.4/LICENSE` & `carica_dynamodb_tools-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `carica_dynamodb_tools-1.4/PKG-INFO` & `carica_dynamodb_tools-1.5/carica_dynamodb_tools.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 Metadata-Version: 2.1
-Name: carica_dynamodb_tools
-Version: 1.4
+Name: carica-dynamodb-tools
+Version: 1.5
 Summary: Tools to manage DynamoDB tables
 Home-page: https://github.com/caricalabs/carica-dynamodb-tools
 Author: Carica Labs, LLC
 Author-email: info@caricalabs.com
 License: APL 2.0
+Description: carica-dynamodb-tools - Tools to manage DynamoDB tables
+        ==================================================================================
+        
+        Simple backup and restore utilities for DynamoDB tables.
+        
+        Development
+        -----------
+        
+        The ``vinstall`` script uses the `venv` module to prepare a Python environment useful
+        for development, so you don't have to build and install carica-dynamodb-tools to be
+        able to run and test it.
+        
+        #. Run ``./vinstall``
+        #. Activate the virtual environment by running ``. ./venv/bin/activate``
+        #. The ``console_scripts`` listed in ``setup.py`` are now in your path, so you
+           can simply run them like:
+        
+           ``carica-dynamodb ...``
+        
+        
 Keywords: dynamodb backup restore archive dump load
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: dev
 Provides-Extra: test
-License-File: LICENSE
-
-carica-dynamodb-tools - Tools to manage DynamoDB tables
-==================================================================================
-
-Simple backup and restore utilities for DynamoDB tables.
-
-Development
------------
-
-The ``vinstall`` script uses the `venv` module to prepare a Python environment useful
-for development, so you don't have to build and install carica-dynamodb-tools to be
-able to run and test it.
-
-#. Run ``./vinstall``
-#. Activate the virtual environment by running ``. ./venv/bin/activate``
-#. The ``console_scripts`` listed in ``setup.py`` are now in your path, so you
-   can simply run them like:
-
-   ``carica-dynamodb ...``
-
-
-
```

### Comparing `carica_dynamodb_tools-1.4/README.rst` & `carica_dynamodb_tools-1.5/README.rst`

 * *Files identical despite different names*

### Comparing `carica_dynamodb_tools-1.4/carica_dynamodb_tools/load.py` & `carica_dynamodb_tools-1.5/carica_dynamodb_tools/load.py`

 * *Files identical despite different names*

### Comparing `carica_dynamodb_tools-1.4/carica_dynamodb_tools/session.py` & `carica_dynamodb_tools-1.5/carica_dynamodb_tools/session.py`

 * *Files identical despite different names*

### Comparing `carica_dynamodb_tools-1.4/setup.py` & `carica_dynamodb_tools-1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,11 +44,13 @@
         'dev': ['check-manifest'],
         'test': [],
     },
     package_data={},
     entry_points={
         'console_scripts': [
             'carica-dynamodb-dump=carica_dynamodb_tools.dump:cli',
+            'carica-dynamodb-dump-s3-export=carica_dynamodb_tools.dump_s3_export:cli',
             'carica-dynamodb-load=carica_dynamodb_tools.load:cli',
+            'carica-dynamodb-s3-export=carica_dynamodb_tools.s3_export:cli',
         ],
     },
 )
```

