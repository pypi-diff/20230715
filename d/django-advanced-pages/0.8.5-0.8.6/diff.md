# Comparing `tmp/django-advanced-pages-0.8.5.tar.gz` & `tmp/django-advanced-pages-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-advanced-pages-0.8.5.tar", last modified: Mon May  8 07:04:00 2023, max compression
+gzip compressed data, was "django-advanced-pages-0.8.6.tar", last modified: Sat Jul 15 10:43:18 2023, max compression
```

## Comparing `django-advanced-pages-0.8.5.tar` & `django-advanced-pages-0.8.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:04:00.503510 django-advanced-pages-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-08 07:04:00.503510 django-advanced-pages-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 07:03:53.000000 django-advanced-pages-0.8.5/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 07:04:00.503510 django-advanced-pages-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:04:00.499510 django-advanced-pages-0.8.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:04:00.499510 django-advanced-pages-0.8.5/src/django_advanced_pages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-08 07:04:00.000000 django-advanced-pages-0.8.5/src/django_advanced_pages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-08 07:04:00.000000 django-advanced-pages-0.8.5/src/django_advanced_pages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 07:04:00.000000 django-advanced-pages-0.8.5/src/django_advanced_pages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-08 07:04:00.000000 django-advanced-pages-0.8.5/src/django_advanced_pages.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-08 07:04:00.000000 django-advanced-pages-0.8.5/src/django_advanced_pages.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:04:00.499510 django-advanced-pages-0.8.5/src/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:04:00.499510 django-advanced-pages-0.8.5/src/pages/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/fixtures/initial_pages.json
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:04:00.503510 django-advanced-pages-0.8.5/src/pages/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/migrations/0002_auto_20210609_2039.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/migrations/0003_auto_20210621_0847.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/src/pages/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 07:04:00.503510 django-advanced-pages-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/tests/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-08 07:03:49.000000 django-advanced-pages-0.8.5/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:43:18.805046 django-advanced-pages-0.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-15 10:43:18.805046 django-advanced-pages-0.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-15 10:43:11.000000 django-advanced-pages-0.8.6/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 10:43:18.805046 django-advanced-pages-0.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:43:18.801046 django-advanced-pages-0.8.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:43:18.801046 django-advanced-pages-0.8.6/src/django_advanced_pages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-15 10:43:18.000000 django-advanced-pages-0.8.6/src/django_advanced_pages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-15 10:43:18.000000 django-advanced-pages-0.8.6/src/django_advanced_pages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 10:43:18.000000 django-advanced-pages-0.8.6/src/django_advanced_pages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 10:43:18.000000 django-advanced-pages-0.8.6/src/django_advanced_pages.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-15 10:43:18.000000 django-advanced-pages-0.8.6/src/django_advanced_pages.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:43:18.801046 django-advanced-pages-0.8.6/src/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/src/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/src/pages/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/src/pages/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:43:18.801046 django-advanced-pages-0.8.6/src/pages/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/src/pages/fixtures/initial_pages.json
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/src/pages/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:43:18.805046 django-advanced-pages-0.8.6/src/pages/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/src/pages/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/src/pages/migrations/0002_auto_20210609_2039.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/src/pages/migrations/0003_auto_20210621_0847.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/src/pages/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/src/pages/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:43:18.805046 django-advanced-pages-0.8.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/tests/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-15 10:43:05.000000 django-advanced-pages-0.8.6/tests/urls.py
```

### Comparing `django-advanced-pages-0.8.5/LICENSE` & `django-advanced-pages-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.5/PKG-INFO` & `django-advanced-pages-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-advanced-pages
-Version: 0.8.5
+Version: 0.8.6
 Summary: Django flatpages with advanced features
 Home-page: https://github.com/snake-soft/django-advanced-pages
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: GPL3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-advanced-pages-0.8.5/README.rst` & `django-advanced-pages-0.8.6/README.rst`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.5/setup.py` & `django-advanced-pages-0.8.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 from setuptools import find_packages, setup
 from src.pages import __version__
 
 
 install_requires = [
-    'django>=3.0,<3.3',
+    'django>=3.0,<5',
 ]
 
 tests_require = [
 ]
 
 setup(
     name='django-advanced-pages',
```

### Comparing `django-advanced-pages-0.8.5/src/django_advanced_pages.egg-info/PKG-INFO` & `django-advanced-pages-0.8.6/src/django_advanced_pages.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-advanced-pages
-Version: 0.8.5
+Version: 0.8.6
 Summary: Django flatpages with advanced features
 Home-page: https://github.com/snake-soft/django-advanced-pages
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: GPL3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-advanced-pages-0.8.5/src/django_advanced_pages.egg-info/SOURCES.txt` & `django-advanced-pages-0.8.6/src/django_advanced_pages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.5/src/pages/admin.py` & `django-advanced-pages-0.8.6/src/pages/admin.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.5/src/pages/fixtures/initial_pages.json` & `django-advanced-pages-0.8.6/src/pages/fixtures/initial_pages.json`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.5/src/pages/migrations/0001_initial.py` & `django-advanced-pages-0.8.6/src/pages/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.5/src/pages/migrations/0003_auto_20210621_0847.py` & `django-advanced-pages-0.8.6/src/pages/migrations/0003_auto_20210621_0847.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.5/src/pages/models.py` & `django-advanced-pages-0.8.6/src/pages/models.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.5/tests/manage.py` & `django-advanced-pages-0.8.6/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.5/tests/settings.py` & `django-advanced-pages-0.8.6/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-advanced-pages-0.8.5/tests/test_models.py` & `django-advanced-pages-0.8.6/tests/test_models.py`

 * *Files identical despite different names*

