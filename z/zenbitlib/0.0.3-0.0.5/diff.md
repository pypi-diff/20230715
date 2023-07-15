# Comparing `tmp/zenbitlib-0.0.3.tar.gz` & `tmp/zenbitlib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenbitlib-0.0.3.tar", last modified: Sat Jul 15 05:55:49 2023, max compression
+gzip compressed data, was "zenbitlib-0.0.5.tar", last modified: Sat Jul 15 13:10:42 2023, max compression
```

## Comparing `zenbitlib-0.0.3.tar` & `zenbitlib-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 05:55:49.625589 zenbitlib-0.0.3/
--rw-rw-rw-   0        0        0     1091 2023-07-15 04:13:46.000000 zenbitlib-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      586 2023-07-15 05:55:49.625589 zenbitlib-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       73 2023-07-15 05:22:08.000000 zenbitlib-0.0.3/README.md
--rw-rw-rw-   0        0        0      591 2023-07-15 05:55:19.000000 zenbitlib-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-15 05:55:49.625589 zenbitlib-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-15 05:55:49.607781 zenbitlib-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-15 05:55:49.613833 zenbitlib-0.0.3/src/zenbitlib/
--rw-rw-rw-   0        0        0        0 2023-07-15 04:08:39.000000 zenbitlib-0.0.3/src/zenbitlib/__init__.py
--rw-rw-rw-   0        0        0       72 2023-07-15 05:52:23.000000 zenbitlib-0.0.3/src/zenbitlib/zenproject.py
--rw-rw-rw-   0        0        0     1981 2023-07-15 05:55:14.000000 zenbitlib-0.0.3/src/zenbitlib/zenutils.py
-drwxrwxrwx   0        0        0        0 2023-07-15 05:55:49.624577 zenbitlib-0.0.3/src/zenbitlib.egg-info/
--rw-rw-rw-   0        0        0      586 2023-07-15 05:55:49.000000 zenbitlib-0.0.3/src/zenbitlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-07-15 05:55:49.000000 zenbitlib-0.0.3/src/zenbitlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 05:55:49.000000 zenbitlib-0.0.3/src/zenbitlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-15 05:55:49.000000 zenbitlib-0.0.3/src/zenbitlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 13:10:42.742583 zenbitlib-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-07-15 04:13:46.000000 zenbitlib-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      586 2023-07-15 13:10:42.742583 zenbitlib-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2023-07-15 05:22:08.000000 zenbitlib-0.0.5/README.md
+-rw-rw-rw-   0        0        0      591 2023-07-15 13:10:10.000000 zenbitlib-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-15 13:10:42.742583 zenbitlib-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-15 13:10:42.718009 zenbitlib-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-15 13:10:42.730586 zenbitlib-0.0.5/src/zenbitlib/
+-rw-rw-rw-   0        0        0        0 2023-07-15 04:08:39.000000 zenbitlib-0.0.5/src/zenbitlib/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-07-15 05:52:23.000000 zenbitlib-0.0.5/src/zenbitlib/zenproject.py
+-rw-rw-rw-   0        0        0     4404 2023-07-15 06:44:06.000000 zenbitlib-0.0.5/src/zenbitlib/zenutils.py
+drwxrwxrwx   0        0        0        0 2023-07-15 13:10:42.741583 zenbitlib-0.0.5/src/zenbitlib.egg-info/
+-rw-rw-rw-   0        0        0      586 2023-07-15 13:10:42.000000 zenbitlib-0.0.5/src/zenbitlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-07-15 13:10:42.000000 zenbitlib-0.0.5/src/zenbitlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 13:10:42.000000 zenbitlib-0.0.5/src/zenbitlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-15 13:10:42.000000 zenbitlib-0.0.5/src/zenbitlib.egg-info/top_level.txt
```

### Comparing `zenbitlib-0.0.3/LICENSE` & `zenbitlib-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zenbitlib-0.0.3/PKG-INFO` & `zenbitlib-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenbitlib
-Version: 0.0.3
+Version: 0.0.5
 Summary: A package for quick qml learning
 Author-email: zenzenwang <zenwang@outlook.com>
 Project-URL: Homepage, https://github.com/zenzen891/zenlib/
 Project-URL: Bug Tracker, https://github.com/zenzen891/zenlib/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `zenbitlib-0.0.3/pyproject.toml` & `zenbitlib-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zenbitlib"
-version = "0.0.3"
+version = "0.0.5"
 authors = [
   { name="zenzenwang", email="zenwang@outlook.com" },
 ]
 description = "A package for quick qml learning"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `zenbitlib-0.0.3/src/zenbitlib.egg-info/PKG-INFO` & `zenbitlib-0.0.5/src/zenbitlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenbitlib
-Version: 0.0.3
+Version: 0.0.5
 Summary: A package for quick qml learning
 Author-email: zenzenwang <zenwang@outlook.com>
 Project-URL: Homepage, https://github.com/zenzen891/zenlib/
 Project-URL: Bug Tracker, https://github.com/zenzen891/zenlib/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

