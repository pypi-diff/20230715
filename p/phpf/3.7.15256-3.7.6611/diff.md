# Comparing `tmp/phpf-3.7.15256.tar.gz` & `tmp/phpf-3.7.6611.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phpf-3.7.15256.tar", last modified: Sat Jul 15 02:56:41 2023, max compression
+gzip compressed data, was "phpf-3.7.6611.tar", last modified: Thu Jul  6 06:12:04 2023, max compression
```

## Comparing `phpf-3.7.15256.tar` & `phpf-3.7.6611.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 02:56:41.490992 phpf-3.7.15256/
--rw-rw-rw-   0        0        0      829 2023-07-15 02:56:38.000000 phpf-3.7.15256/LICENSE
--rw-rw-rw-   0        0        0      204 2023-07-15 02:56:41.490992 phpf-3.7.15256/PKG-INFO
--rw-rw-rw-   0        0        0       81 2023-07-15 02:56:38.000000 phpf-3.7.15256/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 02:56:41.475362 phpf-3.7.15256/phpf/
--rw-rw-rw-   0        0        0    18184 2023-07-15 02:56:38.000000 phpf-3.7.15256/phpf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 02:56:41.490992 phpf-3.7.15256/phpf.egg-info/
--rw-rw-rw-   0        0        0      204 2023-07-15 02:56:41.000000 phpf-3.7.15256/phpf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      155 2023-07-15 02:56:41.000000 phpf-3.7.15256/phpf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 02:56:41.000000 phpf-3.7.15256/phpf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-15 02:56:41.000000 phpf-3.7.15256/phpf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 02:56:41.490992 phpf-3.7.15256/setup.cfg
--rw-rw-rw-   0        0        0      376 2023-07-15 02:56:38.000000 phpf-3.7.15256/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:12:04.058086 phpf-3.7.6611/
+-rw-rw-rw-   0        0        0      829 2023-07-06 06:11:40.000000 phpf-3.7.6611/LICENSE
+-rw-rw-rw-   0        0        0      203 2023-07-06 06:12:04.047727 phpf-3.7.6611/PKG-INFO
+-rw-rw-rw-   0        0        0       81 2023-07-06 06:11:40.000000 phpf-3.7.6611/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 06:12:04.015787 phpf-3.7.6611/phpf/
+-rw-rw-rw-   0        0        0    18076 2023-07-06 06:11:40.000000 phpf-3.7.6611/phpf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:12:04.047727 phpf-3.7.6611/phpf.egg-info/
+-rw-rw-rw-   0        0        0      203 2023-07-06 06:12:03.000000 phpf-3.7.6611/phpf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2023-07-06 06:12:03.000000 phpf-3.7.6611/phpf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 06:12:03.000000 phpf-3.7.6611/phpf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-06 06:12:03.000000 phpf-3.7.6611/phpf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 06:12:04.058086 phpf-3.7.6611/setup.cfg
+-rw-rw-rw-   0        0        0      375 2023-07-06 06:11:40.000000 phpf-3.7.6611/setup.py
```

### Comparing `phpf-3.7.15256/LICENSE` & `phpf-3.7.6611/LICENSE`

 * *Files identical despite different names*

### Comparing `phpf-3.7.15256/phpf/__init__.py` & `phpf-3.7.6611/phpf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,17 +330,15 @@
 def print_r(vv):
 	import pprint
 	pprint.pprint(vv)
 #----------------------------------------------------------------------------------
 def sleep(i):
 	import time
 	time.sleep(i)
-#----------------------------------------------------------------------------------
-def echo(v):
-	print(v)
+
 def is_array(v):
 	v = str(type(v))
 	return True if v == ("<class 'list'>" or "<class 'tuple'>" or "<class 'range'>" or "<class 'dict'>" or "<class 'frozenset'>" or "<class 'set'>") else False
 #----------------------------------------------------------------------------------
 def is_dict(v):
 	v = str(type(v))
 	return True if v == "<class 'dict'>" else False
```

