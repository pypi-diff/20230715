# Comparing `tmp/testmy_toollib-0.0.3.tar.gz` & `tmp/testmy_toollib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testmy_toollib-0.0.3.tar", last modified: Sat Jul 15 14:17:33 2023, max compression
+gzip compressed data, was "testmy_toollib-0.0.4.tar", last modified: Sat Jul 15 14:22:45 2023, max compression
```

## Comparing `testmy_toollib-0.0.3.tar` & `testmy_toollib-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 dci-student  (1001) dci-student  (1001)        0 2023-07-15 14:17:33.299723 testmy_toollib-0.0.3/
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)        0 2023-07-15 12:42:42.000000 testmy_toollib-0.0.3/LICENCE
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      911 2023-07-15 14:17:33.299723 testmy_toollib-0.0.3/PKG-INFO
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)       44 2023-07-15 12:42:46.000000 testmy_toollib-0.0.3/README.md
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)       38 2023-07-15 14:17:33.299723 testmy_toollib-0.0.3/setup.cfg
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)     1422 2023-07-15 14:17:30.000000 testmy_toollib-0.0.3/setup.py
-drwxrwxr-x   0 dci-student  (1001) dci-student  (1001)        0 2023-07-15 14:17:33.299723 testmy_toollib-0.0.3/testmy_toollib.egg-info/
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      911 2023-07-15 14:17:33.000000 testmy_toollib-0.0.3/testmy_toollib.egg-info/PKG-INFO
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      215 2023-07-15 14:17:33.000000 testmy_toollib-0.0.3/testmy_toollib.egg-info/SOURCES.txt
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)        1 2023-07-15 14:17:33.000000 testmy_toollib-0.0.3/testmy_toollib.egg-info/dependency_links.txt
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      214 2023-07-15 14:17:33.000000 testmy_toollib-0.0.3/testmy_toollib.egg-info/requires.txt
--rw-rw-r--   0 dci-student  (1001) dci-student  (1001)        1 2023-07-15 14:17:33.000000 testmy_toollib-0.0.3/testmy_toollib.egg-info/top_level.txt
+drwxrwxr-x   0 dci-student  (1001) dci-student  (1001)        0 2023-07-15 14:22:45.594301 testmy_toollib-0.0.4/
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)        0 2023-07-15 12:42:42.000000 testmy_toollib-0.0.4/LICENCE
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      911 2023-07-15 14:22:45.594301 testmy_toollib-0.0.4/PKG-INFO
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)       44 2023-07-15 12:42:46.000000 testmy_toollib-0.0.4/README.md
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)       38 2023-07-15 14:22:45.594301 testmy_toollib-0.0.4/setup.cfg
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)     1422 2023-07-15 14:22:43.000000 testmy_toollib-0.0.4/setup.py
+drwxrwxr-x   0 dci-student  (1001) dci-student  (1001)        0 2023-07-15 14:22:45.594301 testmy_toollib-0.0.4/testmy_toollib.egg-info/
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      911 2023-07-15 14:22:45.000000 testmy_toollib-0.0.4/testmy_toollib.egg-info/PKG-INFO
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      215 2023-07-15 14:22:45.000000 testmy_toollib-0.0.4/testmy_toollib.egg-info/SOURCES.txt
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)        1 2023-07-15 14:22:45.000000 testmy_toollib-0.0.4/testmy_toollib.egg-info/dependency_links.txt
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)      214 2023-07-15 14:22:45.000000 testmy_toollib-0.0.4/testmy_toollib.egg-info/requires.txt
+-rw-rw-r--   0 dci-student  (1001) dci-student  (1001)        1 2023-07-15 14:22:45.000000 testmy_toollib-0.0.4/testmy_toollib.egg-info/top_level.txt
```

### Comparing `testmy_toollib-0.0.3/PKG-INFO` & `testmy_toollib-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testmy_toollib
-Version: 0.0.3
+Version: 0.0.4
 Summary: A pip generic developer package
 Home-page: https://github.com/AngeloChDev
 Author: AngeloChDev
 Author-email: angeloch.dev@gmail.com
 License: MIT
 Keywords: Generic Developer Tools, Wedapp developer, Offline Software developer,Python package
 Platform: UNKNOWN
```

### Comparing `testmy_toollib-0.0.3/setup.py` & `testmy_toollib-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 try:
     long_description = open("README.md").read()
 except IOError:
     long_description = ""
 
 setup(
     name="testmy_toollib",
-    version="0.0.3",
+    version="0.0.4",
     description="A pip generic developer package",
     license="MIT",
     author="AngeloChDev",
     author_email="angeloch.dev@gmail.com",
     url="https://github.com/AngeloChDev",
-    packages=find_packages(),
+    package='testmy_toollib',
     test_suite='tests',
     install_requires=[
         'requests>=2.25.0',
         'fastecdsa>=2.2.1;platform_system!="Windows"',
         'ecdsa>=0.17;platform_system=="Windows"',
         'SQLAlchemy>=1.4.28',
         'numpy==1.19.5;python_version<"3.8"',
```

### Comparing `testmy_toollib-0.0.3/testmy_toollib.egg-info/PKG-INFO` & `testmy_toollib-0.0.4/testmy_toollib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testmy-toollib
-Version: 0.0.3
+Version: 0.0.4
 Summary: A pip generic developer package
 Home-page: https://github.com/AngeloChDev
 Author: AngeloChDev
 Author-email: angeloch.dev@gmail.com
 License: MIT
 Keywords: Generic Developer Tools, Wedapp developer, Offline Software developer,Python package
 Platform: UNKNOWN
```

