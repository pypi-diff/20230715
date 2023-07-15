# Comparing `tmp/testmy_toollib-0.0.2.tar.gz` & `tmp/testmy_toollib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testmy_toollib-0.0.2.tar", last modified: Sat Jul 15 14:09:39 2023, max compression
+gzip compressed data, was "testmy_toollib-0.0.3.tar", last modified: Sat Jul 15 14:17:33 2023, max compression
```

## Comparing `testmy_toollib-0.0.2.tar` & `testmy_toollib-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,12 @@
-drwxrwxr-x   0 dci-student  (1001) dci-student  (1001)        0 2023-07-15 14:09:39.045660 testmy_toollib-0.0.2/
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)        0 2023-07-15 12:42:42.000000 testmy_toollib-0.0.2/LICENCE
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      911 2023-07-15 14:09:39.045660 testmy_toollib-0.0.2/PKG-INFO
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)       44 2023-07-15 12:42:46.000000 testmy_toollib-0.0.2/README.md
-drwxrwxr-x   0 dci-student  (1001) dci-student  (1001)        0 2023-07-15 14:09:39.041660 testmy_toollib-0.0.2/chdev_tools/
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)       58 2023-07-15 14:02:24.000000 testmy_toollib-0.0.2/chdev_tools/__init__.py
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      124 2023-07-15 13:37:34.000000 testmy_toollib-0.0.2/chdev_tools/ang.py
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)     1265 2023-07-15 13:57:51.000000 testmy_toollib-0.0.2/chdev_tools/numconvert.py
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)       38 2023-07-15 14:09:39.045660 testmy_toollib-0.0.2/setup.cfg
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)     1422 2023-07-15 14:09:30.000000 testmy_toollib-0.0.2/setup.py
-drwxrwxr-x   0 dci-student  (1001) dci-student  (1001)        0 2023-07-15 14:09:39.041660 testmy_toollib-0.0.2/testmy_toollib.egg-info/
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      911 2023-07-15 14:09:39.000000 testmy_toollib-0.0.2/testmy_toollib.egg-info/PKG-INFO
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      284 2023-07-15 14:09:39.000000 testmy_toollib-0.0.2/testmy_toollib.egg-info/SOURCES.txt
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)        1 2023-07-15 14:09:39.000000 testmy_toollib-0.0.2/testmy_toollib.egg-info/dependency_links.txt
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      214 2023-07-15 14:09:39.000000 testmy_toollib-0.0.2/testmy_toollib.egg-info/requires.txt
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)       12 2023-07-15 14:09:39.000000 testmy_toollib-0.0.2/testmy_toollib.egg-info/top_level.txt
+drwxrwxr-x   0 dci-student  (1001) dci-student  (1001)        0 2023-07-15 14:17:33.299723 testmy_toollib-0.0.3/
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)        0 2023-07-15 12:42:42.000000 testmy_toollib-0.0.3/LICENCE
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      911 2023-07-15 14:17:33.299723 testmy_toollib-0.0.3/PKG-INFO
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)       44 2023-07-15 12:42:46.000000 testmy_toollib-0.0.3/README.md
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)       38 2023-07-15 14:17:33.299723 testmy_toollib-0.0.3/setup.cfg
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)     1422 2023-07-15 14:17:30.000000 testmy_toollib-0.0.3/setup.py
+drwxrwxr-x   0 dci-student  (1001) dci-student  (1001)        0 2023-07-15 14:17:33.299723 testmy_toollib-0.0.3/testmy_toollib.egg-info/
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      911 2023-07-15 14:17:33.000000 testmy_toollib-0.0.3/testmy_toollib.egg-info/PKG-INFO
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      215 2023-07-15 14:17:33.000000 testmy_toollib-0.0.3/testmy_toollib.egg-info/SOURCES.txt
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)        1 2023-07-15 14:17:33.000000 testmy_toollib-0.0.3/testmy_toollib.egg-info/dependency_links.txt
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      214 2023-07-15 14:17:33.000000 testmy_toollib-0.0.3/testmy_toollib.egg-info/requires.txt
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)        1 2023-07-15 14:17:33.000000 testmy_toollib-0.0.3/testmy_toollib.egg-info/top_level.txt
```

### Comparing `testmy_toollib-0.0.2/PKG-INFO` & `testmy_toollib-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testmy_toollib
-Version: 0.0.2
+Version: 0.0.3
 Summary: A pip generic developer package
 Home-page: https://github.com/AngeloChDev
 Author: AngeloChDev
 Author-email: angeloch.dev@gmail.com
 License: MIT
 Keywords: Generic Developer Tools, Wedapp developer, Offline Software developer,Python package
 Platform: UNKNOWN
```

### Comparing `testmy_toollib-0.0.2/setup.py` & `testmy_toollib-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 try:
     long_description = open("README.md").read()
 except IOError:
     long_description = ""
 
 setup(
     name="testmy_toollib",
-    version="0.0.2",
+    version="0.0.3",
     description="A pip generic developer package",
     license="MIT",
     author="AngeloChDev",
     author_email="angeloch.dev@gmail.com",
     url="https://github.com/AngeloChDev",
     packages=find_packages(),
     test_suite='tests',
```

### Comparing `testmy_toollib-0.0.2/testmy_toollib.egg-info/PKG-INFO` & `testmy_toollib-0.0.3/testmy_toollib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testmy-toollib
-Version: 0.0.2
+Version: 0.0.3
 Summary: A pip generic developer package
 Home-page: https://github.com/AngeloChDev
 Author: AngeloChDev
 Author-email: angeloch.dev@gmail.com
 License: MIT
 Keywords: Generic Developer Tools, Wedapp developer, Offline Software developer,Python package
 Platform: UNKNOWN
```

