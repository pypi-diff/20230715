# Comparing `tmp/django-hatchway-0.5.1.tar.gz` & `tmp/django-hatchway-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-hatchway-0.5.1.tar", last modified: Wed Mar 22 22:17:59 2023, max compression
+gzip compressed data, was "django-hatchway-0.5.2.tar", last modified: Sat Jul 15 18:42:46 2023, max compression
```

## Comparing `django-hatchway-0.5.1.tar` & `django-hatchway-0.5.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-22 22:17:59.811490 django-hatchway-0.5.1/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1458 2023-02-11 19:37:58.000000 django-hatchway-0.5.1/LICENSE
--rw-r--r--   0 andrew    (1000) andrew    (1000)     7920 2023-03-22 22:17:59.811490 django-hatchway-0.5.1/PKG-INFO
--rw-r--r--   0 andrew    (1000) andrew    (1000)     7559 2023-03-22 22:17:51.000000 django-hatchway-0.5.1/README.rst
-drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-22 22:17:59.811490 django-hatchway-0.5.1/django_hatchway.egg-info/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     7920 2023-03-22 22:17:59.000000 django-hatchway-0.5.1/django_hatchway.egg-info/PKG-INFO
--rw-r--r--   0 andrew    (1000) andrew    (1000)      414 2023-03-22 22:17:59.000000 django-hatchway-0.5.1/django_hatchway.egg-info/SOURCES.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)        1 2023-03-22 22:17:59.000000 django-hatchway-0.5.1/django_hatchway.egg-info/dependency_links.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)       65 2023-03-22 22:17:59.000000 django-hatchway-0.5.1/django_hatchway.egg-info/requires.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)        9 2023-03-22 22:17:59.000000 django-hatchway-0.5.1/django_hatchway.egg-info/top_level.txt
-drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-22 22:17:59.811490 django-hatchway-0.5.1/hatchway/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      252 2023-03-22 22:13:53.000000 django-hatchway-0.5.1/hatchway/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)       86 2023-02-11 18:18:05.000000 django-hatchway-0.5.1/hatchway/apps.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)      237 2023-02-11 18:52:42.000000 django-hatchway-0.5.1/hatchway/constants.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1292 2023-02-11 18:03:40.000000 django-hatchway-0.5.1/hatchway/http.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1440 2023-02-11 18:03:40.000000 django-hatchway-0.5.1/hatchway/schema.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     4168 2023-02-11 19:19:12.000000 django-hatchway-0.5.1/hatchway/types.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)      922 2023-02-11 18:03:40.000000 django-hatchway-0.5.1/hatchway/urls.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)    13319 2023-03-22 22:12:58.000000 django-hatchway-0.5.1/hatchway/view.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)      729 2023-02-11 19:48:57.000000 django-hatchway-0.5.1/pyproject.toml
--rw-r--r--   0 andrew    (1000) andrew    (1000)       38 2023-03-22 22:17:59.811490 django-hatchway-0.5.1/setup.cfg
-drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-22 22:17:59.811490 django-hatchway-0.5.1/tests/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2421 2023-02-11 19:52:16.000000 django-hatchway-0.5.1/tests/test_types.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     8128 2023-03-22 22:13:24.000000 django-hatchway-0.5.1/tests/test_view.py
+drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-15 18:42:46.906518 django-hatchway-0.5.2/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1458 2023-07-15 17:35:56.000000 django-hatchway-0.5.2/LICENSE
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     7919 2023-07-15 18:42:46.906518 django-hatchway-0.5.2/PKG-INFO
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     7558 2023-07-15 18:42:43.000000 django-hatchway-0.5.2/README.rst
+drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-15 18:42:46.906518 django-hatchway-0.5.2/django_hatchway.egg-info/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     7919 2023-07-15 18:42:46.000000 django-hatchway-0.5.2/django_hatchway.egg-info/PKG-INFO
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      414 2023-07-15 18:42:46.000000 django-hatchway-0.5.2/django_hatchway.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew    (1000) andrew    (1000)        1 2023-07-15 18:42:46.000000 django-hatchway-0.5.2/django_hatchway.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew    (1000) andrew    (1000)       65 2023-07-15 18:42:46.000000 django-hatchway-0.5.2/django_hatchway.egg-info/requires.txt
+-rw-r--r--   0 andrew    (1000) andrew    (1000)        9 2023-07-15 18:42:46.000000 django-hatchway-0.5.2/django_hatchway.egg-info/top_level.txt
+drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-15 18:42:46.906518 django-hatchway-0.5.2/hatchway/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      252 2023-07-15 18:40:36.000000 django-hatchway-0.5.2/hatchway/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)       86 2023-07-15 17:35:56.000000 django-hatchway-0.5.2/hatchway/apps.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      237 2023-07-15 17:35:56.000000 django-hatchway-0.5.2/hatchway/constants.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1292 2023-07-15 17:35:56.000000 django-hatchway-0.5.2/hatchway/http.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1440 2023-07-15 17:35:56.000000 django-hatchway-0.5.2/hatchway/schema.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     4168 2023-07-15 17:38:34.000000 django-hatchway-0.5.2/hatchway/types.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      922 2023-07-15 17:35:56.000000 django-hatchway-0.5.2/hatchway/urls.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)    13319 2023-07-15 17:44:55.000000 django-hatchway-0.5.2/hatchway/view.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      729 2023-07-15 17:35:56.000000 django-hatchway-0.5.2/pyproject.toml
+-rw-r--r--   0 andrew    (1000) andrew    (1000)       38 2023-07-15 18:42:46.906518 django-hatchway-0.5.2/setup.cfg
+drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2023-07-15 18:42:46.906518 django-hatchway-0.5.2/tests/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2421 2023-07-15 17:35:56.000000 django-hatchway-0.5.2/tests/test_types.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     8128 2023-07-15 17:35:56.000000 django-hatchway-0.5.2/tests/test_view.py
```

### Comparing `django-hatchway-0.5.1/LICENSE` & `django-hatchway-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-hatchway-0.5.1/PKG-INFO` & `django-hatchway-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hatchway
-Version: 0.5.1
+Version: 0.5.2
 Summary: An unsurprising Django API framework
 Author-email: Andrew Godwin <andrew@aeracode.org>
 License: BSD-3-Clause
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
@@ -25,15 +25,14 @@
 Installation
 ------------
 
 Install Hatchway from PyPI::
 
     pip install django-hatchway
 
-
 And add it to your ``INSTALLED_APPS``::
 
     INSTALLED_APPS = [
         ...
         "hatchway",
     ]
```

### Comparing `django-hatchway-0.5.1/README.rst` & `django-hatchway-0.5.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 Installation
 ------------
 
 Install Hatchway from PyPI::
 
     pip install django-hatchway
 
-
 And add it to your ``INSTALLED_APPS``::
 
     INSTALLED_APPS = [
         ...
         "hatchway",
     ]
```

### Comparing `django-hatchway-0.5.1/django_hatchway.egg-info/PKG-INFO` & `django-hatchway-0.5.2/django_hatchway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hatchway
-Version: 0.5.1
+Version: 0.5.2
 Summary: An unsurprising Django API framework
 Author-email: Andrew Godwin <andrew@aeracode.org>
 License: BSD-3-Clause
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
@@ -25,15 +25,14 @@
 Installation
 ------------
 
 Install Hatchway from PyPI::
 
     pip install django-hatchway
 
-
 And add it to your ``INSTALLED_APPS``::
 
     INSTALLED_APPS = [
         ...
         "hatchway",
     ]
```

### Comparing `django-hatchway-0.5.1/hatchway/http.py` & `django-hatchway-0.5.2/hatchway/http.py`

 * *Files identical despite different names*

### Comparing `django-hatchway-0.5.1/hatchway/schema.py` & `django-hatchway-0.5.2/hatchway/schema.py`

 * *Files identical despite different names*

### Comparing `django-hatchway-0.5.1/hatchway/types.py` & `django-hatchway-0.5.2/hatchway/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
 
 def acceptable_input(annotation) -> bool:
     """
     Returns if this annotation is something we think we can accept as input
     """
     _, inner_type = extract_signifier(annotation)
-    if is_model_subclass(annotation):
+    if is_model_subclass(inner_type):
         return True
     if inner_type in [
         str,
         int,
         list,
         tuple,
         set,
```

### Comparing `django-hatchway-0.5.1/hatchway/urls.py` & `django-hatchway-0.5.2/hatchway/urls.py`

 * *Files identical despite different names*

### Comparing `django-hatchway-0.5.1/hatchway/view.py` & `django-hatchway-0.5.2/hatchway/view.py`

 * *Files identical despite different names*

### Comparing `django-hatchway-0.5.1/pyproject.toml` & `django-hatchway-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-hatchway-0.5.1/tests/test_types.py` & `django-hatchway-0.5.2/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `django-hatchway-0.5.1/tests/test_view.py` & `django-hatchway-0.5.2/tests/test_view.py`

 * *Files identical despite different names*

