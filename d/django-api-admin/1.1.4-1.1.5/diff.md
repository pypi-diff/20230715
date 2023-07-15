# Comparing `tmp/django-api-admin-1.1.4.tar.gz` & `tmp/django-api-admin-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-api-admin-1.1.4.tar", last modified: Sat Jul 15 03:37:56 2023, max compression
+gzip compressed data, was "django-api-admin-1.1.5.tar", last modified: Sat Jul 15 20:37:13 2023, max compression
```

## Comparing `django-api-admin-1.1.4.tar` & `django-api-admin-1.1.5.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.776485 django-api-admin-1.1.4/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1071 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/LICENSE
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       90 2023-07-15 03:29:35.000000 django-api-admin-1.1.4/MANIFEST.in
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3043 2023-07-15 03:37:56.776485 django-api-admin-1.1.4/PKG-INFO
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     2301 2023-07-15 03:29:35.000000 django-api-admin-1.1.4/README.md
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.766485 django-api-admin-1.1.4/django_api_admin/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/__init__.py
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.773152 django-api-admin-1.1.4/django_api_admin/__pycache__/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      202 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3000 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/actions.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     4322 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      591 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3227 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/field_attributes.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3344 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    17261 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/options.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1454 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/pagination.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1124 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/permissions.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     8333 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/serializers.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    17194 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/__pycache__/sites.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1771 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/actions.py
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.773152 django-api-admin-1.1.4/django_api_admin/declarations/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/declarations/__init__.py
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.773152 django-api-admin-1.1.4/django_api_admin/declarations/__pycache__/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      215 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/declarations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3397 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/declarations/__pycache__/classes.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    13367 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/declarations/__pycache__/functions.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1324 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/declarations/classes.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    13151 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/declarations/functions.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3726 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/field_attributes.py
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.763152 django-api-admin-1.1.4/django_api_admin/migrations/
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.773152 django-api-admin-1.1.4/django_api_admin/migrations/__pycache__/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3066 2023-07-15 02:32:57.000000 django-api-admin-1.1.4/django_api_admin/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      213 2023-07-15 02:32:57.000000 django-api-admin-1.1.4/django_api_admin/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    11294 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/options.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      548 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/pagination.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      335 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/permissions.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     5255 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/serializers.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    12948 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/sites.py
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.776485 django-api-admin-1.1.4/django_api_admin/views/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/views/__init__.py
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.776485 django-api-admin-1.1.4/django_api_admin/views/__pycache__/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      208 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/views/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    31514 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/views/__pycache__/admin_views.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    13745 2023-07-15 02:32:56.000000 django-api-admin-1.1.4/django_api_admin/views/__pycache__/fields_test_views.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    14263 2023-07-15 02:58:40.000000 django-api-admin-1.1.4/django_api_admin/views/__pycache__/site_views.cpython-311.pyc
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    26075 2023-07-15 02:28:33.000000 django-api-admin-1.1.4/django_api_admin/views/admin_views.py
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     8315 2023-07-15 03:29:52.000000 django-api-admin-1.1.4/django_api_admin/views/site_views.py
-drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 03:37:56.769819 django-api-admin-1.1.4/django_api_admin.egg-info/
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3043 2023-07-15 03:37:56.000000 django-api-admin-1.1.4/django_api_admin.egg-info/PKG-INFO
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1901 2023-07-15 03:37:56.000000 django-api-admin-1.1.4/django_api_admin.egg-info/SOURCES.txt
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        1 2023-07-15 03:37:56.000000 django-api-admin-1.1.4/django_api_admin.egg-info/dependency_links.txt
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       27 2023-07-15 03:37:56.000000 django-api-admin-1.1.4/django_api_admin.egg-info/requires.txt
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       17 2023-07-15 03:37:56.000000 django-api-admin-1.1.4/django_api_admin.egg-info/top_level.txt
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       38 2023-07-15 03:37:56.776485 django-api-admin-1.1.4/setup.cfg
--rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1161 2023-07-15 03:34:19.000000 django-api-admin-1.1.4/setup.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 20:37:13.042996 django-api-admin-1.1.5/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1071 2023-07-15 19:16:56.000000 django-api-admin-1.1.5/LICENSE
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       90 2023-07-15 20:29:26.000000 django-api-admin-1.1.5/MANIFEST.in
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3043 2023-07-15 20:37:13.042996 django-api-admin-1.1.5/PKG-INFO
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     2301 2023-07-15 20:29:26.000000 django-api-admin-1.1.5/README.md
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 20:37:13.036330 django-api-admin-1.1.5/django_api_admin/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 19:16:56.000000 django-api-admin-1.1.5/django_api_admin/__init__.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 20:37:13.039663 django-api-admin-1.1.5/django_api_admin/__pycache__/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      191 2023-07-15 19:49:05.000000 django-api-admin-1.1.5/django_api_admin/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     2989 2023-07-15 19:49:05.000000 django-api-admin-1.1.5/django_api_admin/__pycache__/actions.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     4311 2023-07-15 19:49:05.000000 django-api-admin-1.1.5/django_api_admin/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      580 2023-07-15 19:49:05.000000 django-api-admin-1.1.5/django_api_admin/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3216 2023-07-15 19:49:05.000000 django-api-admin-1.1.5/django_api_admin/__pycache__/field_attributes.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3333 2023-07-15 19:49:05.000000 django-api-admin-1.1.5/django_api_admin/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    17250 2023-07-15 19:49:05.000000 django-api-admin-1.1.5/django_api_admin/__pycache__/options.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1443 2023-07-15 19:49:51.000000 django-api-admin-1.1.5/django_api_admin/__pycache__/pagination.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1113 2023-07-15 19:49:51.000000 django-api-admin-1.1.5/django_api_admin/__pycache__/permissions.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     8322 2023-07-15 19:49:05.000000 django-api-admin-1.1.5/django_api_admin/__pycache__/serializers.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    17183 2023-07-15 19:49:05.000000 django-api-admin-1.1.5/django_api_admin/__pycache__/sites.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1771 2023-07-15 19:16:56.000000 django-api-admin-1.1.5/django_api_admin/actions.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 20:37:13.039663 django-api-admin-1.1.5/django_api_admin/declarations/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 19:16:56.000000 django-api-admin-1.1.5/django_api_admin/declarations/__init__.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 20:37:13.039663 django-api-admin-1.1.5/django_api_admin/declarations/__pycache__/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      204 2023-07-15 19:49:05.000000 django-api-admin-1.1.5/django_api_admin/declarations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3386 2023-07-15 19:49:05.000000 django-api-admin-1.1.5/django_api_admin/declarations/__pycache__/classes.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    13356 2023-07-15 19:49:05.000000 django-api-admin-1.1.5/django_api_admin/declarations/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1324 2023-07-15 19:16:56.000000 django-api-admin-1.1.5/django_api_admin/declarations/classes.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    13151 2023-07-15 19:16:56.000000 django-api-admin-1.1.5/django_api_admin/declarations/functions.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3726 2023-07-15 19:16:56.000000 django-api-admin-1.1.5/django_api_admin/field_attributes.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 20:37:13.032996 django-api-admin-1.1.5/django_api_admin/migrations/
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 20:37:13.042996 django-api-admin-1.1.5/django_api_admin/migrations/__pycache__/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3055 2023-07-15 19:49:51.000000 django-api-admin-1.1.5/django_api_admin/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      202 2023-07-15 19:49:51.000000 django-api-admin-1.1.5/django_api_admin/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    11294 2023-07-15 19:16:56.000000 django-api-admin-1.1.5/django_api_admin/options.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      548 2023-07-15 19:16:56.000000 django-api-admin-1.1.5/django_api_admin/pagination.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      335 2023-07-15 19:16:56.000000 django-api-admin-1.1.5/django_api_admin/permissions.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     5255 2023-07-15 19:16:56.000000 django-api-admin-1.1.5/django_api_admin/serializers.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    12948 2023-07-15 19:16:56.000000 django-api-admin-1.1.5/django_api_admin/sites.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 20:37:13.042996 django-api-admin-1.1.5/django_api_admin/views/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 19:16:56.000000 django-api-admin-1.1.5/django_api_admin/views/__init__.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 20:37:13.042996 django-api-admin-1.1.5/django_api_admin/views/__pycache__/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)      197 2023-07-15 19:49:05.000000 django-api-admin-1.1.5/django_api_admin/views/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    31290 2023-07-15 19:49:05.000000 django-api-admin-1.1.5/django_api_admin/views/__pycache__/admin_views.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    13734 2023-07-15 19:49:51.000000 django-api-admin-1.1.5/django_api_admin/views/__pycache__/fields_test_views.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    14239 2023-07-15 19:51:48.000000 django-api-admin-1.1.5/django_api_admin/views/__pycache__/site_views.cpython-311.pyc
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)    25925 2023-07-15 20:29:37.000000 django-api-admin-1.1.5/django_api_admin/views/admin_views.py
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     8325 2023-07-15 20:29:37.000000 django-api-admin-1.1.5/django_api_admin/views/site_views.py
+drwxr-xr-x   0 demon-bixia  (1000) demon-bixia  (1000)        0 2023-07-15 20:37:13.036330 django-api-admin-1.1.5/django_api_admin.egg-info/
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     3043 2023-07-15 20:37:13.000000 django-api-admin-1.1.5/django_api_admin.egg-info/PKG-INFO
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1901 2023-07-15 20:37:13.000000 django-api-admin-1.1.5/django_api_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)        1 2023-07-15 20:37:13.000000 django-api-admin-1.1.5/django_api_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       27 2023-07-15 20:37:13.000000 django-api-admin-1.1.5/django_api_admin.egg-info/requires.txt
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       17 2023-07-15 20:37:13.000000 django-api-admin-1.1.5/django_api_admin.egg-info/top_level.txt
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)       38 2023-07-15 20:37:13.042996 django-api-admin-1.1.5/setup.cfg
+-rw-r--r--   0 demon-bixia  (1000) demon-bixia  (1000)     1161 2023-07-15 20:29:26.000000 django-api-admin-1.1.5/setup.py
```

### Comparing `django-api-admin-1.1.4/LICENSE` & `django-api-admin-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.4/PKG-INFO` & `django-api-admin-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-api-admin
-Version: 1.1.4
+Version: 1.1.5
 Summary: Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.
 Home-page: https://github.com/MuhammadSalahAli/django-api-admin
 Author: Muhammad Salah
 Author-email: msmainacc0unt@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-api-admin-1.1.4/README.md` & `django-api-admin-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.4/django_api_admin/__pycache__/actions.cpython-311.pyc` & `django-api-admin-1.1.5/django_api_admin/__pycache__/actions.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5104b264 (Sat Jul 15 02:28:33 2023 UTC)
+moddate:  0xa8f0b264 (Sat Jul 15 19:16:56 2023 UTC)
 files sz: 1771
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
@@ -73,45 +73,45 @@
                 92 PRECALL                  1
                 96 CALL                     1
    
     10         106 KW_NAMES                 9
                108 PRECALL                  2
                112 CALL                     2
    
-    14         122 LOAD_CONST              10 (<code object delete_selected, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/actions.py", line 10>)
+    14         122 LOAD_CONST              10 (<code object delete_selected, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/actions.py", line 10>)
                124 MAKE_FUNCTION            0
    
     10         126 PRECALL                  0
                130 CALL                     0
    
     14         140 STORE_NAME              14 (delete_selected)
    
     41         142 PUSH_NULL
                144 LOAD_NAME                1 (action)
                146 LOAD_CONST              11 ('make all authors old')
                148 KW_NAMES                12
                150 PRECALL                  1
                154 CALL                     1
    
-    42         164 LOAD_CONST              13 (<code object make_old, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/actions.py", line 41>)
+    42         164 LOAD_CONST              13 (<code object make_old, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/actions.py", line 41>)
                166 MAKE_FUNCTION            0
    
     41         168 PRECALL                  0
                172 CALL                     0
    
     42         182 STORE_NAME              15 (make_old)
    
     47         184 PUSH_NULL
                186 LOAD_NAME                1 (action)
                188 LOAD_CONST              14 ('make all authors young')
                190 KW_NAMES                12
                192 PRECALL                  1
                196 CALL                     1
    
-    48         206 LOAD_CONST              15 (<code object make_young, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/actions.py", line 47>)
+    48         206 LOAD_CONST              15 (<code object make_young, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/actions.py", line 47>)
                208 MAKE_FUNCTION            0
    
     47         210 PRECALL                  0
                214 CALL                     0
    
     48         224 STORE_NAME              16 (make_young)
                226 LOAD_CONST              16 (None)
@@ -263,15 +263,15 @@
             ('count', 'items')
             'detail'
             ('status',)
          names      ('get_deleted_objects', 'model_ngettext', '_', 'PermissionDenied', 'count', 'log_deletion', 'str', 'delete_queryset', 'opts', 'Response', 'status', 'HTTP_200_OK')
          varnames   ('modeladmin', 'request', 'queryset', 'deletable_objects', 'model_count', 'perms_needed', 'protected', 'objects_name', 'msg', 'n', 'obj')
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/actions.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/actions.py'
          name       'delete_selected'
          firstlineno 10
          lnotab
             0x0209180104ff1a0404011e01280120032801040108014a032c011c012a
             ff0a02
       'make all authors old'
       ('description',)
@@ -312,15 +312,15 @@
             'detail'
             'All select authors are old now'
             ('status',)
          names      ('update', 'Response', 'status', 'HTTP_200_OK')
          varnames   ('model_admin', 'request', 'queryset')
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/actions.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/actions.py'
          name       'make_old'
          firstlineno 41
          lnotab 0x02022c01
       'make all authors young'
       code
          argcount  : 3
          nlocals   : 3
@@ -358,22 +358,22 @@
             'detail'
             'All select authors are young now'
             ('status',)
          names      ('update', 'Response', 'status', 'HTTP_200_OK')
          varnames   ('model_admin', 'request', 'queryset')
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/actions.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/actions.py'
          name       'make_young'
          firstlineno 47
          lnotab 0x02022c01
       None
    names      ('django.contrib.admin', 'action', 'django.contrib.admin.utils', 'model_ngettext', 'django.utils.translation', 'gettext_lazy', 'gettext', '_', 'rest_framework', 'status', 'rest_framework.exceptions', 'PermissionDenied', 'rest_framework.response', 'Response', 'delete_selected', 'make_old', 'make_young')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/actions.py'
+   filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/actions.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c010c0110020c010c010c030401040114fe100404fc0e0402
       1b160104ff0e010205160104ff0e01
```

### Comparing `django-api-admin-1.1.4/django_api_admin/__pycache__/admin.cpython-311.pyc` & `django-api-admin-1.1.5/django_api_admin/__pycache__/admin.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5105b264 (Sat Jul 15 02:32:49 2023 UTC)
+moddate:  0xdcf0b264 (Sat Jul 15 19:17:48 2023 UTC)
 files sz: 2549
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
@@ -74,15 +74,15 @@
                 78 STORE_NAME              14 (make_old)
                 80 IMPORT_FROM             15 (make_young)
                 82 STORE_NAME              15 (make_young)
                 84 POP_TOP
    
     13          86 PUSH_NULL
                 88 LOAD_BUILD_CLASS
-                90 LOAD_CONST               8 (<code object APIBookInline, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py", line 13>)
+                90 LOAD_CONST               8 (<code object APIBookInline, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py", line 13>)
                 92 MAKE_FUNCTION            0
                 94 LOAD_CONST               9 ('APIBookInline')
                 96 LOAD_NAME               10 (TabularInlineAPI)
                 98 PRECALL                  3
                102 CALL                     3
                112 STORE_NAME              16 (APIBookInline)
    
@@ -93,15 +93,15 @@
                130 LOAD_NAME               12 (site)
                132 KW_NAMES                 6
                134 PRECALL                  2
                138 CALL                     2
    
     18         148 PUSH_NULL
                150 LOAD_BUILD_CLASS
-               152 LOAD_CONST              10 (<code object PublisherAPIAdmin, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py", line 17>)
+               152 LOAD_CONST              10 (<code object PublisherAPIAdmin, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py", line 17>)
                154 MAKE_FUNCTION            0
                156 LOAD_CONST              11 ('PublisherAPIAdmin')
                158 LOAD_NAME                9 (APIModelAdmin)
                160 PRECALL                  3
                164 CALL                     3
    
     17         174 PRECALL                  0
@@ -116,51 +116,51 @@
                206 LOAD_NAME               12 (site)
                208 KW_NAMES                 6
                210 PRECALL                  2
                214 CALL                     2
    
     24         224 PUSH_NULL
                226 LOAD_BUILD_CLASS
-               228 LOAD_CONST              12 (<code object AuthorAPIAdmin, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py", line 23>)
+               228 LOAD_CONST              12 (<code object AuthorAPIAdmin, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py", line 23>)
                230 MAKE_FUNCTION            0
                232 LOAD_CONST              13 ('AuthorAPIAdmin')
                234 LOAD_NAME                9 (APIModelAdmin)
                236 PRECALL                  3
                240 CALL                     3
    
     23         250 PRECALL                  0
                254 CALL                     0
    
     24         264 STORE_NAME              19 (AuthorAPIAdmin)
    
     53         266 PUSH_NULL
                268 LOAD_BUILD_CLASS
-               270 LOAD_CONST              14 (<code object BookInline, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py", line 53>)
+               270 LOAD_CONST              14 (<code object BookInline, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py", line 53>)
                272 MAKE_FUNCTION            0
                274 LOAD_CONST              15 ('BookInline')
                276 LOAD_NAME                2 (admin)
                278 LOAD_ATTR               20 (TabularInline)
                288 PRECALL                  3
                292 CALL                     3
                302 STORE_NAME              21 (BookInline)
    
     57         304 PUSH_NULL
                306 LOAD_BUILD_CLASS
-               308 LOAD_CONST              16 (<code object PublisherAdmin, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py", line 57>)
+               308 LOAD_CONST              16 (<code object PublisherAdmin, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py", line 57>)
                310 MAKE_FUNCTION            0
                312 LOAD_CONST              17 ('PublisherAdmin')
                314 LOAD_NAME                2 (admin)
                316 LOAD_ATTR               22 (ModelAdmin)
                326 PRECALL                  3
                330 CALL                     3
                340 STORE_NAME              23 (PublisherAdmin)
    
     61         342 PUSH_NULL
                344 LOAD_BUILD_CLASS
-               346 LOAD_CONST              18 (<code object AuthorAdmin, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py", line 61>)
+               346 LOAD_CONST              18 (<code object AuthorAdmin, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py", line 61>)
                348 MAKE_FUNCTION            0
                350 LOAD_CONST              19 ('AuthorAdmin')
                352 LOAD_NAME                2 (admin)
                354 LOAD_ATTR               22 (ModelAdmin)
                364 PRECALL                  3
                368 CALL                     3
                378 STORE_NAME              24 (AuthorAdmin)
@@ -220,15 +220,15 @@
          consts
             'APIBookInline'
             None
          names      ('__name__', '__module__', '__qualname__', 'Book', 'model')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py'
          name       'APIBookInline'
          firstlineno 13
          lnotab 0x0a01
       'APIBookInline'
       code
          argcount  : 0
          nlocals   : 0
@@ -249,15 +249,15 @@
             'PublisherAPIAdmin'
             ('name',)
             None
          names      ('__name__', '__module__', '__qualname__', 'search_fields')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py'
          name       'PublisherAPIAdmin'
          firstlineno 17
          lnotab 0x0a02
       'PublisherAPIAdmin'
       code
          argcount  : 0
          nlocals   : 0
@@ -335,15 +335,15 @@
                       88 LOAD_NAME               21 (admin)
                       90 LOAD_ATTR               22 (display)
                      100 LOAD_CONST              15 ('is this author old enough')
                      102 KW_NAMES                16
                      104 PRECALL                  1
                      108 CALL                     1
          
-          48         118 LOAD_CONST              17 (<code object is_old_enough, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py", line 47>)
+          48         118 LOAD_CONST              17 (<code object is_old_enough, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py", line 47>)
                      120 MAKE_FUNCTION            0
          
           47         122 PRECALL                  0
                      126 CALL                     0
          
           48         136 STORE_NAME              23 (is_old_enough)
                      138 LOAD_CONST              18 (None)
@@ -382,24 +382,24 @@
                consts
                   None
                   10
                names      ('age',)
                varnames   ('self', 'obj')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py'
                name       'is_old_enough'
                firstlineno 47
                lnotab 0x0202
             None
          names      ('__name__', '__module__', '__qualname__', 'list_display', 'exclude', 'list_display_links', 'list_filter', 'list_editable', 'list_per_page', 'empty_value_display', 'make_old', 'make_young', 'actions', 'actions_selection_counter', 'date_hierarchy', 'search_fields', 'ordering', 'raw_id_fields', 'fieldsets', 'APIBookInline', 'inlines', 'admin', 'display', 'is_old_enough')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py'
          name       'AuthorAPIAdmin'
          firstlineno 23
          lnotab
             0x0a02040104010401040104010401040208010402040104010402040202
             0104ff04ff04040602200104ff0e01
       'AuthorAPIAdmin'
       code
@@ -421,15 +421,15 @@
          consts
             'BookInline'
             None
          names      ('__name__', '__module__', '__qualname__', 'Book', 'model')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py'
          name       'BookInline'
          firstlineno 53
          lnotab 0x0a01
       'BookInline'
       code
          argcount  : 0
          nlocals   : 0
@@ -450,15 +450,15 @@
             'PublisherAdmin'
             ('name',)
             None
          names      ('__name__', '__module__', '__qualname__', 'search_fields')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py'
          name       'PublisherAdmin'
          firstlineno 57
          lnotab 0x0a01
       'PublisherAdmin'
       code
          argcount  : 0
          nlocals   : 0
@@ -533,15 +533,15 @@
                       84 LOAD_NAME               20 (admin)
                       86 LOAD_ATTR               21 (display)
                       96 LOAD_CONST              14 ('is this author a vip')
                       98 KW_NAMES                15
                      100 PRECALL                  1
                      104 CALL                     1
          
-          87         114 LOAD_CONST              16 (<code object is_a_vip, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py", line 86>)
+          87         114 LOAD_CONST              16 (<code object is_a_vip, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py", line 86>)
                      116 MAKE_FUNCTION            0
          
           86         118 PRECALL                  0
                      122 CALL                     0
          
           87         132 STORE_NAME              22 (is_a_vip)
          
@@ -549,15 +549,15 @@
                      136 LOAD_NAME               20 (admin)
                      138 LOAD_ATTR               21 (display)
                      148 LOAD_CONST              17 ('is this author old enough')
                      150 KW_NAMES                15
                      152 PRECALL                  1
                      156 CALL                     1
          
-          91         166 LOAD_CONST              18 (<code object is_old_enough, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py", line 90>)
+          91         166 LOAD_CONST              18 (<code object is_old_enough, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py", line 90>)
                      168 MAKE_FUNCTION            0
          
           90         170 PRECALL                  0
                      174 CALL                     0
          
           91         184 STORE_NAME              23 (is_old_enough)
                      186 LOAD_CONST              19 (None)
@@ -592,15 +592,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('is_vip',)
                varnames   ('self', 'obj')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py'
                name       'is_a_vip'
                firstlineno 86
                lnotab 0x0202
             'is this author old enough'
             code
                argcount  : 2
                nlocals   : 2
@@ -617,34 +617,34 @@
                consts
                   None
                   10
                names      ('age',)
                varnames   ('self', 'obj')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py'
                name       'is_old_enough'
                firstlineno 90
                lnotab 0x0202
             None
          names      ('__name__', '__module__', '__qualname__', 'list_display', 'list_filter', 'list_editable', 'list_per_page', 'empty_value_display', 'make_old', 'make_young', 'actions', 'raw_id_fields', 'autocomplete_fields', 'date_hierarchy', 'ordering', 'fieldsets', 'exclude', 'filter_horizontal', 'BookInline', 'inlines', 'admin', 'display', 'is_a_vip', 'is_old_enough')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py'
          name       'AuthorAdmin'
          firstlineno 61
          lnotab
             0x0a0104020401040104010402080204010401040204020aff0404040204
             020602200104ff0e010203200104ff0e01
       'AuthorAdmin'
       None
    names      ('__doc__', 'django.contrib', 'admin', 'models', 'Author', 'Publisher', 'Book', 'GuestEntry', 'options', 'APIModelAdmin', 'TabularInlineAPI', 'sites', 'site', 'actions', 'make_old', 'make_young', 'APIBookInline', 'register', 'PublisherAPIAdmin', 'AuthorAPIAdmin', 'TabularInline', 'BookInline', 'ModelAdmin', 'PublisherAdmin', 'AuthorAdmin')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/admin.py'
+   filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/admin.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020104040c02180110010c0110031c0422011aff0e01020522011a
       ff0e01021d26042604262236013601
```

### Comparing `django-api-admin-1.1.4/django_api_admin/__pycache__/apps.cpython-311.pyc` & `django-api-admin-1.1.5/django_api_admin/__pycache__/apps.cpython-311.pyc`

 * *Files 20% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5105b264 (Sat Jul 15 02:32:49 2023 UTC)
+moddate:  0xdcf0b264 (Sat Jul 15 19:17:48 2023 UTC)
 files sz: 162
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -16,15 +16,15 @@
                  6 IMPORT_NAME              0 (django.apps)
                  8 IMPORT_FROM              1 (AppConfig)
                 10 STORE_NAME               1 (AppConfig)
                 12 POP_TOP
    
      4          14 PUSH_NULL
                 16 LOAD_BUILD_CLASS
-                18 LOAD_CONST               2 (<code object DjangoApiAdminConfig, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/apps.py", line 4>)
+                18 LOAD_CONST               2 (<code object DjangoApiAdminConfig, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/apps.py", line 4>)
                 20 MAKE_FUNCTION            0
                 22 LOAD_CONST               3 ('DjangoApiAdminConfig')
                 24 LOAD_NAME                1 (AppConfig)
                 26 PRECALL                  3
                 30 CALL                     3
                 40 STORE_NAME               2 (DjangoApiAdminConfig)
                 42 LOAD_CONST               4 (None)
@@ -56,21 +56,21 @@
             'django.db.models.BigAutoField'
             'django_api_admin'
             None
          names      ('__name__', '__module__', '__qualname__', 'default_auto_field', 'name')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/apps.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/apps.py'
          name       'DjangoApiAdminConfig'
          firstlineno 4
          lnotab 0x0a010401
       'DjangoApiAdminConfig'
       None
    names      ('django.apps', 'AppConfig', 'DjangoApiAdminConfig')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/apps.py'
+   filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/apps.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c03
```

### Comparing `django-api-admin-1.1.4/django_api_admin/__pycache__/field_attributes.cpython-311.pyc` & `django-api-admin-1.1.5/django_api_admin/__pycache__/field_attributes.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5104b264 (Sat Jul 15 02:28:33 2023 UTC)
+moddate:  0xa8f0b264 (Sat Jul 15 19:16:56 2023 UTC)
 files sz: 3726
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -479,15 +479,15 @@
       'SlugRelatedField'
       'HyperlinkedIdentityField'
       None
    names      ('__doc__', 'shared_attributes', 'shared_string_fields_attributes', 'shared_numeric_fields_attributes', 'shared_datetime_fields_attributes', 'shared_choice_fields_attributes', 'shared_file_fields_attributes', 'shared_composite_fields_attributes', 'shared_relationship_fields_attributes', 'field_attributes')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/field_attributes.py'
+   filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/field_attributes.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201040408060803080208020803080208020804020208fe02050c
       fb02060cfa020710f9020810f802090cf7020a10f6020b14f5020c0c0102
       ff020102ff020102ff020102ff020102ff02f402100cf002110cef021214
       0102ff020102ff020102ff02ee02160cea02170ce902180ce802190ce702
```

### Comparing `django-api-admin-1.1.4/django_api_admin/__pycache__/models.cpython-311.pyc` & `django-api-admin-1.1.5/django_api_admin/__pycache__/models.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5105b264 (Sat Jul 15 02:32:49 2023 UTC)
+moddate:  0xdcf0b264 (Sat Jul 15 19:17:48 2023 UTC)
 files sz: 1341
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -45,48 +45,48 @@
                 44 LOAD_NAME                2 (get_user_model)
                 46 PRECALL                  0
                 50 CALL                     0
                 60 STORE_NAME               7 (User)
    
     12          62 PUSH_NULL
                 64 LOAD_BUILD_CLASS
-                66 LOAD_CONST               5 (<code object Publisher, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/models.py", line 12>)
+                66 LOAD_CONST               5 (<code object Publisher, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/models.py", line 12>)
                 68 MAKE_FUNCTION            0
                 70 LOAD_CONST               6 ('Publisher')
                 72 LOAD_NAME                4 (models)
                 74 LOAD_ATTR                8 (Model)
                 84 PRECALL                  3
                 88 CALL                     3
                 98 STORE_NAME               9 (Publisher)
    
     19         100 PUSH_NULL
                102 LOAD_BUILD_CLASS
-               104 LOAD_CONST               7 (<code object Author, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/models.py", line 19>)
+               104 LOAD_CONST               7 (<code object Author, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/models.py", line 19>)
                106 MAKE_FUNCTION            0
                108 LOAD_CONST               8 ('Author')
                110 LOAD_NAME                4 (models)
                112 LOAD_ATTR                8 (Model)
                122 PRECALL                  3
                126 CALL                     3
                136 STORE_NAME              10 (Author)
    
     37         138 PUSH_NULL
                140 LOAD_BUILD_CLASS
-               142 LOAD_CONST               9 (<code object Book, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/models.py", line 37>)
+               142 LOAD_CONST               9 (<code object Book, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/models.py", line 37>)
                144 MAKE_FUNCTION            0
                146 LOAD_CONST              10 ('Book')
                148 LOAD_NAME                4 (models)
                150 LOAD_ATTR                8 (Model)
                160 PRECALL                  3
                164 CALL                     3
                174 STORE_NAME              11 (Book)
    
     46         176 PUSH_NULL
                178 LOAD_BUILD_CLASS
-               180 LOAD_CONST              11 (<code object GuestEntry, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/models.py", line 46>)
+               180 LOAD_CONST              11 (<code object GuestEntry, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/models.py", line 46>)
                182 MAKE_FUNCTION            0
                184 LOAD_CONST              12 ('GuestEntry')
                186 LOAD_NAME                4 (models)
                188 LOAD_ATTR                8 (Model)
                198 PRECALL                  3
                202 CALL                     3
                212 STORE_NAME              12 (GuestEntry)
@@ -117,15 +117,15 @@
                       14 LOAD_ATTR                4 (CharField)
                       24 LOAD_CONST               1 (100)
                       26 KW_NAMES                 2
                       28 PRECALL                  1
                       32 CALL                     1
                       42 STORE_NAME               5 (name)
          
-          15          44 LOAD_CONST               3 (<code object __str__, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/models.py", line 15>)
+          15          44 LOAD_CONST               3 (<code object __str__, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/models.py", line 15>)
                       46 MAKE_FUNCTION            0
                       48 STORE_NAME               6 (__str__)
                       50 LOAD_CONST               4 (None)
                       52 RETURN_VALUE
          consts
             'Publisher'
             100
@@ -143,24 +143,24 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('name',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/models.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/models.py'
                name       '__str__'
                firstlineno 15
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'CharField', 'name', '__str__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/models.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/models.py'
          name       'Publisher'
          firstlineno 12
          lnotab 0x0a012202
       'Publisher'
       code
          argcount  : 0
          nlocals   : 0
@@ -259,19 +259,19 @@
                      280 LOAD_CONST               8 (20)
                      282 LOAD_CONST              10 (True)
                      284 KW_NAMES                12
                      286 PRECALL                  2
                      290 CALL                     2
                      300 STORE_NAME              21 (title)
          
-          30         302 LOAD_CONST              13 (<code object __str__, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/models.py", line 30>)
+          30         302 LOAD_CONST              13 (<code object __str__, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/models.py", line 30>)
                      304 MAKE_FUNCTION            0
                      306 STORE_NAME              22 (__str__)
          
-          33         308 LOAD_CONST              14 (<code object get_absolute_url, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/models.py", line 33>)
+          33         308 LOAD_CONST              14 (<code object get_absolute_url, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/models.py", line 33>)
                      310 MAKE_FUNCTION            0
                      312 STORE_NAME              23 (get_absolute_url)
                      314 LOAD_CONST              15 (None)
                      316 RETURN_VALUE
          consts
             'Author'
             ((60, 'senior'), (1, 'baby'), (2, 'also a baby'))
@@ -299,15 +299,15 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('name',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/models.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/models.py'
                name       '__str__'
                firstlineno 30
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
@@ -332,24 +332,24 @@
                   'author-detail'
                   'pk'
                   ('kwargs',)
                names      ('reverse', 'pk')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/models.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/models.py'
                name       'get_absolute_url'
                firstlineno 33
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'age_choices', 'models', 'CharField', 'name', 'IntegerField', 'age', 'BooleanField', 'is_vip', 'ForeignKey', 'User', 'CASCADE', 'user', 'ManyToManyField', 'Publisher', 'publisher', 'gender', 'DateTimeField', 'date_joined', 'title', '__str__', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/models.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/models.py'
          name       'Author'
          firstlineno 19
          lnotab 0x0a0104012201220122012e0120012601220124020603
       'Author'
       code
          argcount  : 0
          nlocals   : 0
@@ -393,15 +393,15 @@
                      104 LOAD_NAME                7 (Author)
                      106 LOAD_CONST               4 ('credits')
                      108 KW_NAMES                 5
                      110 PRECALL                  2
                      114 CALL                     2
                      124 STORE_NAME              11 (credits)
          
-          42         126 LOAD_CONST               6 (<code object __str__, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/models.py", line 42>)
+          42         126 LOAD_CONST               6 (<code object __str__, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/models.py", line 42>)
                      128 MAKE_FUNCTION            0
                      130 STORE_NAME              12 (__str__)
                      132 LOAD_CONST               7 (None)
                      134 RETURN_VALUE
          consts
             'Book'
             100
@@ -422,24 +422,24 @@
                             14 RETURN_VALUE
                consts
                   None
                names      ('title',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/models.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/models.py'
                name       '__str__'
                firstlineno 42
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'CharField', 'title', 'ForeignKey', 'Author', 'CASCADE', 'author', 'ManyToManyField', 'credits', '__str__')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/models.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/models.py'
          name       'Book'
          firstlineno 37
          lnotab 0x0a0122012e012402
       'Book'
       code
          argcount  : 0
          nlocals   : 0
@@ -465,21 +465,21 @@
          consts
             'GuestEntry'
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'DateField', 'date_entered')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/models.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/models.py'
          name       'GuestEntry'
          firstlineno 46
          lnotab 0x0a01
       'GuestEntry'
       None
    names      ('__doc__', 'django.contrib.auth', 'get_user_model', 'django.db', 'models', 'django.urls', 'reverse', 'User', 'Model', 'Publisher', 'Author', 'Book', 'GuestEntry')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/models.py'
+   filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/models.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020104040c010c010c021403260726122609
```

### Comparing `django-api-admin-1.1.4/django_api_admin/__pycache__/options.cpython-311.pyc` & `django-api-admin-1.1.5/django_api_admin/__pycache__/options.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5104b264 (Sat Jul 15 02:28:33 2023 UTC)
+moddate:  0xa8f0b264 (Sat Jul 15 19:16:56 2023 UTC)
 files sz: 11294
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
@@ -72,56 +72,56 @@
                 90 IMPORT_NAME             15 (django_api_admin.serializers)
                 92 IMPORT_FROM             16 (ActionSerializer)
                 94 STORE_NAME              16 (ActionSerializer)
                 96 POP_TOP
    
     15          98 PUSH_NULL
                100 LOAD_BUILD_CLASS
-               102 LOAD_CONST               9 (<code object BaseAPIModelAdmin, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 15>)
+               102 LOAD_CONST               9 (<code object BaseAPIModelAdmin, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 15>)
                104 MAKE_FUNCTION            0
                106 LOAD_CONST              10 ('BaseAPIModelAdmin')
                108 PRECALL                  2
                112 CALL                     2
                122 STORE_NAME              17 (BaseAPIModelAdmin)
    
    143         124 PUSH_NULL
                126 LOAD_BUILD_CLASS
-               128 LOAD_CONST              11 (<code object APIModelAdmin, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 143>)
+               128 LOAD_CONST              11 (<code object APIModelAdmin, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 143>)
                130 MAKE_FUNCTION            0
                132 LOAD_CONST              12 ('APIModelAdmin')
                134 LOAD_NAME               17 (BaseAPIModelAdmin)
                136 LOAD_NAME                3 (ModelAdmin)
                138 PRECALL                  4
                142 CALL                     4
                152 STORE_NAME              18 (APIModelAdmin)
    
    240         154 PUSH_NULL
                156 LOAD_BUILD_CLASS
-               158 LOAD_CONST              13 (<code object InlineAPIModelAdmin, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 240>)
+               158 LOAD_CONST              13 (<code object InlineAPIModelAdmin, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 240>)
                160 MAKE_FUNCTION            0
                162 LOAD_CONST              14 ('InlineAPIModelAdmin')
                164 LOAD_NAME               17 (BaseAPIModelAdmin)
                166 LOAD_NAME                2 (InlineModelAdmin)
                168 PRECALL                  4
                172 CALL                     4
                182 STORE_NAME              19 (InlineAPIModelAdmin)
    
    282         184 PUSH_NULL
                186 LOAD_BUILD_CLASS
-               188 LOAD_CONST              15 (<code object TabularInlineAPI, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 282>)
+               188 LOAD_CONST              15 (<code object TabularInlineAPI, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 282>)
                190 MAKE_FUNCTION            0
                192 LOAD_CONST              16 ('TabularInlineAPI')
                194 LOAD_NAME               19 (InlineAPIModelAdmin)
                196 PRECALL                  3
                200 CALL                     3
                210 STORE_NAME              20 (TabularInlineAPI)
    
    286         212 PUSH_NULL
                214 LOAD_BUILD_CLASS
-               216 LOAD_CONST              17 (<code object StackedInlineAPI, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 286>)
+               216 LOAD_CONST              17 (<code object StackedInlineAPI, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 286>)
                218 MAKE_FUNCTION            0
                220 LOAD_CONST              18 ('StackedInlineAPI')
                222 LOAD_NAME               19 (InlineAPIModelAdmin)
                224 PRECALL                  3
                228 CALL                     3
                238 STORE_NAME              21 (StackedInlineAPI)
                240 LOAD_CONST              19 (None)
@@ -158,79 +158,79 @@
          
           21          14 BUILD_LIST               0
                       16 LOAD_CONST               2 (('fieldsets', 'fields', 'save_on_top', 'save_as', 'save_as_continue', 'view_on_site'))
                       18 LIST_EXTEND              1
                       20 STORE_NAME               4 (form_options)
          
           29          22 LOAD_CONST              19 ((None, False))
-                      24 LOAD_CONST               5 (<code object get_serializer_class, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 29>)
+                      24 LOAD_CONST               5 (<code object get_serializer_class, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 29>)
                       26 MAKE_FUNCTION            1 (defaults)
                       28 STORE_NAME               5 (get_serializer_class)
          
           57          30 LOAD_CONST              20 ((None,))
-                      32 LOAD_CONST               6 (<code object get_permission_map, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 57>)
+                      32 LOAD_CONST               6 (<code object get_permission_map, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 57>)
                       34 MAKE_FUNCTION            1 (defaults)
                       36 STORE_NAME               6 (get_permission_map)
          
           71          38 LOAD_CONST              20 ((None,))
-                      40 LOAD_CONST               7 (<code object has_add_permission, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 71>)
+                      40 LOAD_CONST               7 (<code object has_add_permission, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 71>)
                       42 MAKE_FUNCTION            1 (defaults)
                       44 STORE_NAME               7 (has_add_permission)
          
           76          46 LOAD_CONST              20 ((None,))
-                      48 LOAD_CONST               8 (<code object has_change_permission, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 76>)
+                      48 LOAD_CONST               8 (<code object has_change_permission, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 76>)
                       50 MAKE_FUNCTION            1 (defaults)
                       52 STORE_NAME               8 (has_change_permission)
          
           81          54 LOAD_CONST              20 ((None,))
-                      56 LOAD_CONST               9 (<code object has_delete_permission, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 81>)
+                      56 LOAD_CONST               9 (<code object has_delete_permission, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 81>)
                       58 MAKE_FUNCTION            1 (defaults)
                       60 STORE_NAME               9 (has_delete_permission)
          
           86          62 LOAD_CONST              20 ((None,))
-                      64 LOAD_CONST              10 (<code object has_view_permission, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 86>)
+                      64 LOAD_CONST              10 (<code object has_view_permission, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 86>)
                       66 MAKE_FUNCTION            1 (defaults)
                       68 STORE_NAME              10 (has_view_permission)
          
           95          70 LOAD_CONST              20 ((None,))
-                      72 LOAD_CONST              11 (<code object has_view_or_change_permission, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 95>)
+                      72 LOAD_CONST              11 (<code object has_view_or_change_permission, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 95>)
                       74 MAKE_FUNCTION            1 (defaults)
                       76 STORE_NAME              11 (has_view_or_change_permission)
          
-          98          78 LOAD_CONST              12 (<code object has_module_permission, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 98>)
+          98          78 LOAD_CONST              12 (<code object has_module_permission, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 98>)
                       80 MAKE_FUNCTION            0
                       82 STORE_NAME              12 (has_module_permission)
          
          101          84 LOAD_NAME               13 (property)
          
-         102          86 LOAD_CONST              13 (<code object is_inline, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 101>)
+         102          86 LOAD_CONST              13 (<code object is_inline, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 101>)
                       88 MAKE_FUNCTION            0
          
          101          90 PRECALL                  0
                       94 CALL                     0
          
          102         104 STORE_NAME              14 (is_inline)
          
-         105         106 LOAD_CONST              14 (<code object list_view, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 105>)
+         105         106 LOAD_CONST              14 (<code object list_view, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 105>)
                      108 MAKE_FUNCTION            0
                      110 STORE_NAME              15 (list_view)
          
-         112         112 LOAD_CONST              15 (<code object detail_view, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 112>)
+         112         112 LOAD_CONST              15 (<code object detail_view, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 112>)
                      114 MAKE_FUNCTION            0
                      116 STORE_NAME              16 (detail_view)
          
-         119         118 LOAD_CONST              16 (<code object add_view, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 119>)
+         119         118 LOAD_CONST              16 (<code object add_view, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 119>)
                      120 MAKE_FUNCTION            0
                      122 STORE_NAME              17 (add_view)
          
-         127         124 LOAD_CONST              17 (<code object change_view, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 127>)
+         127         124 LOAD_CONST              17 (<code object change_view, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 127>)
                      126 MAKE_FUNCTION            0
                      128 STORE_NAME              18 (change_view)
          
-         135         130 LOAD_CONST              18 (<code object delete_view, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 135>)
+         135         130 LOAD_CONST              18 (<code object delete_view, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 135>)
                      132 MAKE_FUNCTION            0
                      134 STORE_NAME              19 (delete_view)
                      136 LOAD_CONST               3 (None)
                      138 RETURN_VALUE
          consts
             'BaseAPIModelAdmin'
             '\n    Shared behavior between APIModelAdmin, APIInlineModelAdmin.\n    '
@@ -304,15 +304,15 @@
                            224 LOAD_FAST                2 (obj)
                            226 PRECALL                  2
                            230 CALL                     2
                            240 STORE_FAST               6 (readonly_fields)
                
                 42         242 LOAD_CLOSURE             8 (exclude)
                            244 BUILD_TUPLE              1
-                           246 LOAD_CONST               3 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 42>)
+                           246 LOAD_CONST               3 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 42>)
                            248 MAKE_FUNCTION            8 (closure)
                            250 LOAD_FAST                4 (fieldsets_fields)
                            252 GET_ITER
                            254 PRECALL                  0
                            258 CALL                     0
                            268 STORE_FAST               7 (fields)
                
@@ -380,27 +380,27 @@
                                   24 JUMP_BACKWARD            9 (to 8)
                              >>   26 RETURN_VALUE
                      consts
                      names      ()
                      varnames   ('.0', 'field')
                      freevars   ('exclude',)
                      cellvars   ()
-                     filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+                     filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                      name       '<listcomp>'
                      firstlineno 42
                      lnotab 0x
                   '__all__'
                   '%sSerializer'
                   'Meta'
                   ('model', 'fields', 'read_only_fields')
                names      ('flatten_fieldsets', 'get_fieldsets', 'append', 'get_exclude', 'list', 'get_readonly_fields', 'type', 'model', '__name__', 'serializers', 'ModelSerializer', 'object')
                varnames   ('self', 'request', 'obj', 'changelist', 'fieldsets_fields', 'excluded', 'readonly_fields', 'fields')
                freevars   ()
                cellvars   ('exclude',)
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'get_serializer_class'
                firstlineno 29
                lnotab
                   0x040546012a022c0126022c021c030401040340011e010c01020102fd12
                   ff
             code
                argcount  : 3
@@ -461,15 +461,15 @@
                consts
                   '\n        return a dictionary of user permissions in this module.\n        '
                   ('has_add_permission', 'has_change_permission', 'has_delete_permission', 'has_view_permission', 'has_view_or_change_permission', 'has_module_permission')
                names      ('has_add_permission', 'has_change_permission', 'has_delete_permission', 'has_view_permission', 'has_view_or_change_permission', 'has_module_permission')
                varnames   ('self', 'request', 'obj')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'get_permission_map'
                firstlineno 57
                lnotab 0x02062801280128012801280128fa
             code
                argcount  : 3
                nlocals   : 5
                stacksize : 5
@@ -510,15 +510,15 @@
                   None
                   'add'
                   '.'
                names      ('opts', 'get_permission_codename', 'user', 'has_perm', 'app_label')
                varnames   ('self', 'request', 'obj', 'opts', 'codename')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'has_add_permission'
                firstlineno 71
                lnotab 0x02010e012001
             code
                argcount  : 3
                nlocals   : 5
                stacksize : 5
@@ -559,15 +559,15 @@
                   None
                   'change'
                   '.'
                names      ('opts', 'get_permission_codename', 'user', 'has_perm', 'app_label')
                varnames   ('self', 'request', 'obj', 'opts', 'codename')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'has_change_permission'
                firstlineno 76
                lnotab 0x02010e012001
             code
                argcount  : 3
                nlocals   : 5
                stacksize : 5
@@ -608,15 +608,15 @@
                   None
                   'delete'
                   '.'
                names      ('opts', 'get_permission_codename', 'user', 'has_perm', 'app_label')
                varnames   ('self', 'request', 'obj', 'opts', 'codename')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'has_delete_permission'
                firstlineno 81
                lnotab 0x02010e012001
             code
                argcount  : 3
                nlocals   : 6
                stacksize : 5
@@ -683,15 +683,15 @@
                   'view'
                   'change'
                   '.'
                names      ('opts', 'get_permission_codename', 'user', 'has_perm', 'app_label')
                varnames   ('self', 'request', 'obj', 'opts', 'codename_view', 'codename_change')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'has_view_permission'
                firstlineno 86
                lnotab 0x02010e0120012002480146fe
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 3
@@ -716,15 +716,15 @@
                        >>   84 RETURN_VALUE
                consts
                   None
                names      ('has_view_permission', 'has_change_permission')
                varnames   ('self', 'request', 'obj')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'has_view_or_change_permission'
                firstlineno 95
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
@@ -746,15 +746,15 @@
                             72 RETURN_VALUE
                consts
                   None
                names      ('user', 'has_module_perms', 'opts', 'app_label')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'has_module_permission'
                firstlineno 98
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
@@ -772,15 +772,15 @@
                             42 RETURN_VALUE
                consts
                   None
                names      ('isinstance', 'InlineModelAdmin')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'is_inline'
                firstlineno 101
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 6
@@ -825,15 +825,15 @@
                   None
                   ('serializer_class', 'permission_classes')
                   ()
                names      ('get_serializer_class', 'admin_site', 'default_permission_classes', 'admin_views', 'ListView', 'as_view')
                varnames   ('self', 'request', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'list_view'
                firstlineno 105
                lnotab 0x0202280116fe0604
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 6
@@ -879,15 +879,15 @@
                   None
                   ('serializer_class', 'permission_classes')
                   ()
                names      ('get_serializer_class', 'admin_site', 'default_permission_classes', 'admin_views', 'DetailView', 'as_view')
                varnames   ('self', 'request', 'object_id', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'detail_view'
                firstlineno 112
                lnotab 0x0202280116fe0604
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 7
@@ -980,15 +980,15 @@
                   ('serializer_class', 'permission_classes')
                   ('using',)
                   ()
                names      ('get_serializer_class', 'admin_site', 'default_permission_classes', 'transaction', 'atomic', 'router', 'db_for_write', 'model', 'admin_views', 'AddView', 'as_view')
                varnames   ('self', 'request', 'kwargs', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'add_view'
                firstlineno 119
                lnotab 0x0202280116fe06045a013aff
             code
                argcount  : 3
                nlocals   : 5
                stacksize : 7
@@ -1082,15 +1082,15 @@
                   ('serializer_class', 'permission_classes')
                   ('using',)
                   ()
                names      ('get_serializer_class', 'admin_site', 'default_permission_classes', 'transaction', 'atomic', 'router', 'db_for_write', 'model', 'admin_views', 'ChangeView', 'as_view')
                varnames   ('self', 'request', 'object_id', 'kwargs', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'change_view'
                firstlineno 127
                lnotab 0x0202280116fe06045a013cff
             code
                argcount  : 3
                nlocals   : 5
                stacksize : 7
@@ -1176,25 +1176,25 @@
                   'permission_classes'
                   ('using',)
                   ()
                names      ('admin_site', 'default_permission_classes', 'transaction', 'atomic', 'router', 'db_for_write', 'model', 'admin_views', 'DeleteView', 'as_view')
                varnames   ('self', 'request', 'object_id', 'kwargs', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'delete_view'
                firstlineno 135
                lnotab 0x020218ff04035a013cff
             (None, False)
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'form_options', 'get_serializer_class', 'get_permission_map', 'has_add_permission', 'has_change_permission', 'has_delete_permission', 'has_view_permission', 'has_view_or_change_permission', 'has_module_permission', 'property', 'is_inline', 'list_view', 'detail_view', 'add_view', 'change_view', 'delete_view')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
          name       'BaseAPIModelAdmin'
          firstlineno 15
          lnotab
             0x0a0104050808081c080e080508050805080908030603020104ff0e0102
             030607060706080608
       'BaseAPIModelAdmin'
       code
@@ -1223,40 +1223,40 @@
          153          20 BUILD_LIST               0
                       22 LOAD_CONST               2 (('actions_on_top', 'actions_on_bottom', 'actions_selection_counter', 'empty_value_display', 'list_display', 'list_display_links', 'list_editable', 'exclude', 'show_full_result_count', 'list_per_page', 'list_max_show_all', 'date_hierarchy', 'search_help_text', 'sortable_by', 'search_fields', 'preserve_filters'))
                       24 LIST_EXTEND              1
                       26 STORE_NAME               6 (changelist_options)
          
          169          28 LOAD_CLOSURE             0 (__class__)
                       30 BUILD_TUPLE              1
-                      32 LOAD_CONST               3 (<code object __init__, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 169>)
+                      32 LOAD_CONST               3 (<code object __init__, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 169>)
                       34 MAKE_FUNCTION            8 (closure)
                       36 STORE_NAME               7 (__init__)
          
-         173          38 LOAD_CONST               4 (<code object get_action_serializer, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 173>)
+         173          38 LOAD_CONST               4 (<code object get_action_serializer, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 173>)
                       40 MAKE_FUNCTION            0
                       42 STORE_NAME               8 (get_action_serializer)
          
-         179          44 LOAD_CONST               5 (<code object get_selected_ids, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 179>)
+         179          44 LOAD_CONST               5 (<code object get_selected_ids, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 179>)
                       46 MAKE_FUNCTION            0
                       48 STORE_NAME               9 (get_selected_ids)
          
-         186          50 LOAD_CONST               6 (<code object get_urls, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 186>)
+         186          50 LOAD_CONST               6 (<code object get_urls, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 186>)
                       52 MAKE_FUNCTION            0
                       54 STORE_NAME              10 (get_urls)
          
-         219          56 LOAD_CONST               7 (<code object changelist_view, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 219>)
+         219          56 LOAD_CONST               7 (<code object changelist_view, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 219>)
                       58 MAKE_FUNCTION            0
                       60 STORE_NAME              11 (changelist_view)
          
-         225          62 LOAD_CONST               8 (<code object handle_action_view, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 225>)
+         225          62 LOAD_CONST               8 (<code object handle_action_view, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 225>)
                       64 MAKE_FUNCTION            0
                       66 STORE_NAME              12 (handle_action_view)
          
          232          68 LOAD_CONST              11 ((None,))
-                      70 LOAD_CONST              10 (<code object history_view, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 232>)
+                      70 LOAD_CONST              10 (<code object history_view, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 232>)
                       72 MAKE_FUNCTION            1 (defaults)
                       74 STORE_NAME              13 (history_view)
                       76 LOAD_CLOSURE             0 (__class__)
                       78 COPY                     1
                       80 STORE_NAME              14 (__classcell__)
                       82 RETURN_VALUE
          consts
@@ -1304,15 +1304,15 @@
                consts
                   None
                   False
                names      ('super', '__init__', 'admin_site', 'include_view_on_site_view', 'view_on_site')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       '__init__'
                firstlineno 169
                lnotab 0x04013201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 11
@@ -1374,15 +1374,15 @@
                   '%sActionSerializer'
                   ('choices',)
                   ('action', 'selected_ids')
                names      ('type', '__class__', '__name__', 'ActionSerializer', 'serializers', 'ChoiceField', 'get_action_choices', 'MultipleChoiceField', 'get_selected_ids')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'get_action_serializer'
                firstlineno 173
                lnotab 0x02013601520152fe
             code
                argcount  : 2
                nlocals   : 5
                stacksize : 7
@@ -1430,15 +1430,15 @@
                            146 RETURN_VALUE
                consts
                   None
                names      ('get_queryset', 'append', 'pk', 'str')
                varnames   ('self', 'request', 'queryset', 'choices', 'item')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'get_selected_ids'
                firstlineno 179
                lnotab 0x02012a01040108015801
             code
                argcount  : 1
                nlocals   : 9
                stacksize : 13
@@ -1721,15 +1721,15 @@
                   '<path:object_id>/change/'
                   '%s_%s_change'
                   '/'
                names      ('django.urls', 'include', 'path', 'model', '_meta', 'app_label', 'model_name', 'admin_site', 'api_admin_view', 'list_view', 'changelist_view', 'handle_action_view', 'add_view', 'detail_view', 'delete_view', 'history_view', 'change_view', 'inlines', 'insert', 'urls')
                varnames   ('self', 'include', 'path', 'info', 'admin_view', 'urlpatterns', 'inline_class', 'inline', 'opts')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'get_urls'
                firstlineno 186
                lnotab
                   0x02011002440118033c01240108ff1002240108ff10023c01240108ff10
                   02240108ff1002060126ff1002240108ff10f3041212012c011801120126
                   011eff0eff0c04
             code
@@ -1770,15 +1770,15 @@
                   None
                   'permission_classes'
                   ()
                names      ('admin_site', 'default_permission_classes', 'admin_views', 'ChangeListView', 'as_view')
                varnames   ('self', 'request', 'kwargs', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'changelist_view'
                firstlineno 219
                lnotab 0x020218ff0403
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 6
@@ -1823,15 +1823,15 @@
                   None
                   ('permission_classes', 'serializer_class')
                   ()
                names      ('admin_site', 'default_permission_classes', 'get_action_serializer', 'admin_views', 'HandleActionView', 'as_view')
                varnames   ('self', 'request', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'handle_action_view'
                firstlineno 225
                lnotab 0x0202160128fe0604
             None
             code
                argcount  : 4
                nlocals   : 5
@@ -1875,24 +1875,24 @@
                   None
                   ('permission_classes', 'serializer_class')
                   ()
                names      ('admin_site', 'default_permission_classes', 'log_entry_serializer', 'admin_views', 'HistoryView', 'as_view')
                varnames   ('self', 'request', 'object_id', 'extra_context', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'history_view'
                firstlineno 232
                lnotab 0x0202160116fe0604
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'ActionSerializer', 'action_serializer', 'changelist_options', '__init__', 'get_action_serializer', 'get_selected_ids', 'get_urls', 'changelist_view', 'handle_action_view', 'history_view', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
          name       'APIModelAdmin'
          firstlineno 143
          lnotab 0x0c010405040408100a0406060607062106060607
       'APIModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
@@ -1914,29 +1914,29 @@
                       14 STORE_NAME               3 (__doc__)
          
          244          16 LOAD_CONST               2 (None)
                       18 STORE_NAME               4 (admin_style)
          
          246          20 LOAD_CLOSURE             0 (__class__)
                       22 BUILD_TUPLE              1
-                      24 LOAD_CONST               3 (<code object __init__, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 246>)
+                      24 LOAD_CONST               3 (<code object __init__, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 246>)
                       26 MAKE_FUNCTION            8 (closure)
                       28 STORE_NAME               5 (__init__)
          
-         249          30 LOAD_CONST               4 (<code object get_object, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 249>)
+         249          30 LOAD_CONST               4 (<code object get_object, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 249>)
                       32 MAKE_FUNCTION            0
                       34 STORE_NAME               6 (get_object)
          
-         257          36 LOAD_CONST               5 (<code object get_urls, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 257>)
+         257          36 LOAD_CONST               5 (<code object get_urls, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 257>)
                       38 MAKE_FUNCTION            0
                       40 STORE_NAME               7 (get_urls)
          
          277          42 LOAD_NAME                8 (property)
          
-         278          44 LOAD_CONST               6 (<code object urls, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py", line 277>)
+         278          44 LOAD_CONST               6 (<code object urls, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py", line 277>)
                       46 MAKE_FUNCTION            0
          
          277          48 PRECALL                  0
                       52 CALL                     0
          
          278          62 STORE_NAME               9 (urls)
                       64 LOAD_CLOSURE             0 (__class__)
@@ -1974,15 +1974,15 @@
                             56 RETURN_VALUE
                consts
                   None
                names      ('super', '__init__')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       '__init__'
                firstlineno 246
                lnotab 0x0401
             code
                argcount  : 3
                nlocals   : 5
                stacksize : 4
@@ -2038,15 +2038,15 @@
                consts
                   None
                   ('pk',)
                names      ('get_queryset', 'model', 'get', 'DoesNotExist')
                varnames   ('self', 'request', 'object_id', 'queryset', 'model')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'get_object'
                firstlineno 249
                lnotab 0x02012a010e0102012e01120106ff
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 10
@@ -2208,15 +2208,15 @@
                   '%s_%s_%s_%s_change'
                   '<path:object_id>/delete/'
                   '%s_%s_%s_%s_delete'
                names      ('django.urls', 'path', 'parent_model', '_meta', 'app_label', 'model_name', 'opts', 'admin_site', 'api_admin_view', 'list_view', 'add_view', 'detail_view', 'change_view', 'delete_view')
                varnames   ('self', 'path', 'info', 'admin_view')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'get_urls'
                firstlineno 257
                lnotab
                   0x02010c0240012cff04021803240108ff1002240108ff1002240108ff10
                   02240108ff1002240108ff10f7
             code
                argcount  : 1
@@ -2235,23 +2235,23 @@
                             40 RETURN_VALUE
                consts
                   None
                names      ('get_urls',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
                name       'urls'
                firstlineno 277
                lnotab 0x0202
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'admin_style', '__init__', 'get_object', 'get_urls', 'property', 'urls', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
          name       'InlineAPIModelAdmin'
          firstlineno 240
          lnotab 0x0c01040304020a0306080614020104ff0e01
       'InlineAPIModelAdmin'
       code
          argcount  : 0
          nlocals   : 0
@@ -2272,15 +2272,15 @@
             'TabularInlineAPI'
             'tabular'
             None
          names      ('__name__', '__module__', '__qualname__', 'admin_style')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
          name       'TabularInlineAPI'
          firstlineno 282
          lnotab 0x0a01
       'TabularInlineAPI'
       code
          argcount  : 0
          nlocals   : 0
@@ -2301,23 +2301,23 @@
             'StackedInlineAPI'
             'stacked'
             None
          names      ('__name__', '__module__', '__qualname__', 'admin_style')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
          name       'StackedInlineAPI'
          firstlineno 286
          lnotab 0x0a01
       'StackedInlineAPI'
       None
    names      ('__doc__', 'django.contrib.admin.options', 'InlineModelAdmin', 'ModelAdmin', 'django.contrib.admin.utils', 'flatten_fieldsets', 'django.contrib.auth', 'get_permission_codename', 'django.db', 'router', 'transaction', 'rest_framework', 'serializers', 'django_api_admin.views', 'admin_views', 'django_api_admin.serializers', 'ActionSerializer', 'BaseAPIModelAdmin', 'APIModelAdmin', 'InlineAPIModelAdmin', 'TabularInlineAPI', 'StackedInlineAPI')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/options.py'
+   filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/options.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201040410010c010c0110010c020c010c031a7f00011e611e2a1c
       04
```

### Comparing `django-api-admin-1.1.4/django_api_admin/__pycache__/pagination.cpython-311.pyc` & `django-api-admin-1.1.5/django_api_admin/__pycache__/pagination.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5104b264 (Sat Jul 15 02:28:33 2023 UTC)
+moddate:  0xa8f0b264 (Sat Jul 15 19:16:56 2023 UTC)
 files sz: 548
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -24,25 +24,25 @@
                 18 IMPORT_NAME              2 (math)
                 20 IMPORT_FROM              3 (ceil)
                 22 STORE_NAME               3 (ceil)
                 24 POP_TOP
    
      5          26 PUSH_NULL
                 28 LOAD_BUILD_CLASS
-                30 LOAD_CONST               3 (<code object AdminResultsListPagination, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/pagination.py", line 5>)
+                30 LOAD_CONST               3 (<code object AdminResultsListPagination, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/pagination.py", line 5>)
                 32 MAKE_FUNCTION            0
                 34 LOAD_CONST               4 ('AdminResultsListPagination')
                 36 LOAD_NAME                1 (PageNumberPagination)
                 38 PRECALL                  3
                 42 CALL                     3
                 52 STORE_NAME               4 (AdminResultsListPagination)
    
     17          54 PUSH_NULL
                 56 LOAD_BUILD_CLASS
-                58 LOAD_CONST               5 (<code object AdminLogPagination, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/pagination.py", line 17>)
+                58 LOAD_CONST               5 (<code object AdminLogPagination, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/pagination.py", line 17>)
                 60 MAKE_FUNCTION            0
                 62 LOAD_CONST               6 ('AdminLogPagination')
                 64 LOAD_NAME                1 (PageNumberPagination)
                 66 PRECALL                  3
                 70 CALL                     3
                 80 STORE_NAME               5 (AdminLogPagination)
                 82 LOAD_CONST               7 (None)
@@ -70,19 +70,19 @@
          
            7          14 LOAD_CONST               2 ('page_size')
                       16 STORE_NAME               4 (page_size_query_param)
          
            8          18 LOAD_CONST               3 ('p')
                       20 STORE_NAME               5 (page_query_param)
          
-          10          22 LOAD_CONST               4 (<code object get_num_of_pages, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/pagination.py", line 10>)
+          10          22 LOAD_CONST               4 (<code object get_num_of_pages, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/pagination.py", line 10>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               6 (get_num_of_pages)
          
-          13          28 LOAD_CONST               5 (<code object get_num_of_items, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/pagination.py", line 13>)
+          13          28 LOAD_CONST               5 (<code object get_num_of_items, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/pagination.py", line 13>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               7 (get_num_of_items)
                       34 LOAD_CONST               6 (None)
                       36 RETURN_VALUE
          consts
             'AdminResultsListPagination'
             100
@@ -112,15 +112,15 @@
                             72 RETURN_VALUE
                consts
                   None
                names      ('ceil', 'len', 'page_size')
                varnames   ('self', 'list_of_items')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/pagination.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/pagination.py'
                name       'get_num_of_pages'
                firstlineno 10
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
@@ -137,24 +137,24 @@
                             30 RETURN_VALUE
                consts
                   None
                names      ('len',)
                varnames   ('self', 'list_of_items')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/pagination.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/pagination.py'
                name       'get_num_of_items'
                firstlineno 13
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'page_size', 'page_size_query_param', 'page_query_param', 'get_num_of_pages', 'get_num_of_items')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/pagination.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/pagination.py'
          name       'AdminResultsListPagination'
          firstlineno 5
          lnotab 0x0a010401040104020603
       'AdminResultsListPagination'
       code
          argcount  : 0
          nlocals   : 0
@@ -183,21 +183,21 @@
             'page_size'
             'p'
             None
          names      ('__name__', '__module__', '__qualname__', 'page_size', 'page_size_query_param', 'page_query_param')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/pagination.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/pagination.py'
          name       'AdminLogPagination'
          firstlineno 17
          lnotab 0x0a0104010401
       'AdminLogPagination'
       None
    names      ('rest_framework.pagination', 'PageNumberPagination', 'math', 'ceil', 'AdminResultsListPagination', 'AdminLogPagination')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/pagination.py'
+   filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/pagination.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c010c031c0c
```

### Comparing `django-api-admin-1.1.4/django_api_admin/__pycache__/permissions.cpython-311.pyc` & `django-api-admin-1.1.5/django_api_admin/__pycache__/permissions.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5104b264 (Sat Jul 15 02:28:33 2023 UTC)
+moddate:  0xa8f0b264 (Sat Jul 15 19:16:56 2023 UTC)
 files sz: 335
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -16,15 +16,15 @@
                  6 IMPORT_NAME              0 (rest_framework)
                  8 IMPORT_FROM              1 (permissions)
                 10 STORE_NAME               1 (permissions)
                 12 POP_TOP
    
      4          14 PUSH_NULL
                 16 LOAD_BUILD_CLASS
-                18 LOAD_CONST               2 (<code object IsAdminUser, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/permissions.py", line 4>)
+                18 LOAD_CONST               2 (<code object IsAdminUser, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/permissions.py", line 4>)
                 20 MAKE_FUNCTION            0
                 22 LOAD_CONST               3 ('IsAdminUser')
                 24 LOAD_NAME                1 (permissions)
                 26 LOAD_ATTR                2 (BasePermission)
                 36 PRECALL                  3
                 40 CALL                     3
                 50 STORE_NAME               3 (IsAdminUser)
@@ -41,19 +41,19 @@
          code 0x970065005a0164005a02640184005a03640284005a0464035300
            4           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('IsAdminUser')
                        8 STORE_NAME               2 (__qualname__)
          
-           6          10 LOAD_CONST               1 (<code object has_permission, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/permissions.py", line 6>)
+           6          10 LOAD_CONST               1 (<code object has_permission, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/permissions.py", line 6>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (has_permission)
          
-           9          16 LOAD_CONST               2 (<code object is_superuser, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/permissions.py", line 9>)
+           9          16 LOAD_CONST               2 (<code object is_superuser, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/permissions.py", line 9>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (is_superuser)
                       22 LOAD_CONST               3 (None)
                       24 RETURN_VALUE
          consts
             'IsAdminUser'
             code
@@ -74,15 +74,15 @@
                             42 RETURN_VALUE
                consts
                   None
                names      ('is_superuser',)
                varnames   ('self', 'request', 'view')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/permissions.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/permissions.py'
                name       'has_permission'
                firstlineno 6
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
@@ -114,30 +114,30 @@
                            112 RETURN_VALUE
                consts
                   None
                names      ('bool', 'user', 'is_authenticated', 'is_staff', 'is_active')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/permissions.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/permissions.py'
                name       'is_superuser'
                firstlineno 9
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'has_permission', 'is_superuser')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/permissions.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/permissions.py'
          name       'IsAdminUser'
          firstlineno 4
          lnotab 0x0a020603
       'IsAdminUser'
       None
    names      ('rest_framework', 'permissions', 'BasePermission', 'IsAdminUser')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/permissions.py'
+   filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/permissions.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c03
```

### Comparing `django-api-admin-1.1.4/django_api_admin/__pycache__/serializers.cpython-311.pyc` & `django-api-admin-1.1.5/django_api_admin/__pycache__/serializers.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5104b264 (Sat Jul 15 02:28:33 2023 UTC)
+moddate:  0xa8f0b264 (Sat Jul 15 19:16:56 2023 UTC)
 files sz: 5255
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -52,59 +52,59 @@
                 56 LOAD_NAME                3 (get_user_model)
                 58 PRECALL                  0
                 62 CALL                     0
                 72 STORE_NAME              10 (UserModel)
    
     10          74 PUSH_NULL
                 76 LOAD_BUILD_CLASS
-                78 LOAD_CONST               5 (<code object UserSerializer, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py", line 10>)
+                78 LOAD_CONST               5 (<code object UserSerializer, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py", line 10>)
                 80 MAKE_FUNCTION            0
                 82 LOAD_CONST               6 ('UserSerializer')
                 84 LOAD_NAME                9 (serializers)
                 86 LOAD_ATTR               11 (ModelSerializer)
                 96 PRECALL                  3
                100 CALL                     3
                110 STORE_NAME              12 (UserSerializer)
    
     16         112 PUSH_NULL
                114 LOAD_BUILD_CLASS
-               116 LOAD_CONST               7 (<code object LoginSerializer, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py", line 16>)
+               116 LOAD_CONST               7 (<code object LoginSerializer, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py", line 16>)
                118 MAKE_FUNCTION            0
                120 LOAD_CONST               8 ('LoginSerializer')
                122 LOAD_NAME                9 (serializers)
                124 LOAD_ATTR               13 (Serializer)
                134 PRECALL                  3
                138 CALL                     3
                148 STORE_NAME              14 (LoginSerializer)
    
     71         150 PUSH_NULL
                152 LOAD_BUILD_CLASS
-               154 LOAD_CONST               9 (<code object LogEntrySerializer, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py", line 71>)
+               154 LOAD_CONST               9 (<code object LogEntrySerializer, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py", line 71>)
                156 MAKE_FUNCTION            0
                158 LOAD_CONST              10 ('LogEntrySerializer')
                160 LOAD_NAME                9 (serializers)
                162 LOAD_ATTR               11 (ModelSerializer)
                172 PRECALL                  3
                176 CALL                     3
                186 STORE_NAME              15 (LogEntrySerializer)
    
     81         188 PUSH_NULL
                190 LOAD_BUILD_CLASS
-               192 LOAD_CONST              11 (<code object PasswordChangeSerializer, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py", line 81>)
+               192 LOAD_CONST              11 (<code object PasswordChangeSerializer, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py", line 81>)
                194 MAKE_FUNCTION            0
                196 LOAD_CONST              12 ('PasswordChangeSerializer')
                198 LOAD_NAME                9 (serializers)
                200 LOAD_ATTR               13 (Serializer)
                210 PRECALL                  3
                214 CALL                     3
                224 STORE_NAME              16 (PasswordChangeSerializer)
    
    130         226 PUSH_NULL
                228 LOAD_BUILD_CLASS
-               230 LOAD_CONST              13 (<code object ActionSerializer, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py", line 130>)
+               230 LOAD_CONST              13 (<code object ActionSerializer, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py", line 130>)
                232 MAKE_FUNCTION            0
                234 LOAD_CONST              14 ('ActionSerializer')
                236 LOAD_NAME                9 (serializers)
                238 LOAD_ATTR               13 (Serializer)
                248 PRECALL                  3
                252 CALL                     3
                262 STORE_NAME              17 (ActionSerializer)
@@ -128,15 +128,15 @@
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('UserSerializer')
                        8 STORE_NAME               2 (__qualname__)
          
           11          10 PUSH_NULL
                       12 LOAD_BUILD_CLASS
-                      14 LOAD_CONST               1 (<code object Meta, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py", line 11>)
+                      14 LOAD_CONST               1 (<code object Meta, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py", line 11>)
                       16 MAKE_FUNCTION            0
                       18 LOAD_CONST               2 ('Meta')
                       20 PRECALL                  2
                       24 CALL                     2
                       34 STORE_NAME               3 (Meta)
                       36 LOAD_CONST               3 (None)
                       38 RETURN_VALUE
@@ -165,25 +165,25 @@
                   'UserSerializer.Meta'
                   ('password',)
                   None
                names      ('__name__', '__module__', '__qualname__', 'UserModel', 'model', 'exclude')
                varnames   ()
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py'
                name       'Meta'
                firstlineno 11
                lnotab 0x0a010401
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py'
          name       'UserSerializer'
          firstlineno 10
          lnotab 0x0a01
       'UserSerializer'
       code
          argcount  : 0
          nlocals   : 0
@@ -201,23 +201,23 @@
                       10 STORE_NAME               2 (__qualname__)
          
           17          12 LOAD_CONST               1 ('\n    Validates login credentials and generates token.\n    ')
                       14 STORE_NAME               3 (__doc__)
          
           21          16 LOAD_CLOSURE             0 (__class__)
                       18 BUILD_TUPLE              1
-                      20 LOAD_CONST               2 (<code object __init__, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py", line 21>)
+                      20 LOAD_CONST               2 (<code object __init__, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py", line 21>)
                       22 MAKE_FUNCTION            8 (closure)
                       24 STORE_NAME               4 (__init__)
          
-          45          26 LOAD_CONST               3 (<code object validate, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py", line 45>)
+          45          26 LOAD_CONST               3 (<code object validate, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py", line 45>)
                       28 MAKE_FUNCTION            0
                       30 STORE_NAME               5 (validate)
          
-          64          32 LOAD_CONST               4 (<code object get_user, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py", line 64>)
+          64          32 LOAD_CONST               4 (<code object get_user, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py", line 64>)
                       34 MAKE_FUNCTION            0
                       36 STORE_NAME               6 (get_user)
                       38 LOAD_CLOSURE             0 (__class__)
                       40 COPY                     1
                       42 STORE_NAME               7 (__classcell__)
                       44 RETURN_VALUE
          consts
@@ -377,15 +377,15 @@
                   'Please login with an account that has permissions to access the admin site'
                   'This account is inactive.'
                   ('invalid_login', 'permission_denied', 'inactive')
                names      ('super', '__init__', 'user_cache', 'UserModel', '_meta', 'get_field', 'USERNAME_FIELD', 'serializers', 'ModelSerializer', 'serializer_field_mapping', '__class__', 'max_length', 'username', '_declared_fields', 'CharField', 'password', 'error_messages', 'update', '_')
                varnames   ('self', 'args', 'kwargs', 'username_field')
                freevars   ('__class__',)
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py'
                name       '__init__'
                firstlineno 21
                lnotab
                   0x040132010e02520136010eff1c0232011c010aff1c021e0322010c0102
                   ff0e031afd04051c021cf8
             code
                argcount  : 2
@@ -518,15 +518,15 @@
                   ('code',)
                   'permission_denied'
                   'inactive'
                names      ('get', 'UserModel', 'USERNAME_FIELD', 'context', 'authenticate', 'user_cache', 'serializers', 'ValidationError', 'error_messages', 'is_staff', 'is_active')
                varnames   ('self', 'data', 'username', 'password', 'request')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py'
                name       'validate'
                firstlineno 45
                lnotab
                   0x02013e012a01340208010c0106ff1c020e0116011aff120218012e0102
                   ff1202180116011aff1202
             code
                argcount  : 1
@@ -561,23 +561,23 @@
                   None
                   '_validated_data'
                   'You must call is valid before calling get_user'
                names      ('hasattr', 'AssertionError', 'user_cache')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py'
                name       'get_user'
                firstlineno 64
                lnotab 0x020120010c0102ff1002
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', 'validate', 'get_user', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py'
          name       'LoginSerializer'
          firstlineno 16
          lnotab 0x0c0104040a180613
       'LoginSerializer'
       code
          argcount  : 0
          nlocals   : 0
@@ -593,15 +593,15 @@
                        8 STORE_NAME               2 (__qualname__)
          
           72          10 LOAD_CONST               1 ('\n    default django.contrib.admin.models.LogEntry serializer.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
           76          14 PUSH_NULL
                       16 LOAD_BUILD_CLASS
-                      18 LOAD_CONST               2 (<code object Meta, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py", line 76>)
+                      18 LOAD_CONST               2 (<code object Meta, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py", line 76>)
                       20 MAKE_FUNCTION            0
                       22 LOAD_CONST               3 ('Meta')
                       24 PRECALL                  2
                       28 CALL                     2
                       38 STORE_NAME               4 (Meta)
                       40 LOAD_CONST               4 (None)
                       42 RETURN_VALUE
@@ -631,25 +631,25 @@
                   'LogEntrySerializer.Meta'
                   '__all__'
                   None
                names      ('__name__', '__module__', '__qualname__', 'LogEntry', 'model', 'fields')
                varnames   ()
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py'
                name       'Meta'
                firstlineno 76
                lnotab 0x0a010401
             'Meta'
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'Meta')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py'
          name       'LogEntrySerializer'
          firstlineno 71
          lnotab 0x0a010404
       'LogEntrySerializer'
       code
          argcount  : 0
          nlocals   : 0
@@ -733,24 +733,24 @@
           89         184 KW_NAMES                 6
                      186 PRECALL                  4
                      190 CALL                     4
                      200 STORE_NAME               9 (new_password2)
          
           92         202 LOAD_CLOSURE             0 (__class__)
                      204 BUILD_TUPLE              1
-                     206 LOAD_CONST               9 (<code object __init__, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py", line 92>)
+                     206 LOAD_CONST               9 (<code object __init__, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py", line 92>)
                      208 MAKE_FUNCTION            8 (closure)
                      210 STORE_NAME              10 (__init__)
          
-         100         212 LOAD_CONST              10 (<code object validate, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py", line 100>)
+         100         212 LOAD_CONST              10 (<code object validate, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py", line 100>)
                      214 MAKE_FUNCTION            0
                      216 STORE_NAME              11 (validate)
          
          121         218 LOAD_CONST              12 ((True,))
-                     220 LOAD_CONST              11 (<code object save, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py", line 121>)
+                     220 LOAD_CONST              11 (<code object save, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py", line 121>)
                      222 MAKE_FUNCTION            1 (defaults)
                      224 STORE_NAME              12 (save)
                      226 LOAD_CLOSURE             0 (__class__)
                      228 COPY                     1
                      230 STORE_NAME              13 (__classcell__)
                      232 RETURN_VALUE
          consts
@@ -817,15 +817,15 @@
                   'The two password fields didn’t match.'
                   'Your old password was entered incorrectly. Please enter it again.'
                   ('password_mismatch', 'password_incorrect')
                names      ('super', '__init__', 'error_messages', 'update', '_')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py'
                name       '__init__'
                firstlineno 92
                lnotab 0x0401320222011c011cfe
             code
                argcount  : 2
                nlocals   : 6
                stacksize : 4
@@ -926,15 +926,15 @@
                   'new_password1'
                   'new_password2'
                   'password_mismatch'
                names      ('context', 'check_password', 'serializers', 'ValidationError', 'error_messages', 'get')
                varnames   ('self', 'data', 'user', 'old_password', 'password1', 'password2')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py'
                name       'validate'
                firstlineno 100
                lnotab
                   0x02011a0210012a011601180102fe12052a012a0214011601180102fe12
                   05
             code
                argcount  : 2
@@ -983,24 +983,24 @@
                   None
                   'new_password1'
                   'user'
                names      ('validated_data', 'context', 'set_password', 'save')
                varnames   ('self', 'commit', 'password', 'user')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py'
                name       'save'
                firstlineno 121
                lnotab 0x02011a011a012a0104012801
             (True,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'serializers', 'CharField', '_', 'old_password', 'new_password1', 'new_password2', '__init__', 'validate', 'save', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py'
          name       'PasswordChangeSerializer'
          firstlineno 81
          lnotab 0x0c010403260106ff1202260106ff1202260106ff12030a080615
       'PasswordChangeSerializer'
       code
          argcount  : 0
          nlocals   : 0
@@ -1062,21 +1062,21 @@
             0
             ('required', 'default')
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'serializers', 'ChoiceField', 'action', 'MultipleChoiceField', 'selected_ids', 'BooleanField', 'select_across')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py'
          name       'ActionSerializer'
          firstlineno 130
          lnotab 0x0a01040324012401
       'ActionSerializer'
       None
    names      ('django.contrib.admin.models', 'LogEntry', 'django.contrib.auth', 'get_user_model', 'authenticate', 'django.utils.translation', 'gettext_lazy', '_', 'rest_framework', 'serializers', 'UserModel', 'ModelSerializer', 'UserSerializer', 'Serializer', 'LoginSerializer', 'LogEntrySerializer', 'PasswordChangeSerializer', 'ActionSerializer')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/serializers.py'
+   filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/serializers.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02010c0110010c010c03140326062637260a2631
```

### Comparing `django-api-admin-1.1.4/django_api_admin/__pycache__/sites.cpython-311.pyc` & `django-api-admin-1.1.5/django_api_admin/__pycache__/sites.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5104b264 (Sat Jul 15 02:28:33 2023 UTC)
+moddate:  0xa8f0b264 (Sat Jul 15 19:16:56 2023 UTC)
 files sz: 12948
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -157,15 +157,15 @@
                232 LOAD_NAME               10 (get_user_model)
                234 PRECALL                  0
                238 CALL                     0
                248 STORE_NAME              39 (UserModel)
    
     29         250 PUSH_NULL
                252 LOAD_BUILD_CLASS
-               254 LOAD_CONST              20 (<code object APIAdminSite, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 29>)
+               254 LOAD_CONST              20 (<code object APIAdminSite, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 29>)
                256 MAKE_FUNCTION            0
                258 LOAD_CONST              21 ('APIAdminSite')
                260 LOAD_NAME                6 (AdminSite)
                262 PRECALL                  3
                266 CALL                     3
                276 STORE_NAME              40 (APIAdminSite)
    
@@ -260,104 +260,104 @@
          
           51          94 LOAD_NAME               21 (AdminLogPagination)
                       96 STORE_NAME              22 (default_log_pagination_class)
          
           53          98 LOAD_CONST              24 ((False,))
                      100 LOAD_CLOSURE             0 (__class__)
                      102 BUILD_TUPLE              1
-                     104 LOAD_CONST               4 (<code object __init__, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 53>)
+                     104 LOAD_CONST               4 (<code object __init__, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 53>)
                      106 MAKE_FUNCTION            9 (defaults, closure)
                      108 STORE_NAME              23 (__init__)
          
           66         110 LOAD_CONST              25 ((None,))
-                     112 LOAD_CONST               6 (<code object register, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 66>)
+                     112 LOAD_CONST               6 (<code object register, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 66>)
                      114 MAKE_FUNCTION            1 (defaults)
                      116 STORE_NAME              24 (register)
          
           91         118 LOAD_CONST              24 ((False,))
-                     120 LOAD_CONST               7 (<code object api_admin_view, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 91>)
+                     120 LOAD_CONST               7 (<code object api_admin_view, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 91>)
                      122 MAKE_FUNCTION            1 (defaults)
                      124 STORE_NAME              25 (api_admin_view)
          
-         106         126 LOAD_CONST               8 (<code object get_urls, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 106>)
+         106         126 LOAD_CONST               8 (<code object get_urls, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 106>)
                      128 MAKE_FUNCTION            0
                      130 STORE_NAME              26 (get_urls)
          
          164         132 LOAD_NAME               27 (property)
          
-         165         134 LOAD_CONST               9 (<code object urls, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 164>)
+         165         134 LOAD_CONST               9 (<code object urls, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 164>)
                      136 MAKE_FUNCTION            0
          
          164         138 PRECALL                  0
                      142 CALL                     0
          
          165         152 STORE_NAME              28 (urls)
          
          168         154 LOAD_CONST              25 ((None,))
-                     156 LOAD_CONST              10 (<code object _build_app_dict, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 168>)
+                     156 LOAD_CONST              10 (<code object _build_app_dict, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 168>)
                      158 MAKE_FUNCTION            1 (defaults)
                      160 STORE_NAME              29 (_build_app_dict)
          
          246         162 LOAD_CONST              25 ((None,))
-                     164 LOAD_CONST              11 (<code object paginate_queryset, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 246>)
+                     164 LOAD_CONST              11 (<code object paginate_queryset, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 246>)
                      166 MAKE_FUNCTION            1 (defaults)
                      168 STORE_NAME              30 (paginate_queryset)
          
-         250         170 LOAD_CONST              12 (<code object get_log_entry_serializer, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 250>)
+         250         170 LOAD_CONST              12 (<code object get_log_entry_serializer, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 250>)
                      172 MAKE_FUNCTION            0
                      174 STORE_NAME              31 (get_log_entry_serializer)
          
          255         176 LOAD_CONST              25 ((None,))
-                     178 LOAD_CONST              13 (<code object index, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 255>)
+                     178 LOAD_CONST              13 (<code object index, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 255>)
                      180 MAKE_FUNCTION            1 (defaults)
                      182 STORE_NAME              32 (index)
          
          261         184 LOAD_CONST              25 ((None,))
-                     186 LOAD_CONST              14 (<code object app_index, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 261>)
+                     186 LOAD_CONST              14 (<code object app_index, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 261>)
                      188 MAKE_FUNCTION            1 (defaults)
                      190 STORE_NAME              33 (app_index)
          
          267         192 LOAD_CONST              25 ((None,))
-                     194 LOAD_CONST              15 (<code object login, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 267>)
+                     194 LOAD_CONST              15 (<code object login, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 267>)
                      196 MAKE_FUNCTION            1 (defaults)
                      198 STORE_NAME              34 (login)
          
          278         200 LOAD_CONST              25 ((None,))
-                     202 LOAD_CONST              16 (<code object logout, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 278>)
+                     202 LOAD_CONST              16 (<code object logout, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 278>)
                      204 MAKE_FUNCTION            1 (defaults)
                      206 STORE_NAME              35 (logout)
          
          284         208 LOAD_CONST              25 ((None,))
-                     210 LOAD_CONST              17 (<code object password_change, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 284>)
+                     210 LOAD_CONST              17 (<code object password_change, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 284>)
                      212 MAKE_FUNCTION            1 (defaults)
                      214 STORE_NAME              36 (password_change)
          
          291         216 LOAD_CONST              25 ((None,))
-                     218 LOAD_CONST              18 (<code object i18n_javascript, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 291>)
+                     218 LOAD_CONST              18 (<code object i18n_javascript, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 291>)
                      220 MAKE_FUNCTION            1 (defaults)
                      222 STORE_NAME              37 (i18n_javascript)
          
-         297         224 LOAD_CONST              19 (<code object autocomplete_view, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 297>)
+         297         224 LOAD_CONST              19 (<code object autocomplete_view, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 297>)
                      226 MAKE_FUNCTION            0
                      228 STORE_NAME              38 (autocomplete_view)
          
-         303         230 LOAD_CONST              20 (<code object site_context_view, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 303>)
+         303         230 LOAD_CONST              20 (<code object site_context_view, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 303>)
                      232 MAKE_FUNCTION            0
                      234 STORE_NAME              39 (site_context_view)
          
-         309         236 LOAD_CONST              21 (<code object admin_log_view, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 309>)
+         309         236 LOAD_CONST              21 (<code object admin_log_view, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 309>)
                      238 MAKE_FUNCTION            0
                      240 STORE_NAME              40 (admin_log_view)
          
          317         242 LOAD_CONST              25 ((None,))
-                     244 LOAD_CONST              22 (<code object csrf_view, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 317>)
+                     244 LOAD_CONST              22 (<code object csrf_view, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 317>)
                      246 MAKE_FUNCTION            1 (defaults)
                      248 STORE_NAME              41 (csrf_view)
          
-         323         250 LOAD_CONST              23 (<code object user_info_view, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 323>)
+         323         250 LOAD_CONST              23 (<code object user_info_view, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 323>)
                      252 MAKE_FUNCTION            0
                      254 STORE_NAME              42 (user_info_view)
                      256 LOAD_CLOSURE             0 (__class__)
                      258 COPY                     1
                      260 STORE_NAME              43 (__classcell__)
                      262 RETURN_VALUE
          consts
@@ -437,15 +437,15 @@
                consts
                   None
                   'delete_selected'
                names      ('super', '__init__', 'actions', 'delete_selected', '_actions', 'copy', '_global_actions', 'admin_class', 'APIModelAdmin', 'register', 'UserModel', 'Group')
                varnames   ('self', 'include_auth', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       '__init__'
                firstlineno 53
                lnotab 0x0402320326013c012603040146ff
             None
             code
                argcount  : 3
                nlocals   : 5
@@ -570,15 +570,15 @@
                   'The model %s is already registered '
                   '__module__'
                   '%sAdmin'
                names      ('admin_class', 'isinstance', 'ModelBase', '_meta', 'abstract', 'ImproperlyConfigured', '__name__', '_registry', 'AlreadyRegistered', 'swapped', 'type')
                varnames   ('self', 'model_or_iterable', 'admin_class', 'options', 'model')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       'register'
                firstlineno 66
                lnotab
                   0x020112022a010602080118010c0112ff100412010c0112ff1003180104
                   0114010e010cff040106ff10042aef
             code
                argcount  : 3
@@ -593,15 +593,15 @@
                   00000000007c038901a6020000ab0200000000000000005300
                              0 MAKE_CELL                1 (view)
                
                 91           2 RESUME                   0
                
                 97           4 LOAD_CLOSURE             1 (view)
                              6 BUILD_TUPLE              1
-                             8 LOAD_CONST               1 (<code object inner, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 97>)
+                             8 LOAD_CONST               1 (<code object inner, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 97>)
                             10 MAKE_FUNCTION            8 (closure)
                             12 STORE_FAST               3 (inner)
                
                100          14 LOAD_FAST                2 (cacheable)
                             16 POP_JUMP_FORWARD_IF_TRUE    15 (to 48)
                
                101          18 LOAD_GLOBAL              1 (NULL + never_cache)
@@ -656,25 +656,25 @@
                                   26 RETURN_VALUE
                      consts
                         None
                      names      ()
                      varnames   ('request', 'args', 'kwargs')
                      freevars   ('view',)
                      cellvars   ()
-                     filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+                     filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                      name       'inner'
                      firstlineno 97
                      lnotab 0x0401
                   'csrf_exempt'
                   False
                names      ('never_cache', 'getattr', 'csrf_protect', 'update_wrapper')
                varnames   ('self', 'view', 'cacheable', 'inner')
                freevars   ()
                cellvars   ('view',)
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       'api_admin_view'
                firstlineno 91
                lnotab 0x04060a0304011e0122011e01
             code
                argcount  : 1
                nlocals   : 12
                stacksize : 15
@@ -911,15 +911,15 @@
                126         736 KW_NAMES                 6
                            738 PRECALL                  3
                            742 CALL                     3
                
                110         752 BUILD_LIST              10
                            754 STORE_FAST               5 (urlpatterns)
                
-               131         756 LOAD_CONST              27 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 131>)
+               131         756 LOAD_CONST              27 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 131>)
                            758 MAKE_FUNCTION            0
                
                132         760 LOAD_FAST                0 (self)
                            762 LOAD_ATTR               18 (_registry)
                            772 LOAD_METHOD             19 (items)
                            794 PRECALL                  0
                            798 CALL                     0
@@ -1036,15 +1036,15 @@
                           1274 LOAD_CONST              35 (('app_list', 'view_on_site', 'language_catalog'))
                           1276 LIST_EXTEND              1
                           1278 STORE_DEREF             13 (excluded_url_names)
                
                157        1280 LOAD_CLOSURE            12 (URLPattern)
                           1282 LOAD_CLOSURE            13 (excluded_url_names)
                           1284 BUILD_TUPLE              2
-                          1286 LOAD_CONST              36 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 157>)
+                          1286 LOAD_CONST              36 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 157>)
                           1288 MAKE_FUNCTION            8 (closure)
                           1290 LOAD_FAST                5 (urlpatterns)
                           1292 GET_ITER
                           1294 PRECALL                  0
                           1298 CALL                     0
                           1308 STORE_FAST              10 (root_urls)
                
@@ -1127,15 +1127,15 @@
                                   40 JUMP_BACKWARD           18 (to 6)
                              >>   42 RETURN_VALUE
                      consts
                      names      ('_meta', 'app_label')
                      varnames   ('.0', 'model', 'model_admin')
                      freevars   ()
                      cellvars   ()
-                     filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+                     filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                      name       '<listcomp>'
                      firstlineno 131
                      lnotab 0x0e0102ff
                   '^(?P<app_label>'
                   '|'
                   ')/$'
                   'app_list'
@@ -1185,26 +1185,26 @@
                              >>   80 JUMP_BACKWARD           37 (to 8)
                              >>   82 RETURN_VALUE
                      consts
                      names      ('isinstance', 'name')
                      varnames   ('.0', 'url')
                      freevars   ('URLPattern', 'excluded_url_names')
                      cellvars   ()
-                     filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+                     filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                      name       '<listcomp>'
                      firstlineno 157
                      lnotab 0x0c011eff02010cff020112ff0201
                   ('root_urls',)
                   ''
                   'api-root'
                names      ('django.contrib.contenttypes', 'views', 'django.urls', 'URLPattern', 'include', 'path', 're_path', 'api_admin_view', 'index', 'csrf_view', 'user_info_view', 'login', 'logout', 'password_change', 'autocomplete_view', 'i18n_javascript', 'site_context_view', 'admin_log_view', '_registry', 'items', 'join', 'append', 'app_index', '_meta', 'app_label', 'model_name', 'urls', 'include_view_on_site_view', 'shortcut', 'include_root_view', 'site_views', 'AdminAPIRootView', 'as_view')
                varnames   ('self', 'contenttype_views', 'include', 'path', 're_path', 'urlpatterns', 'valid_app_labels', 'regex', 'model', 'model_admin', 'root_urls', 'root_view')
                freevars   ()
                cellvars   ('URLPattern', 'excluded_url_names')
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       'get_urls'
                firstlineno 106
                lnotab
                   0x06010c0118034a01380102ff1002380102ff100224014a012a0102ff10
                   0102ff1002380102ff10022a0102ff100102ff1002380102ff1002380102
                   ff10f00415040130ff1202360118014aff10043c0102011e011aff02011e
                   ff0eff0a060e011c0102010c0102fd20070e0208021e022c0102ff120242
@@ -1232,15 +1232,15 @@
                             66 RETURN_VALUE
                consts
                   None
                names      ('get_urls', 'name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       'urls'
                firstlineno 164
                lnotab 0x0202
             code
                argcount  : 3
                nlocals   : 12
                stacksize : 9
@@ -1299,15 +1299,15 @@
                              6 STORE_FAST               3 (app_dict)
                
                175           8 LOAD_DEREF               2 (label)
                             10 POP_JUMP_FORWARD_IF_FALSE    38 (to 88)
                
                176          12 LOAD_CLOSURE             2 (label)
                             14 BUILD_TUPLE              1
-                            16 LOAD_CONST               1 (<code object <dictcomp>, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py", line 176>)
+                            16 LOAD_CONST               1 (<code object <dictcomp>, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py", line 176>)
                             18 MAKE_FUNCTION            8 (closure)
                
                177          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                0 (_registry)
                             32 LOAD_METHOD              1 (items)
                             54 PRECALL                  0
                             58 CALL                     0
@@ -1655,15 +1655,15 @@
                                   56 JUMP_BACKWARD           25 (to 8)
                              >>   58 RETURN_VALUE
                      consts
                      names      ('_meta', 'app_label')
                      varnames   ('.0', 'm', 'm_a')
                      freevars   ('label',)
                      cellvars   ()
-                     filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+                     filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                      name       '<dictcomp>'
                      firstlineno 176
                      lnotab 0x0a01080120ff0401
                   True
                   None
                   ('name', 'object_name', 'perms', 'list_url', 'changelist_url', 'add_url', 'perform_action_url')
                   'change'
@@ -1684,15 +1684,15 @@
                   'app_label'
                   ('kwargs', 'current_app')
                   ('name', 'app_label', 'app_url', 'has_module_perms', 'models')
                names      ('_registry', 'items', '_meta', 'app_label', 'has_module_permission', 'get_model_perms', 'values', 'name', 'model_name', 'capfirst', 'verbose_name_plural', 'object_name', 'get', 'build_absolute_uri', 'reverse', 'NoReverseMatch', 'append', 'apps', 'get_app_config', 'verbose_name')
                varnames   ('self', 'request', 'label', 'app_dict', 'models', 'model', 'model_admin', 'app_label', 'has_module_perms', 'perms', 'info', 'model_dict')
                freevars   ()
                cellvars   ('label',)
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       '_build_app_dict'
                firstlineno 168
                lnotab
                   0x040504020401080130ff14050e02340118022a01040102022a042c0102
                   02280230011601020102010201020102f9060a540132010201180130ff16
                   02180130ff1602180130ff1a02120104ff08032a010201180130ff1a0212
                   0104ff080308014603300102010c01120106010cfd1005020104f7100c04
@@ -1733,15 +1733,15 @@
                   None
                   'pk'
                   ('view',)
                names      ('default_pagination_class', 'paginate_queryset', 'order_by')
                varnames   ('self', 'queryset', 'request', 'view', 'paginator')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       'paginate_queryset'
                firstlineno 246
                lnotab 0x02012801
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 8
@@ -1777,15 +1777,15 @@
                   'user'
                   True
                   ('read_only',)
                names      ('type', 'log_entry_serializer', 'user_serializer')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       'get_log_entry_serializer'
                firstlineno 250
                lnotab 0x02011c012cff
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 6
@@ -1823,15 +1823,15 @@
                   'permission_classes'
                   ('admin_site',)
                   ()
                names      ('default_permission_classes', 'site_views', 'IndexView', 'as_view')
                varnames   ('self', 'request', 'extra_context', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       'index'
                firstlineno 255
                lnotab 0x02020eff0403
             code
                argcount  : 4
                nlocals   : 5
                stacksize : 6
@@ -1870,15 +1870,15 @@
                   'permission_classes'
                   ('app_label', 'admin_site')
                   ()
                names      ('default_permission_classes', 'site_views', 'AppIndexView', 'as_view')
                varnames   ('self', 'request', 'app_label', 'extra_context', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       'app_index'
                firstlineno 261
                lnotab 0x02020eff0403
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 6
@@ -1941,15 +1941,15 @@
                   ('permission_classes', 'serializer_class')
                   'GET'
                   ()
                names      ('login_serializer', 'method', 'site_views', 'LoginView', 'as_view')
                varnames   ('self', 'request', 'extra_context', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       'login'
                firstlineno 267
                lnotab 0x020202010cfe060516014002
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 6
@@ -1984,15 +1984,15 @@
                   None
                   'permission_classes'
                   ()
                names      ('default_permission_classes', 'site_views', 'LogoutView', 'as_view')
                varnames   ('self', 'request', 'extra_context', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       'logout'
                firstlineno 278
                lnotab 0x02020eff0403
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 6
@@ -2031,15 +2031,15 @@
                   None
                   ('permission_classes', 'serializer_class')
                   ()
                names      ('default_permission_classes', 'password_change_serializer', 'site_views', 'PasswordChangeView', 'as_view')
                varnames   ('self', 'request', 'extra_context', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       'password_change'
                firstlineno 284
                lnotab 0x02020c010cfe0604
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 6
@@ -2074,15 +2074,15 @@
                   None
                   'permission_classes'
                   ()
                names      ('default_permission_classes', 'site_views', 'LanguageCatalogView', 'as_view')
                varnames   ('self', 'request', 'extra_context', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       'i18n_javascript'
                firstlineno 291
                lnotab 0x02020eff0403
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 6
@@ -2120,15 +2120,15 @@
                   'permission_classes'
                   ('admin_site',)
                   ()
                names      ('default_permission_classes', 'site_views', 'AutoCompleteView', 'as_view')
                varnames   ('self', 'request', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       'autocomplete_view'
                firstlineno 297
                lnotab 0x02020eff0403
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 6
@@ -2166,15 +2166,15 @@
                   'permission_classes'
                   ('admin_site',)
                   ()
                names      ('default_permission_classes', 'site_views', 'SiteContextView', 'as_view')
                varnames   ('self', 'request', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       'site_context_view'
                firstlineno 303
                lnotab 0x02020eff0403
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 6
@@ -2220,15 +2220,15 @@
                   None
                   ('permission_classes', 'pagination_class', 'serializer_class')
                   ()
                names      ('default_permission_classes', 'default_log_pagination_class', 'get_log_entry_serializer', 'site_views', 'AdminLogView', 'as_view')
                varnames   ('self', 'request', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       'admin_log_view'
                firstlineno 309
                lnotab 0x02020c010c0126fd0605
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 6
@@ -2262,15 +2262,15 @@
                   None
                   'permission_classes'
                   ()
                names      ('site_views', 'CsrfTokenView', 'as_view')
                varnames   ('self', 'request', 'extra_context', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       'csrf_view'
                firstlineno 317
                lnotab 0x020204ff0403
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 6
@@ -2309,25 +2309,25 @@
                   None
                   ('permission_classes', 'serializer_class')
                   ()
                names      ('default_permission_classes', 'user_serializer', 'site_views', 'UserInformation', 'as_view')
                varnames   ('self', 'request', 'defaults')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
                name       'user_info_view'
                firstlineno 323
                lnotab 0x02020c010cfe0604
             (False,)
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'APIModelAdmin', 'admin_class', 'include_view_on_site_view', 'include_root_view', 'IsAdminUser', 'default_permission_classes', 'api_serializers', 'LoginSerializer', 'login_serializer', 'PasswordChangeSerializer', 'password_change_serializer', 'LogEntrySerializer', 'log_entry_serializer', 'UserSerializer', 'user_serializer', 'AdminResultsListPagination', 'default_pagination_class', 'AdminLogPagination', 'default_log_pagination_class', '__init__', 'register', 'api_admin_view', 'get_urls', 'property', 'urls', '_build_app_dict', 'paginate_queryset', 'get_log_entry_serializer', 'index', 'app_index', 'login', 'logout', 'password_change', 'i18n_javascript', 'autocomplete_view', 'site_context_view', 'admin_log_view', 'csrf_view', 'user_info_view', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
          name       'APIAdminSite'
          firstlineno 29
          lnotab
             0x0c01040404030401040306030e010e010e010e03040104020c0d081908
             0f063a020104ff0e010203084e0804060508060806080b08060807080606
             06060606080806
       'APIAdminSite'
@@ -2335,13 +2335,13 @@
       True
       ('name', 'include_auth')
       None
    names      ('__doc__', 'functools', 'update_wrapper', 'django.apps', 'apps', 'django.contrib.admin', 'AdminSite', 'django.contrib.admin.sites', 'AlreadyRegistered', 'django.contrib.auth', 'get_user_model', 'django.contrib.auth.models', 'Group', 'django.core.exceptions', 'ImproperlyConfigured', 'django.db.models.base', 'ModelBase', 'django.urls', 'NoReverseMatch', 'reverse', 'django.utils.text', 'capfirst', 'django.views.decorators.cache', 'never_cache', 'django.views.decorators.csrf', 'csrf_protect', 'django_api_admin', 'actions', 'serializers', 'api_serializers', 'django_api_admin.views', 'site_views', 'django_api_admin.options', 'APIModelAdmin', 'django_api_admin.pagination', 'AdminLogPagination', 'AdminResultsListPagination', 'django_api_admin.permissions', 'IsAdminUser', 'UserModel', 'APIAdminSite', 'site')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/sites.py'
+   filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/sites.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020104040c020c010c010c010c010c010c010c0110010c010c010c
       020c010c010c010c0110010c0214031c7f007f0030
```

### Comparing `django-api-admin-1.1.4/django_api_admin/actions.py` & `django-api-admin-1.1.5/django_api_admin/actions.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.4/django_api_admin/declarations/__pycache__/classes.cpython-311.pyc` & `django-api-admin-1.1.5/django_api_admin/declarations/__pycache__/classes.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5104b264 (Sat Jul 15 02:28:33 2023 UTC)
+moddate:  0xa8f0b264 (Sat Jul 15 19:16:56 2023 UTC)
 files sz: 1324
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -27,15 +27,15 @@
                 22 IMPORT_NAME              3 (django.utils.translation)
                 24 IMPORT_FROM              4 (gettext_lazy)
                 26 STORE_NAME               5 (_)
                 28 POP_TOP
    
      8          30 PUSH_NULL
                 32 LOAD_BUILD_CLASS
-                34 LOAD_CONST               4 (<code object ModelDiffHelper, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py", line 8>)
+                34 LOAD_CONST               4 (<code object ModelDiffHelper, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py", line 8>)
                 36 MAKE_FUNCTION            0
                 38 LOAD_CONST               5 ('ModelDiffHelper')
                 40 LOAD_NAME                6 (object)
                 42 PRECALL                  3
                 46 CALL                     3
                 56 STORE_NAME               7 (ModelDiffHelper)
                 58 LOAD_CONST               6 (None)
@@ -60,57 +60,57 @@
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ModelDiffHelper')
                        8 STORE_NAME               2 (__qualname__)
          
            9          10 LOAD_CONST               1 ('\n    detects the changes after every operation used to log admin changes.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-          13          14 LOAD_CONST               2 (<code object __init__, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py", line 13>)
+          13          14 LOAD_CONST               2 (<code object __init__, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py", line 13>)
                       16 MAKE_FUNCTION            0
                       18 STORE_NAME               4 (__init__)
          
-          17          20 LOAD_CONST               3 (<code object set_changed_model, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py", line 17>)
+          17          20 LOAD_CONST               3 (<code object set_changed_model, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py", line 17>)
                       22 MAKE_FUNCTION            0
                       24 STORE_NAME               5 (set_changed_model)
          
           24          26 LOAD_NAME                6 (property)
          
-          25          28 LOAD_CONST               4 (<code object diff, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py", line 24>)
+          25          28 LOAD_CONST               4 (<code object diff, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py", line 24>)
                       30 MAKE_FUNCTION            0
          
           24          32 PRECALL                  0
                       36 CALL                     0
          
           25          46 STORE_NAME               7 (diff)
          
           33          48 LOAD_NAME                6 (property)
          
-          34          50 LOAD_CONST               5 (<code object has_changed, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py", line 33>)
+          34          50 LOAD_CONST               5 (<code object has_changed, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py", line 33>)
                       52 MAKE_FUNCTION            0
          
           33          54 PRECALL                  0
                       58 CALL                     0
          
           34          68 STORE_NAME               8 (has_changed)
          
           37          70 LOAD_NAME                6 (property)
          
-          38          72 LOAD_CONST               6 (<code object changed_fields, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py", line 37>)
+          38          72 LOAD_CONST               6 (<code object changed_fields, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py", line 37>)
                       74 MAKE_FUNCTION            0
          
           37          76 PRECALL                  0
                       80 CALL                     0
          
           38          90 STORE_NAME               9 (changed_fields)
          
-          41          92 LOAD_CONST               7 (<code object get_field_diff, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py", line 41>)
+          41          92 LOAD_CONST               7 (<code object get_field_diff, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py", line 41>)
                       94 MAKE_FUNCTION            0
                       96 STORE_NAME              10 (get_field_diff)
          
-          47          98 LOAD_CONST               8 (<code object _dict, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py", line 47>)
+          47          98 LOAD_CONST               8 (<code object _dict, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py", line 47>)
                      100 MAKE_FUNCTION            0
                      102 STORE_NAME              11 (_dict)
                      104 LOAD_CONST               9 (None)
                      106 RETURN_VALUE
          consts
             'ModelDiffHelper'
             '\n    detects the changes after every operation used to log admin changes.\n    '
@@ -140,15 +140,15 @@
                             70 RETURN_VALUE
                consts
                   None
                names      ('_dict', '_ModelDiffHelper__initial', '_new_object')
                varnames   ('self', 'initial')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py'
                name       '__init__'
                firstlineno 13
                lnotab 0x02013401
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 3
@@ -183,15 +183,15 @@
                             88 RETURN_VALUE
                consts
                   None
                names      ('_dict', '_new_object', '_ModelDiffHelper__initial')
                varnames   ('self', 'new_object', 'data')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py'
                name       'set_changed_model'
                firstlineno 17
                lnotab 0x02012a010e010e010e01
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 3
@@ -219,15 +219,15 @@
                
                 29          36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                0 (_new_object)
                             48 STORE_DEREF              3 (d2)
                
                 30          50 LOAD_CLOSURE             3 (d2)
                             52 BUILD_TUPLE              1
-                            54 LOAD_CONST               1 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py", line 30>)
+                            54 LOAD_CONST               1 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py", line 30>)
                             56 MAKE_FUNCTION            8 (closure)
                             58 LOAD_FAST                1 (d1)
                             60 LOAD_METHOD              2 (items)
                             82 PRECALL                  0
                             86 CALL                     0
                             96 GET_ITER
                             98 PRECALL                  0
@@ -276,23 +276,23 @@
                                   66 JUMP_BACKWARD           30 (to 8)
                              >>   68 RETURN_VALUE
                      consts
                      names      ()
                      varnames   ('.0', 'k', 'v')
                      freevars   ('d2',)
                      cellvars   ()
-                     filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py'
+                     filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py'
                      name       '<listcomp>'
                      firstlineno 30
                      lnotab 0x
                names      ('_new_object', '_ModelDiffHelper__initial', 'items', 'dict')
                varnames   ('self', 'd1', 'diffs')
                freevars   ()
                cellvars   ('d2',)
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py'
                name       'diff'
                firstlineno 24
                lnotab 0x04020e0104010e010e014001
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
@@ -310,15 +310,15 @@
                             40 RETURN_VALUE
                consts
                   None
                names      ('bool', 'diff')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py'
                name       'has_changed'
                firstlineno 33
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
@@ -340,15 +340,15 @@
                             76 RETURN_VALUE
                consts
                   None
                names      ('list', 'diff', 'keys')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py'
                name       'changed_fields'
                firstlineno 37
                lnotab 0x0202
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
@@ -369,15 +369,15 @@
                consts
                   "\n        Returns a diff for field if it's changed and None otherwise.\n        "
                   None
                names      ('diff', 'get')
                varnames   ('self', 'field_name')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py'
                name       'get_field_diff'
                firstlineno 41
                lnotab 0x0204
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 5
@@ -386,15 +386,15 @@
                   0x97007401000000000000000000007c01640184007c016a010000000000
                   0000006a0200000000000000004400a6000000ab000000000000000000ac
                   02a6020000ab0200000000000000005300
                 47           0 RESUME                   0
                
                 48           2 LOAD_GLOBAL              1 (NULL + model_to_dict)
                             14 LOAD_FAST                1 (model)
-                            16 LOAD_CONST               1 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py", line 48>)
+                            16 LOAD_CONST               1 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py", line 48>)
                             18 MAKE_FUNCTION            0
                
                 49          20 LOAD_FAST                1 (model)
                             22 LOAD_ATTR                1 (_meta)
                             32 LOAD_ATTR                2 (fields)
                
                 48          42 GET_ITER
@@ -423,41 +423,41 @@
                                   24 JUMP_BACKWARD           10 (to 6)
                              >>   26 RETURN_VALUE
                      consts
                      names      ('name',)
                      varnames   ('.0', 'field')
                      freevars   ()
                      cellvars   ()
-                     filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py'
+                     filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py'
                      name       '<listcomp>'
                      firstlineno 48
                      lnotab 0x
                   ('fields',)
                names      ('model_to_dict', '_meta', 'fields')
                varnames   ('self', 'model')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py'
                name       '_dict'
                firstlineno 47
                lnotab 0x0201120116ff
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', 'set_changed_model', 'property', 'diff', 'has_changed', 'changed_fields', 'get_field_diff', '_dict')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py'
          name       'ModelDiffHelper'
          firstlineno 8
          lnotab
             0x0a01040406040607020104ff0e010208020104ff0e010203020104ff0e
             0102030606
       'ModelDiffHelper'
       None
    names      ('__doc__', 'django.forms', 'model_to_dict', 'django.utils.translation', 'gettext_lazy', '_', 'object', 'ModelDiffHelper')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/classes.py'
+   filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/classes.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff020104030c010c03
```

### Comparing `django-api-admin-1.1.4/django_api_admin/declarations/__pycache__/functions.cpython-311.pyc` & `django-api-admin-1.1.5/django_api_admin/declarations/__pycache__/functions.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5104b264 (Sat Jul 15 02:28:33 2023 UTC)
+moddate:  0xa8f0b264 (Sat Jul 15 19:16:56 2023 UTC)
 files sz: 13151
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
@@ -70,50 +70,50 @@
     13          90 LOAD_CONST               1 (0)
                 92 LOAD_CONST               9 (('field_attributes',))
                 94 IMPORT_NAME             16 (django_api_admin.field_attributes)
                 96 IMPORT_FROM             17 (field_attributes)
                 98 STORE_NAME              17 (field_attributes)
                100 POP_TOP
    
-    16         102 LOAD_CONST              10 (<code object get_field_attributes, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py", line 16>)
+    16         102 LOAD_CONST              10 (<code object get_field_attributes, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py", line 16>)
                104 MAKE_FUNCTION            0
                106 STORE_NAME              18 (get_field_attributes)
    
     64         108 LOAD_CONST              22 ((False,))
-               110 LOAD_CONST              12 (<code object get_form_fields, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py", line 64>)
+               110 LOAD_CONST              12 (<code object get_form_fields, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py", line 64>)
                112 MAKE_FUNCTION            1 (defaults)
                114 STORE_NAME              19 (get_form_fields)
    
    103         116 LOAD_CONST              23 ((None,))
-               118 LOAD_CONST              14 (<code object get_inlines, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py", line 103>)
+               118 LOAD_CONST              14 (<code object get_inlines, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py", line 103>)
                120 MAKE_FUNCTION            1 (defaults)
                122 STORE_NAME              20 (get_inlines)
    
-   147         124 LOAD_CONST              15 (<code object remove_field, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py", line 147>)
+   147         124 LOAD_CONST              15 (<code object remove_field, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py", line 147>)
                126 MAKE_FUNCTION            0
                128 STORE_NAME              21 (remove_field)
    
-   158         130 LOAD_CONST              16 (<code object get_form_config, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py", line 158>)
+   158         130 LOAD_CONST              16 (<code object get_form_config, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py", line 158>)
                132 MAKE_FUNCTION            0
                134 STORE_NAME              22 (get_form_config)
    
-   170         136 LOAD_CONST              17 (<code object validate_inline_field_names, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py", line 170>)
+   170         136 LOAD_CONST              17 (<code object validate_inline_field_names, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py", line 170>)
                138 MAKE_FUNCTION            0
                140 STORE_NAME              23 (validate_inline_field_names)
    
-   192         142 LOAD_CONST              18 (<code object get_inline_by_field_name, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py", line 192>)
+   192         142 LOAD_CONST              18 (<code object get_inline_by_field_name, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py", line 192>)
                144 MAKE_FUNCTION            0
                146 STORE_NAME              24 (get_inline_by_field_name)
    
    203         148 LOAD_CONST              24 (('create_inlines',))
-               150 LOAD_CONST              20 (<code object validate_bulk_edits, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py", line 203>)
+               150 LOAD_CONST              20 (<code object validate_bulk_edits, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py", line 203>)
                152 MAKE_FUNCTION            1 (defaults)
                154 STORE_NAME              25 (validate_bulk_edits)
    
-   299         156 LOAD_CONST              21 (<code object get_related_name, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py", line 299>)
+   299         156 LOAD_CONST              21 (<code object get_related_name, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py", line 299>)
                158 MAKE_FUNCTION            0
                160 STORE_NAME              26 (get_related_name)
                162 LOAD_CONST              13 (None)
                164 RETURN_VALUE
    consts
       '\nShared miscellaneous functions.\n'
       0
@@ -434,15 +434,15 @@
             'TimeField'
             'attrs'
             'current_value'
          names      ('type', '__name__', 'field_attributes', 'getattr', 'callable', 'humanize_datetime', 'date_formats', 'split', 'datetime_formats', 'time_formats', 'data', 'get', 'isinstance', 'Model', 'pk')
          varnames   ('name', 'field', 'change', 'serializer', 'form_field', 'attr_name', 'attr', 'value', 'current_value')
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py'
          name       'get_field_attributes'
          firstlineno 16
          lnotab
             0x020730022c01220236010c0102ff0e010cff0c0102ff06031e011a040e
             01300202ff3e0102ff10014eff0402300202ff3e0102ff10014eff040230
             0202ff3e0102ff10014eff040404021a02040134022a010e021602
       False
@@ -661,15 +661,15 @@
             'child'
             None
             ()
          names      ('list', 'fields', 'items', 'read_only', 'type', '__name__', 'serializers', 'ModelField', 'get_field_kwargs', 'model_field', 'verbose_name', 'pop', 'ModelSerializer', 'serializer_field_mapping', '__class__', 'get_field_attributes', 'ListField', 'DictField', 'HStoreField', '_UnvalidatedField', 'child', 'field_name', 'get', 'append')
          varnames   ('serializer', 'change', 'form_fields', 'name', 'field', 'field_kwargs', 'form_field')
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py'
          name       'get_form_fields'
          firstlineno 64
          lnotab
             0x02051c033e024c053a010c0122ff10022a01440102ff06030c0108ff10
             04ac012e01020102fe2404600116022e02
       None
       code
@@ -904,15 +904,15 @@
             ('pk', 'fields')
             'fieldsets'
             'fields'
          names      ('get_inline_instances', 'get_serializer_class', '_get_foreign_key', 'parent_model', 'model', 'fk_name', '_meta', 'verbose_name_plural', 'verbose_name', 'app_label', 'model_name', 'get_form_config', 'name', 'getattr', 'get_related_name', 'all', 'get_form_fields', 'remove_field', 'append', 'pk')
          varnames   ('request', 'model_admin', 'obj', 'inlines', 'inline_admin', 'serializer_class', 'fk', 'inline', 'fk_field', 'related_instances', 'fieldsets', 'instance', 'serializer', 'fields')
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py'
          name       'get_inlines'
          firstlineno 103
          lnotab
             0x0204040234012a01180118ff12042001200174011c010cfb060804023c
             01280104010801180122012a013c010c0314011e022a010a032e02
       code
          argcount  : 2
@@ -952,15 +952,15 @@
          consts
             '\n    removes a field from a list of fields generated by\n    get_form_fields\n    '
             'name'
          names      ('enumerate',)
          varnames   ('fields', 'name', 'idx', 'field')
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py'
          name       'remove_field'
          firstlineno 147
          lnotab 0x0205280118010801
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
@@ -998,15 +998,15 @@
          consts
             '\n    get model admin form attributes.\n    '
             None
          names      ('form_options', 'getattr')
          varnames   ('model_admin', 'config', 'option_name')
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py'
          name       'get_form_config'
          firstlineno 158
          lnotab 0x0204040112010c0106ff1803
       code
          argcount  : 3
          nlocals   : 7
          stacksize : 4
@@ -1105,15 +1105,15 @@
             'there is no inline admin with this name in model admin'
             0
             'inline_errors'
          names      ('get_inline_instances', 'append', 'model', '_meta', 'verbose_name_plural', 'keys', '_', 'len', 'serializers', 'ValidationError')
          varnames   ('request', 'inlines', 'model_admin', 'inline_admin_field_names', 'inline_admin', 'name_errors', 'inline_name')
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py'
          name       'validate_inline_field_names'
          firstlineno 170
          lnotab 0x020504013201180120ff120404012c0108021cff0c0426012cff
       code
          argcount  : 3
          nlocals   : 5
          stacksize : 4
@@ -1157,15 +1157,15 @@
             '\n    extract the InlineModelAdmin from the ModelAdmin based on the name of the InlineModelAdmin\n    '
             None
             ('obj',)
          names      ('get_inline_instances', 'model', '_meta', 'verbose_name_plural')
          varnames   ('request', 'model_admin', 'inline_name', 'inline_admin', 'inline_instance')
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py'
          name       'get_inline_by_field_name'
          firstlineno 192
          lnotab 0x0204040132012a010601
       'create_inlines'
       code
          argcount  : 4
          nlocals   : 22
@@ -1313,15 +1313,15 @@
                      382 PRECALL                  1
                      386 CALL                     1
                      396 LOAD_CONST               2 (None)
                      398 PRECALL                  3
                      402 CALL                     3
                      412 STORE_FAST              11 (fk_field)
          
-         229         414 LOAD_CONST               4 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py", line 229>)
+         229         414 LOAD_CONST               4 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py", line 229>)
                      416 MAKE_FUNCTION            0
                      418 LOAD_FAST                7 (inline_datasets)
                      420 GET_ITER
                      422 PRECALL                  0
                      426 CALL                     0
                      436 STORE_FAST              13 (primary_keys)
          
@@ -1378,15 +1378,15 @@
                      694 LOAD_CONST              10 ('delete_inlines')
                      696 COMPARE_OP               2 (==)
                      702 POP_JUMP_FORWARD_IF_FALSE   220 (to 1144)
          
          243         704 BUILD_LIST               0
                      706 STORE_FAST              14 (deleted_instances)
          
-         245         708 LOAD_CONST              11 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py", line 245>)
+         245         708 LOAD_CONST              11 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py", line 245>)
                      710 MAKE_FUNCTION            0
          
          246         712 LOAD_FAST                7 (inline_datasets)
          
          245         714 GET_ITER
                      716 PRECALL                  0
                      720 CALL                     0
@@ -1618,15 +1618,15 @@
                        >>   28 RETURN_VALUE
                consts
                   'pk'
                names      ()
                varnames   ('.0', 'dataset')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py'
                name       '<listcomp>'
                firstlineno 229
                lnotab 0x
             ('pk__in',)
             0
             'error'
             "you did't include any inline that is related to this model"
@@ -1655,29 +1655,29 @@
                        >>   28 RETURN_VALUE
                consts
                   'pk'
                names      ()
                varnames   ('.0', 'inline_dataset')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py'
                name       '<listcomp>'
                firstlineno 245
                lnotab 0x080110ff
             "you can't delete an inline that is not related to this model"
             True
             ('data', 'partial')
             ('data',)
             ('errors', 'identifier')
             'inline_errors'
          names      ('validate_inline_field_names', 'data', 'get', 'items', 'get_inline_by_field_name', '_get_foreign_key', 'parent_model', 'model', 'fk_name', 'get_serializer_class', 'getattr', 'get_related_name', 'filter', 'count', 'serializers', 'ValidationError', 'len', 'objects', 'append', 'enumerate', 'pk', 'name', 'is_valid', 'errors')
          varnames   ('request', 'model_admin', 'obj', 'operation', 'valid_serializers', 'serializer_errors', 'inline_name', 'inline_datasets', 'inline_admin', 'fk', 'inline_serializer_class', 'fk_field', 'instances', 'primary_keys', 'deleted_instances', 'serializer_class', 'instance', 'serializer', 'idx', 'inline_dataset', 'data', 'inline_serializer')
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py'
          name       'validate_bulk_edits'
          firstlineno 203
          lnotab
             0x02050c0136ff10040401040164020c0106ff1003180118ff12022a0404
             0104010c013c0118012c033001160106ff10034a01160106ff10040c0104
             02040102ff12032c0102ff12033001160106ff10034a01160106ff10042a
             010801160136020c03280104021e0304010c021001040106ff1404180228
@@ -1711,24 +1711,24 @@
          consts
             '\n    returns the name used to link the foreign key relationship.\n    '
             '_set'
          names      ('_related_name', 'model', '_meta', 'model_name')
          varnames   ('fk',)
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py'
          name       'get_related_name'
          firstlineno 299
          lnotab 0x02040e010e01
       (False,)
       (None,)
       ('create_inlines',)
    names      ('__doc__', 'django.db.models', 'Model', 'django.utils.translation', 'gettext_lazy', '_', 'django.forms.models', '_get_foreign_key', 'rest_framework', 'serializers', 'rest_framework.fields', '_UnvalidatedField', 'rest_framework.utils', 'humanize_datetime', 'rest_framework.utils.field_mapping', 'get_field_kwargs', 'django_api_admin.field_attributes', 'field_attributes', 'get_field_attributes', 'get_form_fields', 'get_inlines', 'remove_field', 'get_form_config', 'validate_inline_field_names', 'get_inline_by_field_name', 'validate_bulk_edits', 'get_related_name')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/declarations/functions.py'
+   filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/declarations/functions.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020104030c010c010c020c010c010c010c020c0306300827082c06
       0b060c0616060b0860
```

### Comparing `django-api-admin-1.1.4/django_api_admin/declarations/classes.py` & `django-api-admin-1.1.5/django_api_admin/declarations/classes.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.4/django_api_admin/declarations/functions.py` & `django-api-admin-1.1.5/django_api_admin/declarations/functions.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.4/django_api_admin/field_attributes.py` & `django-api-admin-1.1.5/django_api_admin/field_attributes.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.4/django_api_admin/migrations/__pycache__/0001_initial.cpython-311.pyc` & `django-api-admin-1.1.5/django_api_admin/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5105b264 (Sat Jul 15 02:32:49 2023 UTC)
+moddate:  0xdcf0b264 (Sat Jul 15 19:17:48 2023 UTC)
 files sz: 2463
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
@@ -31,15 +31,15 @@
      5          30 LOAD_CONST               0 (0)
                 32 LOAD_CONST               3 (None)
                 34 IMPORT_NAME              5 (django.db.models.deletion)
                 36 STORE_NAME               6 (django)
    
      8          38 PUSH_NULL
                 40 LOAD_BUILD_CLASS
-                42 LOAD_CONST               4 (<code object Migration, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/migrations/0001_initial.py", line 8>)
+                42 LOAD_CONST               4 (<code object Migration, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/migrations/0001_initial.py", line 8>)
                 44 MAKE_FUNCTION            0
                 46 LOAD_CONST               5 ('Migration')
                 48 LOAD_NAME                3 (migrations)
                 50 LOAD_ATTR                7 (Migration)
                 60 PRECALL                  3
                 64 CALL                     3
                 74 STORE_NAME               7 (Migration)
@@ -415,24 +415,24 @@
             ('model_name', 'name', 'field')
             'user'
             None
          names      ('__name__', '__module__', '__qualname__', 'initial', 'migrations', 'swappable_dependency', 'settings', 'AUTH_USER_MODEL', 'dependencies', 'CreateModel', 'models', 'BigAutoField', 'CharField', 'IntegerField', 'BooleanField', 'DateTimeField', 'DateField', 'ForeignKey', 'django', 'db', 'deletion', 'CASCADE', 'ManyToManyField', 'AddField', 'operations')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/migrations/0001_initial.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/migrations/0001_initial.py'
          name       'Migration'
          firstlineno 8
          lnotab
             0x0a02040328ff04050e0102022a012401280124012401240126f902fe10
             0c0e0102022a0120fe02fe10070e0102022a0124fe02fe10070e0102022a
             0124014e0126fc02fe10090e010201020120fd10050e010201020154fd10
             d7
       'Migration'
    names      ('django.conf', 'settings', 'django.db', 'migrations', 'models', 'django.db.models.deletion', 'django', 'Migration')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/migrations/0001_initial.py'
+   filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/migrations/0001_initial.py'
    name       '<module>'
    firstlineno 1
    lnotab 0x00ff02030c0110010803
```

### Comparing `django-api-admin-1.1.4/django_api_admin/options.py` & `django-api-admin-1.1.5/django_api_admin/options.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.4/django_api_admin/pagination.py` & `django-api-admin-1.1.5/django_api_admin/pagination.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.4/django_api_admin/serializers.py` & `django-api-admin-1.1.5/django_api_admin/serializers.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.4/django_api_admin/sites.py` & `django-api-admin-1.1.5/django_api_admin/sites.py`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.4/django_api_admin/views/__pycache__/admin_views.cpython-311.pyc` & `django-api-admin-1.1.5/django_api_admin/views/__pycache__/admin_views.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x5104b264 (Sat Jul 15 02:28:33 2023 UTC)
-files sz: 26075
+moddate:  0xcff1b264 (Sat Jul 15 19:21:51 2023 UTC)
+files sz: 25925
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x970064005a00640164026c016d025a020100640164036c036d045a0401
@@ -141,85 +141,85 @@
                202 STORE_NAME              37 (validate_bulk_edits)
                204 IMPORT_FROM             38 (get_inlines)
                206 STORE_NAME              38 (get_inlines)
                208 POP_TOP
    
     27         210 PUSH_NULL
                212 LOAD_BUILD_CLASS
-               214 LOAD_CONST              16 (<code object ListView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 27>)
+               214 LOAD_CONST              16 (<code object ListView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 27>)
                216 MAKE_FUNCTION            0
                218 LOAD_CONST              17 ('ListView')
                220 LOAD_NAME               24 (APIView)
                222 PRECALL                  3
                226 CALL                     3
                236 STORE_NAME              39 (ListView)
    
-    56         238 PUSH_NULL
+    55         238 PUSH_NULL
                240 LOAD_BUILD_CLASS
-               242 LOAD_CONST              18 (<code object DetailView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 56>)
+               242 LOAD_CONST              18 (<code object DetailView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 55>)
                244 MAKE_FUNCTION            0
                246 LOAD_CONST              19 ('DetailView')
                248 LOAD_NAME               24 (APIView)
                250 PRECALL                  3
                254 CALL                     3
                264 STORE_NAME              40 (DetailView)
    
-   104         266 PUSH_NULL
+   103         266 PUSH_NULL
                268 LOAD_BUILD_CLASS
-               270 LOAD_CONST              20 (<code object AddView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 104>)
+               270 LOAD_CONST              20 (<code object AddView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 103>)
                272 MAKE_FUNCTION            0
                274 LOAD_CONST              21 ('AddView')
                276 LOAD_NAME               24 (APIView)
                278 PRECALL                  3
                282 CALL                     3
                292 STORE_NAME              41 (AddView)
    
-   193         294 PUSH_NULL
+   192         294 PUSH_NULL
                296 LOAD_BUILD_CLASS
-               298 LOAD_CONST              22 (<code object ChangeView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 193>)
+               298 LOAD_CONST              22 (<code object ChangeView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 192>)
                300 MAKE_FUNCTION            0
                302 LOAD_CONST              23 ('ChangeView')
                304 LOAD_NAME               24 (APIView)
                306 PRECALL                  3
                310 CALL                     3
                320 STORE_NAME              42 (ChangeView)
    
-   358         322 PUSH_NULL
+   357         322 PUSH_NULL
                324 LOAD_BUILD_CLASS
-               326 LOAD_CONST              24 (<code object DeleteView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 358>)
+               326 LOAD_CONST              24 (<code object DeleteView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 357>)
                328 MAKE_FUNCTION            0
                330 LOAD_CONST              25 ('DeleteView')
                332 LOAD_NAME               24 (APIView)
                334 PRECALL                  3
                338 CALL                     3
                348 STORE_NAME              43 (DeleteView)
    
-   402         350 PUSH_NULL
+   401         350 PUSH_NULL
                352 LOAD_BUILD_CLASS
-               354 LOAD_CONST              26 (<code object ChangeListView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 402>)
+               354 LOAD_CONST              26 (<code object ChangeListView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 401>)
                356 MAKE_FUNCTION            0
                358 LOAD_CONST              27 ('ChangeListView')
                360 LOAD_NAME               24 (APIView)
                362 PRECALL                  3
                366 CALL                     3
                376 STORE_NAME              44 (ChangeListView)
    
-   589         378 PUSH_NULL
+   588         378 PUSH_NULL
                380 LOAD_BUILD_CLASS
-               382 LOAD_CONST              28 (<code object HandleActionView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 589>)
+               382 LOAD_CONST              28 (<code object HandleActionView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 588>)
                384 MAKE_FUNCTION            0
                386 LOAD_CONST              29 ('HandleActionView')
                388 LOAD_NAME               24 (APIView)
                390 PRECALL                  3
                394 CALL                     3
                404 STORE_NAME              45 (HandleActionView)
    
-   646         406 PUSH_NULL
+   645         406 PUSH_NULL
                408 LOAD_BUILD_CLASS
-               410 LOAD_CONST              30 (<code object HistoryView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 646>)
+               410 LOAD_CONST              30 (<code object HistoryView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 645>)
                412 MAKE_FUNCTION            0
                414 LOAD_CONST              31 ('HistoryView')
                416 LOAD_NAME               24 (APIView)
                418 PRECALL                  3
                422 CALL                     3
                432 STORE_NAME              46 (HistoryView)
                434 LOAD_CONST              32 (None)
@@ -260,47 +260,46 @@
          
           32          14 LOAD_CONST               2 (None)
                       16 STORE_NAME               4 (serializer_class)
          
           33          18 BUILD_LIST               0
                       20 STORE_NAME               5 (permission_classes)
          
-          35          22 LOAD_CONST               3 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 35>)
+          35          22 LOAD_CONST               3 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 35>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               6 (get)
                       28 LOAD_CONST               2 (None)
                       30 RETURN_VALUE
          consts
             'ListView'
             '\n    Return a list containing all instances of this model.\n    '
             None
             code
                argcount  : 3
-               nlocals   : 13
+               nlocals   : 12
                stacksize : 9
                flags     : 3
                code
                   0x97007c02a00000000000000000000000000000000000000000007c01a6
                   010000ab0100000000000000007d037c026a010000000000000000a00200
                   000000000000000000000000000000000000007c037c017c00ac01a60300
                   00ab0300000000000000007d047c00a00300000000000000000000000000
                   000000000000007c046402ac03a6020000ab0200000000000000007d057c
                   056a0400000000000000007d067c026a0100000000000000006a05000000
                   00000000007c026a0600000000000000006a0700000000000000006a0800
                   000000000000007c026a0600000000000000006a0700000000000000006a
                   09000000000000000066037d0764047d087c01a00a000000000000000000
                   0000000000000000000000a6000000ab0000000000000000007d097c01a0
                   0b0000000000000000000000000000000000000000a6000000ab00000000
-                  0000000000720264056e0164067d0a7c0644005d377d0b74190000000000
+                  0000000000720264056e0164067d0a7c0644005d2f7d0b74190000000000
                   00000000007c087c077a0600006407741b000000000000000000007c0b64
                   0819000000000000000000a6010000ab01000000000000000069017c01ac
-                  09a6030000ab0300000000000000007d0c7c0a7c097a0000007c0c7a0000
-                  007c0b640a3c0000008c38741d000000000000000000007c06741e000000
-                  000000000000006a100000000000000000ac0ba6020000ab020000000000
-                  0000005300
+                  09a6030000ab0300000000000000007c0b640a3c0000008c30741d000000
+                  000000000000007c06741e000000000000000000006a1000000000000000
+                  00ac0ba6020000ab0200000000000000005300
                 35           0 RESUME                   0
                
                 36           2 LOAD_FAST                2 (admin)
                              4 LOAD_METHOD              0 (get_queryset)
                             26 LOAD_FAST                1 (request)
                             28 PRECALL                  1
                             32 CALL                     1
@@ -364,15 +363,15 @@
                            336 LOAD_CONST               5 ('https://')
                            338 JUMP_FORWARD             1 (to 342)
                        >>  340 LOAD_CONST               6 ('http://')
                        >>  342 STORE_FAST              10 (scheme)
                
                 49         344 LOAD_FAST                6 (data)
                            346 GET_ITER
-                       >>  348 FOR_ITER                55 (to 460)
+                       >>  348 FOR_ITER                47 (to 444)
                            350 STORE_FAST              11 (item)
                
                 50         352 LOAD_GLOBAL             25 (NULL + reverse)
                            364 LOAD_FAST                8 (pattern)
                            366 LOAD_FAST                7 (info)
                            368 BINARY_OP                6 (%)
                
@@ -387,102 +386,95 @@
                 50         414 BUILD_MAP                1
                
                 51         416 LOAD_FAST                1 (request)
                
                 50         418 KW_NAMES                 9
                            420 PRECALL                  3
                            424 CALL                     3
-                           434 STORE_FAST              12 (path)
-               
-                52         436 LOAD_FAST               10 (scheme)
-                           438 LOAD_FAST                9 (domain)
-                           440 BINARY_OP                0 (+)
-                           444 LOAD_FAST               12 (path)
-                           446 BINARY_OP                0 (+)
-                           450 LOAD_FAST               11 (item)
-                           452 LOAD_CONST              10 ('detail_url')
-                           454 STORE_SUBSCR
-                           458 JUMP_BACKWARD           56 (to 348)
-               
-                53     >>  460 LOAD_GLOBAL             29 (NULL + Response)
-                           472 LOAD_FAST                6 (data)
-                           474 LOAD_GLOBAL             30 (status)
-                           486 LOAD_ATTR               16 (HTTP_200_OK)
-                           496 KW_NAMES                11
-                           498 PRECALL                  2
-                           502 CALL                     2
-                           512 RETURN_VALUE
+                           434 LOAD_FAST               11 (item)
+                           436 LOAD_CONST              10 ('detail_url')
+                           438 STORE_SUBSCR
+                           442 JUMP_BACKWARD           48 (to 348)
+               
+                52     >>  444 LOAD_GLOBAL             29 (NULL + Response)
+                           456 LOAD_FAST                6 (data)
+                           458 LOAD_GLOBAL             30 (status)
+                           470 LOAD_ATTR               16 (HTTP_200_OK)
+                           480 KW_NAMES                11
+                           482 PRECALL                  2
+                           486 CALL                     2
+                           496 RETURN_VALUE
                consts
                   None
                   ('view',)
                   True
                   ('many',)
                   '%s:%s_%s_detail'
                   'https://'
                   'http://'
                   'object_id'
                   'pk'
                   ('kwargs', 'request')
                   'detail_url'
                   ('status',)
                names      ('get_queryset', 'admin_site', 'paginate_queryset', 'serializer_class', 'data', 'name', 'model', '_meta', 'app_label', 'model_name', 'get_host', 'is_secure', 'reverse', 'int', 'Response', 'status', 'HTTP_200_OK')
-               varnames   ('self', 'request', 'admin', 'queryset', 'page', 'serializer', 'data', 'info', 'pattern', 'domain', 'scheme', 'item', 'path')
+               varnames   ('self', 'request', 'admin', 'queryset', 'page', 'serializer', 'data', 'info', 'pattern', 'domain', 'scheme', 'item')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'get'
                firstlineno 35
                lnotab
                   0x02012a013a012e010e021601200120fd0405040228013001080114012a
-                  ff020102ff12021801
+                  ff020102ff1a02
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'serializer_class', 'permission_classes', 'get')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
          name       'ListView'
          firstlineno 27
          lnotab 0x0a01040404010402
       'ListView'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0367005a0464025a05640384005a0664
             025300
-          56           0 RESUME                   0
+          55           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DetailView')
                        8 STORE_NAME               2 (__qualname__)
          
-          57          10 LOAD_CONST               1 ('\n    GET one instance of this model using pk and to_fields.\n    ')
+          56          10 LOAD_CONST               1 ('\n    GET one instance of this model using pk and to_fields.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-          60          14 BUILD_LIST               0
+          59          14 BUILD_LIST               0
                       16 STORE_NAME               4 (permission_classes)
          
-          61          18 LOAD_CONST               2 (None)
+          60          18 LOAD_CONST               2 (None)
                       20 STORE_NAME               5 (serializer_class)
          
-          63          22 LOAD_CONST               3 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 63>)
+          62          22 LOAD_CONST               3 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 62>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               6 (get)
                       28 LOAD_CONST               2 (None)
                       30 RETURN_VALUE
          consts
             'DetailView'
             '\n    GET one instance of this model using pk and to_fields.\n    '
             None
             code
                argcount  : 4
                nlocals   : 14
-               stacksize : 7
+               stacksize : 6
                flags     : 3
                code
                   0x97007c016a000000000000000000a00100000000000000000000000000
                   00000000000000740400000000000000000000a6010000ab010000000000
                   0000007d047c0472367c03a0030000000000000000000000000000000000
                   0000007c017c04a6020000ab020000000000000000732074090000000000
                   0000000000640164027c047a0600006901740a000000000000000000006a
@@ -501,298 +493,276 @@
                   1200000000000000007c036a0a00000000000000006a0b00000000000000
                   006a13000000000000000066037d0964067d0a7c01a01400000000000000
                   00000000000000000000000000a6000000ab0000000000000000007d0b7c
                   01a0150000000000000000000000000000000000000000a6000000ab0000
                   00000000000000720264076e0164087d0c7c036a16000000000000000072
                   25742e000000000000000000006a180000000000000000a0190000000000
                   0000000000000000000000000000007c036a0a0000000000000000ac09a6
-                  010000ab0100000000000000007d0d7c0c7c0b7a00000074350000000000
-                  0000000000640a7c036a1000000000000000006a1100000000000000007a
-                  0600007c0d6a1b00000000000000007c056a1b0000000000000000640b9c
-                  027c01ac0ca6030000ab0300000000000000007a0000007c08640d3c0000
-                  007c0c7c0b7a0000007435000000000000000000007c0a640e7a0000007c
-                  097a0600007c01ac0fa6020000ab0200000000000000007a0000007c0864
-                  103c0000007c0c7c0b7a0000007435000000000000000000007c0a64117a
-                  0000007c097a06000064127c0864131900000000000000000069017c01ac
-                  0ca6030000ab0300000000000000007a0000007c0864143c0000007c0c7c
-                  0b7a0000007435000000000000000000007c0a64157a0000007c097a0600
-                  0064127c0864131900000000000000000069017c01ac0ca6030000ab0300
-                  000000000000007a0000007c0864163c0000007c0c7c0b7a000000743500
-                  0000000000000000007c0a64177a0000007c097a06000064127c08641319
-                  00000000000000000069017c01ac0ca6030000ab0300000000000000007a
+                  010000ab0100000000000000007d0d743500000000000000000000640a7c
+                  036a1000000000000000006a1100000000000000007a0600007c0d6a1b00
+                  000000000000007c056a1b0000000000000000640b9c027c01ac0ca60300
+                  00ab0300000000000000007c08640d3c0000007435000000000000000000
+                  007c0a640e7a0000007c097a0600007c01ac0fa6020000ab020000000000
+                  0000007c0864103c0000007435000000000000000000007c0a64117a0000
+                  007c097a06000064127c0864131900000000000000000069017c01ac0ca6
+                  030000ab0300000000000000007c0864143c000000743500000000000000
+                  0000007c0a64157a0000007c097a06000064127c08641319000000000000
+                  00000069017c01ac0ca6030000ab0300000000000000007c0864163c0000
+                  007435000000000000000000007c0a64177a0000007c097a06000064127c
+                  0864131900000000000000000069017c01ac0ca6030000ab030000000000
                   0000007c0864183c0000007409000000000000000000007c08740a000000
                   000000000000006a1c0000000000000000ac03a6020000ab020000000000
                   0000005300
-                63           0 RESUME                   0
+                62           0 RESUME                   0
                
-                65           2 LOAD_FAST                1 (request)
+                64           2 LOAD_FAST                1 (request)
                              4 LOAD_ATTR                0 (query_params)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_GLOBAL              4 (TO_FIELD_VAR)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               4 (to_field)
                
-                66          64 LOAD_FAST                4 (to_field)
+                65          64 LOAD_FAST                4 (to_field)
                             66 POP_JUMP_FORWARD_IF_FALSE    54 (to 176)
                             68 LOAD_FAST                3 (admin)
                             70 LOAD_METHOD              3 (to_field_allowed)
                             92 LOAD_FAST                1 (request)
                             94 LOAD_FAST                4 (to_field)
                             96 PRECALL                  2
                            100 CALL                     2
                            110 POP_JUMP_FORWARD_IF_TRUE    32 (to 176)
                
-                67         112 LOAD_GLOBAL              9 (NULL + Response)
+                66         112 LOAD_GLOBAL              9 (NULL + Response)
                            124 LOAD_CONST               1 ('detail')
                            126 LOAD_CONST               2 ('The field %s cannot be referenced.')
                            128 LOAD_FAST                4 (to_field)
                            130 BINARY_OP                6 (%)
                            134 BUILD_MAP                1
                
-                68         136 LOAD_GLOBAL             10 (status)
+                67         136 LOAD_GLOBAL             10 (status)
                            148 LOAD_ATTR                6 (HTTP_400_BAD_REQUEST)
                
-                67         158 KW_NAMES                 3
+                66         158 KW_NAMES                 3
                            160 PRECALL                  2
                            164 CALL                     2
                            174 RETURN_VALUE
                
-                69     >>  176 LOAD_FAST                3 (admin)
+                68     >>  176 LOAD_FAST                3 (admin)
                            178 LOAD_METHOD              7 (get_object)
                            200 LOAD_FAST                1 (request)
                            202 LOAD_GLOBAL             17 (NULL + unquote)
                            214 LOAD_FAST                2 (object_id)
                            216 PRECALL                  1
                            220 CALL                     1
                            230 LOAD_FAST                4 (to_field)
                            232 PRECALL                  3
                            236 CALL                     3
                            246 STORE_FAST               5 (obj)
                
-                72         248 LOAD_FAST                5 (obj)
+                71         248 LOAD_FAST                5 (obj)
                            250 POP_JUMP_FORWARD_IF_NOT_NONE    78 (to 408)
                
-                73         252 LOAD_GLOBAL             19 (NULL + _)
+                72         252 LOAD_GLOBAL             19 (NULL + _)
                            264 LOAD_CONST               4 ("%(name)s with ID “%(key)s” doesn't exist. Perhaps it was deleted?")
                            266 PRECALL                  1
                            270 CALL                     1
                
-                74         280 LOAD_FAST                3 (admin)
+                73         280 LOAD_FAST                3 (admin)
                            282 LOAD_ATTR               10 (model)
                            292 LOAD_ATTR               11 (_meta)
                            302 LOAD_ATTR               12 (verbose_name)
                
-                75         312 LOAD_GLOBAL             17 (NULL + unquote)
+                74         312 LOAD_GLOBAL             17 (NULL + unquote)
                            324 LOAD_FAST                2 (object_id)
                            326 PRECALL                  1
                            330 CALL                     1
                
-                73         340 LOAD_CONST               5 (('name', 'key'))
+                72         340 LOAD_CONST               5 (('name', 'key'))
                            342 BUILD_CONST_KEY_MAP      2
                            344 BINARY_OP                6 (%)
                            348 STORE_FAST               6 (msg)
                
-                77         350 LOAD_GLOBAL              9 (NULL + Response)
+                76         350 LOAD_GLOBAL              9 (NULL + Response)
                            362 LOAD_CONST               1 ('detail')
                            364 LOAD_FAST                6 (msg)
                            366 BUILD_MAP                1
                            368 LOAD_GLOBAL             10 (status)
                            380 LOAD_ATTR               13 (HTTP_404_NOT_FOUND)
                            390 KW_NAMES                 3
                            392 PRECALL                  2
                            396 CALL                     2
                            406 RETURN_VALUE
                
-                79     >>  408 LOAD_FAST                0 (self)
+                78     >>  408 LOAD_FAST                0 (self)
                            410 LOAD_METHOD             14 (serializer_class)
                            432 LOAD_FAST                5 (obj)
                            434 PRECALL                  1
                            438 CALL                     1
                            448 STORE_FAST               7 (serializer)
                
-                80         450 LOAD_FAST                7 (serializer)
+                79         450 LOAD_FAST                7 (serializer)
                            452 LOAD_ATTR               15 (data)
                            462 STORE_FAST               8 (data)
                
-                84         464 LOAD_FAST                3 (admin)
+                83         464 LOAD_FAST                3 (admin)
                            466 LOAD_ATTR               16 (admin_site)
                            476 LOAD_ATTR               17 (name)
                
-                85         486 LOAD_FAST                3 (admin)
+                84         486 LOAD_FAST                3 (admin)
                            488 LOAD_ATTR               10 (model)
                            498 LOAD_ATTR               11 (_meta)
                            508 LOAD_ATTR               18 (app_label)
                
-                86         518 LOAD_FAST                3 (admin)
+                85         518 LOAD_FAST                3 (admin)
                            520 LOAD_ATTR               10 (model)
                            530 LOAD_ATTR               11 (_meta)
                            540 LOAD_ATTR               19 (model_name)
                
-                83         550 BUILD_TUPLE              3
+                82         550 BUILD_TUPLE              3
                            552 STORE_FAST               9 (info)
                
-                88         554 LOAD_CONST               6 ('%s:%s_%s_')
+                87         554 LOAD_CONST               6 ('%s:%s_%s_')
                            556 STORE_FAST              10 (pattern)
                
-                89         558 LOAD_FAST                1 (request)
+                88         558 LOAD_FAST                1 (request)
                            560 LOAD_METHOD             20 (get_host)
                            582 PRECALL                  0
                            586 CALL                     0
                            596 STORE_FAST              11 (domain)
                
-                90         598 LOAD_FAST                1 (request)
+                89         598 LOAD_FAST                1 (request)
                            600 LOAD_METHOD             21 (is_secure)
                            622 PRECALL                  0
                            626 CALL                     0
                            636 POP_JUMP_FORWARD_IF_FALSE     2 (to 642)
                            638 LOAD_CONST               7 ('https://')
                            640 JUMP_FORWARD             1 (to 644)
                        >>  642 LOAD_CONST               8 ('http://')
                        >>  644 STORE_FAST              12 (scheme)
                
-                91         646 LOAD_FAST                3 (admin)
+                90         646 LOAD_FAST                3 (admin)
                            648 LOAD_ATTR               22 (view_on_site)
                            658 POP_JUMP_FORWARD_IF_FALSE    37 (to 734)
                
-                92         660 LOAD_GLOBAL             46 (ContentType)
+                91         660 LOAD_GLOBAL             46 (ContentType)
                            672 LOAD_ATTR               24 (objects)
                            682 LOAD_METHOD             25 (get_for_model)
                
-                93         704 LOAD_FAST                3 (admin)
+                92         704 LOAD_FAST                3 (admin)
                            706 LOAD_ATTR               10 (model)
                
-                92         716 KW_NAMES                 9
+                91         716 KW_NAMES                 9
                            718 PRECALL                  1
                            722 CALL                     1
                            732 STORE_FAST              13 (model_type)
                
-                94     >>  734 LOAD_FAST               12 (scheme)
-                           736 LOAD_FAST               11 (domain)
-                           738 BINARY_OP                0 (+)
-                           742 LOAD_GLOBAL             53 (NULL + reverse)
-                           754 LOAD_CONST              10 ('%s:view_on_site')
-                           756 LOAD_FAST                3 (admin)
-                           758 LOAD_ATTR               16 (admin_site)
-                           768 LOAD_ATTR               17 (name)
-                           778 BINARY_OP                6 (%)
-                           782 LOAD_FAST               13 (model_type)
-                           784 LOAD_ATTR               27 (pk)
-                           794 LOAD_FAST                5 (obj)
-                           796 LOAD_ATTR               27 (pk)
-                           806 LOAD_CONST              11 (('content_type_id', 'object_id'))
-                           808 BUILD_CONST_KEY_MAP      2
-                           810 LOAD_FAST                1 (request)
-                           812 KW_NAMES                12
-                           814 PRECALL                  3
-                           818 CALL                     3
-                           828 BINARY_OP                0 (+)
-                           832 LOAD_FAST                8 (data)
-                           834 LOAD_CONST              13 ('view_on_site')
-                           836 STORE_SUBSCR
-               
-                95         840 LOAD_FAST               12 (scheme)
-                           842 LOAD_FAST               11 (domain)
+                93     >>  734 LOAD_GLOBAL             53 (NULL + reverse)
+                           746 LOAD_CONST              10 ('%s:view_on_site')
+                           748 LOAD_FAST                3 (admin)
+                           750 LOAD_ATTR               16 (admin_site)
+                           760 LOAD_ATTR               17 (name)
+                           770 BINARY_OP                6 (%)
+                           774 LOAD_FAST               13 (model_type)
+                           776 LOAD_ATTR               27 (pk)
+                           786 LOAD_FAST                5 (obj)
+                           788 LOAD_ATTR               27 (pk)
+                           798 LOAD_CONST              11 (('content_type_id', 'object_id'))
+                           800 BUILD_CONST_KEY_MAP      2
+                           802 LOAD_FAST                1 (request)
+                           804 KW_NAMES                12
+                           806 PRECALL                  3
+                           810 CALL                     3
+                           820 LOAD_FAST                8 (data)
+                           822 LOAD_CONST              13 ('view_on_site')
+                           824 STORE_SUBSCR
+               
+                94         828 LOAD_GLOBAL             53 (NULL + reverse)
+                           840 LOAD_FAST               10 (pattern)
+                           842 LOAD_CONST              14 ('list')
                            844 BINARY_OP                0 (+)
-                           848 LOAD_GLOBAL             53 (NULL + reverse)
-                           860 LOAD_FAST               10 (pattern)
-                           862 LOAD_CONST              14 ('list')
-                           864 BINARY_OP                0 (+)
-                           868 LOAD_FAST                9 (info)
-                           870 BINARY_OP                6 (%)
-                           874 LOAD_FAST                1 (request)
-                           876 KW_NAMES                15
-                           878 PRECALL                  2
-                           882 CALL                     2
-                           892 BINARY_OP                0 (+)
-                           896 LOAD_FAST                8 (data)
-                           898 LOAD_CONST              16 ('list_url')
-                           900 STORE_SUBSCR
-               
-                96         904 LOAD_FAST               12 (scheme)
-                           906 LOAD_FAST               11 (domain)
-                           908 BINARY_OP                0 (+)
-                           912 LOAD_GLOBAL             53 (NULL + reverse)
-                           924 LOAD_FAST               10 (pattern)
-                           926 LOAD_CONST              17 ('history')
-                           928 BINARY_OP                0 (+)
-                           932 LOAD_FAST                9 (info)
-                           934 BINARY_OP                6 (%)
-                           938 LOAD_CONST              18 ('object_id')
-                           940 LOAD_FAST                8 (data)
-                           942 LOAD_CONST              19 ('pk')
-                           944 BINARY_SUBSCR
-                           954 BUILD_MAP                1
-                           956 LOAD_FAST                1 (request)
-                           958 KW_NAMES                12
-                           960 PRECALL                  3
-                           964 CALL                     3
-                           974 BINARY_OP                0 (+)
+                           848 LOAD_FAST                9 (info)
+                           850 BINARY_OP                6 (%)
+                           854 LOAD_FAST                1 (request)
+                           856 KW_NAMES                15
+                           858 PRECALL                  2
+                           862 CALL                     2
+                           872 LOAD_FAST                8 (data)
+                           874 LOAD_CONST              16 ('list_url')
+                           876 STORE_SUBSCR
+               
+                95         880 LOAD_GLOBAL             53 (NULL + reverse)
+                           892 LOAD_FAST               10 (pattern)
+                           894 LOAD_CONST              17 ('history')
+                           896 BINARY_OP                0 (+)
+                           900 LOAD_FAST                9 (info)
+                           902 BINARY_OP                6 (%)
+                           906 LOAD_CONST              18 ('object_id')
+                           908 LOAD_FAST                8 (data)
+                           910 LOAD_CONST              19 ('pk')
+                           912 BINARY_SUBSCR
+                           922 BUILD_MAP                1
+                           924 LOAD_FAST                1 (request)
+                           926 KW_NAMES                12
+                           928 PRECALL                  3
+                           932 CALL                     3
+                           942 LOAD_FAST                8 (data)
+                           944 LOAD_CONST              20 ('history_url')
+                           946 STORE_SUBSCR
+               
+                96         950 LOAD_GLOBAL             53 (NULL + reverse)
+               
+                97         962 LOAD_FAST               10 (pattern)
+                           964 LOAD_CONST              21 ('delete')
+                           966 BINARY_OP                0 (+)
+                           970 LOAD_FAST                9 (info)
+                           972 BINARY_OP                6 (%)
+                           976 LOAD_CONST              18 ('object_id')
                            978 LOAD_FAST                8 (data)
-                           980 LOAD_CONST              20 ('history_url')
-                           982 STORE_SUBSCR
-               
-                97         986 LOAD_FAST               12 (scheme)
-                           988 LOAD_FAST               11 (domain)
-                           990 BINARY_OP                0 (+)
-                           994 LOAD_GLOBAL             53 (NULL + reverse)
-               
-                98        1006 LOAD_FAST               10 (pattern)
-                          1008 LOAD_CONST              21 ('delete')
-                          1010 BINARY_OP                0 (+)
-                          1014 LOAD_FAST                9 (info)
-                          1016 BINARY_OP                6 (%)
-                          1020 LOAD_CONST              18 ('object_id')
-                          1022 LOAD_FAST                8 (data)
-                          1024 LOAD_CONST              19 ('pk')
-                          1026 BINARY_SUBSCR
-                          1036 BUILD_MAP                1
-                          1038 LOAD_FAST                1 (request)
-               
-                97        1040 KW_NAMES                12
-                          1042 PRECALL                  3
-                          1046 CALL                     3
-                          1056 BINARY_OP                0 (+)
-                          1060 LOAD_FAST                8 (data)
-                          1062 LOAD_CONST              22 ('delete_url')
-                          1064 STORE_SUBSCR
-               
-                99        1068 LOAD_FAST               12 (scheme)
-                          1070 LOAD_FAST               11 (domain)
-                          1072 BINARY_OP                0 (+)
-                          1076 LOAD_GLOBAL             53 (NULL + reverse)
-               
-               100        1088 LOAD_FAST               10 (pattern)
-                          1090 LOAD_CONST              23 ('change')
-                          1092 BINARY_OP                0 (+)
-                          1096 LOAD_FAST                9 (info)
-                          1098 BINARY_OP                6 (%)
-                          1102 LOAD_CONST              18 ('object_id')
-                          1104 LOAD_FAST                8 (data)
-                          1106 LOAD_CONST              19 ('pk')
-                          1108 BINARY_SUBSCR
-                          1118 BUILD_MAP                1
-                          1120 LOAD_FAST                1 (request)
-               
-                99        1122 KW_NAMES                12
-                          1124 PRECALL                  3
-                          1128 CALL                     3
-                          1138 BINARY_OP                0 (+)
-                          1142 LOAD_FAST                8 (data)
-                          1144 LOAD_CONST              24 ('change_url')
-                          1146 STORE_SUBSCR
-               
-               101        1150 LOAD_GLOBAL              9 (NULL + Response)
-                          1162 LOAD_FAST                8 (data)
-                          1164 LOAD_GLOBAL             10 (status)
-                          1176 LOAD_ATTR               28 (HTTP_200_OK)
-                          1186 KW_NAMES                 3
-                          1188 PRECALL                  2
-                          1192 CALL                     2
-                          1202 RETURN_VALUE
+                           980 LOAD_CONST              19 ('pk')
+                           982 BINARY_SUBSCR
+                           992 BUILD_MAP                1
+                           994 LOAD_FAST                1 (request)
+               
+                96         996 KW_NAMES                12
+                           998 PRECALL                  3
+                          1002 CALL                     3
+                          1012 LOAD_FAST                8 (data)
+                          1014 LOAD_CONST              22 ('delete_url')
+                          1016 STORE_SUBSCR
+               
+                98        1020 LOAD_GLOBAL             53 (NULL + reverse)
+               
+                99        1032 LOAD_FAST               10 (pattern)
+                          1034 LOAD_CONST              23 ('change')
+                          1036 BINARY_OP                0 (+)
+                          1040 LOAD_FAST                9 (info)
+                          1042 BINARY_OP                6 (%)
+                          1046 LOAD_CONST              18 ('object_id')
+                          1048 LOAD_FAST                8 (data)
+                          1050 LOAD_CONST              19 ('pk')
+                          1052 BINARY_SUBSCR
+                          1062 BUILD_MAP                1
+                          1064 LOAD_FAST                1 (request)
+               
+                98        1066 KW_NAMES                12
+                          1068 PRECALL                  3
+                          1072 CALL                     3
+                          1082 LOAD_FAST                8 (data)
+                          1084 LOAD_CONST              24 ('change_url')
+                          1086 STORE_SUBSCR
+               
+               100        1090 LOAD_GLOBAL              9 (NULL + Response)
+                          1102 LOAD_FAST                8 (data)
+                          1104 LOAD_GLOBAL             10 (status)
+                          1116 LOAD_ATTR               28 (HTTP_200_OK)
+                          1126 KW_NAMES                 3
+                          1128 PRECALL                  2
+                          1132 CALL                     2
+                          1142 RETURN_VALUE
                consts
                   None
                   'detail'
                   'The field %s cannot be referenced.'
                   ('status',)
                   "%(name)s with ID “%(key)s” doesn't exist. Perhaps it was deleted?"
                   ('name', 'key')
@@ -815,68 +785,68 @@
                   'delete_url'
                   'change'
                   'change_url'
                names      ('query_params', 'get', 'TO_FIELD_VAR', 'to_field_allowed', 'Response', 'status', 'HTTP_400_BAD_REQUEST', 'get_object', 'unquote', '_', 'model', '_meta', 'verbose_name', 'HTTP_404_NOT_FOUND', 'serializer_class', 'data', 'admin_site', 'name', 'app_label', 'model_name', 'get_host', 'is_secure', 'view_on_site', 'ContentType', 'objects', 'get_for_model', 'reverse', 'pk', 'HTTP_200_OK')
                varnames   ('self', 'request', 'object_id', 'admin', 'to_field', 'obj', 'msg', 'serializer', 'data', 'info', 'pattern', 'domain', 'scheme', 'model_type')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'get'
-               firstlineno 63
+               firstlineno 62
                lnotab
                   0x02023e013001180116ff1202480304011c0120011cfe0a043a022a010e
-                  041601200120fd04050401280130010e012c010cff12026a014001520114
-                  0122ff1c02140122ff1c02
+                  041601200120fd04050401280130010e012c010cff12025e01340146010c
+                  0122ff18020c0122ff1802
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'permission_classes', 'serializer_class', 'get')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
          name       'DetailView'
-         firstlineno 56
+         firstlineno 55
          lnotab 0x0a01040304010402
       'DetailView'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0467005a05640384005a0665
             076a08000000000000000064048400a6000000ab0000000000000000005a
             0964025300
-         104           0 RESUME                   0
+         103           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AddView')
                        8 STORE_NAME               2 (__qualname__)
          
-         105          10 LOAD_CONST               1 ('\n    Add new instances of this model. if this model has inline models associated with it \n    you can also add inline instances to this model.\n\n    a request body should look like this:\n\n    {\n        "data": {\n            // the values to create new instance of the model\n            "name": "lorem ipsum"\n            ...\n        },\n        // the inline instances you want to create (optional)\n        "create_inlines": {\n            "books": [\n                {\n                    "title": "lorem ipsum"\n                    ...\n                },\n                {\n                    "title": "lorem ipsum"\n                    ...\n                },\n            ]\n        }\n    }\n    ')
+         104          10 LOAD_CONST               1 ('\n    Add new instances of this model. if this model has inline models associated with it \n    you can also add inline instances to this model.\n\n    a request body should look like this:\n\n    {\n        "data": {\n            // the values to create new instance of the model\n            "name": "lorem ipsum"\n            ...\n        },\n        // the inline instances you want to create (optional)\n        "create_inlines": {\n            "books": [\n                {\n                    "title": "lorem ipsum"\n                    ...\n                },\n                {\n                    "title": "lorem ipsum"\n                    ...\n                },\n            ]\n        }\n    }\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-         132          14 LOAD_CONST               2 (None)
+         131          14 LOAD_CONST               2 (None)
                       16 STORE_NAME               4 (serializer_class)
          
-         133          18 BUILD_LIST               0
+         132          18 BUILD_LIST               0
                       20 STORE_NAME               5 (permission_classes)
          
-         135          22 LOAD_CONST               3 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 135>)
+         134          22 LOAD_CONST               3 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 134>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               6 (get)
          
-         145          28 LOAD_NAME                7 (transaction)
+         144          28 LOAD_NAME                7 (transaction)
                       30 LOAD_ATTR                8 (atomic)
          
-         146          40 LOAD_CONST               4 (<code object post, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 145>)
+         145          40 LOAD_CONST               4 (<code object post, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 144>)
                       42 MAKE_FUNCTION            0
          
-         145          44 PRECALL                  0
+         144          44 PRECALL                  0
                       48 CALL                     0
          
-         146          58 STORE_NAME               9 (post)
+         145          58 STORE_NAME               9 (post)
                       60 LOAD_CONST               2 (None)
                       62 RETURN_VALUE
          consts
             'AddView'
             '\n    Add new instances of this model. if this model has inline models associated with it \n    you can also add inline instances to this model.\n\n    a request body should look like this:\n\n    {\n        "data": {\n            // the values to create new instance of the model\n            "name": "lorem ipsum"\n            ...\n        },\n        // the inline instances you want to create (optional)\n        "create_inlines": {\n            "books": [\n                {\n                    "title": "lorem ipsum"\n                    ...\n                },\n                {\n                    "title": "lorem ipsum"\n                    ...\n                },\n            ]\n        }\n    }\n    '
             None
             code
@@ -890,62 +860,62 @@
                   0000000000000000007d047405000000000000000000007c04a6010000ab
                   0100000000000000007c0364013c0000007407000000000000000000007c
                   02a6010000ab0100000000000000007c0364023c00000074090000000000
                   00000000007c017c02a6020000ab0200000000000000007d05740b000000
                   000000000000007c05a6010000ab01000000000000000072057c057c0364
                   033c000000740d000000000000000000007c03740e000000000000000000
                   006a080000000000000000ac04a6020000ab0200000000000000005300
-               135           0 RESUME                   0
+               134           0 RESUME                   0
                
-               136           2 LOAD_GLOBAL              1 (NULL + dict)
+               135           2 LOAD_GLOBAL              1 (NULL + dict)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 STORE_FAST               3 (data)
                
-               137          30 LOAD_FAST                0 (self)
+               136          30 LOAD_FAST                0 (self)
                             32 LOAD_METHOD              1 (serializer_class)
                             54 PRECALL                  0
                             58 CALL                     0
                             68 STORE_FAST               4 (serializer)
                
-               138          70 LOAD_GLOBAL              5 (NULL + get_form_fields)
+               137          70 LOAD_GLOBAL              5 (NULL + get_form_fields)
                             82 LOAD_FAST                4 (serializer)
                             84 PRECALL                  1
                             88 CALL                     1
                             98 LOAD_FAST                3 (data)
                            100 LOAD_CONST               1 ('fields')
                            102 STORE_SUBSCR
                
-               139         106 LOAD_GLOBAL              7 (NULL + get_form_config)
+               138         106 LOAD_GLOBAL              7 (NULL + get_form_config)
                            118 LOAD_FAST                2 (model_admin)
                            120 PRECALL                  1
                            124 CALL                     1
                            134 LOAD_FAST                3 (data)
                            136 LOAD_CONST               2 ('config')
                            138 STORE_SUBSCR
                
-               140         142 LOAD_GLOBAL              9 (NULL + get_inlines)
+               139         142 LOAD_GLOBAL              9 (NULL + get_inlines)
                            154 LOAD_FAST                1 (request)
                            156 LOAD_FAST                2 (model_admin)
                            158 PRECALL                  2
                            162 CALL                     2
                            172 STORE_FAST               5 (inlines)
                
-               141         174 LOAD_GLOBAL             11 (NULL + len)
+               140         174 LOAD_GLOBAL             11 (NULL + len)
                            186 LOAD_FAST                5 (inlines)
                            188 PRECALL                  1
                            192 CALL                     1
                            202 POP_JUMP_FORWARD_IF_FALSE     5 (to 214)
                
-               142         204 LOAD_FAST                5 (inlines)
+               141         204 LOAD_FAST                5 (inlines)
                            206 LOAD_FAST                3 (data)
                            208 LOAD_CONST               3 ('inlines')
                            210 STORE_SUBSCR
                
-               143     >>  214 LOAD_GLOBAL             13 (NULL + Response)
+               142     >>  214 LOAD_GLOBAL             13 (NULL + Response)
                            226 LOAD_FAST                3 (data)
                            228 LOAD_GLOBAL             14 (status)
                            240 LOAD_ATTR                8 (HTTP_200_OK)
                            250 KW_NAMES                 4
                            252 PRECALL                  2
                            256 CALL                     2
                            266 RETURN_VALUE
@@ -955,17 +925,17 @@
                   'config'
                   'inlines'
                   ('status',)
                names      ('dict', 'serializer_class', 'get_form_fields', 'get_form_config', 'get_inlines', 'len', 'Response', 'status', 'HTTP_200_OK')
                varnames   ('self', 'request', 'model_admin', 'data', 'serializer', 'inlines')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'get'
-               firstlineno 135
+               firstlineno 134
                lnotab 0x02011c0128012401240120011e010a01
             code
                argcount  : 3
                nlocals   : 12
                stacksize : 9
                flags     : 3
                code
@@ -993,181 +963,181 @@
                   00ab0000000000000000007d087c036a0300000000000000007c06640a9c
                   027d0b741d000000000000000000007c08a6010000ab0100000000000000
                   0072057c087c0b640b3c000000741f000000000000000000007c0b742000
                   0000000000000000006a110000000000000000ac0ca6020000ab02000000
                   00000000005300741f00000000000000000000640d7c036a120000000000
                   00000069017420000000000000000000006a130000000000000000ac0ca6
                   020000ab0200000000000000005300
-               145           0 RESUME                   0
+               144           0 RESUME                   0
                
-               148           2 LOAD_FAST                2 (model_admin)
+               147           2 LOAD_FAST                2 (model_admin)
                              4 LOAD_METHOD              0 (has_add_permission)
                             26 LOAD_FAST                1 (request)
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_JUMP_FORWARD_IF_TRUE     7 (to 58)
                
-               149          44 LOAD_GLOBAL              2 (PermissionDenied)
+               148          44 LOAD_GLOBAL              2 (PermissionDenied)
                             56 RAISE_VARARGS            1
                
-               152     >>   58 LOAD_FAST                0 (self)
+               151     >>   58 LOAD_FAST                0 (self)
                             60 LOAD_METHOD              2 (serializer_class)
                             82 LOAD_FAST                1 (request)
                             84 LOAD_ATTR                3 (data)
                             94 LOAD_METHOD              4 (get)
                            116 LOAD_CONST               1 ('data')
                            118 BUILD_MAP                0
                            120 PRECALL                  2
                            124 CALL                     2
                            134 KW_NAMES                 2
                            136 PRECALL                  1
                            140 CALL                     1
                            150 STORE_FAST               3 (serializer)
                
-               153         152 LOAD_FAST                3 (serializer)
+               152         152 LOAD_FAST                3 (serializer)
                            154 LOAD_METHOD              5 (is_valid)
                            176 PRECALL                  0
                            180 CALL                     0
                            190 EXTENDED_ARG             1
                            192 POP_JUMP_FORWARD_IF_FALSE   281 (to 756)
                
-               155         194 LOAD_FAST                2 (model_admin)
+               154         194 LOAD_FAST                2 (model_admin)
                            196 LOAD_ATTR                6 (model)
                            206 LOAD_ATTR                7 (_meta)
                            216 STORE_FAST               4 (opts)
                
-               156         218 LOAD_FAST                3 (serializer)
+               155         218 LOAD_FAST                3 (serializer)
                            220 LOAD_METHOD              8 (save)
                            242 PRECALL                  0
                            246 CALL                     0
                            256 STORE_FAST               5 (new_object)
                
-               157         258 LOAD_GLOBAL             19 (NULL + _)
+               156         258 LOAD_GLOBAL             19 (NULL + _)
                
-               158         270 LOAD_CONST               3 ('The ')
+               157         270 LOAD_CONST               3 ('The ')
                            272 LOAD_FAST                4 (opts)
                            274 LOAD_ATTR               10 (verbose_name)
                            284 FORMAT_VALUE             0
                            286 LOAD_CONST               4 (' “')
                            288 LOAD_GLOBAL             23 (NULL + str)
                            300 LOAD_FAST                5 (new_object)
                            302 PRECALL                  1
                            306 CALL                     1
                            316 FORMAT_VALUE             0
                            318 LOAD_CONST               5 ('” was added successfully.')
                            320 BUILD_STRING             5
                
-               157         322 PRECALL                  1
+               156         322 PRECALL                  1
                            326 CALL                     1
                            336 STORE_FAST               6 (msg)
                
-               161         338 LOAD_FAST                2 (model_admin)
+               160         338 LOAD_FAST                2 (model_admin)
                            340 STORE_FAST               2 (model_admin)
                
-               162         342 LOAD_FAST                5 (new_object)
+               161         342 LOAD_FAST                5 (new_object)
                            344 STORE_FAST               7 (change_object)
                
-               165         346 LOAD_FAST                2 (model_admin)
+               164         346 LOAD_FAST                2 (model_admin)
                            348 LOAD_METHOD             12 (log_addition)
                            370 LOAD_FAST                1 (request)
                            372 LOAD_FAST                7 (change_object)
                            374 LOAD_CONST               6 ('added')
                
-               166         376 LOAD_GLOBAL             23 (NULL + str)
+               165         376 LOAD_GLOBAL             23 (NULL + str)
                            388 LOAD_FAST                5 (new_object)
                            390 LOAD_ATTR                7 (_meta)
                            400 LOAD_ATTR               10 (verbose_name)
                            410 PRECALL                  1
                            414 CALL                     1
                
-               167         424 LOAD_GLOBAL             23 (NULL + str)
+               166         424 LOAD_GLOBAL             23 (NULL + str)
                            436 LOAD_FAST                5 (new_object)
                            438 PRECALL                  1
                            442 CALL                     1
                
-               165         452 LOAD_CONST               7 (('name', 'object'))
+               164         452 LOAD_CONST               7 (('name', 'object'))
                            454 BUILD_CONST_KEY_MAP      2
                            456 BUILD_MAP                1
                            458 BUILD_LIST               1
                            460 PRECALL                  3
                            464 CALL                     3
                            474 POP_TOP
                
-               171         476 BUILD_LIST               0
+               170         476 BUILD_LIST               0
                            478 STORE_FAST               8 (created_inlines)
                
-               172         480 LOAD_FAST                1 (request)
+               171         480 LOAD_FAST                1 (request)
                            482 LOAD_ATTR                3 (data)
                            492 LOAD_METHOD              4 (get)
                            514 LOAD_CONST               8 ('create_inlines')
                            516 LOAD_CONST               0 (None)
                            518 PRECALL                  2
                            522 CALL                     2
                            532 POP_JUMP_FORWARD_IF_FALSE    54 (to 642)
                
-               173         534 LOAD_GLOBAL             27 (NULL + validate_bulk_edits)
+               172         534 LOAD_GLOBAL             27 (NULL + validate_bulk_edits)
                
-               174         546 LOAD_FAST                1 (request)
+               173         546 LOAD_FAST                1 (request)
                            548 LOAD_FAST                2 (model_admin)
                            550 LOAD_FAST                5 (new_object)
                
-               173         552 PRECALL                  3
+               172         552 PRECALL                  3
                            556 CALL                     3
                            566 STORE_FAST               9 (valid_serializers)
                
-               176         568 LOAD_FAST                9 (valid_serializers)
+               175         568 LOAD_FAST                9 (valid_serializers)
                            570 GET_ITER
                        >>  572 FOR_ITER                22 (to 618)
                            574 STORE_FAST              10 (inline_serializer)
                
-               177         576 LOAD_FAST               10 (inline_serializer)
+               176         576 LOAD_FAST               10 (inline_serializer)
                            578 LOAD_METHOD              8 (save)
                            600 PRECALL                  0
                            604 CALL                     0
                            614 POP_TOP
                            616 JUMP_BACKWARD           23 (to 572)
                
-               179     >>  618 LOAD_CONST               9 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 179>)
+               178     >>  618 LOAD_CONST               9 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 178>)
                            620 MAKE_FUNCTION            0
                
-               180         622 LOAD_FAST                9 (valid_serializers)
+               179         622 LOAD_FAST                9 (valid_serializers)
                
-               179         624 GET_ITER
+               178         624 GET_ITER
                            626 PRECALL                  0
                            630 CALL                     0
                            640 STORE_FAST               8 (created_inlines)
                
-               183     >>  642 LOAD_FAST                3 (serializer)
+               182     >>  642 LOAD_FAST                3 (serializer)
                            644 LOAD_ATTR                3 (data)
                            654 LOAD_FAST                6 (msg)
                            656 LOAD_CONST              10 (('data', 'detail'))
                            658 BUILD_CONST_KEY_MAP      2
                            660 STORE_FAST              11 (data)
                
-               184         662 LOAD_GLOBAL             29 (NULL + len)
+               183         662 LOAD_GLOBAL             29 (NULL + len)
                            674 LOAD_FAST                8 (created_inlines)
                            676 PRECALL                  1
                            680 CALL                     1
                            690 POP_JUMP_FORWARD_IF_FALSE     5 (to 702)
                
-               185         692 LOAD_FAST                8 (created_inlines)
+               184         692 LOAD_FAST                8 (created_inlines)
                            694 LOAD_FAST               11 (data)
                            696 LOAD_CONST              11 ('created_inlines')
                            698 STORE_SUBSCR
                
-               187     >>  702 LOAD_GLOBAL             31 (NULL + Response)
+               186     >>  702 LOAD_GLOBAL             31 (NULL + Response)
                            714 LOAD_FAST               11 (data)
                            716 LOAD_GLOBAL             32 (status)
                            728 LOAD_ATTR               17 (HTTP_201_CREATED)
                            738 KW_NAMES                12
                            740 PRECALL                  2
                            744 CALL                     2
                            754 RETURN_VALUE
                
-               190     >>  756 LOAD_GLOBAL             31 (NULL + Response)
+               189     >>  756 LOAD_GLOBAL             31 (NULL + Response)
                            768 LOAD_CONST              13 ('errors')
                            770 LOAD_FAST                3 (serializer)
                            772 LOAD_ATTR               18 (errors)
                            782 BUILD_MAP                1
                            784 LOAD_GLOBAL             32 (status)
                            796 LOAD_ATTR               19 (HTTP_400_BAD_REQUEST)
                            806 KW_NAMES                12
@@ -1186,107 +1156,107 @@
                   'create_inlines'
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-                     179           0 RESUME                   0
+                     178           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 9 (to 26)
                      
-                     180           8 STORE_FAST               1 (inline_serializer)
+                     179           8 STORE_FAST               1 (inline_serializer)
                                   10 LOAD_FAST                1 (inline_serializer)
                                   12 LOAD_ATTR                0 (data)
                      
-                     179          22 LIST_APPEND              2
+                     178          22 LIST_APPEND              2
                                   24 JUMP_BACKWARD           10 (to 6)
                              >>   26 RETURN_VALUE
                      consts
                      names      ('data',)
                      varnames   ('.0', 'inline_serializer')
                      freevars   ()
                      cellvars   ()
-                     filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+                     filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                      name       '<listcomp>'
-                     firstlineno 179
+                     firstlineno 178
                      lnotab 0x08010eff
                   ('data', 'detail')
                   'created_inlines'
                   ('status',)
                   'errors'
                names      ('has_add_permission', 'PermissionDenied', 'serializer_class', 'data', 'get', 'is_valid', 'model', '_meta', 'save', '_', 'verbose_name', 'str', 'log_addition', 'validate_bulk_edits', 'len', 'Response', 'status', 'HTTP_201_CREATED', 'errors', 'HTTP_400_BAD_REQUEST')
                varnames   ('self', 'request', 'model_admin', 'serializer', 'opts', 'new_object', 'msg', 'change_object', 'created_inlines', 'valid_serializers', 'inline_serializer', 'data')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'post'
-               firstlineno 145
+               firstlineno 144
                lnotab
                   0x02032a010e035e012a02180128010c0134ff1004040104031e0130011c
                   fe1806040136010c0106ff100308012a02040102ff120414011e010a0236
                   03
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'serializer_class', 'permission_classes', 'get', 'transaction', 'atomic', 'post')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
          name       'AddView'
-         firstlineno 104
+         firstlineno 103
          lnotab 0x0a01041b04010402060a0c0104ff0e01
       'AddView'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a0264015a0364025a0467005a05640384005a0665
             076a08000000000000000064048400a6000000ab0000000000000000005a
             09640584005a0a640684005a0b640784005a0c64025300
-         193           0 RESUME                   0
+         192           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ChangeView')
                        8 STORE_NAME               2 (__qualname__)
          
-         194          10 LOAD_CONST               1 ('\n    Change an existing instance of this model. if the models has inline models associated with it you \n    create, update and delete instances of the models associated with it.\n\n        {\n        "data": {\n            // the values to create new instance of the model\n            "name": "lorem ipsum"\n            ...\n        },\n        // the inline instances you want to create (optional)\n        "create_inlines": {\n            "books": [\n                {\n                    "title": "lorem ipsum"\n                    ...\n                },\n            ]\n        },\n        // the inline instances you want to update make sure you include a pk field (optional)\n        "update_inlines": {\n            "books": [\n                {\n                    "pk":10,\n                    "title": "lorem ipsum"\n                    ...\n                },\n            ]\n        },\n        // the inline instances you want to delete make sure you include a pk field (optional)\n        "delete_inlines": {\n            "books": [\n                {\n                    "pk":10\n                },\n            ]\n        }\n    }\n    ')
+         193          10 LOAD_CONST               1 ('\n    Change an existing instance of this model. if the models has inline models associated with it you \n    create, update and delete instances of the models associated with it.\n\n        {\n        "data": {\n            // the values to create new instance of the model\n            "name": "lorem ipsum"\n            ...\n        },\n        // the inline instances you want to create (optional)\n        "create_inlines": {\n            "books": [\n                {\n                    "title": "lorem ipsum"\n                    ...\n                },\n            ]\n        },\n        // the inline instances you want to update make sure you include a pk field (optional)\n        "update_inlines": {\n            "books": [\n                {\n                    "pk":10,\n                    "title": "lorem ipsum"\n                    ...\n                },\n            ]\n        },\n        // the inline instances you want to delete make sure you include a pk field (optional)\n        "delete_inlines": {\n            "books": [\n                {\n                    "pk":10\n                },\n            ]\n        }\n    }\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-         233          14 LOAD_CONST               2 (None)
+         232          14 LOAD_CONST               2 (None)
                       16 STORE_NAME               4 (serializer_class)
          
-         234          18 BUILD_LIST               0
+         233          18 BUILD_LIST               0
                       20 STORE_NAME               5 (permission_classes)
          
-         236          22 LOAD_CONST               3 (<code object get_serializer_instance, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 236>)
+         235          22 LOAD_CONST               3 (<code object get_serializer_instance, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 235>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               6 (get_serializer_instance)
          
-         252          28 LOAD_NAME                7 (transaction)
+         251          28 LOAD_NAME                7 (transaction)
                       30 LOAD_ATTR                8 (atomic)
          
-         253          40 LOAD_CONST               4 (<code object update, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 252>)
+         252          40 LOAD_CONST               4 (<code object update, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 251>)
                       42 MAKE_FUNCTION            0
          
-         252          44 PRECALL                  0
+         251          44 PRECALL                  0
                       48 CALL                     0
          
-         253          58 STORE_NAME               9 (update)
+         252          58 STORE_NAME               9 (update)
          
-         348          60 LOAD_CONST               5 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 348>)
+         347          60 LOAD_CONST               5 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 347>)
                       62 MAKE_FUNCTION            0
                       64 STORE_NAME              10 (get)
          
-         351          66 LOAD_CONST               6 (<code object put, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 351>)
+         350          66 LOAD_CONST               6 (<code object put, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 350>)
                       68 MAKE_FUNCTION            0
                       70 STORE_NAME              11 (put)
          
-         354          72 LOAD_CONST               7 (<code object patch, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 354>)
+         353          72 LOAD_CONST               7 (<code object patch, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 353>)
                       74 MAKE_FUNCTION            0
                       76 STORE_NAME              12 (patch)
                       78 LOAD_CONST               2 (None)
                       80 RETURN_VALUE
          consts
             'ChangeView'
             '\n    Change an existing instance of this model. if the models has inline models associated with it you \n    create, update and delete instances of the models associated with it.\n\n        {\n        "data": {\n            // the values to create new instance of the model\n            "name": "lorem ipsum"\n            ...\n        },\n        // the inline instances you want to create (optional)\n        "create_inlines": {\n            "books": [\n                {\n                    "title": "lorem ipsum"\n                    ...\n                },\n            ]\n        },\n        // the inline instances you want to update make sure you include a pk field (optional)\n        "update_inlines": {\n            "books": [\n                {\n                    "pk":10,\n                    "title": "lorem ipsum"\n                    ...\n                },\n            ]\n        },\n        // the inline instances you want to delete make sure you include a pk field (optional)\n        "delete_inlines": {\n            "books": [\n                {\n                    "pk":10\n                },\n            ]\n        }\n    }\n    '
@@ -1304,83 +1274,83 @@
                   00000000007d036e5d7c016a00000000000000000064056b020000000072
                   317c00a00100000000000000000000000000000000000000007c027c016a
                   020000000000000000a00300000000000000000000000000000000000000
                   0064026900a6020000ab020000000000000000ac06a6020000ab02000000
                   00000000007d036e217c016a00000000000000000064076b020000000072
                   167c00a00100000000000000000000000000000000000000007c02ac08a6
                   010000ab0100000000000000007d037c035300
-               236           0 RESUME                   0
+               235           0 RESUME                   0
                
-               237           2 LOAD_CONST               0 (None)
+               236           2 LOAD_CONST               0 (None)
                              4 STORE_FAST               3 (serializer)
                
-               239           6 LOAD_FAST                1 (request)
+               238           6 LOAD_FAST                1 (request)
                              8 LOAD_ATTR                0 (method)
                             18 LOAD_CONST               1 ('PATCH')
                             20 COMPARE_OP               2 (==)
                             26 POP_JUMP_FORWARD_IF_FALSE    50 (to 128)
                
-               240          28 LOAD_FAST                0 (self)
+               239          28 LOAD_FAST                0 (self)
                             30 LOAD_METHOD              1 (serializer_class)
                
-               241          52 LOAD_FAST                2 (obj)
+               240          52 LOAD_FAST                2 (obj)
                             54 LOAD_FAST                1 (request)
                             56 LOAD_ATTR                2 (data)
                             66 LOAD_METHOD              3 (get)
                             88 LOAD_CONST               2 ('data')
                             90 BUILD_MAP                0
                             92 PRECALL                  2
                             96 CALL                     2
                            106 LOAD_CONST               3 (True)
                
-               240         108 KW_NAMES                 4
+               239         108 KW_NAMES                 4
                            110 PRECALL                  3
                            114 CALL                     3
                            124 STORE_FAST               3 (serializer)
                            126 JUMP_FORWARD            93 (to 314)
                
-               243     >>  128 LOAD_FAST                1 (request)
+               242     >>  128 LOAD_FAST                1 (request)
                            130 LOAD_ATTR                0 (method)
                            140 LOAD_CONST               5 ('PUT')
                            142 COMPARE_OP               2 (==)
                            148 POP_JUMP_FORWARD_IF_FALSE    49 (to 248)
                
-               244         150 LOAD_FAST                0 (self)
+               243         150 LOAD_FAST                0 (self)
                            152 LOAD_METHOD              1 (serializer_class)
                
-               245         174 LOAD_FAST                2 (obj)
+               244         174 LOAD_FAST                2 (obj)
                            176 LOAD_FAST                1 (request)
                            178 LOAD_ATTR                2 (data)
                            188 LOAD_METHOD              3 (get)
                            210 LOAD_CONST               2 ('data')
                            212 BUILD_MAP                0
                            214 PRECALL                  2
                            218 CALL                     2
                
-               244         228 KW_NAMES                 6
+               243         228 KW_NAMES                 6
                            230 PRECALL                  2
                            234 CALL                     2
                            244 STORE_FAST               3 (serializer)
                            246 JUMP_FORWARD            33 (to 314)
                
-               247     >>  248 LOAD_FAST                1 (request)
+               246     >>  248 LOAD_FAST                1 (request)
                            250 LOAD_ATTR                0 (method)
                            260 LOAD_CONST               7 ('GET')
                            262 COMPARE_OP               2 (==)
                            268 POP_JUMP_FORWARD_IF_FALSE    22 (to 314)
                
-               248         270 LOAD_FAST                0 (self)
+               247         270 LOAD_FAST                0 (self)
                            272 LOAD_METHOD              1 (serializer_class)
                            294 LOAD_FAST                2 (obj)
                            296 KW_NAMES                 8
                            298 PRECALL                  1
                            302 CALL                     1
                            312 STORE_FAST               3 (serializer)
                
-               250     >>  314 LOAD_FAST                3 (serializer)
+               249     >>  314 LOAD_FAST                3 (serializer)
                            316 RETURN_VALUE
                consts
                   None
                   'PATCH'
                   'data'
                   True
                   ('instance', 'data', 'partial')
@@ -1388,17 +1358,17 @@
                   ('instance', 'data')
                   'GET'
                   ('instance',)
                names      ('method', 'serializer_class', 'data', 'get')
                varnames   ('self', 'request', 'obj', 'serializer')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'get_serializer_instance'
-               firstlineno 236
+               firstlineno 235
                lnotab 0x020104021601180138ff14031601180136ff140316012c02
             code
                argcount  : 4
                nlocals   : 20
                stacksize : 10
                flags     : 3
                code
@@ -1461,422 +1431,422 @@
                   0000007443000000000000000000007c11a6010000ab0100000000000000
                   0072057c117c0a641a3c0000007443000000000000000000007c12a60100
                   00ab01000000000000000072057c127c0a641b3c00000074090000000000
                   00000000007c0a740a000000000000000000006a170000000000000000ac
                   03a6020000ab02000000000000000053007409000000000000000000007c
                   096a220000000000000000740a000000000000000000006a060000000000
                   000000ac03a6020000ab0200000000000000005300
-               252           0 RESUME                   0
+               251           0 RESUME                   0
                
-               255           2 LOAD_FAST                1 (request)
+               254           2 LOAD_FAST                1 (request)
                              4 LOAD_ATTR                0 (query_params)
                             14 LOAD_METHOD              1 (get)
                             36 LOAD_GLOBAL              4 (TO_FIELD_VAR)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               4 (to_field)
                
-               256          64 LOAD_FAST                4 (to_field)
+               255          64 LOAD_FAST                4 (to_field)
                             66 POP_JUMP_FORWARD_IF_FALSE    54 (to 176)
                             68 LOAD_FAST                3 (model_admin)
                             70 LOAD_METHOD              3 (to_field_allowed)
                             92 LOAD_FAST                1 (request)
                             94 LOAD_FAST                4 (to_field)
                             96 PRECALL                  2
                            100 CALL                     2
                            110 POP_JUMP_FORWARD_IF_TRUE    32 (to 176)
                
-               257         112 LOAD_GLOBAL              9 (NULL + Response)
+               256         112 LOAD_GLOBAL              9 (NULL + Response)
                            124 LOAD_CONST               1 ('detail')
                            126 LOAD_CONST               2 ('The field %s cannot be referenced.')
                            128 LOAD_FAST                4 (to_field)
                            130 BINARY_OP                6 (%)
                            134 BUILD_MAP                1
                
-               258         136 LOAD_GLOBAL             10 (status)
+               257         136 LOAD_GLOBAL             10 (status)
                            148 LOAD_ATTR                6 (HTTP_400_BAD_REQUEST)
                
-               257         158 KW_NAMES                 3
+               256         158 KW_NAMES                 3
                            160 PRECALL                  2
                            164 CALL                     2
                            174 RETURN_VALUE
                
-               259     >>  176 LOAD_FAST                3 (model_admin)
+               258     >>  176 LOAD_FAST                3 (model_admin)
                            178 LOAD_METHOD              7 (get_object)
                            200 LOAD_FAST                1 (request)
                            202 LOAD_GLOBAL             17 (NULL + unquote)
                            214 LOAD_FAST                2 (object_id)
                            216 PRECALL                  1
                            220 CALL                     1
                            230 LOAD_FAST                4 (to_field)
                            232 PRECALL                  3
                            236 CALL                     3
                            246 STORE_FAST               5 (obj)
                
-               260         248 LOAD_FAST                3 (model_admin)
+               259         248 LOAD_FAST                3 (model_admin)
                            250 LOAD_ATTR                9 (model)
                            260 LOAD_ATTR               10 (_meta)
                            270 STORE_FAST               6 (opts)
                
-               261         272 LOAD_GLOBAL             23 (NULL + ModelDiffHelper)
+               260         272 LOAD_GLOBAL             23 (NULL + ModelDiffHelper)
                            284 LOAD_FAST                5 (obj)
                            286 PRECALL                  1
                            290 CALL                     1
                            300 STORE_FAST               7 (helper)
                
-               264         302 LOAD_FAST                5 (obj)
+               263         302 LOAD_FAST                5 (obj)
                            304 POP_JUMP_FORWARD_IF_NOT_NONE    78 (to 462)
                
-               265         306 LOAD_GLOBAL             25 (NULL + _)
+               264         306 LOAD_GLOBAL             25 (NULL + _)
                            318 LOAD_CONST               4 ("%(name)s with ID “%(key)s” doesn't exist. Perhaps it was deleted?")
                            320 PRECALL                  1
                            324 CALL                     1
                
-               266         334 LOAD_FAST                3 (model_admin)
+               265         334 LOAD_FAST                3 (model_admin)
                            336 LOAD_ATTR                9 (model)
                            346 LOAD_ATTR               10 (_meta)
                            356 LOAD_ATTR               13 (verbose_name)
                
-               267         366 LOAD_GLOBAL             17 (NULL + unquote)
+               266         366 LOAD_GLOBAL             17 (NULL + unquote)
                            378 LOAD_FAST                2 (object_id)
                            380 PRECALL                  1
                            384 CALL                     1
                
-               265         394 LOAD_CONST               5 (('name', 'key'))
+               264         394 LOAD_CONST               5 (('name', 'key'))
                            396 BUILD_CONST_KEY_MAP      2
                            398 BINARY_OP                6 (%)
                            402 STORE_FAST               8 (msg)
                
-               269         404 LOAD_GLOBAL              9 (NULL + Response)
+               268         404 LOAD_GLOBAL              9 (NULL + Response)
                            416 LOAD_CONST               1 ('detail')
                            418 LOAD_FAST                8 (msg)
                            420 BUILD_MAP                1
                            422 LOAD_GLOBAL             10 (status)
                            434 LOAD_ATTR               14 (HTTP_404_NOT_FOUND)
                            444 KW_NAMES                 3
                            446 PRECALL                  2
                            450 CALL                     2
                            460 RETURN_VALUE
                
-               272     >>  462 LOAD_FAST                3 (model_admin)
+               271     >>  462 LOAD_FAST                3 (model_admin)
                            464 LOAD_METHOD             15 (has_change_permission)
                            486 LOAD_FAST                1 (request)
                            488 LOAD_FAST                5 (obj)
                            490 PRECALL                  2
                            494 CALL                     2
                            504 POP_JUMP_FORWARD_IF_TRUE     7 (to 520)
                
-               273         506 LOAD_GLOBAL             32 (PermissionDenied)
+               272         506 LOAD_GLOBAL             32 (PermissionDenied)
                            518 RAISE_VARARGS            1
                
-               276     >>  520 LOAD_FAST                0 (self)
+               275     >>  520 LOAD_FAST                0 (self)
                            522 LOAD_METHOD             17 (get_serializer_instance)
                            544 LOAD_FAST                1 (request)
                            546 LOAD_FAST                5 (obj)
                            548 PRECALL                  2
                            552 CALL                     2
                            562 STORE_FAST               9 (serializer)
                
-               279         564 LOAD_FAST                1 (request)
+               278         564 LOAD_FAST                1 (request)
                            566 LOAD_ATTR               18 (method)
                            576 LOAD_CONST               6 ('GET')
                            578 COMPARE_OP               2 (==)
                            584 POP_JUMP_FORWARD_IF_FALSE   104 (to 794)
                
-               280         586 LOAD_GLOBAL             39 (NULL + dict)
+               279         586 LOAD_GLOBAL             39 (NULL + dict)
                            598 PRECALL                  0
                            602 CALL                     0
                            612 STORE_FAST              10 (data)
                
-               281         614 LOAD_GLOBAL             41 (NULL + get_form_fields)
+               280         614 LOAD_GLOBAL             41 (NULL + get_form_fields)
                            626 LOAD_FAST                9 (serializer)
                            628 LOAD_CONST               7 (True)
                            630 KW_NAMES                 8
                            632 PRECALL                  2
                            636 CALL                     2
                            646 LOAD_FAST               10 (data)
                            648 LOAD_CONST               9 ('fields')
                            650 STORE_SUBSCR
                
-               282         654 LOAD_GLOBAL             43 (NULL + get_form_config)
+               281         654 LOAD_GLOBAL             43 (NULL + get_form_config)
                            666 LOAD_FAST                3 (model_admin)
                            668 PRECALL                  1
                            672 CALL                     1
                            682 LOAD_FAST               10 (data)
                            684 LOAD_CONST              10 ('config')
                            686 STORE_SUBSCR
                
-               283         690 LOAD_GLOBAL             45 (NULL + get_inlines)
+               282         690 LOAD_GLOBAL             45 (NULL + get_inlines)
                            702 LOAD_FAST                1 (request)
                            704 LOAD_FAST                3 (model_admin)
                            706 LOAD_FAST                5 (obj)
                            708 KW_NAMES                11
                            710 PRECALL                  3
                            714 CALL                     3
                            724 STORE_FAST              11 (inlines)
                
-               284         726 LOAD_FAST               11 (inlines)
+               283         726 LOAD_FAST               11 (inlines)
                            728 POP_JUMP_FORWARD_IF_FALSE     5 (to 740)
                
-               285         730 LOAD_FAST               11 (inlines)
+               284         730 LOAD_FAST               11 (inlines)
                            732 LOAD_FAST               10 (data)
                            734 LOAD_CONST              12 ('inlines')
                            736 STORE_SUBSCR
                
-               286     >>  740 LOAD_GLOBAL              9 (NULL + Response)
+               285     >>  740 LOAD_GLOBAL              9 (NULL + Response)
                            752 LOAD_FAST               10 (data)
                            754 LOAD_GLOBAL             10 (status)
                            766 LOAD_ATTR               23 (HTTP_200_OK)
                            776 KW_NAMES                 3
                            778 PRECALL                  2
                            782 CALL                     2
                            792 RETURN_VALUE
                
-               289     >>  794 LOAD_FAST                9 (serializer)
+               288     >>  794 LOAD_FAST                9 (serializer)
                            796 LOAD_METHOD             24 (is_valid)
                            818 PRECALL                  0
                            822 CALL                     0
                            832 EXTENDED_ARG             1
                            834 POP_JUMP_FORWARD_IF_FALSE   490 (to 1816)
                
-               290         836 LOAD_FAST                9 (serializer)
+               289         836 LOAD_FAST                9 (serializer)
                            838 LOAD_METHOD             25 (save)
                            860 PRECALL                  0
                            864 CALL                     0
                            874 STORE_FAST              12 (updated_object)
                
-               292         876 LOAD_GLOBAL             25 (NULL + _)
+               291         876 LOAD_GLOBAL             25 (NULL + _)
                
-               293         888 LOAD_CONST              13 ('The ')
+               292         888 LOAD_CONST              13 ('The ')
                            890 LOAD_FAST                6 (opts)
                            892 LOAD_ATTR               13 (verbose_name)
                            902 FORMAT_VALUE             0
                            904 LOAD_CONST              14 (' “')
                            906 LOAD_GLOBAL             53 (NULL + str)
                            918 LOAD_FAST               12 (updated_object)
                            920 PRECALL                  1
                            924 CALL                     1
                            934 FORMAT_VALUE             0
                            936 LOAD_CONST              15 ('” was changed successfully.')
                            938 BUILD_STRING             5
                
-               292         940 PRECALL                  1
+               291         940 PRECALL                  1
                            944 CALL                     1
                            954 STORE_FAST               8 (msg)
                
-               295         956 LOAD_FAST               12 (updated_object)
+               294         956 LOAD_FAST               12 (updated_object)
                            958 STORE_FAST              13 (changed_object)
                
-               297         960 LOAD_FAST                3 (model_admin)
+               296         960 LOAD_FAST                3 (model_admin)
                            962 LOAD_METHOD             27 (log_change)
                            984 LOAD_FAST                1 (request)
                            986 LOAD_FAST               13 (changed_object)
                            988 LOAD_CONST              16 ('changed')
                
-               298         990 LOAD_GLOBAL             53 (NULL + str)
+               297         990 LOAD_GLOBAL             53 (NULL + str)
                           1002 LOAD_FAST               12 (updated_object)
                           1004 LOAD_ATTR               10 (_meta)
                           1014 LOAD_ATTR               13 (verbose_name)
                           1024 PRECALL                  1
                           1028 CALL                     1
                
-               299        1038 LOAD_GLOBAL             53 (NULL + str)
+               298        1038 LOAD_GLOBAL             53 (NULL + str)
                           1050 LOAD_FAST               12 (updated_object)
                           1052 PRECALL                  1
                           1056 CALL                     1
                
-               300        1066 LOAD_FAST                7 (helper)
+               299        1066 LOAD_FAST                7 (helper)
                           1068 LOAD_METHOD             28 (set_changed_model)
                           1090 LOAD_FAST               12 (updated_object)
                           1092 PRECALL                  1
                           1096 CALL                     1
                           1106 LOAD_ATTR               29 (changed_fields)
                
-               297        1116 LOAD_CONST              17 (('name', 'object', 'fields'))
+               296        1116 LOAD_CONST              17 (('name', 'object', 'fields'))
                           1118 BUILD_CONST_KEY_MAP      3
                           1120 BUILD_MAP                1
                           1122 BUILD_LIST               1
                           1124 PRECALL                  3
                           1128 CALL                     3
                           1138 POP_TOP
                
-               304        1140 BUILD_LIST               0
+               303        1140 BUILD_LIST               0
                           1142 STORE_FAST              14 (created_inlines)
                
-               305        1144 LOAD_FAST                1 (request)
+               304        1144 LOAD_FAST                1 (request)
                           1146 LOAD_ATTR               30 (data)
                           1156 LOAD_METHOD              1 (get)
                           1178 LOAD_CONST              18 ('create_inlines')
                           1180 LOAD_CONST               0 (None)
                           1182 PRECALL                  2
                           1186 CALL                     2
                           1196 POP_JUMP_FORWARD_IF_FALSE    56 (to 1310)
                
-               306        1198 LOAD_GLOBAL             63 (NULL + validate_bulk_edits)
+               305        1198 LOAD_GLOBAL             63 (NULL + validate_bulk_edits)
                
-               307        1210 LOAD_FAST                1 (request)
+               306        1210 LOAD_FAST                1 (request)
                           1212 LOAD_FAST                3 (model_admin)
                           1214 LOAD_FAST                5 (obj)
                           1216 LOAD_CONST              18 ('create_inlines')
                
-               306        1218 KW_NAMES                19
+               305        1218 KW_NAMES                19
                           1220 PRECALL                  4
                           1224 CALL                     4
                           1234 STORE_FAST              15 (valid_serializers)
                
-               309        1236 LOAD_FAST               15 (valid_serializers)
+               308        1236 LOAD_FAST               15 (valid_serializers)
                           1238 GET_ITER
                        >> 1240 FOR_ITER                22 (to 1286)
                           1242 STORE_FAST              16 (inline_serializer)
                
-               310        1244 LOAD_FAST               16 (inline_serializer)
+               309        1244 LOAD_FAST               16 (inline_serializer)
                           1246 LOAD_METHOD             25 (save)
                           1268 PRECALL                  0
                           1272 CALL                     0
                           1282 POP_TOP
                           1284 JUMP_BACKWARD           23 (to 1240)
                
-               312     >> 1286 LOAD_CONST              20 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 312>)
+               311     >> 1286 LOAD_CONST              20 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 311>)
                           1288 MAKE_FUNCTION            0
                
-               313        1290 LOAD_FAST               15 (valid_serializers)
+               312        1290 LOAD_FAST               15 (valid_serializers)
                
-               312        1292 GET_ITER
+               311        1292 GET_ITER
                           1294 PRECALL                  0
                           1298 CALL                     0
                           1308 STORE_FAST              14 (created_inlines)
                
-               316     >> 1310 BUILD_LIST               0
+               315     >> 1310 BUILD_LIST               0
                           1312 STORE_FAST              17 (updated_inlines)
                
-               317        1314 LOAD_FAST                1 (request)
+               316        1314 LOAD_FAST                1 (request)
                           1316 LOAD_ATTR               30 (data)
                           1326 LOAD_METHOD              1 (get)
                           1348 LOAD_CONST              21 ('update_inlines')
                           1350 LOAD_CONST               0 (None)
                           1352 PRECALL                  2
                           1356 CALL                     2
                           1366 POP_JUMP_FORWARD_IF_FALSE    56 (to 1480)
                
-               318        1368 LOAD_GLOBAL             63 (NULL + validate_bulk_edits)
+               317        1368 LOAD_GLOBAL             63 (NULL + validate_bulk_edits)
                
-               319        1380 LOAD_FAST                1 (request)
+               318        1380 LOAD_FAST                1 (request)
                           1382 LOAD_FAST                3 (model_admin)
                           1384 LOAD_FAST                5 (obj)
                           1386 LOAD_CONST              21 ('update_inlines')
                
-               318        1388 KW_NAMES                19
+               317        1388 KW_NAMES                19
                           1390 PRECALL                  4
                           1394 CALL                     4
                           1404 STORE_FAST              15 (valid_serializers)
                
-               321        1406 LOAD_FAST               15 (valid_serializers)
+               320        1406 LOAD_FAST               15 (valid_serializers)
                           1408 GET_ITER
                        >> 1410 FOR_ITER                22 (to 1456)
                           1412 STORE_FAST              16 (inline_serializer)
                
-               322        1414 LOAD_FAST               16 (inline_serializer)
+               321        1414 LOAD_FAST               16 (inline_serializer)
                           1416 LOAD_METHOD             25 (save)
                           1438 PRECALL                  0
                           1442 CALL                     0
                           1452 POP_TOP
                           1454 JUMP_BACKWARD           23 (to 1410)
                
-               324     >> 1456 LOAD_CONST              22 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 324>)
+               323     >> 1456 LOAD_CONST              22 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 323>)
                           1458 MAKE_FUNCTION            0
                
-               325        1460 LOAD_FAST               15 (valid_serializers)
+               324        1460 LOAD_FAST               15 (valid_serializers)
                
-               324        1462 GET_ITER
+               323        1462 GET_ITER
                           1464 PRECALL                  0
                           1468 CALL                     0
                           1478 STORE_FAST              17 (updated_inlines)
                
-               328     >> 1480 BUILD_LIST               0
+               327     >> 1480 BUILD_LIST               0
                           1482 STORE_FAST              18 (deleted_inlines)
                
-               329        1484 LOAD_FAST                1 (request)
+               328        1484 LOAD_FAST                1 (request)
                           1486 LOAD_ATTR               30 (data)
                           1496 LOAD_METHOD              1 (get)
                           1518 LOAD_CONST              23 ('delete_inlines')
                           1520 LOAD_CONST               0 (None)
                           1522 PRECALL                  2
                           1526 CALL                     2
                           1536 POP_JUMP_FORWARD_IF_FALSE    42 (to 1622)
                
-               330        1538 LOAD_GLOBAL             63 (NULL + validate_bulk_edits)
+               329        1538 LOAD_GLOBAL             63 (NULL + validate_bulk_edits)
                
-               331        1550 LOAD_FAST                1 (request)
+               330        1550 LOAD_FAST                1 (request)
                           1552 LOAD_FAST                3 (model_admin)
                           1554 LOAD_FAST                5 (obj)
                           1556 LOAD_CONST              23 ('delete_inlines')
                
-               330        1558 KW_NAMES                19
+               329        1558 KW_NAMES                19
                           1560 PRECALL                  4
                           1564 CALL                     4
                           1574 UNPACK_SEQUENCE          2
                           1578 STORE_FAST              19 (instances)
                           1580 STORE_FAST              18 (deleted_inlines)
                
-               333        1582 LOAD_FAST               19 (instances)
+               332        1582 LOAD_FAST               19 (instances)
                           1584 LOAD_METHOD             32 (delete)
                           1606 PRECALL                  0
                           1610 CALL                     0
                           1620 POP_TOP
                
-               336     >> 1622 LOAD_FAST                9 (serializer)
+               335     >> 1622 LOAD_FAST                9 (serializer)
                           1624 LOAD_ATTR               30 (data)
                           1634 LOAD_FAST                8 (msg)
                           1636 LOAD_CONST              24 (('data', 'detail'))
                           1638 BUILD_CONST_KEY_MAP      2
                           1640 STORE_FAST              10 (data)
                
-               337        1642 LOAD_GLOBAL             67 (NULL + len)
+               336        1642 LOAD_GLOBAL             67 (NULL + len)
                           1654 LOAD_FAST               14 (created_inlines)
                           1656 PRECALL                  1
                           1660 CALL                     1
                           1670 POP_JUMP_FORWARD_IF_FALSE     5 (to 1682)
                
-               338        1672 LOAD_FAST               14 (created_inlines)
+               337        1672 LOAD_FAST               14 (created_inlines)
                           1674 LOAD_FAST               10 (data)
                           1676 LOAD_CONST              25 ('created_inlines')
                           1678 STORE_SUBSCR
                
-               339     >> 1682 LOAD_GLOBAL             67 (NULL + len)
+               338     >> 1682 LOAD_GLOBAL             67 (NULL + len)
                           1694 LOAD_FAST               17 (updated_inlines)
                           1696 PRECALL                  1
                           1700 CALL                     1
                           1710 POP_JUMP_FORWARD_IF_FALSE     5 (to 1722)
                
-               340        1712 LOAD_FAST               17 (updated_inlines)
+               339        1712 LOAD_FAST               17 (updated_inlines)
                           1714 LOAD_FAST               10 (data)
                           1716 LOAD_CONST              26 ('updated_inlines')
                           1718 STORE_SUBSCR
                
-               341     >> 1722 LOAD_GLOBAL             67 (NULL + len)
+               340     >> 1722 LOAD_GLOBAL             67 (NULL + len)
                           1734 LOAD_FAST               18 (deleted_inlines)
                           1736 PRECALL                  1
                           1740 CALL                     1
                           1750 POP_JUMP_FORWARD_IF_FALSE     5 (to 1762)
                
-               342        1752 LOAD_FAST               18 (deleted_inlines)
+               341        1752 LOAD_FAST               18 (deleted_inlines)
                           1754 LOAD_FAST               10 (data)
                           1756 LOAD_CONST              27 ('deleted_inlines')
                           1758 STORE_SUBSCR
                
-               344     >> 1762 LOAD_GLOBAL              9 (NULL + Response)
+               343     >> 1762 LOAD_GLOBAL              9 (NULL + Response)
                           1774 LOAD_FAST               10 (data)
                           1776 LOAD_GLOBAL             10 (status)
                           1788 LOAD_ATTR               23 (HTTP_200_OK)
                           1798 KW_NAMES                 3
                           1800 PRECALL                  2
                           1804 CALL                     2
                           1814 RETURN_VALUE
                
-               346     >> 1816 LOAD_GLOBAL              9 (NULL + Response)
+               345     >> 1816 LOAD_GLOBAL              9 (NULL + Response)
                           1828 LOAD_FAST                9 (serializer)
                           1830 LOAD_ATTR               34 (errors)
                           1840 LOAD_GLOBAL             10 (status)
                           1852 LOAD_ATTR                6 (HTTP_400_BAD_REQUEST)
                           1862 KW_NAMES                 3
                           1864 PRECALL                  2
                           1868 CALL                     2
@@ -1904,199 +1874,199 @@
                   ('operation',)
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-                     312           0 RESUME                   0
+                     311           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 9 (to 26)
                      
-                     313           8 STORE_FAST               1 (inline_serializer)
+                     312           8 STORE_FAST               1 (inline_serializer)
                                   10 LOAD_FAST                1 (inline_serializer)
                                   12 LOAD_ATTR                0 (data)
                      
-                     312          22 LIST_APPEND              2
+                     311          22 LIST_APPEND              2
                                   24 JUMP_BACKWARD           10 (to 6)
                              >>   26 RETURN_VALUE
                      consts
                      names      ('data',)
                      varnames   ('.0', 'inline_serializer')
                      freevars   ()
                      cellvars   ()
-                     filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+                     filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                      name       '<listcomp>'
-                     firstlineno 312
+                     firstlineno 311
                      lnotab 0x08010eff
                   'update_inlines'
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-                     324           0 RESUME                   0
+                     323           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 9 (to 26)
                      
-                     325           8 STORE_FAST               1 (inline_serializer)
+                     324           8 STORE_FAST               1 (inline_serializer)
                                   10 LOAD_FAST                1 (inline_serializer)
                                   12 LOAD_ATTR                0 (data)
                      
-                     324          22 LIST_APPEND              2
+                     323          22 LIST_APPEND              2
                                   24 JUMP_BACKWARD           10 (to 6)
                              >>   26 RETURN_VALUE
                      consts
                      names      ('data',)
                      varnames   ('.0', 'inline_serializer')
                      freevars   ()
                      cellvars   ()
-                     filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+                     filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                      name       '<listcomp>'
-                     firstlineno 324
+                     firstlineno 323
                      lnotab 0x08010eff
                   'delete_inlines'
                   ('data', 'detail')
                   'created_inlines'
                   'updated_inlines'
                   'deleted_inlines'
                names      ('query_params', 'get', 'TO_FIELD_VAR', 'to_field_allowed', 'Response', 'status', 'HTTP_400_BAD_REQUEST', 'get_object', 'unquote', 'model', '_meta', 'ModelDiffHelper', '_', 'verbose_name', 'HTTP_404_NOT_FOUND', 'has_change_permission', 'PermissionDenied', 'get_serializer_instance', 'method', 'dict', 'get_form_fields', 'get_form_config', 'get_inlines', 'HTTP_200_OK', 'is_valid', 'save', 'str', 'log_change', 'set_changed_model', 'changed_fields', 'data', 'validate_bulk_edits', 'delete', 'len', 'errors')
                varnames   ('self', 'request', 'object_id', 'model_admin', 'to_field', 'obj', 'opts', 'helper', 'msg', 'serializer', 'data', 'inlines', 'updated_object', 'changed_object', 'created_inlines', 'valid_serializers', 'inline_serializer', 'updated_inlines', 'deleted_inlines', 'instances')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'update'
-               firstlineno 252
+               firstlineno 251
                lnotab
                   0x02033e013001180116ff1202480118011e0304011c0120011cfe0a043a
                   032c010e032c0316011c0128012401240104010a0136032a0128020c0134
                   ff100304021e0130011c0132fd1807040136010c0108ff120308012a0204
                   0102ff1204040136010c0108ff120308012a02040102ff1204040136010c
                   0108ff1803280314011e010a011e010a011e010a023602
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c017c
                   027c03a6030000ab0300000000000000005300
-               348           0 RESUME                   0
+               347           0 RESUME                   0
                
-               349           2 LOAD_FAST                0 (self)
+               348           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (update)
                             26 LOAD_FAST                1 (request)
                             28 LOAD_FAST                2 (object_id)
                             30 LOAD_FAST                3 (admin)
                             32 PRECALL                  3
                             36 CALL                     3
                             46 RETURN_VALUE
                consts
                   None
                names      ('update',)
                varnames   ('self', 'request', 'object_id', 'admin')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'get'
-               firstlineno 348
+               firstlineno 347
                lnotab 0x0201
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c017c
                   027c03a6030000ab0300000000000000005300
-               351           0 RESUME                   0
+               350           0 RESUME                   0
                
-               352           2 LOAD_FAST                0 (self)
+               351           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (update)
                             26 LOAD_FAST                1 (request)
                             28 LOAD_FAST                2 (object_id)
                             30 LOAD_FAST                3 (admin)
                             32 PRECALL                  3
                             36 CALL                     3
                             46 RETURN_VALUE
                consts
                   None
                names      ('update',)
                varnames   ('self', 'request', 'object_id', 'admin')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'put'
-               firstlineno 351
+               firstlineno 350
                lnotab 0x0201
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c017c
                   027c03a6030000ab0300000000000000005300
-               354           0 RESUME                   0
+               353           0 RESUME                   0
                
-               355           2 LOAD_FAST                0 (self)
+               354           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (update)
                             26 LOAD_FAST                1 (request)
                             28 LOAD_FAST                2 (object_id)
                             30 LOAD_FAST                3 (admin)
                             32 PRECALL                  3
                             36 CALL                     3
                             46 RETURN_VALUE
                consts
                   None
                names      ('update',)
                varnames   ('self', 'request', 'object_id', 'admin')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'patch'
-               firstlineno 354
+               firstlineno 353
                lnotab 0x0201
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'serializer_class', 'permission_classes', 'get_serializer_instance', 'transaction', 'atomic', 'update', 'get', 'put', 'patch')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
          name       'ChangeView'
-         firstlineno 193
+         firstlineno 192
          lnotab 0x0a0104270401040206100c0104ff0e01025f06030603
       'ChangeView'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0367005a04640284005a05640384005a
             0664045300
-         358           0 RESUME                   0
+         357           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('DeleteView')
                        8 STORE_NAME               2 (__qualname__)
          
-         359          10 LOAD_CONST               1 ('\n    Delete a single object from this model\n    ')
+         358          10 LOAD_CONST               1 ('\n    Delete a single object from this model\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-         362          14 BUILD_LIST               0
+         361          14 BUILD_LIST               0
                       16 STORE_NAME               4 (permission_classes)
          
-         364          18 LOAD_CONST               2 (<code object delete, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 364>)
+         363          18 LOAD_CONST               2 (<code object delete, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 363>)
                       20 MAKE_FUNCTION            0
                       22 STORE_NAME               5 (delete)
          
-         398          24 LOAD_CONST               3 (<code object post, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 398>)
+         397          24 LOAD_CONST               3 (<code object post, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 397>)
                       26 MAKE_FUNCTION            0
                       28 STORE_NAME               6 (post)
                       30 LOAD_CONST               4 (None)
                       32 RETURN_VALUE
          consts
             'DeleteView'
             '\n    Delete a single object from this model\n    '
@@ -2126,154 +2096,154 @@
                   00000000007c06a6010000ab010000000000000000a6030000ab03000000
                   000000000001007c06a01200000000000000000000000000000000000000
                   00a6000000ab0000000000000000000100740d0000000000000000000064
                   017417000000000000000000006406a6010000ab0100000000000000007c
                   046a0c00000000000000007423000000000000000000007c06a6010000ab
                   01000000000000000064079c027a0600006901740e000000000000000000
                   006a130000000000000000ac03a6020000ab0200000000000000005300
-               364           0 RESUME                   0
+               363           0 RESUME                   0
                
-               365           2 LOAD_FAST                3 (admin)
+               364           2 LOAD_FAST                3 (admin)
                              4 LOAD_ATTR                0 (model)
                             14 LOAD_ATTR                1 (_meta)
                             24 STORE_FAST               4 (opts)
                
-               368          26 LOAD_FAST                1 (request)
+               367          26 LOAD_FAST                1 (request)
                             28 LOAD_ATTR                2 (query_params)
                             38 LOAD_METHOD              3 (get)
                             60 LOAD_GLOBAL              8 (TO_FIELD_VAR)
                             72 PRECALL                  1
                             76 CALL                     1
                             86 STORE_FAST               5 (to_field)
                
-               369          88 LOAD_FAST                5 (to_field)
+               368          88 LOAD_FAST                5 (to_field)
                             90 POP_JUMP_FORWARD_IF_FALSE    54 (to 200)
                             92 LOAD_FAST                3 (admin)
                             94 LOAD_METHOD              5 (to_field_allowed)
                            116 LOAD_FAST                1 (request)
                            118 LOAD_FAST                5 (to_field)
                            120 PRECALL                  2
                            124 CALL                     2
                            134 POP_JUMP_FORWARD_IF_TRUE    32 (to 200)
                
-               370         136 LOAD_GLOBAL             13 (NULL + Response)
+               369         136 LOAD_GLOBAL             13 (NULL + Response)
                            148 LOAD_CONST               1 ('detail')
                            150 LOAD_CONST               2 ('The field %s cannot be referenced.')
                            152 LOAD_FAST                5 (to_field)
                            154 BINARY_OP                6 (%)
                            158 BUILD_MAP                1
                
-               371         160 LOAD_GLOBAL             14 (status)
+               370         160 LOAD_GLOBAL             14 (status)
                            172 LOAD_ATTR                8 (HTTP_400_BAD_REQUEST)
                
-               370         182 KW_NAMES                 3
+               369         182 KW_NAMES                 3
                            184 PRECALL                  2
                            188 CALL                     2
                            198 RETURN_VALUE
                
-               372     >>  200 LOAD_FAST                3 (admin)
+               371     >>  200 LOAD_FAST                3 (admin)
                            202 LOAD_METHOD              9 (get_object)
                            224 LOAD_FAST                1 (request)
                            226 LOAD_GLOBAL             21 (NULL + unquote)
                            238 LOAD_FAST                2 (object_id)
                            240 PRECALL                  1
                            244 CALL                     1
                            254 LOAD_FAST                5 (to_field)
                            256 PRECALL                  3
                            260 CALL                     3
                            270 STORE_FAST               6 (obj)
                
-               374         272 LOAD_FAST                6 (obj)
+               373         272 LOAD_FAST                6 (obj)
                            274 POP_JUMP_FORWARD_IF_NOT_NONE    68 (to 412)
                
-               375         276 LOAD_GLOBAL             23 (NULL + _)
+               374         276 LOAD_GLOBAL             23 (NULL + _)
                            288 LOAD_CONST               4 ("%(name)s with ID “%(key)s” doesn't exist. Perhaps it was deleted?")
                            290 PRECALL                  1
                            294 CALL                     1
                
-               376         304 LOAD_FAST                4 (opts)
+               375         304 LOAD_FAST                4 (opts)
                            306 LOAD_ATTR               12 (verbose_name)
                
-               377         316 LOAD_GLOBAL             21 (NULL + unquote)
+               376         316 LOAD_GLOBAL             21 (NULL + unquote)
                            328 LOAD_FAST                2 (object_id)
                            330 PRECALL                  1
                            334 CALL                     1
                
-               375         344 LOAD_CONST               5 (('name', 'key'))
+               374         344 LOAD_CONST               5 (('name', 'key'))
                            346 BUILD_CONST_KEY_MAP      2
                            348 BINARY_OP                6 (%)
                            352 STORE_FAST               7 (msg)
                
-               379         354 LOAD_GLOBAL             13 (NULL + Response)
+               378         354 LOAD_GLOBAL             13 (NULL + Response)
                            366 LOAD_CONST               1 ('detail')
                            368 LOAD_FAST                7 (msg)
                            370 BUILD_MAP                1
                            372 LOAD_GLOBAL             14 (status)
                            384 LOAD_ATTR               13 (HTTP_404_NOT_FOUND)
                            394 KW_NAMES                 3
                            396 PRECALL                  2
                            400 CALL                     2
                            410 RETURN_VALUE
                
-               382     >>  412 LOAD_FAST                3 (admin)
+               381     >>  412 LOAD_FAST                3 (admin)
                            414 LOAD_METHOD             14 (has_delete_permission)
                            436 LOAD_FAST                1 (request)
                            438 LOAD_FAST                6 (obj)
                            440 PRECALL                  2
                            444 CALL                     2
                            454 POP_JUMP_FORWARD_IF_TRUE     7 (to 470)
                
-               383         456 LOAD_GLOBAL             30 (PermissionDenied)
+               382         456 LOAD_GLOBAL             30 (PermissionDenied)
                            468 RAISE_VARARGS            1
                
-               385     >>  470 LOAD_FAST                3 (admin)
+               384     >>  470 LOAD_FAST                3 (admin)
                            472 STORE_FAST               8 (model_admin)
                
-               388         474 LOAD_FAST                8 (model_admin)
+               387         474 LOAD_FAST                8 (model_admin)
                            476 LOAD_METHOD             16 (log_deletion)
                            498 LOAD_FAST                1 (request)
                            500 LOAD_FAST                6 (obj)
                            502 LOAD_GLOBAL             35 (NULL + str)
                            514 LOAD_FAST                6 (obj)
                            516 PRECALL                  1
                            520 CALL                     1
                            530 PRECALL                  3
                            534 CALL                     3
                            544 POP_TOP
                
-               391         546 LOAD_FAST                6 (obj)
+               390         546 LOAD_FAST                6 (obj)
                            548 LOAD_METHOD             18 (delete)
                            570 PRECALL                  0
                            574 CALL                     0
                            584 POP_TOP
                
-               393         586 LOAD_GLOBAL             13 (NULL + Response)
+               392         586 LOAD_GLOBAL             13 (NULL + Response)
                            598 LOAD_CONST               1 ('detail')
                            600 LOAD_GLOBAL             23 (NULL + _)
                            612 LOAD_CONST               6 ('The %(name)s “%(obj)s” was deleted successfully.')
                            614 PRECALL                  1
                            618 CALL                     1
                
-               394         628 LOAD_FAST                4 (opts)
+               393         628 LOAD_FAST                4 (opts)
                            630 LOAD_ATTR               12 (verbose_name)
                
-               395         640 LOAD_GLOBAL             35 (NULL + str)
+               394         640 LOAD_GLOBAL             35 (NULL + str)
                            652 LOAD_FAST                6 (obj)
                            654 PRECALL                  1
                            658 CALL                     1
                
-               393         668 LOAD_CONST               7 (('name', 'obj'))
+               392         668 LOAD_CONST               7 (('name', 'obj'))
                            670 BUILD_CONST_KEY_MAP      2
                            672 BINARY_OP                6 (%)
                            676 BUILD_MAP                1
                
-               396         678 LOAD_GLOBAL             14 (status)
+               395         678 LOAD_GLOBAL             14 (status)
                            690 LOAD_ATTR               19 (HTTP_200_OK)
                
-               393         700 KW_NAMES                 3
+               392         700 KW_NAMES                 3
                            702 PRECALL                  2
                            706 CALL                     2
                            716 RETURN_VALUE
                consts
                   None
                   'detail'
                   'The field %s cannot be referenced.'
@@ -2282,94 +2252,94 @@
                   ('name', 'key')
                   'The %(name)s “%(obj)s” was deleted successfully.'
                   ('name', 'obj')
                names      ('model', '_meta', 'query_params', 'get', 'TO_FIELD_VAR', 'to_field_allowed', 'Response', 'status', 'HTTP_400_BAD_REQUEST', 'get_object', 'unquote', '_', 'verbose_name', 'HTTP_404_NOT_FOUND', 'has_delete_permission', 'PermissionDenied', 'log_deletion', 'str', 'delete', 'HTTP_200_OK')
                varnames   ('self', 'request', 'object_id', 'admin', 'opts', 'to_field', 'obj', 'msg', 'model_admin')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'delete'
-               firstlineno 364
+               firstlineno 363
                lnotab
                   0x020118033e013001180116ff1202480204011c010c011cfe0a043a032c
                   010e020403480328022a010c011cfe0a0316fd
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code 0x970002007c006a0000000000000000007c0169007c02a4018e015300
-               398           0 RESUME                   0
+               397           0 RESUME                   0
                
-               399           2 PUSH_NULL
+               398           2 PUSH_NULL
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (delete)
                             16 LOAD_FAST                1 (args)
                             18 BUILD_MAP                0
                             20 LOAD_FAST                2 (kwargs)
                             22 DICT_MERGE               1
                             24 CALL_FUNCTION_EX         1
                             26 RETURN_VALUE
                consts
                   None
                names      ('delete',)
                varnames   ('self', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'post'
-               firstlineno 398
+               firstlineno 397
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'permission_classes', 'delete', 'post')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
          name       'DeleteView'
-         firstlineno 358
+         firstlineno 357
          lnotab 0x0a01040304020622
       'DeleteView'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0367005a04640284005a05640384005a
             06640484005a07640584005a08640684005a0964075300
-         402           0 RESUME                   0
+         401           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ChangeListView')
                        8 STORE_NAME               2 (__qualname__)
          
-         403          10 LOAD_CONST               1 ('\n    Return a JSON object representing the django admin changelist table.\n    supports querystring filtering, pagination and search also changes based on list display.\n    Note: this is different from the list all objects view.\n    example of returned JSON object:\n\n    {\n        config: {\n            "list_display": ["name", "age"],\n            "list_display_links": ["name"],\n            "list_filter": ["is_vip"],\n            "result_count": 1,\n            "full_result_count": 1,\n            "list_editable": ["is_vip"],\n\n            actions_list = [\n                [\'delete_selected\', \'delete selected authors\'],\n                [\'make_old\', \'make all others old\']\n            ]\n\n            filters: [\n                {\'name\' : \'is_vip\', \'choices\': [\'All\', \'Yes\', \'No\']}\n            ],\n\n            editing_fields: {\n                "name": {\n                    "name":"name",\n                    "type": "CharField",\n                    "attrs": {},\n                }\n            }\n        },\n\n        "change_list": {\n            "columns": [\n                    {"field": "name", "headerName" "name"},\n                    {"field": "age", "headerName": "age"},\n                    {"field": "is_vip"", "headerName":"is_this_author_a_vip"}\n                ],\n\n            "rows": [\n                {\n                    \'id\': 1,\n                    \'change_url\': \'https://localhost:8000/api_admin/authors/1/change/\',\n                    \'cells\': {\n                        "name": "muhammad",\n                        "age": 20,\n                        "vip": false\n                    }\n                }\n            ],\n        }\n    }\n    ')
+         402          10 LOAD_CONST               1 ('\n    Return a JSON object representing the django admin changelist table.\n    supports querystring filtering, pagination and search also changes based on list display.\n    Note: this is different from the list all objects view.\n    example of returned JSON object:\n\n    {\n        config: {\n            "list_display": ["name", "age"],\n            "list_display_links": ["name"],\n            "list_filter": ["is_vip"],\n            "result_count": 1,\n            "full_result_count": 1,\n            "list_editable": ["is_vip"],\n\n            actions_list = [\n                [\'delete_selected\', \'delete selected authors\'],\n                [\'make_old\', \'make all others old\']\n            ]\n\n            filters: [\n                {\'name\' : \'is_vip\', \'choices\': [\'All\', \'Yes\', \'No\']}\n            ],\n\n            editing_fields: {\n                "name": {\n                    "name":"name",\n                    "type": "CharField",\n                    "attrs": {},\n                }\n            }\n        },\n\n        "change_list": {\n            "columns": [\n                    {"field": "name", "headerName" "name"},\n                    {"field": "age", "headerName": "age"},\n                    {"field": "is_vip"", "headerName":"is_this_author_a_vip"}\n                ],\n\n            "rows": [\n                {\n                    \'id\': 1,\n                    \'change_url\': \'https://localhost:8000/api_admin/authors/1/change/\',\n                    \'cells\': {\n                        "name": "muhammad",\n                        "age": 20,\n                        "vip": false\n                    }\n                }\n            ],\n        }\n    }\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-         457          14 BUILD_LIST               0
+         456          14 BUILD_LIST               0
                       16 STORE_NAME               4 (permission_classes)
          
-         459          18 LOAD_CONST               2 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 459>)
+         458          18 LOAD_CONST               2 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 458>)
                       20 MAKE_FUNCTION            0
                       22 STORE_NAME               5 (get)
          
-         470          24 LOAD_CONST               3 (<code object get_columns, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 470>)
+         469          24 LOAD_CONST               3 (<code object get_columns, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 469>)
                       26 MAKE_FUNCTION            0
                       28 STORE_NAME               6 (get_columns)
          
-         481          30 LOAD_CONST               4 (<code object get_rows, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 481>)
+         480          30 LOAD_CONST               4 (<code object get_rows, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 480>)
                       32 MAKE_FUNCTION            0
                       34 STORE_NAME               7 (get_rows)
          
-         533          36 LOAD_CONST               5 (<code object get_config, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 533>)
+         532          36 LOAD_CONST               5 (<code object get_config, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 532>)
                       38 MAKE_FUNCTION            0
                       40 STORE_NAME               8 (get_config)
          
-         581          42 LOAD_CONST               6 (<code object get_fields_list, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 581>)
+         580          42 LOAD_CONST               6 (<code object get_fields_list, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 580>)
                       44 MAKE_FUNCTION            0
                       46 STORE_NAME               9 (get_fields_list)
                       48 LOAD_CONST               7 (None)
                       50 RETURN_VALUE
          consts
             'ChangeListView'
             '\n    Return a JSON object representing the django admin changelist table.\n    supports querystring filtering, pagination and search also changes based on list display.\n    Note: this is different from the list all objects view.\n    example of returned JSON object:\n\n    {\n        config: {\n            "list_display": ["name", "age"],\n            "list_display_links": ["name"],\n            "list_filter": ["is_vip"],\n            "result_count": 1,\n            "full_result_count": 1,\n            "list_editable": ["is_vip"],\n\n            actions_list = [\n                [\'delete_selected\', \'delete selected authors\'],\n                [\'make_old\', \'make all others old\']\n            ]\n\n            filters: [\n                {\'name\' : \'is_vip\', \'choices\': [\'All\', \'Yes\', \'No\']}\n            ],\n\n            editing_fields: {\n                "name": {\n                    "name":"name",\n                    "type": "CharField",\n                    "attrs": {},\n                }\n            }\n        },\n\n        "change_list": {\n            "columns": [\n                    {"field": "name", "headerName" "name"},\n                    {"field": "age", "headerName": "age"},\n                    {"field": "is_vip"", "headerName":"is_this_author_a_vip"}\n                ],\n\n            "rows": [\n                {\n                    \'id\': 1,\n                    \'change_url\': \'https://localhost:8000/api_admin/authors/1/change/\',\n                    \'cells\': {\n                        "name": "muhammad",\n                        "age": 20,\n                        "vip": false\n                    }\n                }\n            ],\n        }\n    }\n    '
@@ -2387,85 +2357,85 @@
                   0000000000000000000000000000007c017c03a6020000ab020000000000
                   0000007d057c00a00500000000000000000000000000000000000000007c
                   017c03a6020000ab0200000000000000007d067c00a00600000000000000
                   000000000000000000000000007c017c03a6020000ab0200000000000000
                   007d07740f000000000000000000007c077c057c0664019c037410000000
                   000000000000006a090000000000000000ac02a6020000ab020000000000
                   0000005300
-               459           0 RESUME                   0
+               458           0 RESUME                   0
                
-               460           2 NOP
+               459           2 NOP
                
-               461           4 LOAD_FAST                2 (model_admin)
+               460           4 LOAD_FAST                2 (model_admin)
                              6 LOAD_METHOD              0 (get_changelist_instance)
                             28 LOAD_FAST                1 (request)
                             30 PRECALL                  1
                             34 CALL                     1
                             44 STORE_FAST               3 (cl)
                             46 JUMP_FORWARD            46 (to 140)
                        >>   48 PUSH_EXC_INFO
                
-               462          50 LOAD_GLOBAL              2 (IncorrectLookupParameters)
+               461          50 LOAD_GLOBAL              2 (IncorrectLookupParameters)
                             62 CHECK_EXC_MATCH
                             64 POP_JUMP_FORWARD_IF_FALSE    33 (to 132)
                             66 STORE_FAST               4 (e)
                
-               463          68 LOAD_GLOBAL              5 (NULL + NotFound)
+               462          68 LOAD_GLOBAL              5 (NULL + NotFound)
                             80 LOAD_GLOBAL              7 (NULL + str)
                             92 LOAD_FAST                4 (e)
                             94 PRECALL                  1
                             98 CALL                     1
                            108 PRECALL                  1
                            112 CALL                     1
                            122 RAISE_VARARGS            1
                        >>  124 LOAD_CONST               0 (None)
                            126 STORE_FAST               4 (e)
                            128 DELETE_FAST              4 (e)
                            130 RERAISE                  1
                
-               462     >>  132 RERAISE                  0
+               461     >>  132 RERAISE                  0
                        >>  134 COPY                     3
                            136 POP_EXCEPT
                            138 RERAISE                  1
                
-               464     >>  140 LOAD_FAST                0 (self)
+               463     >>  140 LOAD_FAST                0 (self)
                            142 LOAD_METHOD              4 (get_columns)
                            164 LOAD_FAST                1 (request)
                            166 LOAD_FAST                3 (cl)
                            168 PRECALL                  2
                            172 CALL                     2
                            182 STORE_FAST               5 (columns)
                
-               465         184 LOAD_FAST                0 (self)
+               464         184 LOAD_FAST                0 (self)
                            186 LOAD_METHOD              5 (get_rows)
                            208 LOAD_FAST                1 (request)
                            210 LOAD_FAST                3 (cl)
                            212 PRECALL                  2
                            216 CALL                     2
                            226 STORE_FAST               6 (rows)
                
-               466         228 LOAD_FAST                0 (self)
+               465         228 LOAD_FAST                0 (self)
                            230 LOAD_METHOD              6 (get_config)
                            252 LOAD_FAST                1 (request)
                            254 LOAD_FAST                3 (cl)
                            256 PRECALL                  2
                            260 CALL                     2
                            270 STORE_FAST               7 (config)
                
-               467         272 LOAD_GLOBAL             15 (NULL + Response)
+               466         272 LOAD_GLOBAL             15 (NULL + Response)
                            284 LOAD_FAST                7 (config)
                            286 LOAD_FAST                5 (columns)
                            288 LOAD_FAST                6 (rows)
                            290 LOAD_CONST               1 (('config', 'columns', 'rows'))
                            292 BUILD_CONST_KEY_MAP      3
                
-               468         294 LOAD_GLOBAL             16 (status)
+               467         294 LOAD_GLOBAL             16 (status)
                            306 LOAD_ATTR                9 (HTTP_200_OK)
                
-               467         316 KW_NAMES                 2
+               466         316 KW_NAMES                 2
                            318 PRECALL                  2
                            322 CALL                     2
                            332 RETURN_VALUE
                ExceptionTable:
                  4 to 44 -> 48 [0]
                  48 to 66 -> 134 [1] lasti
                  68 to 122 -> 124 [1] lasti
@@ -2474,372 +2444,368 @@
                   None
                   ('config', 'columns', 'rows')
                   ('status',)
                names      ('get_changelist_instance', 'IncorrectLookupParameters', 'NotFound', 'str', 'get_columns', 'get_rows', 'get_config', 'Response', 'status', 'HTTP_200_OK')
                varnames   ('self', 'request', 'model_admin', 'cl', 'e', 'columns', 'rows', 'config')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'get'
-               firstlineno 459
+               firstlineno 458
                lnotab 0x020102012e01120140ff08022c012c012c01160116ff
             code
                argcount  : 3
                nlocals   : 7
                stacksize : 7
                flags     : 3
                code
                   0x970067007d037c00a00000000000000000000000000000000000000000
                   007c017c02a6020000ab02000000000000000044005d3a7d047403000000
                   000000000000007c047c026a0200000000000000007c026a030000000000
                   0000006401ac02a6040000ab0400000000000000005c0200007d057d067c
                   03a00400000000000000000000000000000000000000007c047c0564039c
                   02a6010000ab01000000000000000001008c3b7c035300
-               470           0 RESUME                   0
+               469           0 RESUME                   0
                
-               474           2 BUILD_LIST               0
+               473           2 BUILD_LIST               0
                              4 STORE_FAST               3 (columns)
                
-               475           6 LOAD_FAST                0 (self)
+               474           6 LOAD_FAST                0 (self)
                              8 LOAD_METHOD              0 (get_fields_list)
                             30 LOAD_FAST                1 (request)
                             32 LOAD_FAST                2 (cl)
                             34 PRECALL                  2
                             38 CALL                     2
                             48 GET_ITER
                        >>   50 FOR_ITER                58 (to 168)
                             52 STORE_FAST               4 (field_name)
                
-               476          54 LOAD_GLOBAL              3 (NULL + label_for_field)
+               475          54 LOAD_GLOBAL              3 (NULL + label_for_field)
                
-               477          66 LOAD_FAST                4 (field_name)
+               476          66 LOAD_FAST                4 (field_name)
                             68 LOAD_FAST                2 (cl)
                             70 LOAD_ATTR                2 (model)
                             80 LOAD_FAST                2 (cl)
                             82 LOAD_ATTR                3 (model_admin)
                             92 LOAD_CONST               1 (True)
                
-               476          94 KW_NAMES                 2
+               475          94 KW_NAMES                 2
                             96 PRECALL                  4
                            100 CALL                     4
                            110 UNPACK_SEQUENCE          2
                            114 STORE_FAST               5 (text)
                            116 STORE_FAST               6 (_)
                
-               478         118 LOAD_FAST                3 (columns)
+               477         118 LOAD_FAST                3 (columns)
                            120 LOAD_METHOD              4 (append)
                            142 LOAD_FAST                4 (field_name)
                            144 LOAD_FAST                5 (text)
                            146 LOAD_CONST               3 (('field', 'headerName'))
                            148 BUILD_CONST_KEY_MAP      2
                            150 PRECALL                  1
                            154 CALL                     1
                            164 POP_TOP
                            166 JUMP_BACKWARD           59 (to 50)
                
-               479     >>  168 LOAD_FAST                3 (columns)
+               478     >>  168 LOAD_FAST                3 (columns)
                            170 RETURN_VALUE
                consts
                   '\n        return changelist columns or headers.\n        '
                   True
                   ('model_admin', 'return_attr')
                   ('field', 'headerName')
                names      ('get_fields_list', 'label_for_field', 'model', 'model_admin', 'append')
                varnames   ('self', 'request', 'cl', 'columns', 'field_name', 'text', '_')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'get_columns'
-               firstlineno 470
+               firstlineno 469
                lnotab 0x0204040130010c011cff18023201
             code
                argcount  : 3
                nlocals   : 15
                stacksize : 7
                flags     : 3
                code
                   0x870f970067007d037c02a0000000000000000000000000000000000000
                   0000007c01a6010000ab01000000000000000001007c026a010000000000
                   000000a0020000000000000000000000000000000000000000a6000000ab
                   0000000000000000007d047c01a003000000000000000000000000000000
                   0000000000a6000000ab0000000000000000007d057c01a0040000000000
                   000000000000000000000000000000a6000000ab00000000000000000072
-                  0264016e0164027d067c026a050000000000000000440090015d617d077c
+                  0264016e0164027d067c026a050000000000000000440090015d5b7d077c
                   026a0100000000000000006a0600000000000000006a0700000000000000
                   007411000000000000000000007c07a6010000ab0100000000000000006a
                   0900000000000000006a0a00000000000000007411000000000000000000
                   007c07a6010000ab0100000000000000006a0900000000000000006a0b00
-                  0000000000000066037d087c067c057a0000007419000000000000000000
-                  0064037c087a06000064047c076a0d000000000000000069017c01ac05a6
-                  030000ab0300000000000000007a0000007c076a0d000000000000000069
-                  0064069c037d097c00a00e00000000000000000000000000000000000000
-                  007c017c02a6020000ab02000000000000000044005dc57d0a0900741f00
-                  0000000000000000007c0a7c077c026a010000000000000000a6030000ab
-                  0300000000000000005c0300007d0b7d0b8a0f890f722574210000000000
-                  0000000000890f742200000000000000000000a6020000ab020000000000
-                  0000007210742500000000000000000000890fa6010000ab010000000000
-                  0000007d0c6e02890f7d0c09007c076a090000000000000000a013000000
-                  00000000000000000000000000000000007c0aa6010000ab010000000000
-                  0000007d0d7429000000000000000000007c0d64076408a6030000ab0300
-                  000000000000007d0e7c0e721a880f6601640984087c0e4400a6000000ab
-                  000000000000000000640a19000000000000000000640b19000000000000
-                  0000007d0c6e102300742a0000000000000000000024007203010059006e
-                  047700780359007701890f64086b020000000072027c047d0c6e12230074
-                  2c000000000000000000002400720501007c047d0c59006e047700780359
-                  0077017c0c7c09640c190000000000000000007c0a3c0000008cc67c03a0
-                  1700000000000000000000000000000000000000007c09a6010000ab0100
-                  00000000000000010090018c637c035300
+                  0000000000000066037d0874190000000000000000000064037c087a0600
+                  0064047c076a0d000000000000000069017c01ac05a6030000ab03000000
+                  00000000007c076a0d0000000000000000690064069c037d097c00a00e00
+                  000000000000000000000000000000000000007c017c02a6020000ab0200
+                  0000000000000044005dc57d0a0900741f000000000000000000007c0a7c
+                  077c026a010000000000000000a6030000ab0300000000000000005c0300
+                  007d0b7d0b8a0f890f7225742100000000000000000000890f7422000000
+                  00000000000000a6020000ab020000000000000000721074250000000000
+                  0000000000890fa6010000ab0100000000000000007d0c6e02890f7d0c09
+                  007c076a090000000000000000a013000000000000000000000000000000
+                  00000000007c0aa6010000ab0100000000000000007d0d74290000000000
+                  00000000007c0d64076408a6030000ab0300000000000000007d0e7c0e72
+                  1a880f6601640984087c0e4400a6000000ab000000000000000000640a19
+                  000000000000000000640b190000000000000000007d0c6e102300742a00
+                  00000000000000000024007203010059006e047700780359007701890f64
+                  086b020000000072027c047d0c6e122300742c0000000000000000000024
+                  00720501007c047d0c59006e0477007803590077017c0c7c09640c190000
+                  000000000000007c0a3c0000008cc67c03a0170000000000000000000000
+                  0000000000000000007c09a6010000ab010000000000000000010090018c
+                  5d7c035300
                              0 MAKE_CELL               15 (value)
                
-               481           2 RESUME                   0
+               480           2 RESUME                   0
                
-               485           4 BUILD_LIST               0
+               484           4 BUILD_LIST               0
                              6 STORE_FAST               3 (rows)
                
-               487           8 LOAD_FAST                2 (cl)
+               486           8 LOAD_FAST                2 (cl)
                             10 LOAD_METHOD              0 (get_results)
                             32 LOAD_FAST                1 (request)
                             34 PRECALL                  1
                             38 CALL                     1
                             48 POP_TOP
                
-               488          50 LOAD_FAST                2 (cl)
+               487          50 LOAD_FAST                2 (cl)
                             52 LOAD_ATTR                1 (model_admin)
                             62 LOAD_METHOD              2 (get_empty_value_display)
                             84 PRECALL                  0
                             88 CALL                     0
                             98 STORE_FAST               4 (empty_value_display)
                
-               489         100 LOAD_FAST                1 (request)
+               488         100 LOAD_FAST                1 (request)
                            102 LOAD_METHOD              3 (get_host)
                            124 PRECALL                  0
                            128 CALL                     0
                            138 STORE_FAST               5 (domain)
                
-               490         140 LOAD_FAST                1 (request)
+               489         140 LOAD_FAST                1 (request)
                            142 LOAD_METHOD              4 (is_secure)
                            164 PRECALL                  0
                            168 CALL                     0
                            178 POP_JUMP_FORWARD_IF_FALSE     2 (to 184)
                            180 LOAD_CONST               1 ('https://')
                            182 JUMP_FORWARD             1 (to 186)
                        >>  184 LOAD_CONST               2 ('http://')
                        >>  186 STORE_FAST               6 (scheme)
                
-               491         188 LOAD_FAST                2 (cl)
+               490         188 LOAD_FAST                2 (cl)
                            190 LOAD_ATTR                5 (result_list)
                            200 GET_ITER
                        >>  202 EXTENDED_ARG             1
-                           204 FOR_ITER               353 (to 912)
+                           204 FOR_ITER               347 (to 900)
                            206 STORE_FAST               7 (result)
                
-               492         208 LOAD_FAST                2 (cl)
+               491         208 LOAD_FAST                2 (cl)
                            210 LOAD_ATTR                1 (model_admin)
                            220 LOAD_ATTR                6 (admin_site)
                            230 LOAD_ATTR                7 (name)
                            240 LOAD_GLOBAL             17 (NULL + type)
                
-               493         252 LOAD_FAST                7 (result)
+               492         252 LOAD_FAST                7 (result)
                
-               492         254 PRECALL                  1
+               491         254 PRECALL                  1
                            258 CALL                     1
                
-               493         268 LOAD_ATTR                9 (_meta)
+               492         268 LOAD_ATTR                9 (_meta)
                            278 LOAD_ATTR               10 (app_label)
                            288 LOAD_GLOBAL             17 (NULL + type)
                            300 LOAD_FAST                7 (result)
                            302 PRECALL                  1
                            306 CALL                     1
                            316 LOAD_ATTR                9 (_meta)
                            326 LOAD_ATTR               11 (model_name)
                
-               492         336 BUILD_TUPLE              3
+               491         336 BUILD_TUPLE              3
                            338 STORE_FAST               8 (model_info)
                
-               495         340 LOAD_FAST                6 (scheme)
-                           342 LOAD_FAST                5 (domain)
-                           344 BINARY_OP                0 (+)
-                           348 LOAD_GLOBAL             25 (NULL + reverse)
-                           360 LOAD_CONST               3 ('%s:%s_%s_change')
-                           362 LOAD_FAST                8 (model_info)
-                           364 BINARY_OP                6 (%)
-                           368 LOAD_CONST               4 ('object_id')
-                           370 LOAD_FAST                7 (result)
-                           372 LOAD_ATTR               13 (pk)
-                           382 BUILD_MAP                1
-                           384 LOAD_FAST                1 (request)
-                           386 KW_NAMES                 5
-                           388 PRECALL                  3
-                           392 CALL                     3
-                           402 BINARY_OP                0 (+)
-               
-               496         406 LOAD_FAST                7 (result)
-                           408 LOAD_ATTR               13 (pk)
-               
-               497         418 BUILD_MAP                0
-               
-               494         420 LOAD_CONST               6 (('change_url', 'id', 'cells'))
-                           422 BUILD_CONST_KEY_MAP      3
-                           424 STORE_FAST               9 (row)
-               
-               500         426 LOAD_FAST                0 (self)
-                           428 LOAD_METHOD             14 (get_fields_list)
-                           450 LOAD_FAST                1 (request)
-                           452 LOAD_FAST                2 (cl)
-                           454 PRECALL                  2
-                           458 CALL                     2
-                           468 GET_ITER
-                       >>  470 FOR_ITER               197 (to 866)
-                           472 STORE_FAST              10 (field_name)
-               
-               501         474 NOP
-               
-               502         476 LOAD_GLOBAL             31 (NULL + lookup_field)
-               
-               503         488 LOAD_FAST               10 (field_name)
-                           490 LOAD_FAST                7 (result)
-                           492 LOAD_FAST                2 (cl)
-                           494 LOAD_ATTR                1 (model_admin)
-               
-               502         504 PRECALL                  3
-                           508 CALL                     3
-                           518 UNPACK_SEQUENCE          3
-                           522 STORE_FAST              11 (_)
-                           524 STORE_FAST              11 (_)
-                           526 STORE_DEREF             15 (value)
-               
-               506         528 LOAD_DEREF              15 (value)
-                           530 POP_JUMP_FORWARD_IF_FALSE    37 (to 606)
-                           532 LOAD_GLOBAL             33 (NULL + isinstance)
-                           544 LOAD_DEREF              15 (value)
-                           546 LOAD_GLOBAL             34 (Model)
-                           558 PRECALL                  2
-                           562 CALL                     2
-                           572 POP_JUMP_FORWARD_IF_FALSE    16 (to 606)
-               
-               507         574 LOAD_GLOBAL             37 (NULL + str)
-                           586 LOAD_DEREF              15 (value)
-                           588 PRECALL                  1
-                           592 CALL                     1
-                           602 STORE_FAST              12 (result_repr)
-                           604 JUMP_FORWARD             2 (to 610)
-               
-               509     >>  606 LOAD_DEREF              15 (value)
-                           608 STORE_FAST              12 (result_repr)
-               
-               512     >>  610 NOP
-               
-               513         612 LOAD_FAST                7 (result)
-                           614 LOAD_ATTR                9 (_meta)
-                           624 LOAD_METHOD             19 (get_field)
-                           646 LOAD_FAST               10 (field_name)
-                           648 PRECALL                  1
-                           652 CALL                     1
-                           662 STORE_FAST              13 (model_field)
-               
-               514         664 LOAD_GLOBAL             41 (NULL + getattr)
-                           676 LOAD_FAST               13 (model_field)
-                           678 LOAD_CONST               7 ('choices')
-                           680 LOAD_CONST               8 (None)
-                           682 PRECALL                  3
-                           686 CALL                     3
-                           696 STORE_FAST              14 (choices)
-               
-               515         698 LOAD_FAST               14 (choices)
-                           700 POP_JUMP_FORWARD_IF_FALSE    26 (to 754)
-               
-               516         702 LOAD_CLOSURE            15 (value)
-                           704 BUILD_TUPLE              1
-                           706 LOAD_CONST               9 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 516>)
-                           708 MAKE_FUNCTION            8 (closure)
-               
-               517         710 LOAD_FAST               14 (choices)
-               
-               516         712 GET_ITER
-                           714 PRECALL                  0
-                           718 CALL                     0
-               
-               518         728 LOAD_CONST              10 (0)
-               
-               516         730 BINARY_SUBSCR
-               
-               518         740 LOAD_CONST              11 (1)
-               
-               516         742 BINARY_SUBSCR
-                           752 STORE_FAST              12 (result_repr)
-                       >>  754 JUMP_FORWARD            16 (to 788)
-                       >>  756 PUSH_EXC_INFO
-               
-               519         758 LOAD_GLOBAL             42 (FieldDoesNotExist)
-                           770 CHECK_EXC_MATCH
-                           772 POP_JUMP_FORWARD_IF_FALSE     3 (to 780)
-                           774 POP_TOP
-               
-               520         776 POP_EXCEPT
-                           778 JUMP_FORWARD             4 (to 788)
-               
-               519     >>  780 RERAISE                  0
-                       >>  782 COPY                     3
-                           784 POP_EXCEPT
-                           786 RERAISE                  1
-               
-               523     >>  788 LOAD_DEREF              15 (value)
-                           790 LOAD_CONST               8 (None)
-                           792 COMPARE_OP               2 (==)
-                           798 POP_JUMP_FORWARD_IF_FALSE     2 (to 804)
-               
-               524         800 LOAD_FAST                4 (empty_value_display)
-                           802 STORE_FAST              12 (result_repr)
-                       >>  804 JUMP_FORWARD            18 (to 842)
-                       >>  806 PUSH_EXC_INFO
-               
-               526         808 LOAD_GLOBAL             44 (ObjectDoesNotExist)
-                           820 CHECK_EXC_MATCH
-                           822 POP_JUMP_FORWARD_IF_FALSE     5 (to 834)
-                           824 POP_TOP
-               
-               527         826 LOAD_FAST                4 (empty_value_display)
-                           828 STORE_FAST              12 (result_repr)
-                           830 POP_EXCEPT
-                           832 JUMP_FORWARD             4 (to 842)
-               
-               526     >>  834 RERAISE                  0
-                       >>  836 COPY                     3
-                           838 POP_EXCEPT
-                           840 RERAISE                  1
-               
-               529     >>  842 LOAD_FAST               12 (result_repr)
-                           844 LOAD_FAST                9 (row)
-                           846 LOAD_CONST              12 ('cells')
-                           848 BINARY_SUBSCR
-                           858 LOAD_FAST               10 (field_name)
-                           860 STORE_SUBSCR
-                           864 JUMP_BACKWARD          198 (to 470)
-               
-               530     >>  866 LOAD_FAST                3 (rows)
-                           868 LOAD_METHOD             23 (append)
-                           890 LOAD_FAST                9 (row)
-                           892 PRECALL                  1
-                           896 CALL                     1
-                           906 POP_TOP
-                           908 EXTENDED_ARG             1
-                           910 JUMP_BACKWARD          355 (to 202)
+               494         340 LOAD_GLOBAL             25 (NULL + reverse)
+                           352 LOAD_CONST               3 ('%s:%s_%s_change')
+                           354 LOAD_FAST                8 (model_info)
+                           356 BINARY_OP                6 (%)
+                           360 LOAD_CONST               4 ('object_id')
+                           362 LOAD_FAST                7 (result)
+                           364 LOAD_ATTR               13 (pk)
+                           374 BUILD_MAP                1
+                           376 LOAD_FAST                1 (request)
+                           378 KW_NAMES                 5
+                           380 PRECALL                  3
+                           384 CALL                     3
+               
+               495         394 LOAD_FAST                7 (result)
+                           396 LOAD_ATTR               13 (pk)
+               
+               496         406 BUILD_MAP                0
+               
+               493         408 LOAD_CONST               6 (('change_url', 'id', 'cells'))
+                           410 BUILD_CONST_KEY_MAP      3
+                           412 STORE_FAST               9 (row)
+               
+               499         414 LOAD_FAST                0 (self)
+                           416 LOAD_METHOD             14 (get_fields_list)
+                           438 LOAD_FAST                1 (request)
+                           440 LOAD_FAST                2 (cl)
+                           442 PRECALL                  2
+                           446 CALL                     2
+                           456 GET_ITER
+                       >>  458 FOR_ITER               197 (to 854)
+                           460 STORE_FAST              10 (field_name)
+               
+               500         462 NOP
+               
+               501         464 LOAD_GLOBAL             31 (NULL + lookup_field)
+               
+               502         476 LOAD_FAST               10 (field_name)
+                           478 LOAD_FAST                7 (result)
+                           480 LOAD_FAST                2 (cl)
+                           482 LOAD_ATTR                1 (model_admin)
+               
+               501         492 PRECALL                  3
+                           496 CALL                     3
+                           506 UNPACK_SEQUENCE          3
+                           510 STORE_FAST              11 (_)
+                           512 STORE_FAST              11 (_)
+                           514 STORE_DEREF             15 (value)
+               
+               505         516 LOAD_DEREF              15 (value)
+                           518 POP_JUMP_FORWARD_IF_FALSE    37 (to 594)
+                           520 LOAD_GLOBAL             33 (NULL + isinstance)
+                           532 LOAD_DEREF              15 (value)
+                           534 LOAD_GLOBAL             34 (Model)
+                           546 PRECALL                  2
+                           550 CALL                     2
+                           560 POP_JUMP_FORWARD_IF_FALSE    16 (to 594)
+               
+               506         562 LOAD_GLOBAL             37 (NULL + str)
+                           574 LOAD_DEREF              15 (value)
+                           576 PRECALL                  1
+                           580 CALL                     1
+                           590 STORE_FAST              12 (result_repr)
+                           592 JUMP_FORWARD             2 (to 598)
+               
+               508     >>  594 LOAD_DEREF              15 (value)
+                           596 STORE_FAST              12 (result_repr)
+               
+               511     >>  598 NOP
+               
+               512         600 LOAD_FAST                7 (result)
+                           602 LOAD_ATTR                9 (_meta)
+                           612 LOAD_METHOD             19 (get_field)
+                           634 LOAD_FAST               10 (field_name)
+                           636 PRECALL                  1
+                           640 CALL                     1
+                           650 STORE_FAST              13 (model_field)
+               
+               513         652 LOAD_GLOBAL             41 (NULL + getattr)
+                           664 LOAD_FAST               13 (model_field)
+                           666 LOAD_CONST               7 ('choices')
+                           668 LOAD_CONST               8 (None)
+                           670 PRECALL                  3
+                           674 CALL                     3
+                           684 STORE_FAST              14 (choices)
+               
+               514         686 LOAD_FAST               14 (choices)
+                           688 POP_JUMP_FORWARD_IF_FALSE    26 (to 742)
+               
+               515         690 LOAD_CLOSURE            15 (value)
+                           692 BUILD_TUPLE              1
+                           694 LOAD_CONST               9 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 515>)
+                           696 MAKE_FUNCTION            8 (closure)
+               
+               516         698 LOAD_FAST               14 (choices)
+               
+               515         700 GET_ITER
+                           702 PRECALL                  0
+                           706 CALL                     0
+               
+               517         716 LOAD_CONST              10 (0)
+               
+               515         718 BINARY_SUBSCR
+               
+               517         728 LOAD_CONST              11 (1)
+               
+               515         730 BINARY_SUBSCR
+                           740 STORE_FAST              12 (result_repr)
+                       >>  742 JUMP_FORWARD            16 (to 776)
+                       >>  744 PUSH_EXC_INFO
+               
+               518         746 LOAD_GLOBAL             42 (FieldDoesNotExist)
+                           758 CHECK_EXC_MATCH
+                           760 POP_JUMP_FORWARD_IF_FALSE     3 (to 768)
+                           762 POP_TOP
+               
+               519         764 POP_EXCEPT
+                           766 JUMP_FORWARD             4 (to 776)
+               
+               518     >>  768 RERAISE                  0
+                       >>  770 COPY                     3
+                           772 POP_EXCEPT
+                           774 RERAISE                  1
+               
+               522     >>  776 LOAD_DEREF              15 (value)
+                           778 LOAD_CONST               8 (None)
+                           780 COMPARE_OP               2 (==)
+                           786 POP_JUMP_FORWARD_IF_FALSE     2 (to 792)
+               
+               523         788 LOAD_FAST                4 (empty_value_display)
+                           790 STORE_FAST              12 (result_repr)
+                       >>  792 JUMP_FORWARD            18 (to 830)
+                       >>  794 PUSH_EXC_INFO
+               
+               525         796 LOAD_GLOBAL             44 (ObjectDoesNotExist)
+                           808 CHECK_EXC_MATCH
+                           810 POP_JUMP_FORWARD_IF_FALSE     5 (to 822)
+                           812 POP_TOP
+               
+               526         814 LOAD_FAST                4 (empty_value_display)
+                           816 STORE_FAST              12 (result_repr)
+                           818 POP_EXCEPT
+                           820 JUMP_FORWARD             4 (to 830)
+               
+               525     >>  822 RERAISE                  0
+                       >>  824 COPY                     3
+                           826 POP_EXCEPT
+                           828 RERAISE                  1
+               
+               528     >>  830 LOAD_FAST               12 (result_repr)
+                           832 LOAD_FAST                9 (row)
+                           834 LOAD_CONST              12 ('cells')
+                           836 BINARY_SUBSCR
+                           846 LOAD_FAST               10 (field_name)
+                           848 STORE_SUBSCR
+                           852 JUMP_BACKWARD          198 (to 458)
+               
+               529     >>  854 LOAD_FAST                3 (rows)
+                           856 LOAD_METHOD             23 (append)
+                           878 LOAD_FAST                9 (row)
+                           880 PRECALL                  1
+                           884 CALL                     1
+                           894 POP_TOP
+                           896 EXTENDED_ARG             1
+                           898 JUMP_BACKWARD          349 (to 202)
                
-               531     >>  912 LOAD_FAST                3 (rows)
-                           914 RETURN_VALUE
+               530     >>  900 LOAD_FAST                3 (rows)
+                           902 RETURN_VALUE
                ExceptionTable:
-                 476 to 608 -> 806 [2]
-                 612 to 752 -> 756 [2]
-                 754 to 754 -> 806 [2]
-                 756 to 774 -> 782 [3] lasti
-                 776 to 778 -> 806 [2]
-                 780 to 780 -> 782 [3] lasti
-                 782 to 802 -> 806 [2]
-                 806 to 828 -> 836 [3] lasti
-                 834 to 834 -> 836 [3] lasti
+                 464 to 596 -> 794 [2]
+                 600 to 740 -> 744 [2]
+                 742 to 742 -> 794 [2]
+                 744 to 762 -> 770 [3] lasti
+                 764 to 766 -> 794 [2]
+                 768 to 768 -> 770 [3] lasti
+                 770 to 790 -> 794 [2]
+                 794 to 816 -> 824 [3] lasti
+                 822 to 822 -> 824 [3] lasti
                consts
                   '\n        Return changelist rows actual list of data.\n        '
                   'https://'
                   'http://'
                   '%s:%s_%s_change'
                   'object_id'
                   ('kwargs', 'request')
@@ -2852,20 +2818,20 @@
                      stacksize : 4
                      flags     : 19
                      code
                         0x9501970067007c005d107d017c0164001900000000000000000089026b
                         0200000000af0e7c0191028c115300
                                    0 COPY_FREE_VARS           1
                      
-                     516           2 RESUME                   0
+                     515           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                16 (to 42)
                      
-                     517          10 STORE_FAST               1 (choice)
+                     516          10 STORE_FAST               1 (choice)
                                   12 LOAD_FAST                1 (choice)
                                   14 LOAD_CONST               0 (0)
                                   16 BINARY_SUBSCR
                                   26 LOAD_DEREF               2 (value)
                                   28 COMPARE_OP               2 (==)
                                   34 POP_JUMP_BACKWARD_IF_FALSE    14 (to 8)
                                   36 LOAD_FAST                1 (choice)
@@ -2874,30 +2840,30 @@
                              >>   42 RETURN_VALUE
                      consts
                         0
                      names      ()
                      varnames   ('.0', 'choice')
                      freevars   ('value',)
                      cellvars   ()
-                     filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+                     filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                      name       '<listcomp>'
-                     firstlineno 516
+                     firstlineno 515
                      lnotab 0x0a01
                   0
                   1
                   'cells'
                names      ('get_results', 'model_admin', 'get_empty_value_display', 'get_host', 'is_secure', 'result_list', 'admin_site', 'name', 'type', '_meta', 'app_label', 'model_name', 'reverse', 'pk', 'get_fields_list', 'lookup_field', 'isinstance', 'Model', 'str', 'get_field', 'getattr', 'FieldDoesNotExist', 'ObjectDoesNotExist', 'append')
                varnames   ('self', 'request', 'cl', 'rows', 'empty_value_display', 'domain', 'scheme', 'result', 'model_info', 'row', 'field_name', '_', 'result_repr', 'model_field', 'choices')
                freevars   ()
                cellvars   ('value',)
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'get_rows'
-               firstlineno 481
+               firstlineno 480
                lnotab
-                  0x040404022a0132012801300114012c0102ff0e0144ff040342010c0102
+                  0x040404022a0132012801300114012c0102ff0e0144ff040336010c0102
                   fd0606300102010c0110ff18042e01200204030201340122010401080102
                   ff100202fe0a0202fe1003120104ff08040c010802120108ff080318012e
                   01
             code
                argcount  : 3
                nlocals   : 14
                stacksize : 6
@@ -2924,203 +2890,203 @@
                   020000ab0200000000000000007d0a02007c0aa6000000ab000000000000
                   0000007d0b741d000000000000000000007c0ba6010000ab010000000000
                   0000007d0c7c0c44005d1c7d0d7c0d64091900000000000000000089026a
                   0f00000000000000007600720b7c0d7c097c0d6409190000000000000000
                   003c0000008c1d7c097c03640a3c0000007c035300
                              0 MAKE_CELL                2 (cl)
                
-               533           2 RESUME                   0
+               532           2 RESUME                   0
                
-               534           4 BUILD_MAP                0
+               533           4 BUILD_MAP                0
                              6 STORE_FAST               3 (config)
                
-               537           8 LOAD_DEREF               2 (cl)
+               536           8 LOAD_DEREF               2 (cl)
                             10 LOAD_ATTR                0 (model_admin)
                             20 LOAD_ATTR                1 (changelist_options)
                             30 GET_ITER
                        >>   32 FOR_ITER                27 (to 88)
                             34 STORE_FAST               4 (option_name)
                
-               538          36 LOAD_GLOBAL              5 (NULL + getattr)
+               537          36 LOAD_GLOBAL              5 (NULL + getattr)
                             48 LOAD_DEREF               2 (cl)
                             50 LOAD_ATTR                0 (model_admin)
                             60 LOAD_FAST                4 (option_name)
                             62 LOAD_CONST               0 (None)
                             64 PRECALL                  3
                             68 CALL                     3
                             78 LOAD_FAST                3 (config)
                             80 LOAD_FAST                4 (option_name)
                             82 STORE_SUBSCR
                             86 JUMP_BACKWARD           28 (to 32)
                
-               541     >>   88 LOAD_DEREF               2 (cl)
+               540     >>   88 LOAD_DEREF               2 (cl)
                             90 LOAD_ATTR                3 (full_result_count)
                            100 LOAD_FAST                3 (config)
                            102 LOAD_CONST               1 ('full_count')
                            104 STORE_SUBSCR
                
-               542         108 LOAD_DEREF               2 (cl)
+               541         108 LOAD_DEREF               2 (cl)
                            110 LOAD_ATTR                4 (result_count)
                            120 LOAD_FAST                3 (config)
                            122 LOAD_CONST               2 ('result_count')
                            124 STORE_SUBSCR
                
-               545         128 LOAD_DEREF               2 (cl)
+               544         128 LOAD_DEREF               2 (cl)
                            130 LOAD_ATTR                0 (model_admin)
                            140 LOAD_METHOD              5 (get_action_choices)
                
-               546         162 LOAD_FAST                1 (request)
+               545         162 LOAD_FAST                1 (request)
                            164 BUILD_LIST               0
                
-               545         166 PRECALL                  2
+               544         166 PRECALL                  2
                            170 CALL                     2
                            180 LOAD_FAST                3 (config)
                            182 LOAD_CONST               3 ('action_choices')
                            184 STORE_SUBSCR
                
-               549         188 LOAD_DEREF               2 (cl)
+               548         188 LOAD_DEREF               2 (cl)
                            190 LOAD_METHOD              6 (get_filters)
                            212 LOAD_FAST                1 (request)
                            214 PRECALL                  1
                            218 CALL                     1
                            228 UNPACK_SEQUENCE          5
                            232 STORE_FAST               5 (filters_spec)
                            234 STORE_FAST               6 (_)
                            236 STORE_FAST               6 (_)
                            238 STORE_FAST               6 (_)
                            240 STORE_FAST               6 (_)
                
-               550         242 LOAD_FAST                5 (filters_spec)
+               549         242 LOAD_FAST                5 (filters_spec)
                            244 POP_JUMP_FORWARD_IF_FALSE    18 (to 282)
                
-               551         246 LOAD_CLOSURE             2 (cl)
+               550         246 LOAD_CLOSURE             2 (cl)
                            248 BUILD_TUPLE              1
-                           250 LOAD_CONST               4 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 551>)
+                           250 LOAD_CONST               4 (<code object <listcomp>, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 550>)
                            252 MAKE_FUNCTION            8 (closure)
                
-               552         254 LOAD_FAST                5 (filters_spec)
+               551         254 LOAD_FAST                5 (filters_spec)
                
-               551         256 GET_ITER
+               550         256 GET_ITER
                            258 PRECALL                  0
                            262 CALL                     0
                            272 LOAD_FAST                3 (config)
                            274 LOAD_CONST               5 ('filters')
                            276 STORE_SUBSCR
                            280 JUMP_FORWARD             5 (to 292)
                
-               554     >>  282 BUILD_LIST               0
+               553     >>  282 BUILD_LIST               0
                            284 LOAD_FAST                3 (config)
                            286 LOAD_CONST               5 ('filters')
                            288 STORE_SUBSCR
                
-               557     >>  292 BUILD_LIST               0
+               556     >>  292 BUILD_LIST               0
                            294 STORE_FAST               7 (list_display_fields)
                
-               558         296 LOAD_FAST                0 (self)
+               557         296 LOAD_FAST                0 (self)
                            298 LOAD_METHOD              7 (get_fields_list)
                            320 LOAD_FAST                1 (request)
                            322 LOAD_DEREF               2 (cl)
                            324 PRECALL                  2
                            328 CALL                     2
                            338 GET_ITER
                        >>  340 FOR_ITER                71 (to 484)
                            342 STORE_FAST               8 (field_name)
                
-               559         344 NOP
+               558         344 NOP
                
-               560         346 LOAD_DEREF               2 (cl)
+               559         346 LOAD_DEREF               2 (cl)
                            348 LOAD_ATTR                8 (model)
                            358 LOAD_ATTR                9 (_meta)
                            368 LOAD_METHOD             10 (get_field)
                            390 LOAD_FAST                8 (field_name)
                            392 PRECALL                  1
                            396 CALL                     1
                            406 POP_TOP
                
-               561         408 LOAD_FAST                7 (list_display_fields)
+               560         408 LOAD_FAST                7 (list_display_fields)
                            410 LOAD_METHOD             11 (append)
                            432 LOAD_FAST                8 (field_name)
                            434 PRECALL                  1
                            438 CALL                     1
                            448 POP_TOP
                            450 JUMP_BACKWARD           56 (to 340)
                        >>  452 PUSH_EXC_INFO
                
-               562         454 LOAD_GLOBAL             24 (FieldDoesNotExist)
+               561         454 LOAD_GLOBAL             24 (FieldDoesNotExist)
                            466 CHECK_EXC_MATCH
                            468 POP_JUMP_FORWARD_IF_FALSE     3 (to 476)
                            470 POP_TOP
                
-               563         472 POP_EXCEPT
+               562         472 POP_EXCEPT
                            474 JUMP_BACKWARD           68 (to 340)
                
-               562     >>  476 RERAISE                  0
+               561     >>  476 RERAISE                  0
                        >>  478 COPY                     3
                            480 POP_EXCEPT
                            482 RERAISE                  1
                
-               564     >>  484 LOAD_FAST                7 (list_display_fields)
+               563     >>  484 LOAD_FAST                7 (list_display_fields)
                            486 LOAD_FAST                3 (config)
                            488 LOAD_CONST               6 ('list_display_fields')
                            490 STORE_SUBSCR
                
-               567         494 BUILD_MAP                0
+               566         494 BUILD_MAP                0
                            496 STORE_FAST               9 (editing_fields)
                
-               568         498 LOAD_DEREF               2 (cl)
+               567         498 LOAD_DEREF               2 (cl)
                            500 LOAD_ATTR                0 (model_admin)
                            510 LOAD_METHOD             13 (get_serializer_class)
                
-               569         532 LOAD_FAST                1 (request)
+               568         532 LOAD_FAST                1 (request)
                            534 LOAD_CONST               7 (True)
                
-               568         536 KW_NAMES                 8
+               567         536 KW_NAMES                 8
                            538 PRECALL                  2
                            542 CALL                     2
                            552 STORE_FAST              10 (serializer_class)
                
-               570         554 PUSH_NULL
+               569         554 PUSH_NULL
                            556 LOAD_FAST               10 (serializer_class)
                            558 PRECALL                  0
                            562 CALL                     0
                            572 STORE_FAST              11 (serializer)
                
-               571         574 LOAD_GLOBAL             29 (NULL + get_form_fields)
+               570         574 LOAD_GLOBAL             29 (NULL + get_form_fields)
                            586 LOAD_FAST               11 (serializer)
                            588 PRECALL                  1
                            592 CALL                     1
                            602 STORE_FAST              12 (form_fields)
                
-               573         604 LOAD_FAST               12 (form_fields)
+               572         604 LOAD_FAST               12 (form_fields)
                            606 GET_ITER
                        >>  608 FOR_ITER                28 (to 666)
                            610 STORE_FAST              13 (field)
                
-               574         612 LOAD_FAST               13 (field)
+               573         612 LOAD_FAST               13 (field)
                            614 LOAD_CONST               9 ('name')
                            616 BINARY_SUBSCR
                            626 LOAD_DEREF               2 (cl)
                            628 LOAD_ATTR               15 (list_editable)
                            638 CONTAINS_OP              0
                            640 POP_JUMP_FORWARD_IF_FALSE    11 (to 664)
                
-               575         642 LOAD_FAST               13 (field)
+               574         642 LOAD_FAST               13 (field)
                            644 LOAD_FAST                9 (editing_fields)
                            646 LOAD_FAST               13 (field)
                            648 LOAD_CONST               9 ('name')
                            650 BINARY_SUBSCR
                            660 STORE_SUBSCR
                        >>  664 JUMP_BACKWARD           29 (to 608)
                
-               577     >>  666 LOAD_FAST                9 (editing_fields)
+               576     >>  666 LOAD_FAST                9 (editing_fields)
                            668 LOAD_FAST                3 (config)
                            670 LOAD_CONST              10 ('editing_fields')
                            672 STORE_SUBSCR
                
-               579         676 LOAD_FAST                3 (config)
+               578         676 LOAD_FAST                3 (config)
                            678 RETURN_VALUE
                ExceptionTable:
                  346 to 448 -> 452 [1]
                  452 to 470 -> 478 [2] lasti
                  476 to 476 -> 478 [2] lasti
                consts
                   None
@@ -3134,56 +3100,56 @@
                      flags     : 19
                      code
                         0x9501970067007c005d1f7d017c016a0000000000000000007c01a00100
                         000000000000000000000000000000000000008902a6010000ab01000000
                         000000000064009c0291028c205300
                                    0 COPY_FREE_VARS           1
                      
-                     551           2 RESUME                   0
+                     550           2 RESUME                   0
                                    4 BUILD_LIST               0
                                    6 LOAD_FAST                0 (.0)
                              >>    8 FOR_ITER                31 (to 72)
                      
-                     552          10 STORE_FAST               1 (filter)
+                     551          10 STORE_FAST               1 (filter)
                                   12 LOAD_FAST                1 (filter)
                                   14 LOAD_ATTR                0 (title)
                                   24 LOAD_FAST                1 (filter)
                                   26 LOAD_METHOD              1 (choices)
                                   48 LOAD_DEREF               2 (cl)
                                   50 PRECALL                  1
                                   54 CALL                     1
                                   64 LOAD_CONST               0 (('title', 'choices'))
                                   66 BUILD_CONST_KEY_MAP      2
                      
-                     551          68 LIST_APPEND              2
+                     550          68 LIST_APPEND              2
                                   70 JUMP_BACKWARD           32 (to 8)
                              >>   72 RETURN_VALUE
                      consts
                         ('title', 'choices')
                      names      ('title', 'choices')
                      varnames   ('.0', 'filter')
                      freevars   ('cl',)
                      cellvars   ()
-                     filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+                     filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                      name       '<listcomp>'
-                     firstlineno 551
+                     firstlineno 550
                      lnotab 0x0a013aff
                   'filters'
                   'list_display_fields'
                   True
                   ('changelist',)
                   'name'
                   'editing_fields'
                names      ('model_admin', 'changelist_options', 'getattr', 'full_result_count', 'result_count', 'get_action_choices', 'get_filters', 'get_fields_list', 'model', '_meta', 'get_field', 'append', 'FieldDoesNotExist', 'get_serializer_class', 'get_form_fields', 'list_editable')
                varnames   ('self', 'request', 'cl', 'config', 'option_name', 'filters_spec', '_', 'list_display_fields', 'field_name', 'editing_fields', 'serializer_class', 'serializer', 'form_fields', 'field')
                freevars   ()
                cellvars   ('cl',)
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'get_config'
-               firstlineno 533
+               firstlineno 532
                lnotab
                   0x040104031c01340314011403220104ff160436010401080102ff1a030a
                   030401300102013e012e01120104ff08020a030401220104ff120214011e
                   0208011e0118020a02
             code
                argcount  : 3
                nlocals   : 5
@@ -3194,121 +3160,121 @@
                   0000000000000000007c01a6010000ab0100000000000000007d037c026a
                   0000000000000000006a020000000000000000700d740700000000000000
                   000000a6000000ab0000000000000000008a057407000000000000000000
                   0074090000000000000000000088056601640184087c03a6020000ab0200
                   00000000000000a6010000ab0100000000000000007d047c045300
                              0 MAKE_CELL                5 (exclude)
                
-               581           2 RESUME                   0
+               580           2 RESUME                   0
                
-               582           4 LOAD_FAST                2 (cl)
+               581           4 LOAD_FAST                2 (cl)
                              6 LOAD_ATTR                0 (model_admin)
                             16 LOAD_METHOD              1 (get_list_display)
                             38 LOAD_FAST                1 (request)
                             40 PRECALL                  1
                             44 CALL                     1
                             54 STORE_FAST               3 (list_display)
                
-               583          56 LOAD_FAST                2 (cl)
+               582          56 LOAD_FAST                2 (cl)
                             58 LOAD_ATTR                0 (model_admin)
                             68 LOAD_ATTR                2 (exclude)
                             78 JUMP_IF_TRUE_OR_POP     13 (to 106)
                             80 LOAD_GLOBAL              7 (NULL + tuple)
                             92 PRECALL                  0
                             96 CALL                     0
                        >>  106 STORE_DEREF              5 (exclude)
                
-               584         108 LOAD_GLOBAL              7 (NULL + tuple)
+               583         108 LOAD_GLOBAL              7 (NULL + tuple)
                
-               585         120 LOAD_GLOBAL              9 (NULL + filter)
+               584         120 LOAD_GLOBAL              9 (NULL + filter)
                            132 LOAD_CLOSURE             5 (exclude)
                            134 BUILD_TUPLE              1
-                           136 LOAD_CONST               1 (<code object <lambda>, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 585>)
+                           136 LOAD_CONST               1 (<code object <lambda>, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 584>)
                            138 MAKE_FUNCTION            8 (closure)
                            140 LOAD_FAST                3 (list_display)
                            142 PRECALL                  2
                            146 CALL                     2
                
-               584         156 PRECALL                  1
+               583         156 PRECALL                  1
                            160 CALL                     1
                            170 STORE_FAST               4 (fields_list)
                
-               586         172 LOAD_FAST                4 (fields_list)
+               585         172 LOAD_FAST                4 (fields_list)
                            174 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 2
                      flags     : 19
                      code 0x950197007c00890176015300
                                    0 COPY_FREE_VARS           1
                      
-                     585           2 RESUME                   0
+                     584           2 RESUME                   0
                                    4 LOAD_FAST                0 (item)
                                    6 LOAD_DEREF               1 (exclude)
                                    8 CONTAINS_OP              1
                                   10 RETURN_VALUE
                      consts
                         None
                      names      ()
                      varnames   ('item',)
                      freevars   ('exclude',)
                      cellvars   ()
-                     filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+                     filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                      name       '<lambda>'
-                     firstlineno 585
+                     firstlineno 584
                      lnotab 0x
                names      ('model_admin', 'get_list_display', 'exclude', 'tuple', 'filter')
                varnames   ('self', 'request', 'cl', 'list_display', 'fields_list')
                freevars   ()
                cellvars   ('exclude',)
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'get_fields_list'
-               firstlineno 581
+               firstlineno 580
                lnotab 0x0401340134010c0124ff1002
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'permission_classes', 'get', 'get_columns', 'get_rows', 'get_config', 'get_fields_list')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
          name       'ChangeListView'
-         firstlineno 402
+         firstlineno 401
          lnotab 0x0a0104360402060b060b06340630
       'ChangeListView'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0367005a0464025a05640384005a0664
             0484005a0764025300
-         589           0 RESUME                   0
+         588           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('HandleActionView')
                        8 STORE_NAME               2 (__qualname__)
          
-         590          10 LOAD_CONST               1 ("\n        Preform admin actions using json.\n        json object would look like:\n        {\n        action: 'delete_selected',\n        selected_ids: [\n                1,\n                2,\n                3\n            ],\n        select_across: false\n        }\n    ")
+         589          10 LOAD_CONST               1 ("\n        Preform admin actions using json.\n        json object would look like:\n        {\n        action: 'delete_selected',\n        selected_ids: [\n                1,\n                2,\n                3\n            ],\n        select_across: false\n        }\n    ")
                       12 STORE_NAME               3 (__doc__)
          
-         603          14 BUILD_LIST               0
+         602          14 BUILD_LIST               0
                       16 STORE_NAME               4 (permission_classes)
          
-         604          18 LOAD_CONST               2 (None)
+         603          18 LOAD_CONST               2 (None)
                       20 STORE_NAME               5 (serializer_class)
          
-         606          22 LOAD_CONST               3 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 606>)
+         605          22 LOAD_CONST               3 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 605>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               6 (get)
          
-         611          28 LOAD_CONST               4 (<code object post, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 611>)
+         610          28 LOAD_CONST               4 (<code object post, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 610>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               7 (post)
                       34 LOAD_CONST               2 (None)
                       36 RETURN_VALUE
          consts
             'HandleActionView'
             "\n        Preform admin actions using json.\n        json object would look like:\n        {\n        action: 'delete_selected',\n        selected_ids: [\n                1,\n                2,\n                3\n            ],\n        select_across: false\n        }\n    "
@@ -3320,29 +3286,29 @@
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab0000000000000000007d037403000000000000000000007c03a60100
                   00ab0100000000000000007d0474050000000000000000000064017c0469
                   017406000000000000000000006a040000000000000000ac02a6020000ab
                   0200000000000000005300
-               606           0 RESUME                   0
+               605           0 RESUME                   0
                
-               607           2 LOAD_FAST                0 (self)
+               606           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (serializer_class)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 STORE_FAST               3 (serializer)
                
-               608          42 LOAD_GLOBAL              3 (NULL + get_form_fields)
+               607          42 LOAD_GLOBAL              3 (NULL + get_form_fields)
                             54 LOAD_FAST                3 (serializer)
                             56 PRECALL                  1
                             60 CALL                     1
                             70 STORE_FAST               4 (form_fields)
                
-               609          72 LOAD_GLOBAL              5 (NULL + Response)
+               608          72 LOAD_GLOBAL              5 (NULL + Response)
                             84 LOAD_CONST               1 ('fields')
                             86 LOAD_FAST                4 (form_fields)
                             88 BUILD_MAP                1
                             90 LOAD_GLOBAL              6 (status)
                            102 LOAD_ATTR                4 (HTTP_200_OK)
                            112 KW_NAMES                 2
                            114 PRECALL                  2
@@ -3352,17 +3318,17 @@
                   None
                   'fields'
                   ('status',)
                names      ('serializer_class', 'get_form_fields', 'Response', 'status', 'HTTP_200_OK')
                varnames   ('self', 'request', 'admin', 'serializer', 'form_fields')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'get'
-               firstlineno 606
+               firstlineno 605
                lnotab 0x020128011e01
             code
                argcount  : 3
                nlocals   : 13
                stacksize : 6
                flags     : 3
                code
@@ -3390,175 +3356,175 @@
                   09a6010000ab0100000000000000007d0902007c067c027c017c09a60300
                   00ab0300000000000000007d0c7c0c72027c0c5300741700000000000000
                   000000640aa6010000ab0100000000000000007d0b741900000000000000
                   00000064077c0b6901741a000000000000000000006a1000000000000000
                   00ac08a6020000ab02000000000000000053007419000000000000000000
                   007c036a110000000000000000741a000000000000000000006a0e000000
                   0000000000ac08a6020000ab0200000000000000005300
-               611           0 RESUME                   0
+               610           0 RESUME                   0
                
-               612           2 LOAD_FAST                0 (self)
+               611           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (serializer_class)
                             26 LOAD_FAST                1 (request)
                             28 LOAD_ATTR                1 (data)
                             38 KW_NAMES                 1
                             40 PRECALL                  1
                             44 CALL                     1
                             54 STORE_FAST               3 (serializer)
                
-               614          56 LOAD_FAST                3 (serializer)
+               613          56 LOAD_FAST                3 (serializer)
                             58 LOAD_METHOD              2 (is_valid)
                             80 PRECALL                  0
                             84 CALL                     0
                             94 EXTENDED_ARG             1
                             96 POP_JUMP_FORWARD_IF_FALSE   335 (to 768)
                
-               616          98 LOAD_FAST                3 (serializer)
+               615          98 LOAD_FAST                3 (serializer)
                            100 LOAD_ATTR                3 (validated_data)
                            110 LOAD_METHOD              4 (get)
                            132 LOAD_CONST               2 ('action')
                            134 PRECALL                  1
                            138 CALL                     1
                            148 STORE_FAST               4 (action)
                
-               617         150 LOAD_FAST                3 (serializer)
+               616         150 LOAD_FAST                3 (serializer)
                            152 LOAD_ATTR                3 (validated_data)
                            162 LOAD_METHOD              4 (get)
                            184 LOAD_CONST               3 ('select_across')
                            186 PRECALL                  1
                            190 CALL                     1
                            200 STORE_FAST               5 (select_across)
                
-               618         202 LOAD_FAST                2 (model_admin)
+               617         202 LOAD_FAST                2 (model_admin)
                            204 LOAD_METHOD              5 (get_actions)
                            226 LOAD_FAST                1 (request)
                            228 PRECALL                  1
                            232 CALL                     1
                            242 LOAD_FAST                4 (action)
                            244 BINARY_SUBSCR
                            254 LOAD_CONST               4 (0)
                            256 BINARY_SUBSCR
                            266 STORE_FAST               6 (func)
                
-               619         268 NOP
+               618         268 NOP
                
-               620         270 LOAD_FAST                2 (model_admin)
+               619         270 LOAD_FAST                2 (model_admin)
                            272 LOAD_METHOD              6 (get_changelist_instance)
                            294 LOAD_FAST                1 (request)
                            296 PRECALL                  1
                            300 CALL                     1
                            310 STORE_FAST               7 (cl)
                            312 JUMP_FORWARD            46 (to 406)
                        >>  314 PUSH_EXC_INFO
                
-               621         316 LOAD_GLOBAL             14 (IncorrectLookupParameters)
+               620         316 LOAD_GLOBAL             14 (IncorrectLookupParameters)
                            328 CHECK_EXC_MATCH
                            330 POP_JUMP_FORWARD_IF_FALSE    33 (to 398)
                            332 STORE_FAST               8 (e)
                
-               622         334 LOAD_GLOBAL             17 (NULL + NotFound)
+               621         334 LOAD_GLOBAL             17 (NULL + NotFound)
                            346 LOAD_GLOBAL             19 (NULL + str)
                            358 LOAD_FAST                8 (e)
                            360 PRECALL                  1
                            364 CALL                     1
                            374 PRECALL                  1
                            378 CALL                     1
                            388 RAISE_VARARGS            1
                        >>  390 LOAD_CONST               0 (None)
                            392 STORE_FAST               8 (e)
                            394 DELETE_FAST              8 (e)
                            396 RERAISE                  1
                
-               621     >>  398 RERAISE                  0
+               620     >>  398 RERAISE                  0
                        >>  400 COPY                     3
                            402 POP_EXCEPT
                            404 RERAISE                  1
                
-               623     >>  406 LOAD_FAST                7 (cl)
+               622     >>  406 LOAD_FAST                7 (cl)
                            408 LOAD_METHOD             10 (get_queryset)
                            430 LOAD_FAST                1 (request)
                            432 PRECALL                  1
                            436 CALL                     1
                            446 STORE_FAST               9 (queryset)
                
-               626         448 LOAD_FAST                1 (request)
+               625         448 LOAD_FAST                1 (request)
                            450 LOAD_ATTR                1 (data)
                            460 LOAD_METHOD              4 (get)
                            482 LOAD_CONST               5 ('selected_ids')
                            484 LOAD_CONST               0 (None)
                            486 PRECALL                  2
                            490 CALL                     2
                            500 STORE_FAST              10 (selected)
                
-               627         502 LOAD_FAST               10 (selected)
+               626         502 LOAD_FAST               10 (selected)
                            504 POP_JUMP_FORWARD_IF_TRUE    46 (to 598)
                            506 LOAD_FAST                5 (select_across)
                            508 POP_JUMP_FORWARD_IF_TRUE    44 (to 598)
                
-               628         510 LOAD_GLOBAL             23 (NULL + _)
+               627         510 LOAD_GLOBAL             23 (NULL + _)
                            522 LOAD_CONST               6 ('Items must be selected in order to perform actions on them. No items have been changed.')
                            524 PRECALL                  1
                            528 CALL                     1
                            538 STORE_FAST              11 (msg)
                
-               630         540 LOAD_GLOBAL             25 (NULL + Response)
+               629         540 LOAD_GLOBAL             25 (NULL + Response)
                            552 LOAD_CONST               7 ('detail')
                            554 LOAD_FAST               11 (msg)
                            556 BUILD_MAP                1
                            558 LOAD_GLOBAL             26 (status)
                            570 LOAD_ATTR               14 (HTTP_400_BAD_REQUEST)
                            580 KW_NAMES                 8
                            582 PRECALL                  2
                            586 CALL                     2
                            596 RETURN_VALUE
                
-               631     >>  598 LOAD_FAST                5 (select_across)
+               630     >>  598 LOAD_FAST                5 (select_across)
                            600 POP_JUMP_FORWARD_IF_TRUE    22 (to 646)
                
-               632         602 LOAD_FAST                9 (queryset)
+               631         602 LOAD_FAST                9 (queryset)
                            604 LOAD_METHOD             15 (filter)
                            626 LOAD_FAST               10 (selected)
                            628 KW_NAMES                 9
                            630 PRECALL                  1
                            634 CALL                     1
                            644 STORE_FAST               9 (queryset)
                
-               635     >>  646 PUSH_NULL
+               634     >>  646 PUSH_NULL
                            648 LOAD_FAST                6 (func)
                            650 LOAD_FAST                2 (model_admin)
                            652 LOAD_FAST                1 (request)
                            654 LOAD_FAST                9 (queryset)
                            656 PRECALL                  3
                            660 CALL                     3
                            670 STORE_FAST              12 (response)
                
-               637         672 LOAD_FAST               12 (response)
+               636         672 LOAD_FAST               12 (response)
                            674 POP_JUMP_FORWARD_IF_FALSE     2 (to 680)
                
-               638         676 LOAD_FAST               12 (response)
+               637         676 LOAD_FAST               12 (response)
                            678 RETURN_VALUE
                
-               640     >>  680 LOAD_GLOBAL             23 (NULL + _)
+               639     >>  680 LOAD_GLOBAL             23 (NULL + _)
                            692 LOAD_CONST              10 ('action was performed successfully')
                            694 PRECALL                  1
                            698 CALL                     1
                            708 STORE_FAST              11 (msg)
                
-               641         710 LOAD_GLOBAL             25 (NULL + Response)
+               640         710 LOAD_GLOBAL             25 (NULL + Response)
                            722 LOAD_CONST               7 ('detail')
                            724 LOAD_FAST               11 (msg)
                            726 BUILD_MAP                1
                            728 LOAD_GLOBAL             26 (status)
                            740 LOAD_ATTR               16 (HTTP_200_OK)
                            750 KW_NAMES                 8
                            752 PRECALL                  2
                            756 CALL                     2
                            766 RETURN_VALUE
                
-               643     >>  768 LOAD_GLOBAL             25 (NULL + Response)
+               642     >>  768 LOAD_GLOBAL             25 (NULL + Response)
                            780 LOAD_FAST                3 (serializer)
                            782 LOAD_ATTR               17 (errors)
                            792 LOAD_GLOBAL             26 (status)
                            804 LOAD_ATTR               14 (HTTP_400_BAD_REQUEST)
                            814 KW_NAMES                 8
                            816 PRECALL                  2
                            820 CALL                     2
@@ -3580,53 +3546,53 @@
                   ('status',)
                   ('pk__in',)
                   'action was performed successfully'
                names      ('serializer_class', 'data', 'is_valid', 'validated_data', 'get', 'get_actions', 'get_changelist_instance', 'IncorrectLookupParameters', 'NotFound', 'str', 'get_queryset', '_', 'Response', 'status', 'HTTP_400_BAD_REQUEST', 'filter', 'HTTP_200_OK', 'errors')
                varnames   ('self', 'request', 'model_admin', 'serializer', 'action', 'select_across', 'func', 'cl', 'e', 'queryset', 'selected', 'msg', 'response')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'post'
-               firstlineno 611
+               firstlineno 610
                lnotab
                   0x020136022a0234013401420102012e01120140ff08022a03360108011e
                   023a0104012c031a02040104021e013a02
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'permission_classes', 'serializer_class', 'get', 'post')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
          name       'HandleActionView'
-         firstlineno 589
+         firstlineno 588
          lnotab 0x0a01040d040104020605
       'HandleActionView'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code
             0x970065005a0164005a0264015a0367005a0464025a05640384005a0664
             025300
-         646           0 RESUME                   0
+         645           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('HistoryView')
                        8 STORE_NAME               2 (__qualname__)
          
-         647          10 LOAD_CONST               1 ('\n    History of actions that happened to this object.\n    ')
+         646          10 LOAD_CONST               1 ('\n    History of actions that happened to this object.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-         650          14 BUILD_LIST               0
+         649          14 BUILD_LIST               0
                       16 STORE_NAME               4 (permission_classes)
          
-         651          18 LOAD_CONST               2 (None)
+         650          18 LOAD_CONST               2 (None)
                       20 STORE_NAME               5 (serializer_class)
          
-         653          22 LOAD_CONST               3 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py", line 653>)
+         652          22 LOAD_CONST               3 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py", line 652>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               6 (get)
                       28 LOAD_CONST               2 (None)
                       30 RETURN_VALUE
          consts
             'HistoryView'
             '\n    History of actions that happened to this object.\n    '
@@ -3656,136 +3622,136 @@
                   00ab0100000000000000007d097c036a120000000000000000a013000000
                   00000000000000000000000000000000007c097c017c00ac09a6030000ab
                   0300000000000000007d0a7c00a014000000000000000000000000000000
                   00000000007c0a640aac0ba6020000ab0200000000000000007d0b741100
                   0000000000000000007c0b6a150000000000000000741200000000000000
                   0000006a160000000000000000ac06a6020000ab02000000000000000053
                   00
-               653           0 RESUME                   0
+               652           0 RESUME                   0
                
-               654           2 LOAD_CONST               1 (0)
+               653           2 LOAD_CONST               1 (0)
                              4 LOAD_CONST               2 (('LogEntry',))
                              6 IMPORT_NAME              0 (django.contrib.admin.models)
                              8 IMPORT_FROM              1 (LogEntry)
                             10 STORE_FAST               4 (LogEntry)
                             12 POP_TOP
                
-               655          14 LOAD_FAST                3 (model_admin)
+               654          14 LOAD_FAST                3 (model_admin)
                             16 LOAD_ATTR                2 (model)
                             26 STORE_FAST               5 (model)
                
-               656          28 LOAD_FAST                5 (model)
+               655          28 LOAD_FAST                5 (model)
                             30 LOAD_ATTR                3 (_meta)
                             40 STORE_FAST               6 (opts)
                
-               657          42 LOAD_FAST                3 (model_admin)
+               656          42 LOAD_FAST                3 (model_admin)
                             44 LOAD_METHOD              4 (get_object)
                             66 LOAD_FAST                1 (request)
                             68 LOAD_GLOBAL             11 (NULL + unquote)
                             80 LOAD_FAST                2 (object_id)
                             82 PRECALL                  1
                             86 CALL                     1
                             96 PRECALL                  2
                            100 CALL                     2
                            110 STORE_FAST               7 (obj)
                
-               660         112 LOAD_FAST                7 (obj)
+               659         112 LOAD_FAST                7 (obj)
                            114 POP_JUMP_FORWARD_IF_NOT_NONE    68 (to 252)
                
-               661         116 LOAD_GLOBAL             13 (NULL + _)
+               660         116 LOAD_GLOBAL             13 (NULL + _)
                            128 LOAD_CONST               3 ("%(name)s with ID “%(key)s” doesn't exist. Perhaps it was deleted?")
                            130 PRECALL                  1
                            134 CALL                     1
                
-               662         144 LOAD_FAST                6 (opts)
+               661         144 LOAD_FAST                6 (opts)
                            146 LOAD_ATTR                7 (verbose_name)
                
-               663         156 LOAD_GLOBAL             11 (NULL + unquote)
+               662         156 LOAD_GLOBAL             11 (NULL + unquote)
                            168 LOAD_FAST                2 (object_id)
                            170 PRECALL                  1
                            174 CALL                     1
                
-               661         184 LOAD_CONST               4 (('name', 'key'))
+               660         184 LOAD_CONST               4 (('name', 'key'))
                            186 BUILD_CONST_KEY_MAP      2
                            188 BINARY_OP                6 (%)
                            192 STORE_FAST               8 (msg)
                
-               665         194 LOAD_GLOBAL             17 (NULL + Response)
+               664         194 LOAD_GLOBAL             17 (NULL + Response)
                            206 LOAD_CONST               5 ('detail')
                            208 LOAD_FAST                8 (msg)
                            210 BUILD_MAP                1
                            212 LOAD_GLOBAL             18 (status)
                            224 LOAD_ATTR               10 (HTTP_404_NOT_FOUND)
                            234 KW_NAMES                 6
                            236 PRECALL                  2
                            240 CALL                     2
                            250 RETURN_VALUE
                
-               668     >>  252 LOAD_FAST                3 (model_admin)
+               667     >>  252 LOAD_FAST                3 (model_admin)
                            254 LOAD_METHOD             11 (has_view_or_change_permission)
                            276 LOAD_FAST                1 (request)
                            278 LOAD_FAST                7 (obj)
                            280 PRECALL                  2
                            284 CALL                     2
                            294 POP_JUMP_FORWARD_IF_TRUE     7 (to 310)
                
-               669         296 LOAD_GLOBAL             24 (PermissionDenied)
+               668         296 LOAD_GLOBAL             24 (PermissionDenied)
                            308 RAISE_VARARGS            1
                
-               672     >>  310 LOAD_FAST                4 (LogEntry)
+               671     >>  310 LOAD_FAST                4 (LogEntry)
                            312 LOAD_ATTR               13 (objects)
                            322 LOAD_METHOD             14 (filter)
                
-               673         344 LOAD_GLOBAL             11 (NULL + unquote)
+               672         344 LOAD_GLOBAL             11 (NULL + unquote)
                            356 LOAD_FAST                2 (object_id)
                            358 PRECALL                  1
                            362 CALL                     1
                
-               674         372 LOAD_GLOBAL             31 (NULL + get_content_type_for_model)
+               673         372 LOAD_GLOBAL             31 (NULL + get_content_type_for_model)
                            384 LOAD_FAST                5 (model)
                            386 PRECALL                  1
                            390 CALL                     1
                
-               672         400 KW_NAMES                 7
+               671         400 KW_NAMES                 7
                            402 PRECALL                  2
                            406 CALL                     2
                
-               675         416 LOAD_METHOD             16 (select_related)
+               674         416 LOAD_METHOD             16 (select_related)
                            438 PRECALL                  0
                            442 CALL                     0
                            452 LOAD_METHOD             17 (order_by)
                            474 LOAD_CONST               8 ('action_time')
                            476 PRECALL                  1
                            480 CALL                     1
                
-               672         490 STORE_FAST               9 (action_list)
+               671         490 STORE_FAST               9 (action_list)
                
-               678         492 LOAD_FAST                3 (model_admin)
+               677         492 LOAD_FAST                3 (model_admin)
                            494 LOAD_ATTR               18 (admin_site)
                            504 LOAD_METHOD             19 (paginate_queryset)
                
-               679         526 LOAD_FAST                9 (action_list)
+               678         526 LOAD_FAST                9 (action_list)
                            528 LOAD_FAST                1 (request)
                            530 LOAD_FAST                0 (self)
                
-               678         532 KW_NAMES                 9
+               677         532 KW_NAMES                 9
                            534 PRECALL                  3
                            538 CALL                     3
                            548 STORE_FAST              10 (page)
                
-               682         550 LOAD_FAST                0 (self)
+               681         550 LOAD_FAST                0 (self)
                            552 LOAD_METHOD             20 (serializer_class)
                            574 LOAD_FAST               10 (page)
                            576 LOAD_CONST              10 (True)
                            578 KW_NAMES                11
                            580 PRECALL                  2
                            584 CALL                     2
                            594 STORE_FAST              11 (serializer)
                
-               684         596 LOAD_GLOBAL             17 (NULL + Response)
+               683         596 LOAD_GLOBAL             17 (NULL + Response)
                            608 LOAD_FAST               11 (serializer)
                            610 LOAD_ATTR               21 (data)
                            620 LOAD_GLOBAL             18 (status)
                            632 LOAD_ATTR               22 (HTTP_200_OK)
                            642 KW_NAMES                 6
                            644 PRECALL                  2
                            648 CALL                     2
@@ -3803,33 +3769,33 @@
                   ('view',)
                   True
                   ('many',)
                names      ('django.contrib.admin.models', 'LogEntry', 'model', '_meta', 'get_object', 'unquote', '_', 'verbose_name', 'Response', 'status', 'HTTP_404_NOT_FOUND', 'has_view_or_change_permission', 'PermissionDenied', 'objects', 'filter', 'get_content_type_for_model', 'select_related', 'order_by', 'admin_site', 'paginate_queryset', 'serializer_class', 'data', 'HTTP_200_OK')
                varnames   ('self', 'request', 'object_id', 'model_admin', 'LogEntry', 'model', 'opts', 'obj', 'msg', 'action_list', 'page', 'serializer')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
                name       'get'
-               firstlineno 653
+               firstlineno 652
                lnotab
                   0x02010c010e010e01460304011c010c011cfe0a043a032c010e0322011c
                   011cfe10034afd0206220106ff12042e02
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'permission_classes', 'serializer_class', 'get')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
          name       'HistoryView'
-         firstlineno 646
+         firstlineno 645
          lnotab 0x0a01040304010402
       'HistoryView'
       None
    names      ('__doc__', 'django.db.models', 'Model', 'django.db', 'transaction', 'django.utils.translation', 'gettext_lazy', '_', 'django.contrib.contenttypes.models', 'ContentType', 'django.core.exceptions', 'FieldDoesNotExist', 'ObjectDoesNotExist', 'django.contrib.admin.utils', 'label_for_field', 'lookup_field', 'unquote', 'django.contrib.admin.options', 'TO_FIELD_VAR', 'IncorrectLookupParameters', 'get_content_type_for_model', 'rest_framework', 'status', 'rest_framework.views', 'APIView', 'rest_framework.reverse', 'reverse', 'rest_framework.response', 'Response', 'rest_framework.exceptions', 'NotFound', 'PermissionDenied', 'django_api_admin.declarations.classes', 'ModelDiffHelper', 'django_api_admin.declarations.functions', 'get_form_fields', 'get_form_config', 'validate_bulk_edits', 'get_inlines', 'ListView', 'DetailView', 'AddView', 'ChangeView', 'DeleteView', 'ChangeListView', 'HandleActionView', 'HistoryView')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/admin_views.py'
+   filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/admin_views.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020104030c010c010c010c011001140114040c010c010c010c0110
-      020c0118061c1d1c301c591c7f00261c2c1c7f003c1c39
+      020c0118061c1c1c301c591c7f00261c2c1c7f003c1c39
```

### Comparing `django-api-admin-1.1.4/django_api_admin/views/__pycache__/fields_test_views.cpython-311.pyc` & `django-api-admin-1.1.5/django_api_admin/views/__pycache__/fields_test_views.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x5104b264 (Sat Jul 15 02:28:33 2023 UTC)
+moddate:  0xdcf0b264 (Sat Jul 15 19:17:48 2023 UTC)
 files sz: 11410
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
@@ -1309,25 +1309,25 @@
     16        3392 LOAD_CONST             158 (('primary_key_related_field_many_test', 'hyperlinked_related_field_test', 'hyperlinked_related_field_many_test', 'slug_related_field_test', 'slug_related_field_many_test'))
               3394 BUILD_CONST_KEY_MAP      5
               3396 DICT_UPDATE              1
               3398 STORE_NAME              52 (tests)
    
    384        3400 PUSH_NULL
               3402 LOAD_BUILD_CLASS
-              3404 LOAD_CONST             159 (<code object TestView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/fields_test_views.py", line 384>)
+              3404 LOAD_CONST             159 (<code object TestView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/fields_test_views.py", line 384>)
               3406 MAKE_FUNCTION            0
               3408 LOAD_CONST             160 ('TestView')
               3410 LOAD_NAME               11 (APIView)
               3412 PRECALL                  3
               3416 CALL                     3
               3426 STORE_NAME              53 (TestView)
    
    445        3428 PUSH_NULL
               3430 LOAD_BUILD_CLASS
-              3432 LOAD_CONST             161 (<code object TestDetailView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/fields_test_views.py", line 445>)
+              3432 LOAD_CONST             161 (<code object TestDetailView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/fields_test_views.py", line 445>)
               3434 MAKE_FUNCTION            0
               3436 LOAD_CONST             162 ('TestDetailView')
               3438 LOAD_NAME               11 (APIView)
               3440 PRECALL                  3
               3444 CALL                     3
               3454 STORE_NAME              54 (TestDetailView)
               3456 LOAD_CONST               2 (None)
@@ -1511,27 +1511,27 @@
          
          388          14 BUILD_LIST               0
                       16 STORE_NAME               4 (authentication_classes)
          
          389          18 LOAD_CONST               2 (None)
                       20 STORE_NAME               5 (serializer_class)
          
-         391          22 LOAD_CONST               3 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/fields_test_views.py", line 391>)
+         391          22 LOAD_CONST               3 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/fields_test_views.py", line 391>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               6 (get)
          
-         404          28 LOAD_CONST               4 (<code object post, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/fields_test_views.py", line 404>)
+         404          28 LOAD_CONST               4 (<code object post, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/fields_test_views.py", line 404>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               7 (post)
          
-         418          34 LOAD_CONST               5 (<code object generate_test_serializer, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/fields_test_views.py", line 418>)
+         418          34 LOAD_CONST               5 (<code object generate_test_serializer, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/fields_test_views.py", line 418>)
                       36 MAKE_FUNCTION            0
                       38 STORE_NAME               8 (generate_test_serializer)
          
-         421          40 LOAD_CONST               6 (<code object get_test, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/fields_test_views.py", line 421>)
+         421          40 LOAD_CONST               6 (<code object get_test, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/fields_test_views.py", line 421>)
                       42 MAKE_FUNCTION            0
                       44 STORE_NAME               9 (get_test)
                       46 LOAD_CONST               2 (None)
                       48 RETURN_VALUE
          consts
             'TestView'
             '\n    A view used for integrated tests.\n    '
@@ -1639,15 +1639,15 @@
                   'test field not supported'
                   'fields'
                   ('status',)
                names      ('get_test', 'generate_test_serializer', 'serializer_class', 'get_form_fields', 'KeyError', 'Response', 'status', 'HTTP_200_OK')
                varnames   ('self', 'request', 'test_name', 'fields', 'SerializerClass', 'meta', 'serializer', 'form_fields')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/fields_test_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/fields_test_views.py'
                name       'get'
                firstlineno 391
                lnotab 0x020102013201180106ff1a0330012201120126ff0803
             code
                argcount  : 3
                nlocals   : 8
                stacksize : 5
@@ -1764,15 +1764,15 @@
                   ('status',)
                   'detail'
                   'test field not supported'
                names      ('print', 'data', 'get_test', 'generate_test_serializer', 'is_valid', 'Response', 'errors', 'status', 'HTTP_400_BAD_REQUEST', 'KeyError')
                varnames   ('self', 'request', 'test_name', 'fields', 'SerializerClass', 'meta', 'serializer_class', 'serializer')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/fields_test_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/fields_test_views.py'
                name       'post'
                firstlineno 404
                lnotab 0x0201280102013201180106ff10022202280122014201120126ff
             code
                argcount  : 4
                nlocals   : 4
                stacksize : 12
@@ -1810,15 +1810,15 @@
                   None
                   'TestSerializer'
                   'Meta'
                names      ('type', 'object')
                varnames   ('self', 'SerializerClass', 'meta', 'fields')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/fields_test_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/fields_test_views.py'
                name       'generate_test_serializer'
                firstlineno 418
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 6
                stacksize : 4
@@ -1935,25 +1935,25 @@
                   0
                   1
                   2
                names      ('tests', 'serializers', 'Serializer', 'IndexError')
                varnames   ('self', 'test_name', 'test', 'fields', 'SerializerClass', 'meta')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/fields_test_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/fields_test_views.py'
                name       'get_test'
                firstlineno 421
                lnotab
                   0x02011a0104011801040202011401120104ff080302011401120104ff08
                   0302011401120104ff0803
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'authentication_classes', 'serializer_class', 'get', 'post', 'generate_test_serializer', 'get_test')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/fields_test_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/fields_test_views.py'
          name       'TestView'
          firstlineno 384
          lnotab 0x0a01040304010402060d060e0603
       'TestView'
       code
          argcount  : 0
          nlocals   : 0
@@ -1963,15 +1963,15 @@
          445           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('TestDetailView')
                        8 STORE_NAME               2 (__qualname__)
          
          446          10 LOAD_CONST               3 ((None,))
-                      12 LOAD_CONST               2 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/fields_test_views.py", line 446>)
+                      12 LOAD_CONST               2 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/fields_test_views.py", line 446>)
                       14 MAKE_FUNCTION            1 (defaults)
                       16 STORE_NAME               3 (get)
                       18 LOAD_CONST               1 (None)
                       20 RETURN_VALUE
          consts
             'TestDetailView'
             None
@@ -1996,33 +1996,33 @@
                consts
                   None
                   ('status',)
                names      ('Response', 'status', 'HTTP_200_OK')
                varnames   ('request', 'pk', 'format')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/fields_test_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/fields_test_views.py'
                name       'get'
                firstlineno 446
                lnotab 0x0201
             (None,)
          names      ('__name__', '__module__', '__qualname__', 'get')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/fields_test_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/fields_test_views.py'
          name       'TestDetailView'
          firstlineno 445
          lnotab 0x0a01
       'TestDetailView'
    names      ('__doc__', 'datetime', 'json', 'django.conf', 'settings', 'rest_framework', 'serializers', 'status', 'rest_framework.response', 'Response', 'rest_framework.views', 'APIView', 'django_api_admin.models', 'Author', 'django_api_admin.declarations.functions', 'get_form_fields', 'CharField', 'EmailField', 'RegexField', 'SlugField', 'URLField', 'UUIDField', 'IPAddressField', 'IntegerField', 'FloatField', 'DecimalField', 'JSONField', 'dumps', 'ChoiceField', 'MultipleChoiceField', 'FilePathField', 'BASE_DIR', 'BooleanField', 'DateField', 'date', 'today', 'DateTimeField', 'now', 'TimeField', 'time', 'DurationField', 'FileField', 'ImageField', 'ListField', 'DictField', 'HStoreField', 'PrimaryKeyRelatedField', 'objects', 'all', 'HyperlinkedRelatedField', 'ModelSerializer', 'SlugRelatedField', 'tests', 'TestView', 'TestDetailView')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/fields_test_views.py'
+   filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/fields_test_views.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010403080108020c0210010c010c020c010c020202020226ff02
       ff02fe0208020228ff02ff02f8020e020228ff02ff02f2021402022cff02
       ff02ec021a020226ff02ff02e60220020228ff02ff02e00226020226ff02
       ff02da022c020226ff02ff02d40232020224ff02ff02ce0238020228ff02
```

### Comparing `django-api-admin-1.1.4/django_api_admin/views/__pycache__/site_views.cpython-311.pyc` & `django-api-admin-1.1.5/django_api_admin/views/__pycache__/site_views.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,32 +1,32 @@
 magic:    0xa70d0d0a
-moddate:  0x5f0bb264 (Sat Jul 15 02:58:39 2023 UTC)
-files sz: 8315
+moddate:  0xd3f8b264 (Sat Jul 15 19:51:47 2023 UTC)
+files sz: 8325
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x970064005a00640164026c015a01640164036c026d035a030100640164
       046c046d055a056d065a060100640164056c076d085a080100640164066c
       096d0a5a0b0100640164076c0c6d0d5a0d0100640164086c0e6d0f5a0f01
       00640164096c106d115a1101006401640a6c126d135a1301006401640b6c
       146d155a1501006401640c6c166d175a17010002004700640d8400640e65
-      15a6030000ab0300000000000000005a1802004700640f840064106515a6
-      030000ab0300000000000000005a19020047006411840064126515a60300
-      00ab0300000000000000005a1a020047006413840064146515a6030000ab
-      0300000000000000005a1b020047006415840064166515a6030000ab0300
-      000000000000005a1c020047006417840064186515a6030000ab03000000
-      00000000005a1d0200470064198400641a6515a6030000ab030000000000
-      0000005a1e02004700641b8400641c6515a6030000ab0300000000000000
-      005a1f02004700641d8400641e6515a6030000ab0300000000000000005a
-      2002004700641f840064206515a6030000ab0300000000000000005a2102
-      0047006421840064226515a6030000ab0300000000000000005a22020047
-      006423840064246515a6030000ab0300000000000000005a2364025300
+      13a6030000ab0300000000000000005a1802004700640f840064106513a6
+      030000ab0300000000000000005a19020047006411840064126513a60300
+      00ab0300000000000000005a1a020047006413840064146513a6030000ab
+      0300000000000000005a1b020047006415840064166513a6030000ab0300
+      000000000000005a1c020047006417840064186513a6030000ab03000000
+      00000000005a1d0200470064198400641a6513a6030000ab030000000000
+      0000005a1e02004700641b8400641c6513a6030000ab0300000000000000
+      005a1f02004700641d8400641e6513a6030000ab0300000000000000005a
+      2002004700641f840064206513a6030000ab0300000000000000005a2102
+      0047006421840064226513a6030000ab0300000000000000005a22020047
+      006423840064246513a6030000ab0300000000000000005a2364025300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('\nadmin site views\n')
                  4 STORE_NAME               0 (__doc__)
    
      4           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (None)
@@ -66,183 +66,183 @@
     10          66 LOAD_CONST               1 (0)
                 68 LOAD_CONST               7 (('JSONCatalog',))
                 70 IMPORT_NAME             12 (django.views.i18n)
                 72 IMPORT_FROM             13 (JSONCatalog)
                 74 STORE_NAME              13 (JSONCatalog)
                 76 POP_TOP
    
-    11          78 LOAD_CONST               1 (0)
-                80 LOAD_CONST               8 (('reverse',))
-                82 IMPORT_NAME             14 (django.urls)
-                84 IMPORT_FROM             15 (reverse)
-                86 STORE_NAME              15 (reverse)
+    12          78 LOAD_CONST               1 (0)
+                80 LOAD_CONST               8 (('status',))
+                82 IMPORT_NAME             14 (rest_framework)
+                84 IMPORT_FROM             15 (status)
+                86 STORE_NAME              15 (status)
                 88 POP_TOP
    
     13          90 LOAD_CONST               1 (0)
-                92 LOAD_CONST               9 (('status',))
-                94 IMPORT_NAME             16 (rest_framework)
-                96 IMPORT_FROM             17 (status)
-                98 STORE_NAME              17 (status)
+                92 LOAD_CONST               9 (('Response',))
+                94 IMPORT_NAME             16 (rest_framework.response)
+                96 IMPORT_FROM             17 (Response)
+                98 STORE_NAME              17 (Response)
                100 POP_TOP
    
     14         102 LOAD_CONST               1 (0)
-               104 LOAD_CONST              10 (('Response',))
-               106 IMPORT_NAME             18 (rest_framework.response)
-               108 IMPORT_FROM             19 (Response)
-               110 STORE_NAME              19 (Response)
+               104 LOAD_CONST              10 (('APIView',))
+               106 IMPORT_NAME             18 (rest_framework.views)
+               108 IMPORT_FROM             19 (APIView)
+               110 STORE_NAME              19 (APIView)
                112 POP_TOP
    
     15         114 LOAD_CONST               1 (0)
-               116 LOAD_CONST              11 (('APIView',))
-               118 IMPORT_NAME             20 (rest_framework.views)
-               120 IMPORT_FROM             21 (APIView)
-               122 STORE_NAME              21 (APIView)
+               116 LOAD_CONST              11 (('reverse',))
+               118 IMPORT_NAME             20 (rest_framework.reverse)
+               120 IMPORT_FROM             21 (reverse)
+               122 STORE_NAME              21 (reverse)
                124 POP_TOP
    
     17         126 LOAD_CONST               1 (0)
                128 LOAD_CONST              12 (('get_form_fields',))
                130 IMPORT_NAME             22 (django_api_admin.declarations.functions)
                132 IMPORT_FROM             23 (get_form_fields)
                134 STORE_NAME              23 (get_form_fields)
                136 POP_TOP
    
     23         138 PUSH_NULL
                140 LOAD_BUILD_CLASS
-               142 LOAD_CONST              13 (<code object CsrfTokenView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 23>)
+               142 LOAD_CONST              13 (<code object CsrfTokenView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 23>)
                144 MAKE_FUNCTION            0
                146 LOAD_CONST              14 ('CsrfTokenView')
-               148 LOAD_NAME               21 (APIView)
+               148 LOAD_NAME               19 (APIView)
                150 PRECALL                  3
                154 CALL                     3
                164 STORE_NAME              24 (CsrfTokenView)
    
     31         166 PUSH_NULL
                168 LOAD_BUILD_CLASS
-               170 LOAD_CONST              15 (<code object UserInformation, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 31>)
+               170 LOAD_CONST              15 (<code object UserInformation, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 31>)
                172 MAKE_FUNCTION            0
                174 LOAD_CONST              16 ('UserInformation')
-               176 LOAD_NAME               21 (APIView)
+               176 LOAD_NAME               19 (APIView)
                178 PRECALL                  3
                182 CALL                     3
                192 STORE_NAME              25 (UserInformation)
    
     40         194 PUSH_NULL
                196 LOAD_BUILD_CLASS
-               198 LOAD_CONST              17 (<code object LoginView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 40>)
+               198 LOAD_CONST              17 (<code object LoginView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 40>)
                200 MAKE_FUNCTION            0
                202 LOAD_CONST              18 ('LoginView')
-               204 LOAD_NAME               21 (APIView)
+               204 LOAD_NAME               19 (APIView)
                206 PRECALL                  3
                210 CALL                     3
                220 STORE_NAME              26 (LoginView)
    
     71         222 PUSH_NULL
                224 LOAD_BUILD_CLASS
-               226 LOAD_CONST              19 (<code object LogoutView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 71>)
+               226 LOAD_CONST              19 (<code object LogoutView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 71>)
                228 MAKE_FUNCTION            0
                230 LOAD_CONST              20 ('LogoutView')
-               232 LOAD_NAME               21 (APIView)
+               232 LOAD_NAME               19 (APIView)
                234 PRECALL                  3
                238 CALL                     3
                248 STORE_NAME              27 (LogoutView)
    
     85         250 PUSH_NULL
                252 LOAD_BUILD_CLASS
-               254 LOAD_CONST              21 (<code object PasswordChangeView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 85>)
+               254 LOAD_CONST              21 (<code object PasswordChangeView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 85>)
                256 MAKE_FUNCTION            0
                258 LOAD_CONST              22 ('PasswordChangeView')
-               260 LOAD_NAME               21 (APIView)
+               260 LOAD_NAME               19 (APIView)
                262 PRECALL                  3
                266 CALL                     3
                276 STORE_NAME              28 (PasswordChangeView)
    
    103         278 PUSH_NULL
                280 LOAD_BUILD_CLASS
-               282 LOAD_CONST              23 (<code object IndexView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 103>)
+               282 LOAD_CONST              23 (<code object IndexView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 103>)
                284 MAKE_FUNCTION            0
                286 LOAD_CONST              24 ('IndexView')
-               288 LOAD_NAME               21 (APIView)
+               288 LOAD_NAME               19 (APIView)
                290 PRECALL                  3
                294 CALL                     3
                304 STORE_NAME              29 (IndexView)
    
    125         306 PUSH_NULL
                308 LOAD_BUILD_CLASS
-               310 LOAD_CONST              25 (<code object AppIndexView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 125>)
+               310 LOAD_CONST              25 (<code object AppIndexView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 125>)
                312 MAKE_FUNCTION            0
                314 LOAD_CONST              26 ('AppIndexView')
-               316 LOAD_NAME               21 (APIView)
+               316 LOAD_NAME               19 (APIView)
                318 PRECALL                  3
                322 CALL                     3
                332 STORE_NAME              30 (AppIndexView)
    
    150         334 PUSH_NULL
                336 LOAD_BUILD_CLASS
-               338 LOAD_CONST              27 (<code object LanguageCatalogView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 150>)
+               338 LOAD_CONST              27 (<code object LanguageCatalogView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 150>)
                340 MAKE_FUNCTION            0
                342 LOAD_CONST              28 ('LanguageCatalogView')
-               344 LOAD_NAME               21 (APIView)
+               344 LOAD_NAME               19 (APIView)
                346 PRECALL                  3
                350 CALL                     3
                360 STORE_NAME              31 (LanguageCatalogView)
    
    162         362 PUSH_NULL
                364 LOAD_BUILD_CLASS
-               366 LOAD_CONST              29 (<code object AutoCompleteView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 162>)
+               366 LOAD_CONST              29 (<code object AutoCompleteView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 162>)
                368 MAKE_FUNCTION            0
                370 LOAD_CONST              30 ('AutoCompleteView')
-               372 LOAD_NAME               21 (APIView)
+               372 LOAD_NAME               19 (APIView)
                374 PRECALL                  3
                378 CALL                     3
                388 STORE_NAME              32 (AutoCompleteView)
    
    171         390 PUSH_NULL
                392 LOAD_BUILD_CLASS
-               394 LOAD_CONST              31 (<code object SiteContextView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 171>)
+               394 LOAD_CONST              31 (<code object SiteContextView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 171>)
                396 MAKE_FUNCTION            0
                398 LOAD_CONST              32 ('SiteContextView')
-               400 LOAD_NAME               21 (APIView)
+               400 LOAD_NAME               19 (APIView)
                402 PRECALL                  3
                406 CALL                     3
                416 STORE_NAME              33 (SiteContextView)
    
    182         418 PUSH_NULL
                420 LOAD_BUILD_CLASS
-               422 LOAD_CONST              33 (<code object AdminLogView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 182>)
+               422 LOAD_CONST              33 (<code object AdminLogView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 182>)
                424 MAKE_FUNCTION            0
                426 LOAD_CONST              34 ('AdminLogView')
-               428 LOAD_NAME               21 (APIView)
+               428 LOAD_NAME               19 (APIView)
                430 PRECALL                  3
                434 CALL                     3
                444 STORE_NAME              34 (AdminLogView)
    
    239         446 PUSH_NULL
                448 LOAD_BUILD_CLASS
-               450 LOAD_CONST              35 (<code object AdminAPIRootView, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 239>)
+               450 LOAD_CONST              35 (<code object AdminAPIRootView, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 239>)
                452 MAKE_FUNCTION            0
                454 LOAD_CONST              36 ('AdminAPIRootView')
-               456 LOAD_NAME               21 (APIView)
+               456 LOAD_NAME               19 (APIView)
                458 PRECALL                  3
                462 CALL                     3
                472 STORE_NAME              35 (AdminAPIRootView)
                474 LOAD_CONST               2 (None)
                476 RETURN_VALUE
    consts
       '\nadmin site views\n'
       0
       None
       ('AutocompleteJsonView',)
       ('login', 'logout')
       ('get_token',)
       ('gettext_lazy',)
       ('JSONCatalog',)
-      ('reverse',)
       ('status',)
       ('Response',)
       ('APIView',)
+      ('reverse',)
       ('get_form_fields',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a0264015a0367005a04640284005a0564015300
@@ -254,15 +254,15 @@
          
           24          10 LOAD_CONST               1 (None)
                       12 STORE_NAME               3 (serializer_class)
          
           25          14 BUILD_LIST               0
                       16 STORE_NAME               4 (permission_classes)
          
-          27          18 LOAD_CONST               2 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 27>)
+          27          18 LOAD_CONST               2 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 27>)
                       20 MAKE_FUNCTION            0
                       22 STORE_NAME               5 (get)
                       24 LOAD_CONST               1 (None)
                       26 RETURN_VALUE
          consts
             'CsrfTokenView'
             None
@@ -290,23 +290,23 @@
                consts
                   None
                   'csrftoken'
                names      ('Response', 'get_token')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
                name       'get'
                firstlineno 27
                lnotab 0x0201
          names      ('__name__', '__module__', '__qualname__', 'serializer_class', 'permission_classes', 'get')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
          name       'CsrfTokenView'
          firstlineno 23
          lnotab 0x0a0104010402
       'CsrfTokenView'
       code
          argcount  : 0
          nlocals   : 0
@@ -321,15 +321,15 @@
          
           32          10 LOAD_CONST               1 (None)
                       12 STORE_NAME               3 (serializer_class)
          
           33          14 BUILD_LIST               0
                       16 STORE_NAME               4 (permission_classes)
          
-          35          18 LOAD_CONST               2 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 35>)
+          35          18 LOAD_CONST               2 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 35>)
                       20 MAKE_FUNCTION            0
                       22 STORE_NAME               5 (get)
                       24 LOAD_CONST               1 (None)
                       26 RETURN_VALUE
          consts
             'UserInformation'
             None
@@ -364,23 +364,23 @@
                consts
                   None
                   'user'
                names      ('serializer_class', 'user', 'Response', 'data')
                varnames   ('self', 'request', 'serializer')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
                name       'get'
                firstlineno 35
                lnotab 0x02013401
          names      ('__name__', '__module__', '__qualname__', 'serializer_class', 'permission_classes', 'get')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
          name       'UserInformation'
          firstlineno 31
          lnotab 0x0a0104010402
       'UserInformation'
       code
          argcount  : 0
          nlocals   : 0
@@ -400,19 +400,19 @@
          
           44          14 LOAD_CONST               2 (None)
                       16 STORE_NAME               4 (serializer_class)
          
           45          18 BUILD_LIST               0
                       20 STORE_NAME               5 (permission_classes)
          
-          47          22 LOAD_CONST               3 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 47>)
+          47          22 LOAD_CONST               3 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 47>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               6 (get)
          
-          52          28 LOAD_CONST               4 (<code object post, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 52>)
+          52          28 LOAD_CONST               4 (<code object post, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 52>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               7 (post)
                       34 LOAD_CONST               2 (None)
                       36 RETURN_VALUE
          consts
             'LoginView'
             '\n    Allow users to login using username and password.\n    '
@@ -456,15 +456,15 @@
                   None
                   'fields'
                   ('status',)
                names      ('serializer_class', 'get_form_fields', 'Response', 'status', 'HTTP_200_OK')
                varnames   ('self', 'request', 'admin_site', 'serializer', 'form_fields')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
                name       'get'
                firstlineno 47
                lnotab 0x020128011e01
             code
                argcount  : 3
                nlocals   : 8
                stacksize : 5
@@ -600,25 +600,25 @@
                   ('status',)
                   'non_field_errors'
                   'permission_denied'
                names      ('serializer_class', 'data', 'is_valid', 'get_user', 'login', 'user_serializer', '_', 'Response', 'status', 'HTTP_200_OK', 'errors', 'get', 'code', 'HTTP_403_FORBIDDEN', 'HTTP_400_BAD_REQUEST')
                varnames   ('self', 'request', 'admin_site', 'serializer', 'user', 'user_serializer', 'data', 'error')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
                name       'post'
                firstlineno 52
                lnotab
                   0x0201180112ff12022801280120012a021c010cfe060436023a01160144
                   ff0202
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'serializer_class', 'permission_classes', 'get', 'post')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
          name       'LoginView'
          firstlineno 40
          lnotab 0x0a010403040104020605
       'LoginView'
       code
          argcount  : 0
          nlocals   : 0
@@ -635,19 +635,19 @@
          
           72          10 LOAD_CONST               1 ("\n    Logout and display a 'you are logged out ' message.\n    ")
                       12 STORE_NAME               3 (__doc__)
          
           75          14 BUILD_LIST               0
                       16 STORE_NAME               4 (permission_classes)
          
-          77          18 LOAD_CONST               2 (<code object post, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 77>)
+          77          18 LOAD_CONST               2 (<code object post, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 77>)
                       20 MAKE_FUNCTION            0
                       22 STORE_NAME               5 (post)
          
-          81          24 LOAD_CONST               3 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 81>)
+          81          24 LOAD_CONST               3 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 81>)
                       26 MAKE_FUNCTION            0
                       28 STORE_NAME               6 (get)
                       30 LOAD_CONST               4 (None)
                       32 RETURN_VALUE
          consts
             'LogoutView'
             "\n    Logout and display a 'you are logged out ' message.\n    "
@@ -687,15 +687,15 @@
                   'detail'
                   'You are logged out.'
                   ('status',)
                names      ('logout', 'Response', '_', 'status', 'HTTP_200_OK')
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
                name       'post'
                firstlineno 77
                lnotab 0x02011e01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
@@ -713,24 +713,24 @@
                             42 RETURN_VALUE
                consts
                   None
                names      ('post',)
                varnames   ('self', 'request')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
                name       'get'
                firstlineno 81
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'permission_classes', 'post', 'get')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
          name       'LogoutView'
          firstlineno 71
          lnotab 0x0a01040304020604
       'LogoutView'
       code
          argcount  : 0
          nlocals   : 0
@@ -750,15 +750,15 @@
          
           89          14 LOAD_CONST               2 (None)
                       16 STORE_NAME               4 (serializer_class)
          
           90          18 BUILD_LIST               0
                       20 STORE_NAME               5 (permission_classes)
          
-          92          22 LOAD_CONST               3 (<code object post, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 92>)
+          92          22 LOAD_CONST               3 (<code object post, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 92>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               6 (post)
                       28 LOAD_CONST               2 (None)
                       30 RETURN_VALUE
          consts
             'PasswordChangeView'
             '\n        Handle the "change password" task -- both form display and validation.\n    '
@@ -844,23 +844,23 @@
                   'detail'
                   'Your password was changed'
                   ('status',)
                names      ('serializer_class', 'data', 'user', 'is_valid', 'save', 'Response', '_', 'status', 'HTTP_200_OK', 'errors', 'HTTP_400_BAD_REQUEST')
                varnames   ('self', 'request', 'serializer_class', 'serializer')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
                name       'post'
                firstlineno 92
                lnotab 0x02010e0104011cff1202280128012c0116ff1202
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'serializer_class', 'permission_classes', 'post')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
          name       'PasswordChangeView'
          firstlineno 85
          lnotab 0x0a01040304010402
       'PasswordChangeView'
       code
          argcount  : 0
          nlocals   : 0
@@ -875,39 +875,39 @@
          
          104          10 LOAD_CONST               1 ('\n    Return json object that lists all the installed\n    apps that have been registered by the admin site.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
          108          14 BUILD_LIST               0
                       16 STORE_NAME               4 (permission_classes)
          
-         110          18 LOAD_CONST               2 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 110>)
+         110          18 LOAD_CONST               2 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 110>)
                       20 MAKE_FUNCTION            0
                       22 STORE_NAME               5 (get)
                       24 LOAD_CONST               3 (None)
                       26 RETURN_VALUE
          consts
             'IndexView'
             '\n    Return json object that lists all the installed\n    apps that have been registered by the admin site.\n    '
             code
                argcount  : 3
                nlocals   : 8
-               stacksize : 8
+               stacksize : 7
                flags     : 3
                code
                   0x97007c02a00000000000000000000000000000000000000000007c01a6
                   010000ab0100000000000000007d037c01a0010000000000000000000000
                   000000000000000000a6000000ab0000000000000000007d047c01a00200
                   00000000000000000000000000000000000000a6000000ab000000000000
-                  000000720264016e0164027d057c0344005d2c7d067c057c047a00000074
-                  07000000000000000000007c026a0400000000000000009b0064039d0264
-                  047c066404190000000000000000006901ac05a6020000ab020000000000
-                  0000007a0000007c0664063c0000008c2d64077c0369017d077c026a0400
-                  000000000000007c015f050000000000000000740d000000000000000000
-                  007c07740e000000000000000000006a080000000000000000ac08a60200
-                  00ab0200000000000000005300
+                  000000720264016e0164027d057c0344005d277d06740700000000000000
+                  0000007c026a0400000000000000009b0064039d0264047c066404190000
+                  0000000000000069017c01ac05a6030000ab0300000000000000007c0664
+                  063c0000008c2864077c0369017d077c026a0400000000000000007c015f
+                  050000000000000000740d000000000000000000007c07740e0000000000
+                  00000000006a080000000000000000ac08a6020000ab0200000000000000
+                  005300
                110           0 RESUME                   0
                
                111           2 LOAD_FAST                2 (admin_site)
                              4 LOAD_METHOD              0 (get_app_list)
                             26 LOAD_FAST                1 (request)
                             28 PRECALL                  1
                             32 CALL                     1
@@ -927,83 +927,80 @@
                            124 LOAD_CONST               1 ('https://')
                            126 JUMP_FORWARD             1 (to 130)
                        >>  128 LOAD_CONST               2 ('http://')
                        >>  130 STORE_FAST               5 (scheme)
                
                116         132 LOAD_FAST                3 (app_list)
                            134 GET_ITER
-                       >>  136 FOR_ITER                44 (to 226)
+                       >>  136 FOR_ITER                39 (to 216)
                            138 STORE_FAST               6 (app)
                
-               117         140 LOAD_FAST                5 (scheme)
-                           142 LOAD_FAST                4 (domain)
-                           144 BINARY_OP                0 (+)
-                           148 LOAD_GLOBAL              7 (NULL + reverse)
-                           160 LOAD_FAST                2 (admin_site)
-                           162 LOAD_ATTR                4 (name)
-                           172 FORMAT_VALUE             0
-                           174 LOAD_CONST               3 (':app_list')
-                           176 BUILD_STRING             2
-                           178 LOAD_CONST               4 ('app_label')
-                           180 LOAD_FAST                6 (app)
-                           182 LOAD_CONST               4 ('app_label')
-                           184 BINARY_SUBSCR
-                           194 BUILD_MAP                1
-                           196 KW_NAMES                 5
-                           198 PRECALL                  2
-                           202 CALL                     2
-                           212 BINARY_OP                0 (+)
-                           216 LOAD_FAST                6 (app)
-                           218 LOAD_CONST               6 ('url')
-                           220 STORE_SUBSCR
-                           224 JUMP_BACKWARD           45 (to 136)
-               
-               119     >>  226 LOAD_CONST               7 ('app_list')
-                           228 LOAD_FAST                3 (app_list)
-               
-               118         230 BUILD_MAP                1
-                           232 STORE_FAST               7 (data)
-               
-               121         234 LOAD_FAST                2 (admin_site)
-                           236 LOAD_ATTR                4 (name)
-                           246 LOAD_FAST                1 (request)
-                           248 STORE_ATTR               5 (current_app)
-               
-               122         258 LOAD_GLOBAL             13 (NULL + Response)
-                           270 LOAD_FAST                7 (data)
-                           272 LOAD_GLOBAL             14 (status)
-                           284 LOAD_ATTR                8 (HTTP_200_OK)
-                           294 KW_NAMES                 8
-                           296 PRECALL                  2
-                           300 CALL                     2
-                           310 RETURN_VALUE
+               117         140 LOAD_GLOBAL              7 (NULL + reverse)
+                           152 LOAD_FAST                2 (admin_site)
+                           154 LOAD_ATTR                4 (name)
+                           164 FORMAT_VALUE             0
+                           166 LOAD_CONST               3 (':app_list')
+                           168 BUILD_STRING             2
+                           170 LOAD_CONST               4 ('app_label')
+                           172 LOAD_FAST                6 (app)
+                           174 LOAD_CONST               4 ('app_label')
+                           176 BINARY_SUBSCR
+                           186 BUILD_MAP                1
+                           188 LOAD_FAST                1 (request)
+                           190 KW_NAMES                 5
+                           192 PRECALL                  3
+                           196 CALL                     3
+                           206 LOAD_FAST                6 (app)
+                           208 LOAD_CONST               6 ('url')
+                           210 STORE_SUBSCR
+                           214 JUMP_BACKWARD           40 (to 136)
+               
+               119     >>  216 LOAD_CONST               7 ('app_list')
+                           218 LOAD_FAST                3 (app_list)
+               
+               118         220 BUILD_MAP                1
+                           222 STORE_FAST               7 (data)
+               
+               121         224 LOAD_FAST                2 (admin_site)
+                           226 LOAD_ATTR                4 (name)
+                           236 LOAD_FAST                1 (request)
+                           238 STORE_ATTR               5 (current_app)
+               
+               122         248 LOAD_GLOBAL             13 (NULL + Response)
+                           260 LOAD_FAST                7 (data)
+                           262 LOAD_GLOBAL             14 (status)
+                           274 LOAD_ATTR                8 (HTTP_200_OK)
+                           284 KW_NAMES                 8
+                           286 PRECALL                  2
+                           290 CALL                     2
+                           300 RETURN_VALUE
                consts
                   None
                   'https://'
                   'http://'
                   ':app_list'
                   'app_label'
-                  ('kwargs',)
+                  ('kwargs', 'request')
                   'url'
                   'app_list'
                   ('status',)
                names      ('get_app_list', 'get_host', 'is_secure', 'reverse', 'name', 'current_app', 'Response', 'status', 'HTTP_200_OK')
                varnames   ('self', 'request', 'admin_site', 'app_list', 'domain', 'scheme', 'app', 'data')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
                name       'get'
                firstlineno 110
-               lnotab 0x02012a03280130010801560204ff04031801
+               lnotab 0x02012a032801300108014c0204ff04031801
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'permission_classes', 'get')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
          name       'IndexView'
          firstlineno 103
          lnotab 0x0a0104040402
       'IndexView'
       code
          argcount  : 0
          nlocals   : 0
@@ -1018,15 +1015,15 @@
          
          126          10 LOAD_CONST               1 ('\n    Lists models inside a given app.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
          130          14 BUILD_LIST               0
                       16 STORE_NAME               4 (permission_classes)
          
-         132          18 LOAD_CONST               2 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 132>)
+         132          18 LOAD_CONST               2 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 132>)
                       20 MAKE_FUNCTION            0
                       22 STORE_NAME               5 (get)
                       24 LOAD_CONST               3 (None)
                       26 RETURN_VALUE
          consts
             'AppIndexView'
             '\n    Lists models inside a given app.\n    '
@@ -1074,15 +1071,15 @@
                            122 CALL                     2
                            132 RETURN_VALUE
                
                140     >>  134 LOAD_FAST                4 (app_dict)
                            136 LOAD_CONST               4 ('models')
                            138 BINARY_SUBSCR
                            148 LOAD_METHOD              5 (sort)
-                           170 LOAD_CONST               5 (<code object <lambda>, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 140>)
+                           170 LOAD_CONST               5 (<code object <lambda>, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 140>)
                            172 MAKE_FUNCTION            0
                            174 KW_NAMES                 6
                            176 PRECALL                  1
                            180 CALL                     1
                            190 POP_TOP
                
                143         192 LOAD_FAST                2 (app_label)
@@ -1121,34 +1118,34 @@
                      consts
                         None
                         'name'
                      names      ()
                      varnames   ('x',)
                      freevars   ()
                      cellvars   ()
-                     filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+                     filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
                      name       '<lambda>'
                      firstlineno 140
                      lnotab 0x
                   ('key',)
                   ('app_label', 'app')
                names      ('_build_app_dict', 'Response', '_', 'status', 'HTTP_404_NOT_FOUND', 'sort', 'HTTP_200_OK')
                varnames   ('self', 'request', 'app_label', 'admin_site', 'app_dict', 'data')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
                name       'get'
                firstlineno 132
                lnotab 0x02012c0204012c0116ff12043a03020102fe0605
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'permission_classes', 'get')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
          name       'AppIndexView'
          firstlineno 125
          lnotab 0x0a0104040402
       'AppIndexView'
       code
          argcount  : 0
          nlocals   : 0
@@ -1163,15 +1160,15 @@
          
          151          10 LOAD_CONST               1 ('\n      Returns json object with django.contrib.admin i18n translation catalog\n      to be used by a client site javascript library\n    ')
                       12 STORE_NAME               3 (__doc__)
          
          155          14 BUILD_LIST               0
                       16 STORE_NAME               4 (permission_classes)
          
-         157          18 LOAD_CONST               2 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 157>)
+         157          18 LOAD_CONST               2 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 157>)
                       20 MAKE_FUNCTION            0
                       22 STORE_NAME               5 (get)
                       24 LOAD_CONST               3 (None)
                       26 RETURN_VALUE
          consts
             'LanguageCatalogView'
             '\n      Returns json object with django.contrib.admin i18n translation catalog\n      to be used by a client site javascript library\n    '
@@ -1214,24 +1211,24 @@
                   'django_api_admin'
                   ('packages',)
                   ('status',)
                names      ('JSONCatalog', 'as_view', 'Response', 'content', 'status_code')
                varnames   ('self', 'request', 'response')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
                name       'get'
                firstlineno 157
                lnotab 0x02013e01
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'permission_classes', 'get')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
          name       'LanguageCatalogView'
          firstlineno 150
          lnotab 0x0a0104040402
       'LanguageCatalogView'
       code
          argcount  : 0
          nlocals   : 0
@@ -1246,15 +1243,15 @@
          
          163          10 LOAD_CONST               1 ("Handle AutocompleteWidget's AJAX requests for data.")
                       12 STORE_NAME               3 (__doc__)
          
          164          14 BUILD_LIST               0
                       16 STORE_NAME               4 (permission_classes)
          
-         166          18 LOAD_CONST               2 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 166>)
+         166          18 LOAD_CONST               2 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 166>)
                       20 MAKE_FUNCTION            0
                       22 STORE_NAME               5 (get)
                       24 LOAD_CONST               3 (None)
                       26 RETURN_VALUE
          consts
             'AutoCompleteView'
             "Handle AutocompleteWidget's AJAX requests for data."
@@ -1299,24 +1296,24 @@
                   ('admin_site',)
                   'content'
                   ('status',)
                names      ('AutocompleteJsonView', 'as_view', 'Response', 'content', 'status_code')
                varnames   ('self', 'request', 'admin_site', 'response')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
                name       'get'
                firstlineno 166
                lnotab 0x02013c01
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'permission_classes', 'get')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
          name       'AutoCompleteView'
          firstlineno 162
          lnotab 0x0a0104010402
       'AutoCompleteView'
       code
          argcount  : 0
          nlocals   : 0
@@ -1331,15 +1328,15 @@
          
          172          10 LOAD_CONST               1 ('\n    Returns the Attributes of AdminSite class (e.g. site_title, site_header)\n    ')
                       12 STORE_NAME               3 (__doc__)
          
          175          14 BUILD_LIST               0
                       16 STORE_NAME               4 (permission_classes)
          
-         177          18 LOAD_CONST               2 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 177>)
+         177          18 LOAD_CONST               2 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 177>)
                       20 MAKE_FUNCTION            0
                       22 STORE_NAME               5 (get)
                       24 LOAD_CONST               3 (None)
                       26 RETURN_VALUE
          consts
             'SiteContextView'
             '\n    Returns the Attributes of AdminSite class (e.g. site_title, site_header)\n    '
@@ -1373,24 +1370,24 @@
                consts
                   None
                   ('status',)
                names      ('each_context', 'Response', 'status', 'HTTP_200_OK')
                varnames   ('self', 'request', 'admin_site', 'context')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
                name       'get'
                firstlineno 177
                lnotab 0x02012a01
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'permission_classes', 'get')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
          name       'SiteContextView'
          firstlineno 171
          lnotab 0x0a0104030402
       'SiteContextView'
       code
          argcount  : 0
          nlocals   : 0
@@ -1418,23 +1415,23 @@
                       24 STORE_NAME               6 (permission_classes)
          
          189          26 LOAD_CONST               3 ('action_time')
                       28 LOAD_CONST               4 ('-action_time')
                       30 BUILD_LIST               2
                       32 STORE_NAME               7 (ordering_fields)
          
-         191          34 LOAD_CONST               5 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 191>)
+         191          34 LOAD_CONST               5 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 191>)
                       36 MAKE_FUNCTION            0
                       38 STORE_NAME               8 (get)
          
-         226          40 LOAD_CONST               6 (<code object serialize_messages, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 226>)
+         226          40 LOAD_CONST               6 (<code object serialize_messages, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 226>)
                       42 MAKE_FUNCTION            0
                       44 STORE_NAME               9 (serialize_messages)
          
-         232          46 LOAD_CONST               7 (<code object get_config, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 232>)
+         232          46 LOAD_CONST               7 (<code object get_config, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 232>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME              10 (get_config)
                       52 LOAD_CONST               2 (None)
                       54 RETURN_VALUE
          consts
             'AdminLogView'
             '\n    Returns a list of actions that were preformed using django admin.\n    '
@@ -1651,15 +1648,15 @@
                   True
                   ('many',)
                   ('action_list', 'config')
                names      ('django.contrib.admin.models', 'LogEntry', 'objects', 'all', 'request', 'query_params', 'get', 'ordering_fields', 'KeyError', 'order_by', 'Response', 'status', 'HTTP_400_BAD_REQUEST', 'filter', 'pagination_class', 'paginate_queryset', 'serializer_class', 'serialize_messages', 'data', 'get_config', 'HTTP_200_OK')
                varnames   ('self', 'request', 'admin_site', 'LogEntry', 'queryset', 'ordering', 'object_id', 'paginator', 'page', 'serializer')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
                name       'get'
                firstlineno 191
                lnotab
                   0x02010c02320302013e01040112010e012e010201440302013e01040130
                   0102014403280130032e020c0132012afe040316fd
             code
                argcount  : 2
@@ -1712,15 +1709,15 @@
                   ('start',)
                   'change_message'
                   '[]'
                names      ('enumerate', 'json', 'loads')
                varnames   ('self', 'data', 'idx', 'item')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
                name       'serialize_messages'
                firstlineno 226
                lnotab 0x02012c01160112ff2402
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 3
@@ -1747,23 +1744,23 @@
                consts
                   None
                   ('result_count', 'full_result_count')
                names      ('len', 'count')
                varnames   ('self', 'page', 'queryset')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
                name       'get_config'
                firstlineno 232
                lnotab 0x02021c0126fe
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'serializer_class', 'pagination_class', 'permission_classes', 'ordering_fields', 'get', 'serialize_messages', 'get_config')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
          name       'AdminLogView'
          firstlineno 182
          lnotab 0x0a010403040104010401080206230606
       'AdminLogView'
       code
          argcount  : 0
          nlocals   : 0
@@ -1778,15 +1775,15 @@
          
          240          10 LOAD_CONST               1 ('\n    A list of all root urls in django_api_admin\n    ')
                       12 STORE_NAME               3 (__doc__)
          
          243          14 LOAD_CONST               2 (None)
                       16 STORE_NAME               4 (root_urls)
          
-         245          18 LOAD_CONST               3 (<code object get, file "/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py", line 245>)
+         245          18 LOAD_CONST               3 (<code object get, file "/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py", line 245>)
                       20 MAKE_FUNCTION            0
                       22 STORE_NAME               5 (get)
                       24 LOAD_CONST               2 (None)
                       26 RETURN_VALUE
          consts
             'AdminAPIRootView'
             '\n    A list of all root urls in django_api_admin\n    '
@@ -1795,26 +1792,25 @@
                argcount  : 2
                nlocals   : 9
                stacksize : 7
                flags     : 15
                code
                   0x97007c016a0000000000000000006a0100000000000000007d04740500
                   000000000000000000a6000000ab0000000000000000007d057c006a0300
-                  0000000000000044005d877d067c016a0400000000000000006a05000000
+                  0000000000000044005d827d067c016a0400000000000000006a05000000
                   0000000000720c7c066a06000000000000000064016b020000000072018c
                   1a7c016a0400000000000000006a050000000000000000730a7c066a0600
                   000000000000006402760072018c307c01a0070000000000000000000000
                   000000000000000000a6000000ab0000000000000000007d077c01a00800
                   00000000000000000000000000000000000000a6000000ab000000000000
-                  000000720264036e0164047d087c087c077a000000741300000000000000
-                  0000007c0464057a0000007c066a0600000000000000007a0000007c027c
-                  03ac06a6030000ab0300000000000000007a0000007c057c066a06000000
-                  00000000003c0000008c887415000000000000000000007c057001690074
-                  16000000000000000000006a0c0000000000000000ac07a6020000ab0200
-                  000000000000005300
+                  000000720264036e0164047d087413000000000000000000007c0464057a
+                  0000007c066a0600000000000000007a0000007c027c037c01ac06a60400
+                  00ab0400000000000000007c057c066a0600000000000000003c0000008c
+                  837415000000000000000000007c05700169007416000000000000000000
+                  006a0c0000000000000000ac07a6020000ab0200000000000000005300
                245           0 RESUME                   0
                
                246           2 LOAD_FAST                1 (request)
                              4 LOAD_ATTR                0 (resolver_match)
                             14 LOAD_ATTR                1 (namespace)
                             24 STORE_FAST               4 (namespace)
                
@@ -1822,15 +1818,15 @@
                             38 PRECALL                  0
                             42 CALL                     0
                             52 STORE_FAST               5 (data)
                
                249          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                3 (root_urls)
                             66 GET_ITER
-                       >>   68 FOR_ITER               135 (to 340)
+                       >>   68 FOR_ITER               130 (to 330)
                             70 STORE_FAST               6 (url)
                
                250          72 LOAD_FAST                1 (request)
                             74 LOAD_ATTR                4 (user)
                             84 LOAD_ATTR                5 (is_authenticated)
                             94 POP_JUMP_FORWARD_IF_FALSE    12 (to 120)
                             96 LOAD_FAST                6 (url)
@@ -1865,75 +1861,72 @@
                            232 CALL                     0
                            242 POP_JUMP_FORWARD_IF_FALSE     2 (to 248)
                            244 LOAD_CONST               3 ('https://')
                            246 JUMP_FORWARD             1 (to 250)
                        >>  248 LOAD_CONST               4 ('http://')
                        >>  250 STORE_FAST               8 (scheme)
                
-               257         252 LOAD_FAST                8 (scheme)
-                           254 LOAD_FAST                7 (domain)
-                           256 BINARY_OP                0 (+)
-                           260 LOAD_GLOBAL             19 (NULL + reverse)
-                           272 LOAD_FAST                4 (namespace)
-                           274 LOAD_CONST               5 (':')
-                           276 BINARY_OP                0 (+)
-                           280 LOAD_FAST                6 (url)
-                           282 LOAD_ATTR                6 (name)
-                           292 BINARY_OP                0 (+)
-                           296 LOAD_FAST                2 (args)
-                           298 LOAD_FAST                3 (kwargs)
-                           300 KW_NAMES                 6
-                           302 PRECALL                  3
-                           306 CALL                     3
-                           316 BINARY_OP                0 (+)
-                           320 LOAD_FAST                5 (data)
-                           322 LOAD_FAST                6 (url)
-                           324 LOAD_ATTR                6 (name)
-                           334 STORE_SUBSCR
-                           338 JUMP_BACKWARD          136 (to 68)
-               
-               259     >>  340 LOAD_GLOBAL             21 (NULL + Response)
-                           352 LOAD_FAST                5 (data)
-                           354 JUMP_IF_TRUE_OR_POP      1 (to 358)
-                           356 BUILD_MAP                0
-                       >>  358 LOAD_GLOBAL             22 (status)
-                           370 LOAD_ATTR               12 (HTTP_200_OK)
-                           380 KW_NAMES                 7
-                           382 PRECALL                  2
-                           386 CALL                     2
-                           396 RETURN_VALUE
+               257         252 LOAD_GLOBAL             19 (NULL + reverse)
+                           264 LOAD_FAST                4 (namespace)
+                           266 LOAD_CONST               5 (':')
+                           268 BINARY_OP                0 (+)
+                           272 LOAD_FAST                6 (url)
+                           274 LOAD_ATTR                6 (name)
+                           284 BINARY_OP                0 (+)
+                           288 LOAD_FAST                2 (args)
+                           290 LOAD_FAST                3 (kwargs)
+                           292 LOAD_FAST                1 (request)
+                           294 KW_NAMES                 6
+                           296 PRECALL                  4
+                           300 CALL                     4
+                           310 LOAD_FAST                5 (data)
+                           312 LOAD_FAST                6 (url)
+                           314 LOAD_ATTR                6 (name)
+                           324 STORE_SUBSCR
+                           328 JUMP_BACKWARD          131 (to 68)
+               
+               259     >>  330 LOAD_GLOBAL             21 (NULL + Response)
+                           342 LOAD_FAST                5 (data)
+                           344 JUMP_IF_TRUE_OR_POP      1 (to 348)
+                           346 BUILD_MAP                0
+                       >>  348 LOAD_GLOBAL             22 (status)
+                           360 LOAD_ATTR               12 (HTTP_200_OK)
+                           370 KW_NAMES                 7
+                           372 PRECALL                  2
+                           376 CALL                     2
+                           386 RETURN_VALUE
                consts
                   None
                   'login'
                   ('logout', 'password_change')
                   'https://'
                   'http://'
                   ':'
-                  ('args', 'kwargs')
+                  ('args', 'kwargs', 'request')
                   ('status',)
                names      ('resolver_match', 'namespace', 'dict', 'root_urls', 'user', 'is_authenticated', 'name', 'get_host', 'is_secure', 'reverse', 'Response', 'status', 'HTTP_200_OK')
                varnames   ('self', 'request', 'args', 'kwargs', 'namespace', 'data', 'url', 'domain', 'scheme')
                freevars   ()
                cellvars   ()
-               filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+               filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
                name       'get'
                firstlineno 245
-               lnotab 0x020118011c0212012e0102012a010202280130015802
+               lnotab 0x020118011c0212012e0102012a010202280130014e02
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'root_urls', 'get')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+         filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
          name       'AdminAPIRootView'
          firstlineno 239
          lnotab 0x0a0104030402
       'AdminAPIRootView'
-   names      ('__doc__', 'json', 'django.contrib.admin.views.autocomplete', 'AutocompleteJsonView', 'django.contrib.auth', 'login', 'logout', 'django.middleware.csrf', 'get_token', 'django.utils.translation', 'gettext_lazy', '_', 'django.views.i18n', 'JSONCatalog', 'django.urls', 'reverse', 'rest_framework', 'status', 'rest_framework.response', 'Response', 'rest_framework.views', 'APIView', 'django_api_admin.declarations.functions', 'get_form_fields', 'CsrfTokenView', 'UserInformation', 'LoginView', 'LogoutView', 'PasswordChangeView', 'IndexView', 'AppIndexView', 'LanguageCatalogView', 'AutoCompleteView', 'SiteContextView', 'AdminLogView', 'AdminAPIRootView')
+   names      ('__doc__', 'json', 'django.contrib.admin.views.autocomplete', 'AutocompleteJsonView', 'django.contrib.auth', 'login', 'logout', 'django.middleware.csrf', 'get_token', 'django.utils.translation', 'gettext_lazy', '_', 'django.views.i18n', 'JSONCatalog', 'rest_framework', 'status', 'rest_framework.response', 'Response', 'rest_framework.views', 'APIView', 'rest_framework.reverse', 'reverse', 'django_api_admin.declarations.functions', 'get_form_fields', 'CsrfTokenView', 'UserInformation', 'LoginView', 'LogoutView', 'PasswordChangeView', 'IndexView', 'AppIndexView', 'LanguageCatalogView', 'AutoCompleteView', 'SiteContextView', 'AdminLogView', 'AdminAPIRootView')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/demon-bixia/Documents/projects/bolt-theme/django-api-admin/django_api_admin/views/site_views.py'
+   filename   '/home/demon-bixia/Documents/projects/django-api-admin/django_api_admin/views/site_views.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201040308020c0110010c010c010c010c020c010c010c020c061c
+      0x00ff0201040308020c0110010c010c010c020c010c010c010c020c061c
       081c091c1f1c0e1c121c161c191c0c1c091c0b1c39
```

### Comparing `django-api-admin-1.1.4/django_api_admin/views/admin_views.py` & `django-api-admin-1.1.5/django_api_admin/views/admin_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,16 @@
             admin.model._meta.model_name
         )
         pattern = '%s:%s_%s_detail'
 
         domain = request.get_host()
         scheme = 'https://' if request.is_secure() else 'http://'
         for item in data:
-            path = reverse(pattern % info, kwargs={
+            item['detail_url'] = reverse(pattern % info, kwargs={
                 'object_id': int(item['pk'])}, request=request)
-            item['detail_url'] = scheme + domain + path
         return Response(data, status=status.HTTP_200_OK)
 
 
 class DetailView(APIView):
     """
     GET one instance of this model using pk and to_fields.
     """
@@ -87,20 +86,20 @@
         )
         pattern = '%s:%s_%s_'
         domain = request.get_host()
         scheme = 'https://' if request.is_secure() else 'http://'
         if admin.view_on_site:
             model_type = ContentType.objects.get_for_model(
                 model=admin.model)    
-        data['view_on_site'] = scheme + domain + reverse('%s:view_on_site' % admin.admin_site.name, kwargs={ 'content_type_id': model_type.pk, 'object_id': obj.pk}, request=request)
-        data['list_url'] = scheme + domain + reverse((pattern + 'list') % info, request=request)
-        data['history_url'] = scheme + domain + reverse((pattern + 'history') % info, kwargs={'object_id': data['pk']}, request=request)
-        data['delete_url'] = scheme + domain + reverse(
+        data['view_on_site'] = reverse('%s:view_on_site' % admin.admin_site.name, kwargs={ 'content_type_id': model_type.pk, 'object_id': obj.pk}, request=request)
+        data['list_url'] = reverse((pattern + 'list') % info, request=request)
+        data['history_url'] = reverse((pattern + 'history') % info, kwargs={'object_id': data['pk']}, request=request)
+        data['delete_url'] = reverse(
             (pattern + 'delete') % info, kwargs={'object_id': data['pk']}, request=request)
-        data['change_url'] = scheme + domain + reverse(
+        data['change_url'] = reverse(
             (pattern + 'change') % info, kwargs={'object_id': data['pk']}, request=request)
         return Response(data, status=status.HTTP_200_OK)
 
 
 class AddView(APIView):
     """
     Add new instances of this model. if this model has inline models associated with it 
@@ -488,15 +487,15 @@
         empty_value_display = cl.model_admin.get_empty_value_display()
         domain = request.get_host()
         scheme = 'https://' if request.is_secure() else 'http://'
         for result in cl.result_list:
             model_info = (cl.model_admin.admin_site.name, type(
                 result)._meta.app_label, type(result)._meta.model_name)
             row = {
-                'change_url': scheme + domain + reverse('%s:%s_%s_change' % model_info, kwargs={'object_id': result.pk}, request=request),
+                'change_url': reverse('%s:%s_%s_change' % model_info, kwargs={'object_id': result.pk}, request=request),
                 'id': result.pk,
                 'cells': {}
             }
 
             for field_name in self.get_fields_list(request, cl):
                 try:
                     _, _, value = lookup_field(
```

### Comparing `django-api-admin-1.1.4/django_api_admin/views/site_views.py` & `django-api-admin-1.1.5/django_api_admin/views/site_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 import json
 
 from django.contrib.admin.views.autocomplete import AutocompleteJsonView
 from django.contrib.auth import login, logout
 from django.middleware.csrf import get_token
 from django.utils.translation import gettext_lazy as _
 from django.views.i18n import JSONCatalog
-from django.urls import reverse
 
 from rest_framework import status
 from rest_framework.response import Response
 from rest_framework.views import APIView
+from rest_framework.reverse import reverse
 
 from django_api_admin.declarations.functions import get_form_fields
 # todo split the views file.
 # todo add more comments.
 # todo add support for bulk edits.
 
 
@@ -110,15 +110,15 @@
     def get(self, request, admin_site):
         app_list = admin_site.get_app_list(request)
 
         # add an url to app_index in every app in app_list
         domain = request.get_host()
         scheme = 'https://' if request.is_secure() else 'http://'
         for app in app_list:
-            app['url'] = scheme + domain + reverse(f'{admin_site.name}:app_list', kwargs={ 'app_label': app['app_label']})
+            app['url'] =  reverse(f'{admin_site.name}:app_list', kwargs={ 'app_label': app['app_label']}, request=request)
         data = {
             'app_list': app_list,
         }
         request.current_app = admin_site.name
         return Response(data, status=status.HTTP_200_OK)
 
 
@@ -250,10 +250,10 @@
             if request.user.is_authenticated and url.name == 'login':
                 continue
             elif not request.user.is_authenticated and url.name in ('logout', 'password_change'):
                 continue
 
             domain = request.get_host()
             scheme = 'https://' if request.is_secure() else 'http://'
-            data[url.name] = scheme + domain + reverse(namespace + ':' + url.name, args=args, kwargs=kwargs)
+            data[url.name] = reverse(namespace + ':' + url.name, args=args, kwargs=kwargs, request=request)
 
         return Response(data or {}, status=status.HTTP_200_OK)
```

### Comparing `django-api-admin-1.1.4/django_api_admin.egg-info/PKG-INFO` & `django-api-admin-1.1.5/django_api_admin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-api-admin
-Version: 1.1.4
+Version: 1.1.5
 Summary: Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.
 Home-page: https://github.com/MuhammadSalahAli/django-api-admin
 Author: Muhammad Salah
 Author-email: msmainacc0unt@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `django-api-admin-1.1.4/django_api_admin.egg-info/SOURCES.txt` & `django-api-admin-1.1.5/django_api_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-api-admin-1.1.4/setup.py` & `django-api-admin-1.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="django-api-admin",
-    version="1.1.4",
+    version="1.1.5",
     description="Expose django.contrib.admin as a restful service. useful for adding new features to django admin or writing a new admin.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/MuhammadSalahAli/django-api-admin",
     author="Muhammad Salah",
     author_email="msmainacc0unt@gmail.com",
     license="MIT",
```

