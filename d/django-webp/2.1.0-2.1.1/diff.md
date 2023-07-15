# Comparing `tmp/django-webp-2.1.0.tar.gz` & `tmp/django-webp-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-webp-2.1.0.tar", last modified: Tue Jul 11 21:10:38 2023, max compression
+gzip compressed data, was "django-webp-2.1.1.tar", last modified: Sat Jul 15 15:17:00 2023, max compression
```

## Comparing `django-webp-2.1.0.tar` & `django-webp-2.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:38.578149 django-webp-2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:38.570149 django-webp-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:38.570149 django-webp-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-11 21:10:25.000000 django-webp-2.1.0/.github/workflows/django.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-11 21:10:25.000000 django-webp-2.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-11 21:10:25.000000 django-webp-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-11 21:10:25.000000 django-webp-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-07-11 21:10:38.578149 django-webp-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-11 21:10:25.000000 django-webp-2.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-11 21:10:25.000000 django-webp-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 21:10:38.578149 django-webp-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:38.570149 django-webp-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:38.570149 django-webp-2.1.0/src/django_webp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:25.000000 django-webp-2.1.0/src/django_webp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-11 21:10:25.000000 django-webp-2.1.0/src/django_webp/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:38.574149 django-webp-2.1.0/src/django_webp/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:25.000000 django-webp-2.1.0/src/django_webp/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:38.574149 django-webp-2.1.0/src/django_webp/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:25.000000 django-webp-2.1.0/src/django_webp/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-11 21:10:25.000000 django-webp-2.1.0/src/django_webp/management/commands/clean_webp_images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:38.574149 django-webp-2.1.0/src/django_webp/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:25.000000 django-webp-2.1.0/src/django_webp/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-07-11 21:10:25.000000 django-webp-2.1.0/src/django_webp/templatetags/webp.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-11 21:10:25.000000 django-webp-2.1.0/src/django_webp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:38.574149 django-webp-2.1.0/src/django_webp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-07-11 21:10:38.000000 django-webp-2.1.0/src/django_webp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-11 21:10:38.000000 django-webp-2.1.0/src/django_webp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 21:10:38.000000 django-webp-2.1.0/src/django_webp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 21:10:38.000000 django-webp-2.1.0/src/django_webp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-11 21:10:38.000000 django-webp-2.1.0/src/django_webp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:38.574149 django-webp-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:25.000000 django-webp-2.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-11 21:10:25.000000 django-webp-2.1.0/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:38.570149 django-webp-2.1.0/tests/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:38.574149 django-webp-2.1.0/tests/static/django_webp/
--rw-r--r--   0 runner    (1001) docker     (123)   129327 2023-07-11 21:10:25.000000 django-webp-2.1.0/tests/static/django_webp/python.png
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-11 21:10:25.000000 django-webp-2.1.0/tests/test_WEBPImageConverter.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-11 21:10:25.000000 django-webp-2.1.0/tests/test_context_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-11 21:10:25.000000 django-webp-2.1.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-11 21:10:25.000000 django-webp-2.1.0/tests/test_templatetags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:38.578149 django-webp-2.1.0/tests/testapp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:25.000000 django-webp-2.1.0/tests/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 21:10:25.000000 django-webp-2.1.0/tests/testapp/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 21:10:25.000000 django-webp-2.1.0/tests/testapp/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:38.578149 django-webp-2.1.0/tests/testapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:25.000000 django-webp-2.1.0/tests/testapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-11 21:10:25.000000 django-webp-2.1.0/tests/testapp/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:38.570149 django-webp-2.1.0/tests/testapp/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:10:38.578149 django-webp-2.1.0/tests/testapp/templates/django_webp/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-11 21:10:25.000000 django-webp-2.1.0/tests/testapp/templates/django_webp/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 21:10:25.000000 django-webp-2.1.0/tests/testapp/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-11 21:10:25.000000 django-webp-2.1.0/tests/testapp/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 21:10:25.000000 django-webp-2.1.0/tests/testapp/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:17:00.051370 django-webp-2.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:17:00.047370 django-webp-2.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:17:00.047370 django-webp-2.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-15 15:16:40.000000 django-webp-2.1.1/.github/workflows/django.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-15 15:16:40.000000 django-webp-2.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-15 15:16:40.000000 django-webp-2.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-15 15:16:40.000000 django-webp-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-07-15 15:17:00.051370 django-webp-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-15 15:16:40.000000 django-webp-2.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-15 15:16:40.000000 django-webp-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 15:17:00.051370 django-webp-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:17:00.047370 django-webp-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:17:00.047370 django-webp-2.1.1/src/django_webp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:40.000000 django-webp-2.1.1/src/django_webp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-15 15:16:40.000000 django-webp-2.1.1/src/django_webp/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:17:00.047370 django-webp-2.1.1/src/django_webp/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:40.000000 django-webp-2.1.1/src/django_webp/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:17:00.047370 django-webp-2.1.1/src/django_webp/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:40.000000 django-webp-2.1.1/src/django_webp/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-15 15:16:40.000000 django-webp-2.1.1/src/django_webp/management/commands/clean_webp_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:17:00.047370 django-webp-2.1.1/src/django_webp/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:40.000000 django-webp-2.1.1/src/django_webp/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-07-15 15:16:40.000000 django-webp-2.1.1/src/django_webp/templatetags/webp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-15 15:16:40.000000 django-webp-2.1.1/src/django_webp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:17:00.047370 django-webp-2.1.1/src/django_webp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-07-15 15:17:00.000000 django-webp-2.1.1/src/django_webp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-15 15:17:00.000000 django-webp-2.1.1/src/django_webp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 15:17:00.000000 django-webp-2.1.1/src/django_webp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-15 15:17:00.000000 django-webp-2.1.1/src/django_webp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 15:17:00.000000 django-webp-2.1.1/src/django_webp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:17:00.051370 django-webp-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:40.000000 django-webp-2.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-15 15:16:40.000000 django-webp-2.1.1/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:17:00.047370 django-webp-2.1.1/tests/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:17:00.051370 django-webp-2.1.1/tests/static/django_webp/
+-rw-r--r--   0 runner    (1001) docker     (123)   129327 2023-07-15 15:16:40.000000 django-webp-2.1.1/tests/static/django_webp/python.png
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-15 15:16:40.000000 django-webp-2.1.1/tests/test_WEBPImageConverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-15 15:16:40.000000 django-webp-2.1.1/tests/test_context_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-15 15:16:40.000000 django-webp-2.1.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-15 15:16:40.000000 django-webp-2.1.1/tests/test_templatetags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:17:00.051370 django-webp-2.1.1/tests/testapp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:40.000000 django-webp-2.1.1/tests/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-15 15:16:40.000000 django-webp-2.1.1/tests/testapp/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-15 15:16:40.000000 django-webp-2.1.1/tests/testapp/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:17:00.051370 django-webp-2.1.1/tests/testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 15:16:40.000000 django-webp-2.1.1/tests/testapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-15 15:16:40.000000 django-webp-2.1.1/tests/testapp/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:17:00.047370 django-webp-2.1.1/tests/testapp/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:17:00.051370 django-webp-2.1.1/tests/testapp/templates/django_webp/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-15 15:16:40.000000 django-webp-2.1.1/tests/testapp/templates/django_webp/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-15 15:16:40.000000 django-webp-2.1.1/tests/testapp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-15 15:16:40.000000 django-webp-2.1.1/tests/testapp/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-15 15:16:40.000000 django-webp-2.1.1/tests/testapp/wsgi.py
```

### Comparing `django-webp-2.1.0/.github/workflows/django.yml` & `django-webp-2.1.1/.github/workflows/django.yml`

 * *Files identical despite different names*

### Comparing `django-webp-2.1.0/.github/workflows/python-publish.yml` & `django-webp-2.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `django-webp-2.1.0/.gitignore` & `django-webp-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `django-webp-2.1.0/LICENSE` & `django-webp-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webp-2.1.0/PKG-INFO` & `django-webp-2.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webp
-Version: 2.1.0
+Version: 2.1.1
 Summary: Returns a webp image instead of jpg, gif or png to browsers
 Author-email: Andre Farzat <andrefarzat@gmail.com>, Daniel Opara <daniel.opara@tufts.edu>
 Maintainer-email: Andre Farzat <andrefarzat@gmail.com>, Daniel Opara <daniel.opara@tufts.edu>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 André Farzat
         
@@ -37,16 +37,15 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 django-webp
 ===========
 
-Returns a webp image instead of jpg, gif or png to browsers which have
-support.
+Speeds up static file load times by generating a webp image to load to a webpage instead of a jpg, gif or png
 
 |Build Status| |Coverage Status|
 
 
 Usage
 -----
```

### Comparing `django-webp-2.1.0/README.rst` & `django-webp-2.1.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 django-webp
 ===========
 
-Returns a webp image instead of jpg, gif or png to browsers which have
-support.
+Speeds up static file load times by generating a webp image to load to a webpage instead of a jpg, gif or png
 
 |Build Status| |Coverage Status|
 
 
 Usage
 -----
```

### Comparing `django-webp-2.1.0/pyproject.toml` & `django-webp-2.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires      = ["setuptools>=61.0.0", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 
 [project]
 name = "django-webp"
-version = "2.1.0"
+version = "2.1.1"
 description = "Returns a webp image instead of jpg, gif or png to browsers"
 readme = "README.rst"
 requires-python = ">=3.5"
 keywords = ["django", "webp", "python"]
 authors = [
     { name = "Andre Farzat", email = "andrefarzat@gmail.com" },
     { name = "Daniel Opara", email = "daniel.opara@tufts.edu" }
```

### Comparing `django-webp-2.1.0/src/django_webp/templatetags/webp.py` & `django-webp-2.1.1/src/django_webp/templatetags/webp.py`

 * *Files identical despite different names*

### Comparing `django-webp-2.1.0/src/django_webp/utils.py` & `django-webp-2.1.1/src/django_webp/utils.py`

 * *Files identical despite different names*

### Comparing `django-webp-2.1.0/src/django_webp.egg-info/PKG-INFO` & `django-webp-2.1.1/src/django_webp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webp
-Version: 2.1.0
+Version: 2.1.1
 Summary: Returns a webp image instead of jpg, gif or png to browsers
 Author-email: Andre Farzat <andrefarzat@gmail.com>, Daniel Opara <daniel.opara@tufts.edu>
 Maintainer-email: Andre Farzat <andrefarzat@gmail.com>, Daniel Opara <daniel.opara@tufts.edu>
 License: The MIT License (MIT)
         
         Copyright (c) 2023 André Farzat
         
@@ -37,16 +37,15 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 django-webp
 ===========
 
-Returns a webp image instead of jpg, gif or png to browsers which have
-support.
+Speeds up static file load times by generating a webp image to load to a webpage instead of a jpg, gif or png
 
 |Build Status| |Coverage Status|
 
 
 Usage
 -----
```

### Comparing `django-webp-2.1.0/src/django_webp.egg-info/SOURCES.txt` & `django-webp-2.1.1/src/django_webp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-webp-2.1.0/tests/manage.py` & `django-webp-2.1.1/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-webp-2.1.0/tests/static/django_webp/python.png` & `django-webp-2.1.1/tests/static/django_webp/python.png`

 * *Files identical despite different names*

### Comparing `django-webp-2.1.0/tests/test_WEBPImageConverter.py` & `django-webp-2.1.1/tests/test_WEBPImageConverter.py`

 * *Files identical despite different names*

### Comparing `django-webp-2.1.0/tests/test_context_processor.py` & `django-webp-2.1.1/tests/test_context_processor.py`

 * *Files identical despite different names*

### Comparing `django-webp-2.1.0/tests/test_main.py` & `django-webp-2.1.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `django-webp-2.1.0/tests/test_templatetags.py` & `django-webp-2.1.1/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-webp-2.1.0/tests/testapp/settings.py` & `django-webp-2.1.1/tests/testapp/settings.py`

 * *Files identical despite different names*

