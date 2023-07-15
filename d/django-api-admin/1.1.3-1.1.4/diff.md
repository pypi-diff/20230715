# Comparing `tmp/django-api-admin-1.1.3.tar.gz` & `tmp/django-api-admin-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-api-admin-1.1.3.tar", last modified: Sat Jun 17 11:58:18 2023, max compression
+gzip compressed data, was "django-api-admin-1.1.4.tar", last modified: Sat Jul 15 03:37:56 2023, max compression
```

## Comparing `django-api-admin-1.1.3.tar` & `django-api-admin-1.1.4.tar`

### file list

```diff
@@ -1,31 +1,55 @@
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 11:58:18.216513 django-api-admin-1.1.3/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1071 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/LICENSE
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       90 2023-06-17 11:37:37.000000 django-api-admin-1.1.3/MANIFEST.in
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     2982 2023-06-17 11:58:18.216513 django-api-admin-1.1.3/PKG-INFO
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     2291 2023-06-17 11:38:23.000000 django-api-admin-1.1.3/README.md
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 11:58:18.213180 django-api-admin-1.1.3/django_api_admin/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/__init__.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1771 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/actions.py
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 11:58:18.213180 django-api-admin-1.1.3/django_api_admin/declarations/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/declarations/__init__.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1324 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/declarations/classes.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    13151 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/declarations/functions.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3726 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/field_attributes.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    11294 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/options.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      548 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/pagination.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      335 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/permissions.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     5255 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/serializers.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    12948 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/sites.py
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 11:58:18.216513 django-api-admin-1.1.3/django_api_admin/views/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/views/__init__.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    26075 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/views/admin_views.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    11410 2023-06-17 06:59:46.000000 django-api-admin-1.1.3/django_api_admin/views/fields_test_views.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     8327 2023-06-17 11:36:49.000000 django-api-admin-1.1.3/django_api_admin/views/site_views.py
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-06-17 11:58:18.213180 django-api-admin-1.1.3/django_api_admin.egg-info/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     2982 2023-06-17 11:58:18.000000 django-api-admin-1.1.3/django_api_admin.egg-info/PKG-INFO
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      760 2023-06-17 11:58:18.000000 django-api-admin-1.1.3/django_api_admin.egg-info/SOURCES.txt
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        1 2023-06-17 11:58:18.000000 django-api-admin-1.1.3/django_api_admin.egg-info/dependency_links.txt
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       27 2023-06-17 11:58:18.000000 django-api-admin-1.1.3/django_api_admin.egg-info/requires.txt
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       17 2023-06-17 11:58:18.000000 django-api-admin-1.1.3/django_api_admin.egg-info/top_level.txt
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       38 2023-06-17 11:58:18.216513 django-api-admin-1.1.3/setup.cfg
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1111 2023-06-17 11:57:33.000000 django-api-admin-1.1.3/setup.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.776485 django-api-admin-1.1.4/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1071 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/LICENSE
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       90 2023-07-15 03:29:35.000000 django-api-admin-1.1.4/MANIFEST.in
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3043 2023-07-15 03:37:56.776485 django-api-admin-1.1.4/PKG-INFO
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     2301 2023-07-15 03:29:35.000000 django-api-admin-1.1.4/README.md
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.766485 django-api-admin-1.1.4/django_api_admin/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/__init__.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.773152 django-api-admin-1.1.4/django_api_admin/__pycache__/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      202 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3000 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/actions.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     4322 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      591 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3227 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/field_attributes.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3344 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    17261 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/options.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1454 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/pagination.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1124 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/permissions.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     8333 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/serializers.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    17194 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/sites.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1771 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/actions.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.773152 django-api-admin-1.1.4/django_api_admin/declarations/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/declarations/__init__.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.773152 django-api-admin-1.1.4/django_api_admin/declarations/__pycache__/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      215 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/declarations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3397 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/declarations/__pycache__/classes.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    13367 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/declarations/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1324 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/declarations/classes.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    13151 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/declarations/functions.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3726 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/field_attributes.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.763152 django-api-admin-1.1.4/django_api_admin/migrations/
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.773152 django-api-admin-1.1.4/django_api_admin/migrations/__pycache__/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3066 2023-07-15 02:32:57.000000 django-api-admin-1.1.4/django_api_admin/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      213 2023-07-15 02:32:57.000000 django-api-admin-1.1.4/django_api_admin/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    11294 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/options.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      548 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/pagination.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      335 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/permissions.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     5255 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/serializers.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    12948 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/sites.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.776485 django-api-admin-1.1.4/django_api_admin/views/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/views/__init__.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.776485 django-api-admin-1.1.4/django_api_admin/views/__pycache__/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      208 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/views/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    31514 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/views/__pycache__/admin_views.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    13745 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/views/__pycache__/fields_test_views.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    14263 2023-07-15 02:58:40.000000 django-api-admin-1.1.4/django_api_admin/views/__pycache__/site_views.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    26075 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/views/admin_views.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     8315 2023-07-15 03:29:52.000000 django-api-admin-1.1.4/django_api_admin/views/site_views.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.769819 django-api-admin-1.1.4/django_api_admin.egg-info/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3043 2023-07-15 03:37:56.000000 django-api-admin-1.1.4/django_api_admin.egg-info/PKG-INFO
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1901 2023-07-15 03:37:56.000000 django-api-admin-1.1.4/django_api_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        1 2023-07-15 03:37:56.000000 django-api-admin-1.1.4/django_api_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       27 2023-07-15 03:37:56.000000 django-api-admin-1.1.4/django_api_admin.egg-info/requires.txt
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       17 2023-07-15 03:37:56.000000 django-api-admin-1.1.4/django_api_admin.egg-info/top_level.txt
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       38 2023-07-15 03:37:56.776485 django-api-admin-1.1.4/setup.cfg
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1161 2023-07-15 03:34:19.000000 django-api-admin-1.1.4/setup.py
```

### Comparing `django-api-admin-1.1.3/LICENSE` & `django-api-admin-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.3/PKG-INFO` & `django-api-admin-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: django-api-admin
-Version: 1.1.3
+Version: 1.1.4
 Summary: Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.
 Home-page: https://github.com/MuhammadSalahAli/django-api-admin
 Author: Muhammad Salah
 Author-email: msmainacc0unt@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.
 
 ## Features ⚡
 
@@ -24,15 +25,15 @@
 - [x] Customizable AdminSite and ModelAdmin.
 - [x] Supports InlineModelAdmins and bulk edits.
 - [x] Provides data to dynamically create forms on clients from serializers.
 - [x] Extensively tested
 
 ## Demo 🚀
 
-You can also test it in this <a href="https://django-api-admin.demon-bixia.repl.co/" target="_blank">demo</a> that is hosted on replit. use these credentials to login
+You can also test it in this <a href="https://django-api-admin.demon-bixia.repl.co/api_admin/" target="_blank">demo</a> that is hosted on replit. use these credentials to login
 
 * username: admin
 * password: password
 
 ## Requirements 📄
 
 <p>Python 3.9+</p>
```

### Comparing `django-api-admin-1.1.3/README.md` & `django-api-admin-1.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 - [x] Customizable AdminSite and ModelAdmin.
 - [x] Supports InlineModelAdmins and bulk edits.
 - [x] Provides data to dynamically create forms on clients from serializers.
 - [x] Extensively tested
 
 ## Demo 🚀
 
-You can also test it in this <a href="https://django-api-admin.demon-bixia.repl.co/" target="_blank">demo</a> that is hosted on replit. use these credentials to login
+You can also test it in this <a href="https://django-api-admin.demon-bixia.repl.co/api_admin/" target="_blank">demo</a> that is hosted on replit. use these credentials to login
 
 * username: admin
 * password: password
 
 ## Requirements 📄
 
 <p>Python 3.9+</p>
```

### Comparing `django-api-admin-1.1.3/django_api_admin/actions.py` & `django-api-admin-1.1.4/django_api_admin/actions.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.3/django_api_admin/declarations/classes.py` & `django-api-admin-1.1.4/django_api_admin/declarations/classes.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.3/django_api_admin/declarations/functions.py` & `django-api-admin-1.1.4/django_api_admin/declarations/functions.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.3/django_api_admin/field_attributes.py` & `django-api-admin-1.1.4/django_api_admin/field_attributes.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.3/django_api_admin/options.py` & `django-api-admin-1.1.4/django_api_admin/options.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.3/django_api_admin/pagination.py` & `django-api-admin-1.1.4/django_api_admin/pagination.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.3/django_api_admin/serializers.py` & `django-api-admin-1.1.4/django_api_admin/serializers.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.3/django_api_admin/sites.py` & `django-api-admin-1.1.4/django_api_admin/sites.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.3/django_api_admin/views/admin_views.py` & `django-api-admin-1.1.4/django_api_admin/views/admin_views.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.3/django_api_admin/views/site_views.py` & `django-api-admin-1.1.4/django_api_admin/views/site_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def get(self, request, admin_site):
         serializer = self.serializer_class()
         form_fields = get_form_fields(serializer)
         return Response({'fields': form_fields}, status=status.HTTP_200_OK)
 
     def post(self, request, admin_site):
         serializer = self.serializer_class(
-            data=request.data.get('data'), context={'request': request})
+            data=request.data, context={'request': request})
         if serializer.is_valid():
             user = serializer.get_user()
             login(request, user)
             user_serializer = admin_site.user_serializer(user)
             data = {
                 'detail': _('you are logged in successfully'),
                 'user': user_serializer.data
```

### Comparing `django-api-admin-1.1.3/django_api_admin.egg-info/PKG-INFO` & `django-api-admin-1.1.4/django_api_admin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: django-api-admin
-Version: 1.1.3
+Version: 1.1.4
 Summary: Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.
 Home-page: https://github.com/MuhammadSalahAli/django-api-admin
 Author: Muhammad Salah
 Author-email: msmainacc0unt@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.
 
 ## Features ⚡
 
@@ -24,15 +25,15 @@
 - [x] Customizable AdminSite and ModelAdmin.
 - [x] Supports InlineModelAdmins and bulk edits.
 - [x] Provides data to dynamically create forms on clients from serializers.
 - [x] Extensively tested
 
 ## Demo 🚀
 
-You can also test it in this <a href="https://django-api-admin.demon-bixia.repl.co/" target="_blank">demo</a> that is hosted on replit. use these credentials to login
+You can also test it in this <a href="https://django-api-admin.demon-bixia.repl.co/api_admin/" target="_blank">demo</a> that is hosted on replit. use these credentials to login
 
 * username: admin
 * password: password
 
 ## Requirements 📄
 
 <p>Python 3.9+</p>
```

### Comparing `django-api-admin-1.1.3/setup.py` & `django-api-admin-1.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,27 +7,28 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="django-api-admin",
-    version="1.1.3",
+    version="1.1.4",
     description="Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/MuhammadSalahAli/django-api-admin",
     author="Muhammad Salah",
     author_email="msmainacc0unt@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     packages=["django_api_admin"],
     include_package_data=True,
     install_requires=["django", "djangorestframework"],
 )
```

