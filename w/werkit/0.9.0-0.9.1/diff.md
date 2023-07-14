# Comparing `tmp/werkit-0.9.0.tar.gz` & `tmp/werkit-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/werkit-0.9.0.tar", last modified: Fri Jun 12 19:54:20 2020, max compression
+gzip compressed data, was "dist/werkit-0.9.1.tar", last modified: Sat Jun 13 00:29:20 2020, max compression
```

## Comparing `werkit-0.9.0.tar` & `werkit-0.9.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 pnm        (503) staff       (20)        0 2020-06-12 19:54:20.000000 werkit-0.9.0/
--rw-r--r--   0 pnm        (503) staff       (20)     1071 2019-07-22 17:09:56.000000 werkit-0.9.0/LICENSE
--rw-r--r--   0 pnm        (503) staff       (20)       80 2020-05-31 02:59:45.000000 werkit-0.9.0/MANIFEST.in
--rw-r--r--   0 pnm        (503) staff       (20)     7700 2020-06-12 19:54:20.000000 werkit-0.9.0/PKG-INFO
--rw-r--r--   0 pnm        (503) staff       (20)     5077 2020-05-25 02:49:13.000000 werkit-0.9.0/README.md
--rw-r--r--   0 pnm        (503) staff       (20)        0 2020-05-31 04:42:18.000000 werkit-0.9.0/requirements.txt
--rw-r--r--   0 pnm        (503) staff       (20)       38 2020-06-12 19:54:20.000000 werkit-0.9.0/setup.cfg
--rwxr-xr-x   0 pnm        (503) staff       (20)     1248 2020-05-31 04:42:18.000000 werkit-0.9.0/setup.py
-drwxr-xr-x   0 pnm        (503) staff       (20)        0 2020-06-12 19:54:20.000000 werkit-0.9.0/werkit/
--rw-r--r--   0 pnm        (503) staff       (20)       70 2019-07-22 18:32:13.000000 werkit-0.9.0/werkit/__init__.py
-drwxr-xr-x   0 pnm        (503) staff       (20)        0 2020-06-12 19:54:20.000000 werkit-0.9.0/werkit/aws_lambda/
--rw-r--r--   0 pnm        (503) staff       (20)        0 2020-05-25 02:49:13.000000 werkit-0.9.0/werkit/aws_lambda/__init__.py
--rw-r--r--   0 pnm        (503) staff       (20)     3140 2020-06-04 23:41:01.000000 werkit-0.9.0/werkit/aws_lambda/build.py
--rw-r--r--   0 pnm        (503) staff       (20)     2731 2020-06-12 16:20:14.000000 werkit-0.9.0/werkit/aws_lambda/default_handler.py
--rw-r--r--   0 pnm        (503) staff       (20)     2808 2020-06-12 19:50:47.000000 werkit-0.9.0/werkit/aws_lambda/deploy.py
--rw-r--r--   0 pnm        (503) staff       (20)     2079 2020-06-12 16:00:44.000000 werkit-0.9.0/werkit/aws_lambda/orchestrator_deploy.py
--rw-r--r--   0 pnm        (503) staff       (20)     2346 2020-06-12 16:20:14.000000 werkit-0.9.0/werkit/aws_lambda/parallel.py
--rw-r--r--   0 pnm        (503) staff       (20)      196 2020-06-01 20:37:18.000000 werkit-0.9.0/werkit/formatting.py
--rw-r--r--   0 pnm        (503) staff       (20)     3648 2020-06-12 16:20:14.000000 werkit-0.9.0/werkit/manager.py
--rw-r--r--   0 pnm        (503) staff       (20)       22 2020-06-12 19:54:12.000000 werkit-0.9.0/werkit/package_version.py
-drwxr-xr-x   0 pnm        (503) staff       (20)        0 2020-06-12 19:54:20.000000 werkit-0.9.0/werkit/parallel/
--rw-r--r--   0 pnm        (503) staff       (20)      217 2020-05-31 02:59:45.000000 werkit-0.9.0/werkit/parallel/__init__.py
--rw-r--r--   0 pnm        (503) staff       (20)     3259 2020-05-23 08:12:00.000000 werkit-0.9.0/werkit/parallel/cloud_manager.py
--rw-r--r--   0 pnm        (503) staff       (20)     4275 2020-05-31 02:59:45.000000 werkit-0.9.0/werkit/parallel/invoke.py
--rw-r--r--   0 pnm        (503) staff       (20)      109 2019-07-26 16:49:19.000000 werkit-0.9.0/werkit/parallel/testing.py
--rw-r--r--   0 pnm        (503) staff       (20)      830 2020-06-12 19:50:47.000000 werkit-0.9.0/werkit/s3.py
--rw-r--r--   0 pnm        (503) staff       (20)     2274 2020-06-01 20:37:18.000000 werkit-0.9.0/werkit/schema.py
-drwxr-xr-x   0 pnm        (503) staff       (20)        0 2020-06-12 19:54:20.000000 werkit-0.9.0/werkit.egg-info/
--rw-r--r--   0 pnm        (503) staff       (20)     7700 2020-06-12 19:54:20.000000 werkit-0.9.0/werkit.egg-info/PKG-INFO
--rw-r--r--   0 pnm        (503) staff       (20)      625 2020-06-12 19:54:20.000000 werkit-0.9.0/werkit.egg-info/SOURCES.txt
--rw-r--r--   0 pnm        (503) staff       (20)        1 2020-06-12 19:54:20.000000 werkit-0.9.0/werkit.egg-info/dependency_links.txt
--rw-r--r--   0 pnm        (503) staff       (20)       44 2020-06-12 19:54:20.000000 werkit-0.9.0/werkit.egg-info/requires.txt
--rw-r--r--   0 pnm        (503) staff       (20)        7 2020-06-12 19:54:20.000000 werkit-0.9.0/werkit.egg-info/top_level.txt
+drwxr-xr-x   0 pnm        (503) staff       (20)        0 2020-06-13 00:29:20.000000 werkit-0.9.1/
+-rw-r--r--   0 pnm        (503) staff       (20)     1071 2019-07-22 17:09:56.000000 werkit-0.9.1/LICENSE
+-rw-r--r--   0 pnm        (503) staff       (20)       80 2020-05-31 02:59:45.000000 werkit-0.9.1/MANIFEST.in
+-rw-r--r--   0 pnm        (503) staff       (20)     7700 2020-06-13 00:29:20.000000 werkit-0.9.1/PKG-INFO
+-rw-r--r--   0 pnm        (503) staff       (20)     5077 2020-05-25 02:49:13.000000 werkit-0.9.1/README.md
+-rw-r--r--   0 pnm        (503) staff       (20)        0 2020-05-31 04:42:18.000000 werkit-0.9.1/requirements.txt
+-rw-r--r--   0 pnm        (503) staff       (20)       38 2020-06-13 00:29:20.000000 werkit-0.9.1/setup.cfg
+-rwxr-xr-x   0 pnm        (503) staff       (20)     1248 2020-05-31 04:42:18.000000 werkit-0.9.1/setup.py
+drwxr-xr-x   0 pnm        (503) staff       (20)        0 2020-06-13 00:29:20.000000 werkit-0.9.1/werkit/
+-rw-r--r--   0 pnm        (503) staff       (20)       70 2019-07-22 18:32:13.000000 werkit-0.9.1/werkit/__init__.py
+drwxr-xr-x   0 pnm        (503) staff       (20)        0 2020-06-13 00:29:20.000000 werkit-0.9.1/werkit/aws_lambda/
+-rw-r--r--   0 pnm        (503) staff       (20)        0 2020-05-25 02:49:13.000000 werkit-0.9.1/werkit/aws_lambda/__init__.py
+-rw-r--r--   0 pnm        (503) staff       (20)     3170 2020-06-13 00:27:47.000000 werkit-0.9.1/werkit/aws_lambda/build.py
+-rw-r--r--   0 pnm        (503) staff       (20)     2731 2020-06-12 16:20:14.000000 werkit-0.9.1/werkit/aws_lambda/default_handler.py
+-rw-r--r--   0 pnm        (503) staff       (20)     2808 2020-06-12 19:50:47.000000 werkit-0.9.1/werkit/aws_lambda/deploy.py
+-rw-r--r--   0 pnm        (503) staff       (20)     2079 2020-06-12 16:00:44.000000 werkit-0.9.1/werkit/aws_lambda/orchestrator_deploy.py
+-rw-r--r--   0 pnm        (503) staff       (20)     2346 2020-06-12 16:20:14.000000 werkit-0.9.1/werkit/aws_lambda/parallel.py
+-rw-r--r--   0 pnm        (503) staff       (20)      196 2020-06-01 20:37:18.000000 werkit-0.9.1/werkit/formatting.py
+-rw-r--r--   0 pnm        (503) staff       (20)     3648 2020-06-12 16:20:14.000000 werkit-0.9.1/werkit/manager.py
+-rw-r--r--   0 pnm        (503) staff       (20)       22 2020-06-13 00:29:13.000000 werkit-0.9.1/werkit/package_version.py
+drwxr-xr-x   0 pnm        (503) staff       (20)        0 2020-06-13 00:29:20.000000 werkit-0.9.1/werkit/parallel/
+-rw-r--r--   0 pnm        (503) staff       (20)      217 2020-05-31 02:59:45.000000 werkit-0.9.1/werkit/parallel/__init__.py
+-rw-r--r--   0 pnm        (503) staff       (20)     3259 2020-05-23 08:12:00.000000 werkit-0.9.1/werkit/parallel/cloud_manager.py
+-rw-r--r--   0 pnm        (503) staff       (20)     4275 2020-05-31 02:59:45.000000 werkit-0.9.1/werkit/parallel/invoke.py
+-rw-r--r--   0 pnm        (503) staff       (20)      109 2019-07-26 16:49:19.000000 werkit-0.9.1/werkit/parallel/testing.py
+-rw-r--r--   0 pnm        (503) staff       (20)      830 2020-06-12 19:50:47.000000 werkit-0.9.1/werkit/s3.py
+-rw-r--r--   0 pnm        (503) staff       (20)     2274 2020-06-01 20:37:18.000000 werkit-0.9.1/werkit/schema.py
+drwxr-xr-x   0 pnm        (503) staff       (20)        0 2020-06-13 00:29:20.000000 werkit-0.9.1/werkit.egg-info/
+-rw-r--r--   0 pnm        (503) staff       (20)     7700 2020-06-13 00:29:19.000000 werkit-0.9.1/werkit.egg-info/PKG-INFO
+-rw-r--r--   0 pnm        (503) staff       (20)      625 2020-06-13 00:29:19.000000 werkit-0.9.1/werkit.egg-info/SOURCES.txt
+-rw-r--r--   0 pnm        (503) staff       (20)        1 2020-06-13 00:29:19.000000 werkit-0.9.1/werkit.egg-info/dependency_links.txt
+-rw-r--r--   0 pnm        (503) staff       (20)       44 2020-06-13 00:29:19.000000 werkit-0.9.1/werkit.egg-info/requires.txt
+-rw-r--r--   0 pnm        (503) staff       (20)        7 2020-06-13 00:29:19.000000 werkit-0.9.1/werkit.egg-info/top_level.txt
```

### Comparing `werkit-0.9.0/LICENSE` & `werkit-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `werkit-0.9.0/PKG-INFO` & `werkit-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: werkit
-Version: 0.9.0
+Version: 0.9.1
 Summary: Toolkit for encapsulating Python-based computation into deployable and distributable tasks
 Home-page: https://github.com/metabolize/werkit
 Author: Metabolize
 Author-email: github@paulmelnikow.com
 License: UNKNOWN
 Project-URL: Issue Tracker, https://github.com/metabolize/werkit/issues
 Project-URL: Documentation, https://werkit.readthedocs.io/en/stable/
```

### Comparing `werkit-0.9.0/README.md` & `werkit-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `werkit-0.9.0/setup.py` & `werkit-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `werkit-0.9.0/werkit/aws_lambda/build.py` & `werkit-0.9.1/werkit/aws_lambda/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 
     if install_werkit:
         execute(
             python,
             "-m",
             "pip",
             "install",
-            f"werkit@git+https://github.com/metabolize/werkit.git@{__version__}",
+            f"werkit=={__version__}",
+            # f"werkit@git+https://github.com/metabolize/werkit.git@...",
             environment=environment,
         )
 
     if len(install_requirements_from) > 0:
         args = [
             python,
             "-m",
```

### Comparing `werkit-0.9.0/werkit/aws_lambda/default_handler.py` & `werkit-0.9.1/werkit/aws_lambda/default_handler.py`

 * *Files identical despite different names*

### Comparing `werkit-0.9.0/werkit/aws_lambda/deploy.py` & `werkit-0.9.1/werkit/aws_lambda/deploy.py`

 * *Files identical despite different names*

### Comparing `werkit-0.9.0/werkit/aws_lambda/orchestrator_deploy.py` & `werkit-0.9.1/werkit/aws_lambda/orchestrator_deploy.py`

 * *Files identical despite different names*

### Comparing `werkit-0.9.0/werkit/aws_lambda/parallel.py` & `werkit-0.9.1/werkit/aws_lambda/parallel.py`

 * *Files identical despite different names*

### Comparing `werkit-0.9.0/werkit/manager.py` & `werkit-0.9.1/werkit/manager.py`

 * *Files identical despite different names*

### Comparing `werkit-0.9.0/werkit/parallel/cloud_manager.py` & `werkit-0.9.1/werkit/parallel/cloud_manager.py`

 * *Files identical despite different names*

### Comparing `werkit-0.9.0/werkit/parallel/invoke.py` & `werkit-0.9.1/werkit/parallel/invoke.py`

 * *Files identical despite different names*

### Comparing `werkit-0.9.0/werkit/s3.py` & `werkit-0.9.1/werkit/s3.py`

 * *Files identical despite different names*

### Comparing `werkit-0.9.0/werkit/schema.py` & `werkit-0.9.1/werkit/schema.py`

 * *Files identical despite different names*

### Comparing `werkit-0.9.0/werkit.egg-info/PKG-INFO` & `werkit-0.9.1/werkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: werkit
-Version: 0.9.0
+Version: 0.9.1
 Summary: Toolkit for encapsulating Python-based computation into deployable and distributable tasks
 Home-page: https://github.com/metabolize/werkit
 Author: Metabolize
 Author-email: github@paulmelnikow.com
 License: UNKNOWN
 Project-URL: Issue Tracker, https://github.com/metabolize/werkit/issues
 Project-URL: Documentation, https://werkit.readthedocs.io/en/stable/
```

### Comparing `werkit-0.9.0/werkit.egg-info/SOURCES.txt` & `werkit-0.9.1/werkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

