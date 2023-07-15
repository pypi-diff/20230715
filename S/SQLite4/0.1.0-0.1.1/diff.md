# Comparing `tmp/SQLite4-0.1.0.tar.gz` & `tmp/SQLite4-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SQLite4-0.1.0.tar", last modified: Sat Jul 15 03:54:27 2023, max compression
+gzip compressed data, was "SQLite4-0.1.1.tar", last modified: Sat Jul 15 04:35:00 2023, max compression
```

## Comparing `SQLite4-0.1.0.tar` & `SQLite4-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 okay      (1000) okay      (1000)        0 2023-07-15 03:54:27.766514 SQLite4-0.1.0/
--rw-rw-r--   0 okay      (1000) okay      (1000)     1067 2023-07-15 01:51:25.000000 SQLite4-0.1.0/LICENSE
--rw-rw-r--   0 okay      (1000) okay      (1000)      672 2023-07-15 03:54:27.766514 SQLite4-0.1.0/PKG-INFO
--rw-rw-r--   0 okay      (1000) okay      (1000)       79 2023-07-15 03:37:23.000000 SQLite4-0.1.0/README.md
-drwxrwxr-x   0 okay      (1000) okay      (1000)        0 2023-07-15 03:54:27.762514 SQLite4-0.1.0/SQLite4.egg-info/
--rw-rw-r--   0 okay      (1000) okay      (1000)      672 2023-07-15 03:54:27.000000 SQLite4-0.1.0/SQLite4.egg-info/PKG-INFO
--rw-rw-r--   0 okay      (1000) okay      (1000)      282 2023-07-15 03:54:27.000000 SQLite4-0.1.0/SQLite4.egg-info/SOURCES.txt
--rw-rw-r--   0 okay      (1000) okay      (1000)        1 2023-07-15 03:54:27.000000 SQLite4-0.1.0/SQLite4.egg-info/dependency_links.txt
--rw-rw-r--   0 okay      (1000) okay      (1000)       14 2023-07-15 03:54:27.000000 SQLite4-0.1.0/SQLite4.egg-info/top_level.txt
--rw-rw-r--   0 okay      (1000) okay      (1000)       38 2023-07-15 03:54:27.766514 SQLite4-0.1.0/setup.cfg
--rw-rw-r--   0 okay      (1000) okay      (1000)      717 2023-07-15 03:47:26.000000 SQLite4-0.1.0/setup.py
-drwxrwxr-x   0 okay      (1000) okay      (1000)        0 2023-07-15 03:54:27.766514 SQLite4-0.1.0/sqlite4/
--rw-rw-r--   0 okay      (1000) okay      (1000)     5445 2023-07-15 03:37:09.000000 SQLite4-0.1.0/sqlite4/SQLite4.py
--rw-rw-r--   0 okay      (1000) okay      (1000)       36 2023-07-15 03:47:26.000000 SQLite4-0.1.0/sqlite4/__init__.py
-drwxrwxr-x   0 okay      (1000) okay      (1000)        0 2023-07-15 03:54:27.766514 SQLite4-0.1.0/tests/
--rw-rw-r--   0 okay      (1000) okay      (1000)        0 2023-07-15 03:33:21.000000 SQLite4-0.1.0/tests/__init__.py
--rw-rw-r--   0 okay      (1000) okay      (1000)      646 2023-07-15 03:48:53.000000 SQLite4-0.1.0/tests/test_crud_class.py
--rw-rw-r--   0 okay      (1000) okay      (1000)      532 2023-07-15 03:49:11.000000 SQLite4-0.1.0/tests/test_multithread.py
--rw-rw-r--   0 okay      (1000) okay      (1000)      308 2023-07-15 03:49:16.000000 SQLite4-0.1.0/tests/test_singleton.py
+drwxrwxr-x   0 okay      (1000) okay      (1000)        0 2023-07-15 04:35:00.767462 SQLite4-0.1.1/
+-rw-rw-r--   0 okay      (1000) okay      (1000)     1067 2023-07-15 01:51:25.000000 SQLite4-0.1.1/LICENSE
+-rw-rw-r--   0 okay      (1000) okay      (1000)     5817 2023-07-15 04:35:00.767462 SQLite4-0.1.1/PKG-INFO
+-rw-rw-r--   0 okay      (1000) okay      (1000)     5089 2023-07-15 04:33:43.000000 SQLite4-0.1.1/README.md
+drwxrwxr-x   0 okay      (1000) okay      (1000)        0 2023-07-15 04:35:00.767462 SQLite4-0.1.1/SQLite4.egg-info/
+-rw-rw-r--   0 okay      (1000) okay      (1000)     5817 2023-07-15 04:35:00.000000 SQLite4-0.1.1/SQLite4.egg-info/PKG-INFO
+-rw-rw-r--   0 okay      (1000) okay      (1000)      282 2023-07-15 04:35:00.000000 SQLite4-0.1.1/SQLite4.egg-info/SOURCES.txt
+-rw-rw-r--   0 okay      (1000) okay      (1000)        1 2023-07-15 04:35:00.000000 SQLite4-0.1.1/SQLite4.egg-info/dependency_links.txt
+-rw-rw-r--   0 okay      (1000) okay      (1000)       14 2023-07-15 04:35:00.000000 SQLite4-0.1.1/SQLite4.egg-info/top_level.txt
+-rw-rw-r--   0 okay      (1000) okay      (1000)       38 2023-07-15 04:35:00.767462 SQLite4-0.1.1/setup.cfg
+-rw-rw-r--   0 okay      (1000) okay      (1000)      915 2023-07-15 04:34:43.000000 SQLite4-0.1.1/setup.py
+drwxrwxr-x   0 okay      (1000) okay      (1000)        0 2023-07-15 04:35:00.767462 SQLite4-0.1.1/sqlite4/
+-rw-rw-r--   0 okay      (1000) okay      (1000)     5445 2023-07-15 03:37:09.000000 SQLite4-0.1.1/sqlite4/SQLite4.py
+-rw-rw-r--   0 okay      (1000) okay      (1000)       36 2023-07-15 03:47:26.000000 SQLite4-0.1.1/sqlite4/__init__.py
+drwxrwxr-x   0 okay      (1000) okay      (1000)        0 2023-07-15 04:35:00.767462 SQLite4-0.1.1/tests/
+-rw-rw-r--   0 okay      (1000) okay      (1000)        0 2023-07-15 03:33:21.000000 SQLite4-0.1.1/tests/__init__.py
+-rw-rw-r--   0 okay      (1000) okay      (1000)      646 2023-07-15 03:48:53.000000 SQLite4-0.1.1/tests/test_crud_class.py
+-rw-rw-r--   0 okay      (1000) okay      (1000)      532 2023-07-15 03:49:11.000000 SQLite4-0.1.1/tests/test_multithread.py
+-rw-rw-r--   0 okay      (1000) okay      (1000)      308 2023-07-15 03:49:16.000000 SQLite4-0.1.1/tests/test_singleton.py
```

### Comparing `SQLite4-0.1.0/LICENSE` & `SQLite4-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SQLite4-0.1.0/setup.py` & `SQLite4-0.1.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from setuptools import setup, find_packages
 
+with open('README.md', 'r', encoding='utf-8') as f:
+    long_description = f.read()
+
 setup(
     name="SQLite4",
-    version="0.1.0",
+    version="0.1.1",
     author="Ali Chaayb",
-    description="Simplified SQLite3 Package with CRUD Class and Multithreading Safety",
+    description="SQLite4 provides a simplified wrapper for SQLite3, along with built-in multi-thread safety.",
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `SQLite4-0.1.0/sqlite4/SQLite4.py` & `SQLite4-0.1.1/sqlite4/SQLite4.py`

 * *Files identical despite different names*

### Comparing `SQLite4-0.1.0/tests/test_crud_class.py` & `SQLite4-0.1.1/tests/test_crud_class.py`

 * *Files identical despite different names*

### Comparing `SQLite4-0.1.0/tests/test_multithread.py` & `SQLite4-0.1.1/tests/test_multithread.py`

 * *Files identical despite different names*

