# Comparing `tmp/django-oscar-pg-search-0.9.4.tar.gz` & `tmp/django-oscar-pg-search-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oscar-pg-search-0.9.4.tar", last modified: Tue Jun 20 14:43:28 2023, max compression
+gzip compressed data, was "django-oscar-pg-search-0.9.5.tar", last modified: Sat Jul 15 10:37:08 2023, max compression
```

## Comparing `django-oscar-pg-search-0.9.4.tar` & `django-oscar-pg-search-0.9.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:28.590494 django-oscar-pg-search-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-06-20 14:43:28.590494 django-oscar-pg-search-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 14:43:20.000000 django-oscar-pg-search-0.9.4/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:43:28.590494 django-oscar-pg-search-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:28.586494 django-oscar-pg-search-0.9.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:28.586494 django-oscar-pg-search-0.9.4/src/django_oscar_pg_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-06-20 14:43:28.000000 django-oscar-pg-search-0.9.4/src/django_oscar_pg_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-20 14:43:28.000000 django-oscar-pg-search-0.9.4/src/django_oscar_pg_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:43:28.000000 django-oscar-pg-search-0.9.4/src/django_oscar_pg_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 14:43:28.000000 django-oscar-pg-search-0.9.4/src/django_oscar_pg_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 14:43:28.000000 django-oscar-pg-search-0.9.4/src/django_oscar_pg_search.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:28.590494 django-oscar-pg-search-0.9.4/src/oscar_pg_search/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/src/oscar_pg_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/src/oscar_pg_search/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:28.590494 django-oscar-pg-search-0.9.4/src/oscar_pg_search/filter_options/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/src/oscar_pg_search/filter_options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/src/oscar_pg_search/filter_options/attribute_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/src/oscar_pg_search/filter_options/base_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/src/oscar_pg_search/filter_options/base_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/src/oscar_pg_search/filter_options/filter_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/src/oscar_pg_search/filter_options/offer_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/src/oscar_pg_search/filter_options/product_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/src/oscar_pg_search/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/src/oscar_pg_search/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/src/oscar_pg_search/order_by_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/src/oscar_pg_search/postgres_search_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:28.586494 django-oscar-pg-search-0.9.4/src/oscar_pg_search/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:28.586494 django-oscar-pg-search-0.9.4/src/oscar_pg_search/templates/oscar_pg_search/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:28.586494 django-oscar-pg-search-0.9.4/src/oscar_pg_search/templates/oscar_pg_search/catalogue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:28.590494 django-oscar-pg-search-0.9.4/src/oscar_pg_search/templates/oscar_pg_search/catalogue/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/src/oscar_pg_search/templates/oscar_pg_search/catalogue/partials/filter_forms.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:28.590494 django-oscar-pg-search-0.9.4/src/oscar_pg_search/templates/oscar_pg_search/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/src/oscar_pg_search/templates/oscar_pg_search/partials/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:28.590494 django-oscar-pg-search-0.9.4/src/oscar_pg_search/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/src/oscar_pg_search/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/src/oscar_pg_search/templatetags/oscar_pg_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/src/oscar_pg_search/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:28.590494 django-oscar-pg-search-0.9.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/tests/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/tests/test_search_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-20 14:43:17.000000 django-oscar-pg-search-0.9.4/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:08.942492 django-oscar-pg-search-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-15 10:37:08.942492 django-oscar-pg-search-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-15 10:37:01.000000 django-oscar-pg-search-0.9.5/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 10:37:08.942492 django-oscar-pg-search-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:08.934492 django-oscar-pg-search-0.9.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:08.938492 django-oscar-pg-search-0.9.5/src/django_oscar_pg_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-15 10:37:08.000000 django-oscar-pg-search-0.9.5/src/django_oscar_pg_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-15 10:37:08.000000 django-oscar-pg-search-0.9.5/src/django_oscar_pg_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 10:37:08.000000 django-oscar-pg-search-0.9.5/src/django_oscar_pg_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-15 10:37:08.000000 django-oscar-pg-search-0.9.5/src/django_oscar_pg_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-15 10:37:08.000000 django-oscar-pg-search-0.9.5/src/django_oscar_pg_search.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:08.938492 django-oscar-pg-search-0.9.5/src/oscar_pg_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/src/oscar_pg_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/src/oscar_pg_search/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:08.938492 django-oscar-pg-search-0.9.5/src/oscar_pg_search/filter_options/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/src/oscar_pg_search/filter_options/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/src/oscar_pg_search/filter_options/attribute_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/src/oscar_pg_search/filter_options/base_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/src/oscar_pg_search/filter_options/base_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/src/oscar_pg_search/filter_options/filter_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/src/oscar_pg_search/filter_options/offer_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/src/oscar_pg_search/filter_options/product_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/src/oscar_pg_search/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/src/oscar_pg_search/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/src/oscar_pg_search/order_by_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/src/oscar_pg_search/postgres_search_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:08.938492 django-oscar-pg-search-0.9.5/src/oscar_pg_search/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:08.938492 django-oscar-pg-search-0.9.5/src/oscar_pg_search/templates/oscar_pg_search/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:08.938492 django-oscar-pg-search-0.9.5/src/oscar_pg_search/templates/oscar_pg_search/catalogue/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:08.938492 django-oscar-pg-search-0.9.5/src/oscar_pg_search/templates/oscar_pg_search/catalogue/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/src/oscar_pg_search/templates/oscar_pg_search/catalogue/partials/filter_forms.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:08.938492 django-oscar-pg-search-0.9.5/src/oscar_pg_search/templates/oscar_pg_search/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/src/oscar_pg_search/templates/oscar_pg_search/partials/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:08.942492 django-oscar-pg-search-0.9.5/src/oscar_pg_search/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/src/oscar_pg_search/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/src/oscar_pg_search/templatetags/oscar_pg_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/src/oscar_pg_search/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 10:37:08.942492 django-oscar-pg-search-0.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      655 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/tests/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/tests/test_search_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-15 10:36:56.000000 django-oscar-pg-search-0.9.5/tests/urls.py
```

### Comparing `django-oscar-pg-search-0.9.4/LICENSE` & `django-oscar-pg-search-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.4/PKG-INFO` & `django-oscar-pg-search-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscar-pg-search
-Version: 0.9.4
+Version: 0.9.5
 Summary: Pure Postgresql search backend for Django Oscar
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-oscar-pg-search-0.9.4/README.md` & `django-oscar-pg-search-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.4/setup.py` & `django-oscar-pg-search-0.9.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 from setuptools import find_packages, setup
 from src.oscar_pg_search import __version__
 
 
 install_requires = [
-    'django>=3.0,<3.3',
+    'django>=3.0,<5',
     'django-oscar>=2.0,<3.3',
 ]
 
 tests_require = [
     'coverage>=5.5,<5.6',
 ]
```

### Comparing `django-oscar-pg-search-0.9.4/src/django_oscar_pg_search.egg-info/PKG-INFO` & `django-oscar-pg-search-0.9.5/src/django_oscar_pg_search.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscar-pg-search
-Version: 0.9.4
+Version: 0.9.5
 Summary: Pure Postgresql search backend for Django Oscar
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-oscar-pg-search-0.9.4/src/django_oscar_pg_search.egg-info/SOURCES.txt` & `django-oscar-pg-search-0.9.5/src/django_oscar_pg_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.4/src/oscar_pg_search/apps.py` & `django-oscar-pg-search-0.9.5/src/oscar_pg_search/apps.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.4/src/oscar_pg_search/filter_options/attribute_fields.py` & `django-oscar-pg-search-0.9.5/src/oscar_pg_search/filter_options/attribute_fields.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.4/src/oscar_pg_search/filter_options/base_fields.py` & `django-oscar-pg-search-0.9.5/src/oscar_pg_search/filter_options/base_fields.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.4/src/oscar_pg_search/filter_options/filter_forms.py` & `django-oscar-pg-search-0.9.5/src/oscar_pg_search/filter_options/filter_forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.4/src/oscar_pg_search/filter_options/offer_fields.py` & `django-oscar-pg-search-0.9.5/src/oscar_pg_search/filter_options/offer_fields.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.4/src/oscar_pg_search/filter_options/product_fields.py` & `django-oscar-pg-search-0.9.5/src/oscar_pg_search/filter_options/product_fields.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.4/src/oscar_pg_search/forms.py` & `django-oscar-pg-search-0.9.5/src/oscar_pg_search/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.4/src/oscar_pg_search/mixins.py` & `django-oscar-pg-search-0.9.5/src/oscar_pg_search/mixins.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.4/src/oscar_pg_search/order_by_options.py` & `django-oscar-pg-search-0.9.5/src/oscar_pg_search/order_by_options.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.4/src/oscar_pg_search/postgres_search_handler.py` & `django-oscar-pg-search-0.9.5/src/oscar_pg_search/postgres_search_handler.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.4/src/oscar_pg_search/templates/oscar_pg_search/catalogue/partials/filter_forms.html` & `django-oscar-pg-search-0.9.5/src/oscar_pg_search/templates/oscar_pg_search/catalogue/partials/filter_forms.html`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.4/src/oscar_pg_search/templates/oscar_pg_search/partials/search.html` & `django-oscar-pg-search-0.9.5/src/oscar_pg_search/templates/oscar_pg_search/partials/search.html`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.4/src/oscar_pg_search/templatetags/oscar_pg_search.py` & `django-oscar-pg-search-0.9.5/src/oscar_pg_search/templatetags/oscar_pg_search.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.4/src/oscar_pg_search/utils.py` & `django-oscar-pg-search-0.9.5/src/oscar_pg_search/utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.4/tests/manage.py` & `django-oscar-pg-search-0.9.5/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-oscar-pg-search-0.9.4/tests/settings.py` & `django-oscar-pg-search-0.9.5/tests/settings.py`

 * *Files identical despite different names*

