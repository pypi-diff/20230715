# Comparing `tmp/django-glue-0.4.0.tar.gz` & `tmp/django-glue-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-glue-0.4.0.tar", last modified: Mon Jul 10 19:18:47 2023, max compression
+gzip compressed data, was "django-glue-0.4.1.tar", last modified: Sat Jul 15 03:10:35 2023, max compression
```

## Comparing `django-glue-0.4.0.tar` & `django-glue-0.4.1.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.818792 django-glue-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-10 19:18:36.000000 django-glue-0.4.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-10 19:18:36.000000 django-glue-0.4.0/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-10 19:18:36.000000 django-glue-0.4.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-10 19:18:36.000000 django-glue-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-10 19:18:47.818792 django-glue-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-10 19:18:36.000000 django-glue-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.814792 django-glue-0.4.0/django_glue/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.814792 django-glue-0.4.0/django_glue/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/glue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.814792 django-glue-0.4.0/django_glue/services/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/services/model_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/services/query_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/services/services.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/services/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.810792 django-glue-0.4.0/django_glue/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.810792 django-glue-0.4.0/django_glue/static/django_glue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.814792 django-glue-0.4.0/django_glue/static/django_glue/js/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_ajax.js
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_csrf.js
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_event.js
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_message.js
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_model_object.js
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_query_set.js
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_response.js
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_template.js
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_view.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.810792 django-glue-0.4.0/django_glue/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.818792 django-glue-0.4.0/django_glue/templates/django_glue/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/templates/django_glue/django_glue.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.818792 django-glue-0.4.0/django_glue/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/templatetags/django_glue.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-10 19:18:36.000000 django-glue-0.4.0/django_glue/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.814792 django-glue-0.4.0/django_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-10 19:18:47.000000 django-glue-0.4.0/django_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-10 19:18:47.000000 django-glue-0.4.0/django_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:18:47.000000 django-glue-0.4.0/django_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:18:47.000000 django-glue-0.4.0/django_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 19:18:47.000000 django-glue-0.4.0/django_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 19:18:47.000000 django-glue-0.4.0/django_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-10 19:18:36.000000 django-glue-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 19:18:47.818792 django-glue-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-10 19:18:36.000000 django-glue-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.818792 django-glue-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:47.818792 django-glue-0.4.0/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-10 19:18:36.000000 django-glue-0.4.0/tests/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.604376 django-glue-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-15 03:10:24.000000 django-glue-0.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-15 03:10:24.000000 django-glue-0.4.1/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-15 03:10:24.000000 django-glue-0.4.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-15 03:10:24.000000 django-glue-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-15 03:10:35.604376 django-glue-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-15 03:10:24.000000 django-glue-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.600376 django-glue-0.4.1/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.600376 django-glue-0.4.1/django_glue/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.600376 django-glue-0.4.1/django_glue/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/services/model_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/services/query_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/services/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/services/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.596377 django-glue-0.4.1/django_glue/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.596377 django-glue-0.4.1/django_glue/static/django_glue/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.604376 django-glue-0.4.1/django_glue/static/django_glue/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_ajax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_csrf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_event.js
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_keep_live.js
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_message.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_model_object.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_query_set.js
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_response.js
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_template.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_view.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.596377 django-glue-0.4.1/django_glue/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.604376 django-glue-0.4.1/django_glue/templates/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/templates/django_glue/django_glue.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.604376 django-glue-0.4.1/django_glue/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/templatetags/django_glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-15 03:10:24.000000 django-glue-0.4.1/django_glue/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.600376 django-glue-0.4.1/django_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-15 03:10:35.000000 django-glue-0.4.1/django_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-15 03:10:35.000000 django-glue-0.4.1/django_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 03:10:35.000000 django-glue-0.4.1/django_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 03:10:35.000000 django-glue-0.4.1/django_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 03:10:35.000000 django-glue-0.4.1/django_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-15 03:10:35.000000 django-glue-0.4.1/django_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-15 03:10:24.000000 django-glue-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-15 03:10:35.604376 django-glue-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-15 03:10:24.000000 django-glue-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.604376 django-glue-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:35.604376 django-glue-0.4.1/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-15 03:10:24.000000 django-glue-0.4.1/tests/wsgi.py
```

### Comparing `django-glue-0.4.0/CHANGELOG.md` & `django-glue-0.4.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 ## 0.4.1
 
 #### Features
 - Event system implement for responses.
 
 #### Changes
-
-#### Bugs
+- Keep live system update to work with template and view loading.
+- Context removed from Javascript
 
 ## 0.4.0
 
 #### Features
 - You can now glue templates by submitting a full template path as a string to add_glue function call.
 - You can now use the experimental load views in your templates with GlueView.
```

### Comparing `django-glue-0.4.0/LICENSE.md` & `django-glue-0.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/PKG-INFO` & `django-glue-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.4.0
+Version: 0.4.1
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
 Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-glue-0.4.0/README.md` & `django-glue-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/django_glue/context_processors.py` & `django-glue-0.4.1/django_glue/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/django_glue/data_classes.py` & `django-glue-0.4.1/django_glue/data_classes.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/django_glue/enums.py` & `django-glue-0.4.1/django_glue/enums.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/django_glue/glue.py` & `django-glue-0.4.1/django_glue/glue.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/django_glue/handlers.py` & `django-glue-0.4.1/django_glue/handlers.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/django_glue/middleware.py` & `django-glue-0.4.1/django_glue/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,10 +15,10 @@
     def process_view(request, view_func, view_args, view_kwargs):
         current_url = resolve(request.path_info).url_name
 
         if current_url != 'django_glue_handler':
             glue_session = GlueSession(request)
             glue_keep_live_session = GlueKeepLiveSession(request)
 
-            glue_session.clean(glue_keep_live_session.clean_and_get_expired_unique_name_set())
+            glue_session.clean(glue_keep_live_session.clean_and_get_expired_unique_names())
 
         return None
```

### Comparing `django-glue-0.4.0/django_glue/responses.py` & `django-glue-0.4.1/django_glue/responses.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/django_glue/services/model_objects.py` & `django-glue-0.4.1/django_glue/services/model_objects.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/django_glue/services/query_sets.py` & `django-glue-0.4.1/django_glue/services/query_sets.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/django_glue/services/services.py` & `django-glue-0.4.1/django_glue/services/services.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/django_glue/services/templates.py` & `django-glue-0.4.1/django_glue/services/templates.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/django_glue/sessions.py` & `django-glue-0.4.1/django_glue/sessions.py`

 * *Files 13% similar despite different names*

```diff
@@ -117,16 +117,16 @@
     def add_meta(self, unique_name, meta_data: GlueMetaData) -> None:
         self.session['meta'][unique_name] = meta_data.to_dict()
 
     def check_unique_name(self, unique_name):
         if self.unique_name_unused(unique_name):
             self.purge_unique_name(unique_name)
 
-    def clean(self, removable_unique_name_set):
-        for unique_name in removable_unique_name_set:
+    def clean(self, removable_unique_names):
+        for unique_name in removable_unique_names:
             self.purge_unique_name(unique_name)
 
         self.set_modified()
 
     def purge_unique_name(self, unique_name):
         for session_type in GLUE_SESSION_TYPES:
             if unique_name in self.session[session_type]:
@@ -149,49 +149,39 @@
 
     def __getitem__(self, key):
         return self.session[key]
 
     def __setitem__(self, key, value):
         self.session[key] = value
 
-    def clean_and_get_expired_unique_name_set(self) -> set:
-        expired_session_list = list()
-
-        expired_unique_name_set = set()
-        active_unique_name_set = set()
+    def clean_and_get_expired_unique_names(self) -> list:
+        expired_unique_names = []
 
         for key, val in self.session.items():
-            if time() > val['expire_time']:
-                expired_unique_name_set.update(val['unique_name_list'])
-                expired_session_list.append(key)
-            else:
-                active_unique_name_set.update(val['unique_name_list'])
+            if time() > val:
+                expired_unique_names.append(key)
 
-        for expired_session in expired_session_list:
-            self.session.pop(expired_session)
+        for expired_unique_name in expired_unique_names:
+            self.session.pop(expired_unique_name)
 
         self.set_modified()
 
-        return expired_unique_name_set.difference(active_unique_name_set)
+        return expired_unique_names
 
     @staticmethod
     def get_next_expire_time():
         return time() + settings.DJANGO_GLUE_KEEP_LIVE_EXPIRE_TIME_SECONDS
 
     def set_unique_name(self, unique_name):
-
-        self.setdefault = self.session.setdefault(self.request.path, {'expire_time': self.get_next_expire_time(),
-                                                                      'unique_name_list': [], })
-
-        if unique_name not in self.session[self.request.path]['unique_name_list']:
-            self.session[self.request.path]['unique_name_list'].append(unique_name)
+        self.session.setdefault(unique_name, self.get_next_expire_time())
 
         self.set_modified()
 
     def set_modified(self):
         self.request.session.modified = True
 
-    def update_url_path(self, url_path):
-        if url_path in self.session:
-            self.session[url_path]['expire_time'] = self.get_next_expire_time()
+    def update_unique_names(self, unique_names: list):
+        for unique_name in unique_names:
+            if unique_name in self.session:
+                self.session[unique_name] = self.get_next_expire_time()
 
         self.set_modified()
```

### Comparing `django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_ajax.js` & `django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_ajax.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -12,15 +12,15 @@
             'X-CSRFToken': glue_get_cookie('csrftoken'),
         },
         body: JSON.stringify({
             'unique_name': unique_name,
             'action': action,
             'data': data,
         }),
-    };
+    }
 
     const response = await fetch(DJANGO_GLUE_AJAX_URL, request_options);
     if (!response.ok) {
         throw new Error(`HTTP error ${response.status}`);
     }
 
     if (content_type === 'application/json') {
```

### Comparing `django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_model_object.js` & `django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_model_object.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,11 @@
 class GlueModelObject {
     constructor(unique_name) {
         this.unique_name = unique_name
+        window.glue_keep_live.add_unique_name(unique_name)
         this.context_data = {
             fields: {}
         }
     }
 
     generate_field_data() {
         let data = {}
@@ -16,14 +17,15 @@
 
     async get(load_value = true) {
         await glue_ajax_request(
             this.unique_name,
             'get'
         ).then((response) => {
             console.log(response)
+            glue_dispatch_response_event(response)
             let simple_fields = response.data.simple_fields
             for (let key in simple_fields) {
                 if (load_value) {
                     this[key] = simple_fields[key]
                 } else {
                     this[key] = null
                 }
@@ -43,27 +45,29 @@
         }
 
         await glue_ajax_request(
             this.unique_name,
             'update',
             data
         ).then((response) => {
+            glue_dispatch_response_event(response)
             console.log(response)
         })
     }
 
     async create() {
         let data = this.generate_field_data()
 
         return await glue_ajax_request(
             this.unique_name,
             'create',
             data
         ).then((response) => {
             console.log(response)
+            glue_dispatch_response_event(response)
             let model_object = new GlueModelObject(this.unique_name)
 
             let simple_fields = response.data.simple_fields
             for (let key in simple_fields) {
                 model_object[key] = simple_fields[key]
             }
             return model_object
@@ -73,14 +77,15 @@
 
     delete() {
         glue_ajax_request(
             this.unique_name,
             'delete'
         ).then((response) => {
             console.log(response)
+            glue_dispatch_response_event(response)
         })
     }
 
     async method(method, kwargs = {}) {
         let data = {
             'method': method,
             'kwargs': kwargs,
@@ -88,12 +93,13 @@
 
         return await glue_ajax_request(
             this.unique_name,
             'method',
             data
         ).then((response) => {
             console.log(response)
+            glue_dispatch_response_event(response)
             return response.data.method_return
         })
     }
 
 }
```

### Comparing `django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_query_set.js` & `django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_query_set.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,26 @@
 class GlueQuerySet {
     constructor(unique_name) {
         this.unique_name = unique_name
+        window.glue_keep_live.add_unique_name(unique_name)
         this.context_data = {
             fields: []
         }
     }
 
     async get(id) {
         let model_object_list = []
         let model_object = null
         return await glue_ajax_request(this.unique_name, 'get', {
                 'id': id
             })
             .then((response) => {
                 model_object = new GlueModelObject(this.unique_name);
                 console.log(response)
+                glue_dispatch_response_event(response)
                 let simple_fields = response.data.simple_fields;
                 for (let key in simple_fields) {
                     model_object[key] = simple_fields[key];
                 }
                 model_object_list.push(model_object)
                 return model_object_list
             });
@@ -29,14 +31,15 @@
         let model_object = null
 
         return await glue_ajax_request(this.unique_name, 'get', {
                 'all': true
             })
             .then((response) => {
                 console.log(response)
+                glue_dispatch_response_event(response)
                 for (let object in response.data) {
                     model_object = new GlueModelObject(this.unique_name);
 
                     let simple_fields = response.data[object].simple_fields;
                     for (let key in simple_fields) {
                         model_object[key] = simple_fields[key];
                     }
@@ -60,26 +63,28 @@
 
         glue_ajax_request(
             this.unique_name,
             'update',
             data
         ).then((response) => {
             console.log(response)
+            glue_dispatch_response_event(response)
         })
     }
 
     async filter(filter_params) {
         let model_object_list = []
         let model_object = null
 
         return await glue_ajax_request(this.unique_name, 'get', {
                 'filter_params': filter_params
             })
             .then((response) => {
                 console.log(response)
+                glue_dispatch_response_event(response)
                 for (let object in response.data) {
                     model_object = new GlueModelObject(this.unique_name);
 
                     let simple_fields = response.data[object].simple_fields;
                     for (let key in simple_fields) {
                         model_object[key] = simple_fields[key];
                     }
@@ -99,14 +104,15 @@
 
         return await glue_ajax_request(
             this.unique_name,
             'create',
             data
         ).then((response) => {
             console.log(response)
+            glue_dispatch_response_event(response)
             let model_object = new GlueModelObject(this.unique_name)
 
             let simple_fields = response.data.simple_fields
             for (let key in simple_fields) {
                 model_object[key] = simple_fields[key]
             }
             return model_object
@@ -120,14 +126,15 @@
         }
         glue_ajax_request(
             this.unique_name,
             'delete',
             data
         ).then((response) => {
             console.log(response)
+            glue_dispatch_response_event(response)
         })
     }
 
     async method(id, method, kwargs = {}) {
         let data = {
             'id': id,
             'method': method,
@@ -136,12 +143,13 @@
 
         return await glue_ajax_request(
             this.unique_name,
             'method',
             data
         ).then((response) => {
             console.log(response)
+            glue_dispatch_response_event(response)
             return response.data.method_return
         })
     }
 
 }
```

### Comparing `django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_template.js` & `django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_template.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/django_glue/static/django_glue/js/django_glue_view.js` & `django-glue-0.4.1/django_glue/static/django_glue/js/django_glue_view.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/django_glue/templates/django_glue/django_glue.html` & `django-glue-0.4.1/django_glue/templates/django_glue/django_glue.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 {% load static %}
 
 {% load django_glue %}
 
-<!-- This is required to force a csrf_token to be used do not remove -->
 {% csrf_token %}
 
+<script type="application/javascript" src="{% static 'django_glue/js/django_glue_keep_live.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
+
 <script type="application/javascript">
-    const DJANGO_GLUE_AJAX_URL = '{% url 'django_glue:django_glue_data_handler' %}'
     const DJANGO_DEBUG = {% if debug %}true{% else %}false{% endif %}
-    const DJANGO_GLUE_CONTEXT_DATA = JSON.parse('{% glue_context_data_str %}')
-    const DJANGO_GLUE_KEEP_LIVE = JSON.parse('{% glue_context_keep_live_str %}')
-    const DJANGO_GLUE_KEEP_LIVE_URL = '{% url 'django_glue:django_glue_keep_live_handler' %}?keep_live_url_path={{ request.path|urlencode }}'
+    const DJANGO_GLUE_AJAX_URL = '{% url 'django_glue:django_glue_data_handler' %}'
+    const DJANGO_GLUE_KEEP_LIVE_URL = '{% url 'django_glue:django_glue_keep_live_handler' %}'
+
+    window.glue_keep_live = new GlueKeepLive()
 
-    fetch(DJANGO_GLUE_KEEP_LIVE_URL)
     setInterval(() => {
-        fetch(DJANGO_GLUE_KEEP_LIVE_URL)
-    }, {{ DJANGO_GLUE_KEEP_LIVE_INTERVAL_TIME_MILLISECONDS }})
+        window.glue_keep_live.update(DJANGO_GLUE_KEEP_LIVE_URL)
+    }, 2000)
+
 </script>
 
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_csrf.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_ajax.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_event.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_response.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
 <script type="application/javascript" src="{% static 'django_glue/js/django_glue_message.js' %}?v={{ DJANGO_GLUE_VERSION }}"></script>
```

#### html2text {}

```diff
@@ -1,2 +1,2 @@
-{% load static %} {% load django_glue %}  {% csrf_token %}
+{% load static %} {% load django_glue %} {% csrf_token %}
```

### Comparing `django-glue-0.4.0/django_glue/templatetags/django_glue.py` & `django-glue-0.4.1/django_glue/templatetags/django_glue.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/django_glue/utils.py` & `django-glue-0.4.1/django_glue/utils.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/django_glue.egg-info/PKG-INFO` & `django-glue-0.4.1/django_glue.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.4.0
+Version: 0.4.1
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
 Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-glue-0.4.0/django_glue.egg-info/SOURCES.txt` & `django-glue-0.4.1/django_glue.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 django_glue/services/model_objects.py
 django_glue/services/query_sets.py
 django_glue/services/services.py
 django_glue/services/templates.py
 django_glue/static/django_glue/js/django_glue_ajax.js
 django_glue/static/django_glue/js/django_glue_csrf.js
 django_glue/static/django_glue/js/django_glue_event.js
+django_glue/static/django_glue/js/django_glue_keep_live.js
 django_glue/static/django_glue/js/django_glue_message.js
 django_glue/static/django_glue/js/django_glue_model_object.js
 django_glue/static/django_glue/js/django_glue_query_set.js
 django_glue/static/django_glue/js/django_glue_response.js
 django_glue/static/django_glue/js/django_glue_shortcuts.js
 django_glue/static/django_glue/js/django_glue_template.js
 django_glue/static/django_glue/js/django_glue_view.js
```

### Comparing `django-glue-0.4.0/setup.py` & `django-glue-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/tests/manage.py` & `django-glue-0.4.1/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/tests/migrations/0001_initial.py` & `django-glue-0.4.1/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/tests/models.py` & `django-glue-0.4.1/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/tests/settings.py` & `django-glue-0.4.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/tests/urls.py` & `django-glue-0.4.1/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/tests/utils.py` & `django-glue-0.4.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.0/tests/views.py` & `django-glue-0.4.1/tests/views.py`

 * *Files identical despite different names*

