# Comparing `tmp/django-eskiz-sms-0.1.1.tar.gz` & `tmp/django-eskiz-sms-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-eskiz-sms-0.1.1.tar", last modified: Sat Jul 15 02:58:52 2023, max compression
+gzip compressed data, was "django-eskiz-sms-0.1.2.tar", last modified: Sat Jul 15 08:58:44 2023, max compression
```

## Comparing `django-eskiz-sms-0.1.1.tar` & `django-eskiz-sms-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 02:58:52.884720 django-eskiz-sms-0.1.1/
--rw-rw-rw-   0        0        0     1075 2023-07-15 02:08:16.000000 django-eskiz-sms-0.1.1/LICENCE
--rw-rw-rw-   0        0        0       78 2023-07-15 02:08:52.000000 django-eskiz-sms-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      987 2023-07-15 02:58:52.884720 django-eskiz-sms-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-07-15 02:57:44.000000 django-eskiz-sms-0.1.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-15 02:58:52.836739 django-eskiz-sms-0.1.1/django_eskiz_sms.egg-info/
--rw-rw-rw-   0        0        0      987 2023-07-15 02:58:52.000000 django-eskiz-sms-0.1.1/django_eskiz_sms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-07-15 02:58:52.000000 django-eskiz-sms-0.1.1/django_eskiz_sms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 02:58:52.000000 django-eskiz-sms-0.1.1/django_eskiz_sms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-15 02:58:52.000000 django-eskiz-sms-0.1.1/django_eskiz_sms.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-15 02:58:52.868733 django-eskiz-sms-0.1.1/eskiz_sms/
--rw-rw-rw-   0        0        0        0 2023-07-14 21:50:03.000000 django-eskiz-sms-0.1.1/eskiz_sms/__init__.py
--rw-rw-rw-   0        0        0      548 2023-07-15 01:07:25.000000 django-eskiz-sms-0.1.1/eskiz_sms/admin.py
--rw-rw-rw-   0        0        0      155 2023-07-14 21:50:04.000000 django-eskiz-sms-0.1.1/eskiz_sms/apps.py
-drwxrwxrwx   0        0        0        0 2023-07-15 02:58:52.876721 django-eskiz-sms-0.1.1/eskiz_sms/migrations/
--rw-rw-rw-   0        0        0     2927 2023-07-15 01:14:42.000000 django-eskiz-sms-0.1.1/eskiz_sms/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-07-14 21:50:03.000000 django-eskiz-sms-0.1.1/eskiz_sms/migrations/__init__.py
--rw-rw-rw-   0        0        0     2064 2023-07-15 01:07:52.000000 django-eskiz-sms-0.1.1/eskiz_sms/models.py
-drwxrwxrwx   0        0        0        0 2023-07-15 02:58:52.884720 django-eskiz-sms-0.1.1/eskiz_sms/templates/
--rw-rw-rw-   0        0        0      931 2023-07-15 01:13:57.000000 django-eskiz-sms-0.1.1/eskiz_sms/templates/send_sms.html
--rw-rw-rw-   0        0        0      161 2023-07-15 01:08:28.000000 django-eskiz-sms-0.1.1/eskiz_sms/urls.py
--rw-rw-rw-   0        0        0     1651 2023-07-15 01:07:39.000000 django-eskiz-sms-0.1.1/eskiz_sms/views.py
--rw-rw-rw-   0        0        0      894 2023-07-15 02:58:52.892728 django-eskiz-sms-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-07-15 02:27:20.000000 django-eskiz-sms-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 08:58:44.075863 django-eskiz-sms-0.1.2/
+-rw-rw-rw-   0        0        0       78 2023-07-15 02:08:52.000000 django-eskiz-sms-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2285 2023-07-15 08:58:44.075863 django-eskiz-sms-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      969 2023-07-15 08:58:18.000000 django-eskiz-sms-0.1.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-15 08:58:44.019740 django-eskiz-sms-0.1.2/django_eskiz_sms.egg-info/
+-rw-rw-rw-   0        0        0     2285 2023-07-15 08:58:43.000000 django-eskiz-sms-0.1.2/django_eskiz_sms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2023-07-15 08:58:43.000000 django-eskiz-sms-0.1.2/django_eskiz_sms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 08:58:43.000000 django-eskiz-sms-0.1.2/django_eskiz_sms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-15 08:58:43.000000 django-eskiz-sms-0.1.2/django_eskiz_sms.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-07-15 08:58:43.000000 django-eskiz-sms-0.1.2/django_eskiz_sms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-15 08:58:43.000000 django-eskiz-sms-0.1.2/django_eskiz_sms.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 08:58:44.057302 django-eskiz-sms-0.1.2/eskiz_sms/
+-rw-rw-rw-   0        0        0        0 2023-07-14 21:50:03.000000 django-eskiz-sms-0.1.2/eskiz_sms/__init__.py
+-rw-rw-rw-   0        0        0      548 2023-07-15 01:07:25.000000 django-eskiz-sms-0.1.2/eskiz_sms/admin.py
+-rw-rw-rw-   0        0        0      155 2023-07-14 21:50:04.000000 django-eskiz-sms-0.1.2/eskiz_sms/apps.py
+drwxrwxrwx   0        0        0        0 2023-07-15 08:58:44.067866 django-eskiz-sms-0.1.2/eskiz_sms/migrations/
+-rw-rw-rw-   0        0        0     2927 2023-07-15 01:14:42.000000 django-eskiz-sms-0.1.2/eskiz_sms/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2023-07-14 21:50:03.000000 django-eskiz-sms-0.1.2/eskiz_sms/migrations/__init__.py
+-rw-rw-rw-   0        0        0     2064 2023-07-15 01:07:52.000000 django-eskiz-sms-0.1.2/eskiz_sms/models.py
+drwxrwxrwx   0        0        0        0 2023-07-15 08:58:44.075863 django-eskiz-sms-0.1.2/eskiz_sms/templates/
+-rw-rw-rw-   0        0        0      931 2023-07-15 01:13:57.000000 django-eskiz-sms-0.1.2/eskiz_sms/templates/send_sms.html
+-rw-rw-rw-   0        0        0      161 2023-07-15 01:08:28.000000 django-eskiz-sms-0.1.2/eskiz_sms/urls.py
+-rw-rw-rw-   0        0        0     1651 2023-07-15 01:07:39.000000 django-eskiz-sms-0.1.2/eskiz_sms/views.py
+-rw-rw-rw-   0        0        0       93 2023-07-15 08:41:20.000000 django-eskiz-sms-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      252 2023-07-15 08:58:44.084863 django-eskiz-sms-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1750 2023-07-15 08:56:03.000000 django-eskiz-sms-0.1.2/setup.py
```

### Comparing `django-eskiz-sms-0.1.1/eskiz_sms/admin.py` & `django-eskiz-sms-0.1.2/eskiz_sms/admin.py`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1.1/eskiz_sms/migrations/0001_initial.py` & `django-eskiz-sms-0.1.2/eskiz_sms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1.1/eskiz_sms/models.py` & `django-eskiz-sms-0.1.2/eskiz_sms/models.py`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1.1/eskiz_sms/templates/send_sms.html` & `django-eskiz-sms-0.1.2/eskiz_sms/templates/send_sms.html`

 * *Files identical despite different names*

### Comparing `django-eskiz-sms-0.1.1/eskiz_sms/views.py` & `django-eskiz-sms-0.1.2/eskiz_sms/views.py`

 * *Files identical despite different names*

