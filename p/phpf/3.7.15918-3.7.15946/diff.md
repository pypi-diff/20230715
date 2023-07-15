# Comparing `tmp/phpf-3.7.15918.tar.gz` & `tmp/phpf-3.7.15946.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phpf-3.7.15918.tar", last modified: Sat Jul 15 09:19:17 2023, max compression
+gzip compressed data, was "phpf-3.7.15946.tar", last modified: Sat Jul 15 09:47:46 2023, max compression
```

## Comparing `phpf-3.7.15918.tar` & `phpf-3.7.15946.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 09:19:17.085143 phpf-3.7.15918/
--rw-rw-rw-   0        0        0      829 2023-07-15 09:18:31.000000 phpf-3.7.15918/LICENSE
--rw-rw-rw-   0        0        0      204 2023-07-15 09:19:17.084275 phpf-3.7.15918/PKG-INFO
--rw-rw-rw-   0        0        0       81 2023-07-15 09:18:31.000000 phpf-3.7.15918/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 09:19:17.062277 phpf-3.7.15918/phpf/
--rw-rw-rw-   0        0        0    23611 2023-07-15 09:18:31.000000 phpf-3.7.15918/phpf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:19:17.081276 phpf-3.7.15918/phpf.egg-info/
--rw-rw-rw-   0        0        0      204 2023-07-15 09:19:16.000000 phpf-3.7.15918/phpf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      155 2023-07-15 09:19:16.000000 phpf-3.7.15918/phpf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 09:19:16.000000 phpf-3.7.15918/phpf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-15 09:19:16.000000 phpf-3.7.15918/phpf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 09:19:17.085143 phpf-3.7.15918/setup.cfg
--rw-rw-rw-   0        0        0      376 2023-07-15 09:18:31.000000 phpf-3.7.15918/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:47:46.134168 phpf-3.7.15946/
+-rw-rw-rw-   0        0        0      829 2023-07-15 09:46:56.000000 phpf-3.7.15946/LICENSE
+-rw-rw-rw-   0        0        0      204 2023-07-15 09:47:46.134168 phpf-3.7.15946/PKG-INFO
+-rw-rw-rw-   0        0        0       81 2023-07-15 09:46:56.000000 phpf-3.7.15946/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 09:47:46.112260 phpf-3.7.15946/phpf/
+-rw-rw-rw-   0        0        0    23603 2023-07-15 09:46:56.000000 phpf-3.7.15946/phpf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:47:46.134168 phpf-3.7.15946/phpf.egg-info/
+-rw-rw-rw-   0        0        0      204 2023-07-15 09:47:45.000000 phpf-3.7.15946/phpf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2023-07-15 09:47:46.000000 phpf-3.7.15946/phpf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 09:47:45.000000 phpf-3.7.15946/phpf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-15 09:47:45.000000 phpf-3.7.15946/phpf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 09:47:46.134168 phpf-3.7.15946/setup.cfg
+-rw-rw-rw-   0        0        0      376 2023-07-15 09:46:56.000000 phpf-3.7.15946/setup.py
```

### Comparing `phpf-3.7.15918/LICENSE` & `phpf-3.7.15946/LICENSE`

 * *Files identical despite different names*

### Comparing `phpf-3.7.15918/phpf/__init__.py` & `phpf-3.7.15946/phpf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -586,17 +586,17 @@
 #----------------------------------------------------------------------------------
 
 def chdir(path):
 	import os
 	os.chdir(path)
 #----------------------------------------------------------------------------------
 
-def getcwd(path):
+def getcwd():
 	import os
-	return os.getcwd(path)
+	return os.getcwd()
 #----------------------------------------------------------------------------------
 
 def scandir(path):
 	import os
 	return os.listdir(path)
 #----------------------------------------------------------------------------------
```

