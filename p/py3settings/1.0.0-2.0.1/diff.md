# Comparing `tmp/py3settings-1.0.0.tar.gz` & `tmp/py3settings-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3settings-1.0.0.tar", last modified: Fri Jul 14 16:31:53 2023, max compression
+gzip compressed data, was "py3settings-2.0.1.tar", last modified: Fri Jul 14 22:20:08 2023, max compression
```

## Comparing `py3settings-1.0.0.tar` & `py3settings-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 16:31:53.925856 py3settings-1.0.0/
--rw-rw-rw-   0        0        0      588 2023-07-14 16:31:53.925856 py3settings-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-07-14 16:12:21.000000 py3settings-1.0.0/README.md
--rw-rw-rw-   0        0        0      108 2023-07-14 16:31:07.000000 py3settings-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      695 2023-07-14 16:31:53.926856 py3settings-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-14 16:31:53.905357 py3settings-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:31:53.911863 py3settings-1.0.0/src/py3Settings/
--rw-rw-rw-   0        0        0       94 2023-07-14 16:11:52.000000 py3settings-1.0.0/src/py3Settings/__init__.py
--rw-rw-rw-   0        0        0      482 2023-07-14 16:24:20.000000 py3settings-1.0.0/src/py3Settings/example.py
--rw-rw-rw-   0        0        0     3143 2023-07-14 16:08:38.000000 py3settings-1.0.0/src/py3Settings/main.py
-drwxrwxrwx   0        0        0        0 2023-07-14 16:31:53.924852 py3settings-1.0.0/src/py3settings.egg-info/
--rw-rw-rw-   0        0        0      588 2023-07-14 16:31:53.000000 py3settings-1.0.0/src/py3settings.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-07-14 16:31:53.000000 py3settings-1.0.0/src/py3settings.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 16:31:53.000000 py3settings-1.0.0/src/py3settings.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-14 16:31:53.000000 py3settings-1.0.0/src/py3settings.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 22:20:08.559549 py3settings-2.0.1/
+-rw-rw-rw-   0        0        0      588 2023-07-14 22:20:08.559549 py3settings-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-07-14 16:12:21.000000 py3settings-2.0.1/README.md
+-rw-rw-rw-   0        0        0      108 2023-07-14 16:31:07.000000 py3settings-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      695 2023-07-14 22:20:08.560561 py3settings-2.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-14 22:20:08.540549 py3settings-2.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-14 22:20:08.547552 py3settings-2.0.1/src/py3Settings/
+-rw-rw-rw-   0        0        0      113 2023-07-14 22:17:00.000000 py3settings-2.0.1/src/py3Settings/__init__.py
+-rw-rw-rw-   0        0        0      616 2023-07-14 22:06:08.000000 py3settings-2.0.1/src/py3Settings/example.py
+-rw-rw-rw-   0        0        0      353 2023-07-14 22:00:44.000000 py3settings-2.0.1/src/py3Settings/file.py
+-rw-rw-rw-   0        0        0     6333 2023-07-14 22:07:29.000000 py3settings-2.0.1/src/py3Settings/main.py
+drwxrwxrwx   0        0        0        0 2023-07-14 22:20:08.558548 py3settings-2.0.1/src/py3settings.egg-info/
+-rw-rw-rw-   0        0        0      588 2023-07-14 22:20:08.000000 py3settings-2.0.1/src/py3settings.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-07-14 22:20:08.000000 py3settings-2.0.1/src/py3settings.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 22:20:08.000000 py3settings-2.0.1/src/py3settings.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-14 22:20:08.000000 py3settings-2.0.1/src/py3settings.egg-info/top_level.txt
```

### Comparing `py3settings-1.0.0/PKG-INFO` & `py3settings-2.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3settings
-Version: 1.0.0
+Version: 2.0.1
 Summary: A powerful json file settings manager for Python 3
 Home-page: https://github.com/acalasanzs/py3Settings
 Author: Albert Calasanz Sallen
 Author-email: acalasanzs@gmail.com
 Project-URL: Bug Tracker, https://github.com/acalasanzs/py3Settings/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3settings-1.0.0/setup.cfg` & `py3settings-2.0.1/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7933 7365 7474 696e 6773 0d0a   = py3settings..
-00000020: 7665 7273 696f 6e20 3d20 312e 302e 300d  version = 1.0.0.
+00000020: 7665 7273 696f 6e20 3d20 322e 302e 310d  version = 2.0.1.
 00000030: 0a61 7574 686f 7220 3d20 416c 6265 7274  .author = Albert
 00000040: 2043 616c 6173 616e 7a20 5361 6c6c 656e   Calasanz Sallen
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2061 6361 6c61 7361 6e7a 7340 676d 6169   acalasanzs@gmai
 00000070: 6c2e 636f 6d0d 0a64 6573 6372 6970 7469  l.com..descripti
 00000080: 6f6e 203d 2041 2070 6f77 6572 6675 6c20  on = A powerful 
 00000090: 6a73 6f6e 2066 696c 6520 7365 7474 696e  json file settin
```

### Comparing `py3settings-1.0.0/src/py3settings.egg-info/PKG-INFO` & `py3settings-2.0.1/src/py3settings.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3settings
-Version: 1.0.0
+Version: 2.0.1
 Summary: A powerful json file settings manager for Python 3
 Home-page: https://github.com/acalasanzs/py3Settings
 Author: Albert Calasanz Sallen
 Author-email: acalasanzs@gmail.com
 Project-URL: Bug Tracker, https://github.com/acalasanzs/py3Settings/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

