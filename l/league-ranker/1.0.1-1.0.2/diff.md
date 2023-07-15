# Comparing `tmp/league-ranker-1.0.1.tar.gz` & `tmp/league-ranker-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/league-ranker-1.0.1.tar", last modified: Sat Mar 12 14:22:03 2022, max compression
+gzip compressed data, was "dist/league-ranker-1.0.2.tar", last modified: Sat Jul 15 14:09:30 2023, max compression
```

## Comparing `league-ranker-1.0.1.tar` & `league-ranker-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-03-12 14:22:03.000000 league-ranker-1.0.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3243 2022-03-12 14:22:03.000000 league-ranker-1.0.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1763 2022-03-12 14:21:38.000000 league-ranker-1.0.1/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-03-12 14:22:03.000000 league-ranker-1.0.1/league_ranker/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8604 2022-03-12 14:21:38.000000 league-ranker-1.0.1/league_ranker/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-03-12 14:21:38.000000 league-ranker-1.0.1/league_ranker/py.typed
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-03-12 14:22:03.000000 league-ranker-1.0.1/league_ranker.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3243 2022-03-12 14:22:03.000000 league-ranker-1.0.1/league_ranker.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      258 2022-03-12 14:22:03.000000 league-ranker-1.0.1/league_ranker.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-03-12 14:22:03.000000 league-ranker-1.0.1/league_ranker.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2022-03-12 14:22:03.000000 league-ranker-1.0.1/league_ranker.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-03-12 14:22:03.000000 league-ranker-1.0.1/league_ranker.egg-info/zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      980 2022-03-12 14:22:03.000000 league-ranker-1.0.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1492 2022-03-12 14:21:38.000000 league-ranker-1.0.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-15 14:09:30.000000 league-ranker-1.0.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3294 2023-07-15 14:09:30.000000 league-ranker-1.0.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1763 2023-07-15 14:09:07.000000 league-ranker-1.0.2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-15 14:09:30.000000 league-ranker-1.0.2/league_ranker/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8604 2023-07-15 14:09:07.000000 league-ranker-1.0.2/league_ranker/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-15 14:09:07.000000 league-ranker-1.0.2/league_ranker/py.typed
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-15 14:09:30.000000 league-ranker-1.0.2/league_ranker.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3294 2023-07-15 14:09:30.000000 league-ranker-1.0.2/league_ranker.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      258 2023-07-15 14:09:30.000000 league-ranker-1.0.2/league_ranker.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-15 14:09:30.000000 league-ranker-1.0.2/league_ranker.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2023-07-15 14:09:30.000000 league-ranker-1.0.2/league_ranker.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-15 14:09:30.000000 league-ranker-1.0.2/league_ranker.egg-info/zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1007 2023-07-15 14:09:30.000000 league-ranker-1.0.2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1542 2023-07-15 14:09:07.000000 league-ranker-1.0.2/setup.py
```

### Comparing `league-ranker-1.0.1/PKG-INFO` & `league-ranker-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: league-ranker
-Version: 1.0.1
+Version: 1.0.2
 Summary: League ranking for arbitrary numbers of competitors.
 Home-page: https://ranker.readthedocs.io/en/latest/
 Author: Student Robotics Competition Software SIG
 Author-email: srobo-devel@googlegroups.com
 License: MIT
 Project-URL: Documentation, https://ranker.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/PeterJCLaw/ranker
@@ -61,10 +61,11 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
```

### Comparing `league-ranker-1.0.1/README.rst` & `league-ranker-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `league-ranker-1.0.1/league_ranker/__init__.py` & `league-ranker-1.0.2/league_ranker/__init__.py`

 * *Files identical despite different names*

### Comparing `league-ranker-1.0.1/league_ranker.egg-info/PKG-INFO` & `league-ranker-1.0.2/league_ranker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: league-ranker
-Version: 1.0.1
+Version: 1.0.2
 Summary: League ranking for arbitrary numbers of competitors.
 Home-page: https://ranker.readthedocs.io/en/latest/
 Author: Student Robotics Competition Software SIG
 Author-email: srobo-devel@googlegroups.com
 License: MIT
 Project-URL: Documentation, https://ranker.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/PeterJCLaw/ranker
@@ -61,10 +61,11 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
```

### Comparing `league-ranker-1.0.1/setup.cfg` & `league-ranker-1.0.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 order_by_type = False
 float_to_top = True
 default_section = THIRDPARTY
 sections = FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER
 
 [mypy]
 warn_unused_configs = True
+show_column_numbers = True
 show_error_codes = True
 enable_error_code = ignore-without-code
 warn_incomplete_stub = True
 warn_unused_ignores = True
 warn_redundant_casts = True
 no_implicit_optional = True
 strict = True
```

### Comparing `league-ranker-1.0.1/setup.py` & `league-ranker-1.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open('README.rst') as f:
     long_description = f.read()
 
 
 setup(
     name='league-ranker',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(exclude=('tests',)),
     package_data={'league_ranker': ['py.typed']},
     url='https://ranker.readthedocs.io/en/latest/',
     project_urls={
         'Documentation': 'https://ranker.readthedocs.io/en/latest/',
         'Code': 'https://github.com/PeterJCLaw/ranker',
         'Issue tracker': 'https://github.com/PeterJCLaw/ranker/issues',
@@ -28,14 +28,15 @@
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Typing :: Typed',
     ],
     python_requires='>=3.7',
     setup_requires=[
         'Sphinx >=1.8.5, <5',
     ],
```

