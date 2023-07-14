# Comparing `tmp/django-jet-new-2.3.2.tar.gz` & `tmp/django-jet-new-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-jet-new-2.3.2.tar", last modified: Tue Jul 11 01:17:01 2023, max compression
+gzip compressed data, was "dist/django-jet-new-2.3.3.tar", last modified: Fri Jul 14 22:47:01 2023, max compression
```

## Comparing `django-jet-new-2.3.2.tar` & `django-jet-new-2.3.3.tar`

### file list

```diff
@@ -1,564 +1,564 @@
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.125983 django-jet-new-2.3.2/
--rw-r--r--   0 munisisazade   (501) staff       (20)    34520 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/LICENSE
--rw-r--r--   0 munisisazade   (501) staff       (20)      257 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/MANIFEST.in
--rw-r--r--   0 munisisazade   (501) staff       (20)     8014 2023-07-11 01:17:01.125814 django-jet-new-2.3.2/PKG-INFO
--rw-r--r--   0 munisisazade   (501) staff       (20)     6613 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/README.rst
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.039248 django-jet-new-2.3.2/django_jet_new.egg-info/
--rw-r--r--   0 munisisazade   (501) staff       (20)     8014 2023-07-11 01:17:01.000000 django-jet-new-2.3.2/django_jet_new.egg-info/PKG-INFO
--rw-r--r--   0 munisisazade   (501) staff       (20)    20881 2023-07-11 01:17:01.000000 django-jet-new-2.3.2/django_jet_new.egg-info/SOURCES.txt
--rw-r--r--   0 munisisazade   (501) staff       (20)        1 2023-07-11 01:17:01.000000 django-jet-new-2.3.2/django_jet_new.egg-info/dependency_links.txt
--rw-r--r--   0 munisisazade   (501) staff       (20)        1 2023-07-11 01:17:01.000000 django-jet-new-2.3.2/django_jet_new.egg-info/not-zip-safe
--rw-r--r--   0 munisisazade   (501) staff       (20)        7 2023-07-11 01:17:01.000000 django-jet-new-2.3.2/django_jet_new.egg-info/requires.txt
--rw-r--r--   0 munisisazade   (501) staff       (20)        4 2023-07-11 01:17:01.000000 django-jet-new-2.3.2/django_jet_new.egg-info/top_level.txt
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.041642 django-jet-new-2.3.2/jet/
--rw-r--r--   0 munisisazade   (501) staff       (20)       18 2023-07-11 01:16:49.000000 django-jet-new-2.3.2/jet/__init__.py
--rw-r--r--   0 munisisazade   (501) staff       (20)      136 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/admin.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.044124 django-jet-new-2.3.2/jet/dashboard/
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/__init__.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     9833 2023-07-11 00:15:37.000000 django-jet-new-2.3.2/jet/dashboard/dashboard.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.045281 django-jet-new-2.3.2/jet/dashboard/dashboard_modules/
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/dashboard_modules/__init__.py
--rw-r--r--   0 munisisazade   (501) staff       (20)    15773 2023-07-11 01:14:54.000000 django-jet-new-2.3.2/jet/dashboard/dashboard_modules/google_analytics.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     2423 2023-07-11 00:15:37.000000 django-jet-new-2.3.2/jet/dashboard/dashboard_modules/google_analytics_views.py
--rw-r--r--   0 munisisazade   (501) staff       (20)    13655 2023-07-11 01:14:43.000000 django-jet-new-2.3.2/jet/dashboard/dashboard_modules/yandex_metrika.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     2142 2023-07-11 00:15:37.000000 django-jet-new-2.3.2/jet/dashboard/dashboard_modules/yandex_metrika_views.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     5577 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/forms.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.033074 django-jet-new-2.3.2/jet/dashboard/locale/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.031962 django-jet-new-2.3.2/jet/dashboard/locale/ar/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.046171 django-jet-new-2.3.2/jet/dashboard/locale/ar/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     6102 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)    13370 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      473 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)      852 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/ar/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.032078 django-jet-new-2.3.2/jet/dashboard/locale/cs/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.046790 django-jet-new-2.3.2/jet/dashboard/locale/cs/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     4470 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)    12226 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      471 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/cs/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)      843 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/cs/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.032192 django-jet-new-2.3.2/jet/dashboard/locale/de/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.047373 django-jet-new-2.3.2/jet/dashboard/locale/de/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     4947 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     6200 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      393 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/de/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)      842 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/de/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.032308 django-jet-new-2.3.2/jet/dashboard/locale/en/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.048117 django-jet-new-2.3.2/jet/dashboard/locale/en/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)      495 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)    10871 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      378 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/en/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)      827 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.032426 django-jet-new-2.3.2/jet/dashboard/locale/es/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.048722 django-jet-new-2.3.2/jet/dashboard/locale/es/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     6524 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)    15268 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      474 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/es/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)      846 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/es/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.032539 django-jet-new-2.3.2/jet/dashboard/locale/fa/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.049012 django-jet-new-2.3.2/jet/dashboard/locale/fa/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)    16058 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/fa/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      851 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/fa/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.032655 django-jet-new-2.3.2/jet/dashboard/locale/fr/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.049299 django-jet-new-2.3.2/jet/dashboard/locale/fr/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)    12295 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      845 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.032776 django-jet-new-2.3.2/jet/dashboard/locale/pl/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.049616 django-jet-new-2.3.2/jet/dashboard/locale/pl/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     4327 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)    14998 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.032897 django-jet-new-2.3.2/jet/dashboard/locale/pt-br/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.050336 django-jet-new-2.3.2/jet/dashboard/locale/pt-br/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     5245 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/pt-br/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)    12513 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/pt-br/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      499 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/pt-br/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)      871 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/pt-br/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.033008 django-jet-new-2.3.2/jet/dashboard/locale/ru/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.050988 django-jet-new-2.3.2/jet/dashboard/locale/ru/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     6409 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)    13673 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      485 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)      857 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/ru/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.033121 django-jet-new-2.3.2/jet/dashboard/locale/zh_cn/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.051283 django-jet-new-2.3.2/jet/dashboard/locale/zh_cn/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     3891 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/zh_cn/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)    12159 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/locale/zh_cn/LC_MESSAGES/django.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.051570 django-jet-new-2.3.2/jet/dashboard/migrations/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1445 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/migrations/0001_initial.py
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/migrations/__init__.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1972 2023-07-11 00:41:50.000000 django-jet-new-2.3.2/jet/dashboard/models.py
--rw-r--r--   0 munisisazade   (501) staff       (20)    19375 2023-07-11 00:15:37.000000 django-jet-new-2.3.2/jet/dashboard/modules.py
--rw-r--r--   0 munisisazade   (501) staff       (20)      280 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/settings.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.051877 django-jet-new-2.3.2/jet/dashboard/south_migrations/
--rw-r--r--   0 munisisazade   (501) staff       (20)     2561 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/south_migrations/0001_initial.py
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/south_migrations/__init__.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.033368 django-jet-new-2.3.2/jet/dashboard/static/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.033483 django-jet-new-2.3.2/jet/dashboard/static/jet.dashboard/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.052134 django-jet-new-2.3.2/jet/dashboard/static/jet.dashboard/dashboard_modules/
--rw-r--r--   0 munisisazade   (501) staff       (20)     2424 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/static/jet.dashboard/dashboard_modules/google_analytics.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     2422 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/static/jet.dashboard/dashboard_modules/yandex_metrika.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.033531 django-jet-new-2.3.2/jet/dashboard/static/jet.dashboard/vendor/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.053318 django-jet-new-2.3.2/jet/dashboard/static/jet.dashboard/vendor/chart.js/
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     2991 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/static/jet.dashboard/vendor/chart.js/CONTRIBUTING.md
--rwxr-xr-x   0 munisisazade   (501) staff       (20)   109612 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/static/jet.dashboard/vendor/chart.js/Chart.js
--rwxr-xr-x   0 munisisazade   (501) staff       (20)    52091 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/static/jet.dashboard/vendor/chart.js/Chart.min.js
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     1060 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/static/jet.dashboard/vendor/chart.js/LICENSE.md
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     1144 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/static/jet.dashboard/vendor/chart.js/README.md
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.033713 django-jet-new-2.3.2/jet/dashboard/templates/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.053642 django-jet-new-2.3.2/jet/dashboard/templates/admin/
--rw-r--r--   0 munisisazade   (501) staff       (20)      949 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templates/admin/app_index.html
--rw-r--r--   0 munisisazade   (501) staff       (20)      938 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templates/admin/index.html
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.054388 django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1411 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/dashboard.html
--rw-r--r--   0 munisisazade   (501) staff       (20)     2060 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/dashboard_tools.html
--rw-r--r--   0 munisisazade   (501) staff       (20)     2163 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/module.html
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.055937 django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1473 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/app_list.html
--rw-r--r--   0 munisisazade   (501) staff       (20)      587 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/feed.html
--rw-r--r--   0 munisisazade   (501) staff       (20)     1056 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/google_analytics_period_visitors.html
--rw-r--r--   0 munisisazade   (501) staff       (20)     1099 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/google_analytics_visitors_chart.html
--rw-r--r--   0 munisisazade   (501) staff       (20)      597 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/google_analytics_visitors_totals.html
--rw-r--r--   0 munisisazade   (501) staff       (20)      922 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/link_list.html
--rw-r--r--   0 munisisazade   (501) staff       (20)      804 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/model_list.html
--rw-r--r--   0 munisisazade   (501) staff       (20)     1667 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/recent_actions.html
--rw-r--r--   0 munisisazade   (501) staff       (20)     1050 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_period_visitors.html
--rw-r--r--   0 munisisazade   (501) staff       (20)     1097 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_visitors_chart.html
--rw-r--r--   0 munisisazade   (501) staff       (20)      597 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_visitors_totals.html
--rw-r--r--   0 munisisazade   (501) staff       (20)     4140 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/update_module.html
--rw-r--r--   0 munisisazade   (501) staff       (20)      950 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/update_module_fieldset.html
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.056178 django-jet-new-2.3.2/jet/dashboard/templatetags/
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templatetags/__init__.py
--rw-r--r--   0 munisisazade   (501) staff       (20)      738 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/templatetags/jet_dashboard_tags.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1694 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/urls.py
--rw-r--r--   0 munisisazade   (501) staff       (20)      562 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/dashboard/utils.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     8113 2023-07-11 00:15:37.000000 django-jet-new-2.3.2/jet/dashboard/views.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     3097 2023-07-11 00:42:46.000000 django-jet-new-2.3.2/jet/filters.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     5221 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/forms.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.035077 django-jet-new-2.3.2/jet/locale/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.034006 django-jet-new-2.3.2/jet/locale/ar/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.056871 django-jet-new-2.3.2/jet/locale/ar/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1242 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1877 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      739 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1389 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/ar/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.034119 django-jet-new-2.3.2/jet/locale/cs/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.057422 django-jet-new-2.3.2/jet/locale/cs/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1148 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1779 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      703 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/cs/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1343 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/cs/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.034228 django-jet-new-2.3.2/jet/locale/de/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.058247 django-jet-new-2.3.2/jet/locale/de/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1418 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1867 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      622 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/de/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1347 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/de/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.034338 django-jet-new-2.3.2/jet/locale/en/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.058903 django-jet-new-2.3.2/jet/locale/en/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)      495 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1592 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      378 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/en/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1253 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.034447 django-jet-new-2.3.2/jet/locale/es/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.059739 django-jet-new-2.3.2/jet/locale/es/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1770 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     2860 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      724 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/es/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1365 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/es/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.034560 django-jet-new-2.3.2/jet/locale/fa/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.060125 django-jet-new-2.3.2/jet/locale/fa/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     3933 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/fa/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)     1401 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/fa/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.034672 django-jet-new-2.3.2/jet/locale/fr/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.060485 django-jet-new-2.3.2/jet/locale/fr/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1770 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)     1379 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.034783 django-jet-new-2.3.2/jet/locale/pl/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.061270 django-jet-new-2.3.2/jet/locale/pl/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1926 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     3852 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      479 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/pl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)      751 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/pl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.034896 django-jet-new-2.3.2/jet/locale/pt_BR/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.061971 django-jet-new-2.3.2/jet/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1197 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1828 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      761 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1401 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.035008 django-jet-new-2.3.2/jet/locale/ru/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.062576 django-jet-new-2.3.2/jet/locale/ru/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1305 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1936 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 munisisazade   (501) staff       (20)      787 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     1427 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/ru/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.035124 django-jet-new-2.3.2/jet/locale/zh_CN/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.062860 django-jet-new-2.3.2/jet/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 munisisazade   (501) staff       (20)     2005 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 munisisazade   (501) staff       (20)     3729 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.063002 django-jet-new-2.3.2/jet/management/
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/management/__init__.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.063345 django-jet-new-2.3.2/jet/management/commands/
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/management/commands/__init__.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1430 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/management/commands/jet_custom_apps_example.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1509 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/management/commands/jet_side_menu_items_example.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.063823 django-jet-new-2.3.2/jet/migrations/
--rw-r--r--   0 munisisazade   (501) staff       (20)     2930 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/migrations/0001_initial.py
--rw-r--r--   0 munisisazade   (501) staff       (20)      317 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/migrations/0002_delete_userdashboardmodule.py
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/migrations/__init__.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1093 2023-07-11 00:41:50.000000 django-jet-new-2.3.2/jet/models.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1652 2023-07-11 00:47:03.000000 django-jet-new-2.3.2/jet/ordered_set.py
--rw-r--r--   0 munisisazade   (501) staff       (20)      509 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/settings.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.064224 django-jet-new-2.3.2/jet/south_migrations/
--rw-r--r--   0 munisisazade   (501) staff       (20)     4874 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/south_migrations/0001_initial.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     2532 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/south_migrations/0002_auto__del_userdashboardmodule.py
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/south_migrations/__init__.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.037206 django-jet-new-2.3.2/jet/static/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.035605 django-jet-new-2.3.2/jet/static/admin/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.064998 django-jet-new-2.3.2/jet/static/admin/css/
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/admin/css/base.css
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/admin/css/changelists.css
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/admin/css/dashboard.css
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/admin/css/fonts.css
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/admin/css/forms.css
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/admin/css/login.css
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/admin/css/rtl.css
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/admin/css/widgets.css
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.065239 django-jet-new-2.3.2/jet/static/admin/js/
--rw-r--r--   0 munisisazade   (501) staff       (20)       85 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/admin/js/SelectFilter2.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.065440 django-jet-new-2.3.2/jet/static/admin/js/admin/
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/admin/js/admin/DateTimeShortcuts.js
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/admin/js/admin/RelatedObjectLookups.js
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/admin/js/related-widget-wrapper.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.036560 django-jet-new-2.3.2/jet/static/jet/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.068421 django-jet-new-2.3.2/jet/static/jet/css/
--rw-r--r--   0 munisisazade   (501) staff       (20)     2211 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_base.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)      880 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_breadcrumbs.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)    17750 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_changeform.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     7749 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_changelist.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     4029 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_content.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     8804 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_dashboard.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     1783 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_delete-confirmation.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     3534 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_forms.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)       67 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_globals.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     5165 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_header.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     4119 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_helpers.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     1959 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_login.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     1656 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_messages.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)      740 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_modules.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     1042 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_object-tools.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     2051 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_relatedpopup.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)    11150 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_sidebar.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     3249 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_tables.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)     6284 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/_variables.scss
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.069121 django-jet-new-2.3.2/jet/static/jet/css/icons/
--rwxr-xr-x   0 munisisazade   (501) staff       (20)      800 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/icons/_variables.scss
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.069809 django-jet-new-2.3.2/jet/static/jet/css/icons/fonts/
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     6412 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/icons/fonts/jet-icons.eot
--rwxr-xr-x   0 munisisazade   (501) staff       (20)    19664 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/icons/fonts/jet-icons.svg
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     6240 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/icons/fonts/jet-icons.ttf
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     6316 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/icons/fonts/jet-icons.woff
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     2248 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/icons/style.css
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.069958 django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     3192 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/_jquery-ui.theme.scss
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.072145 django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/
--rw-r--r--   0 munisisazade   (501) staff       (20)      180 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-r--r--   0 munisisazade   (501) staff       (20)      178 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/ui-bg_flat_75_ffffff_40x100.png
--rw-r--r--   0 munisisazade   (501) staff       (20)      120 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0 munisisazade   (501) staff       (20)      105 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 munisisazade   (501) staff       (20)      111 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0 munisisazade   (501) staff       (20)      110 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 munisisazade   (501) staff       (20)      119 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 munisisazade   (501) staff       (20)      101 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/ui-icons_222222_256x240.png
--rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/ui-icons_454545_256x240.png
--rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/ui-icons_888888_256x240.png
--rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/ui-icons_cd0a0a_256x240.png
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.072562 django-jet-new-2.3.2/jet/static/jet/css/select2/
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     3095 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/select2/_layout.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     1662 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/select2/_multiple.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)      937 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/select2/_single.scss
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.036501 django-jet-new-2.3.2/jet/static/jet/css/themes/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.075528 django-jet-new-2.3.2/jet/static/jet/css/themes/default/
--rw-r--r--   0 munisisazade   (501) staff       (20)       66 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/default/_variables.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)   178918 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/default/base.css
--rw-r--r--   0 munisisazade   (501) staff       (20)   303057 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/default/base.css.map
--rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/default/base.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     6760 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/default/jquery-ui.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    23121 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/default/jquery-ui.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/default/jquery-ui.theme.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)    23574 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/default/select2.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    44244 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/default/select2.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/default/select2.theme.scss
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.078434 django-jet-new-2.3.2/jet/static/jet/css/themes/green/
--rw-r--r--   0 munisisazade   (501) staff       (20)     4956 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/green/_variables.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)   178918 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/green/base.css
--rw-r--r--   0 munisisazade   (501) staff       (20)   308261 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/green/base.css.map
--rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/green/base.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     6760 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/green/jquery-ui.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    21794 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/green/jquery-ui.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/green/jquery-ui.theme.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)    23574 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/green/select2.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    49427 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/green/select2.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/green/select2.theme.scss
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.081568 django-jet-new-2.3.2/jet/static/jet/css/themes/light-blue/
--rw-r--r--   0 munisisazade   (501) staff       (20)     5310 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-blue/_variables.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)   178850 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-blue/base.css
--rw-r--r--   0 munisisazade   (501) staff       (20)   308602 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-blue/base.css.map
--rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-blue/base.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     6769 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-blue/jquery-ui.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    22166 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-blue/jquery-ui.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-blue/jquery-ui.theme.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)    23571 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-blue/select2.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    49792 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-blue/select2.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-blue/select2.theme.scss
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.086880 django-jet-new-2.3.2/jet/static/jet/css/themes/light-gray/
--rw-r--r--   0 munisisazade   (501) staff       (20)     5310 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-gray/_variables.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)   178844 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-gray/base.css
--rw-r--r--   0 munisisazade   (501) staff       (20)   308599 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-gray/base.css.map
--rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-gray/base.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     6769 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-gray/jquery-ui.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    22166 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-gray/jquery-ui.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-gray/jquery-ui.theme.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)    23569 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-gray/select2.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    49791 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-gray/select2.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-gray/select2.theme.scss
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.090001 django-jet-new-2.3.2/jet/static/jet/css/themes/light-green/
--rw-r--r--   0 munisisazade   (501) staff       (20)     5318 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-green/_variables.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)   178844 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-green/base.css
--rw-r--r--   0 munisisazade   (501) staff       (20)   308610 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-green/base.css.map
--rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-green/base.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     6769 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-green/jquery-ui.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    22177 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-green/jquery-ui.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-green/jquery-ui.theme.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)    23569 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-green/select2.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    49802 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-green/select2.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-green/select2.theme.scss
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.092871 django-jet-new-2.3.2/jet/static/jet/css/themes/light-violet/
--rw-r--r--   0 munisisazade   (501) staff       (20)     5310 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-violet/_variables.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)   178805 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-violet/base.css
--rw-r--r--   0 munisisazade   (501) staff       (20)   308556 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-violet/base.css.map
--rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-violet/base.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)     6769 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-violet/jquery-ui.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    22172 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-violet/jquery-ui.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-violet/jquery-ui.theme.scss
--rwxr-xr-x   0 munisisazade   (501) staff       (20)    23573 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-violet/select2.theme.css
--rw-r--r--   0 munisisazade   (501) staff       (20)    49799 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-violet/select2.theme.css.map
--rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/themes/light-violet/select2.theme.scss
--rw-r--r--   0 munisisazade   (501) staff       (20)    53889 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/css/vendor.css
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.036886 django-jet-new-2.3.2/jet/static/jet/js/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.093015 django-jet-new-2.3.2/jet/static/jet/js/build/
--rw-r--r--   0 munisisazade   (501) staff       (20)   417084 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/build/bundle.min.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.036822 django-jet-new-2.3.2/jet/static/jet/js/i18n/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.106529 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1144 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-af.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1458 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ar-DZ.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1458 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ar.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1168 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-az.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1394 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-be.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1371 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-bg.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1092 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-bs.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1122 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ca.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1171 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-cs.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1155 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-cy-GB.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1138 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-da.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1129 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-de.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1436 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-el.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1148 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-en-AU.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1125 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-en-GB.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1150 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-en-NZ.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1141 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-eo.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1136 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-es.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1199 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-et.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1091 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-eu.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1382 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-fa.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1193 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-fi.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1166 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-fo.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1161 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-fr-CA.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1208 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-fr-CH.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1289 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-fr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1138 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-gl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1264 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-he.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1561 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-hi.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1117 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-hr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1140 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-hu.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1422 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-hy.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1130 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-id.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1194 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-is.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1169 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-it-CH.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1160 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-it.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1150 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ja.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1664 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ka.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1365 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-kk.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1578 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-km.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1159 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ko.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1356 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ky.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1182 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-lb.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1209 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-lt.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1190 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-lv.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1305 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-mk.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1684 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ml.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1139 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ms.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1145 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-nb.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1169 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-nl-BE.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1167 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-nl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1142 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-nn.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1137 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-no.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1165 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-pl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1196 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-pt-BR.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1116 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-pt.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1155 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-rm.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1237 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ro.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1365 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ru.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1153 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-sk.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1191 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-sl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1135 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-sq.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1099 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-sr-SR.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1285 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-sr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1138 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-sv.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1744 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ta.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1522 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-th.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1322 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-tj.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1131 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-tr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1431 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-uk.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1342 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-vi.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1234 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-CN.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1232 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-HK.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1228 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-TW.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.109321 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/
--rw-r--r--   0 munisisazade   (501) staff       (20)      480 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-cs.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      462 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-de.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      493 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-es.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      550 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-fr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      503 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-hr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      458 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-hu.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      485 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-it.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      500 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-ja.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      510 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-mk.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      424 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-nl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      457 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-pl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      480 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-pt-BR.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      520 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-ru.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      492 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-sl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      468 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-sv.js
--rwxr-xr-x   0 munisisazade   (501) staff       (20)      503 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-tr.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.116496 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/
--rw-r--r--   0 munisisazade   (501) staff       (20)      701 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/az.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      906 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/bg.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      876 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/ca.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1236 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/cs.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      816 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/da.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      775 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/de.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      827 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/en.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      871 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/es.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      775 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/et.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      844 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/eu.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1004 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/fa.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      703 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/fi.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      823 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/fr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      800 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/gl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      894 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/he.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1125 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/hi.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      780 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/hr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      727 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/hu.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      693 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/id.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      773 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/is.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      876 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/it.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      854 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/ko.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      878 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/lt.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      872 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/lv.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      979 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/mk.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      723 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/nb.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      867 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/nl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      926 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/pl.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      853 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/pt-BR.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      859 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/pt.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      834 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/ro.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1127 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/ru.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1184 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/sk.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      880 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/sr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      786 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/sv.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      948 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/th.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      720 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/tr.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1117 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/uk.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      801 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/vi.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      769 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/zh-CN.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      708 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/zh-TW.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.116648 django-jet-new-2.3.2/jet/static/jet/js/src/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.119226 django-jet-new-2.3.2/jet/static/jet/js/src/features/
--rw-r--r--   0 munisisazade   (501) staff       (20)     2852 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/changeform-tabs.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1354 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/changeform.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     3803 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/changelist.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1117 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/checkboxes.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     6694 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/compact-inline.js
--rw-r--r--   0 munisisazade   (501) staff       (20)    11563 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/dashboard.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     4309 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/date-time-widgets.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     2350 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/filters.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      895 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/inlines.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     8343 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/related-popups.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      824 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/scroll-to-bottom-detector.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     8381 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/selects.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      575 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/siblings.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.119816 django-jet-new-2.3.2/jet/static/jet/js/src/features/sidebar/
--rw-r--r--   0 munisisazade   (501) staff       (20)     3652 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/sidebar/application-pinning.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     4219 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/sidebar/bookmarks.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     3391 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/sidebar/main.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     7484 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/sidebar/popup.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1952 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/themes.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      709 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/tooltips.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      986 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/features/touchmove-non-scrollable.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.121739 django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1529 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/actions.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      746 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/branding.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1050 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/breadcrumbs.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     2552 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/changeform-tabs.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      449 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/delete-confirmation.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      730 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/icons.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      367 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/object-tools.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     2635 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/paginator.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1187 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/related-widget-wrapper.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      857 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/stacked-inline.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1226 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/tabular-inline.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     4842 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/toolbar.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1445 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/user-tools.js
--rw-r--r--   0 munisisazade   (501) staff       (20)     1199 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/main.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.122351 django-jet-new-2.3.2/jet/static/jet/js/src/utils/
--rw-r--r--   0 munisisazade   (501) staff       (20)      206 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/utils/jquery-icontains.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      178 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/utils/jquery-slidefade.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      132 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/utils/translate.js
--rw-r--r--   0 munisisazade   (501) staff       (20)      779 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/jet/js/src/utils/window-storage.js
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.037253 django-jet-new-2.3.2/jet/static/range_filter/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.122494 django-jet-new-2.3.2/jet/static/range_filter/css/
--rw-r--r--   0 munisisazade   (501) staff       (20)      244 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/static/range_filter/css/style.css
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.037617 django-jet-new-2.3.2/jet/templates/
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.122833 django-jet-new-2.3.2/jet/templates/admin/
--rw-r--r--   0 munisisazade   (501) staff       (20)    21995 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/templates/admin/base.html
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.122966 django-jet-new-2.3.2/jet/templates/admin/edit_inline/
--rw-r--r--   0 munisisazade   (501) staff       (20)     3630 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/templates/admin/edit_inline/compact.html
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.123112 django-jet-new-2.3.2/jet/templates/admin/includes/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1808 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/templates/admin/includes/fieldset.html
--rw-r--r--   0 munisisazade   (501) staff       (20)      379 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/templates/admin/popup_response.html
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.123252 django-jet-new-2.3.2/jet/templates/jet/
--rw-r--r--   0 munisisazade   (501) staff       (20)      450 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/templates/jet/related_field_ajax_list_filter.html
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.123390 django-jet-new-2.3.2/jet/templates/rangefilter/
--rw-r--r--   0 munisisazade   (501) staff       (20)     1940 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/templates/rangefilter/date_filter.html
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.123615 django-jet-new-2.3.2/jet/templatetags/
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/templatetags/__init__.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     7774 2023-07-11 00:42:46.000000 django-jet-new-2.3.2/jet/templatetags/jet_tags.py
-drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-11 01:17:01.125527 django-jet-new-2.3.2/jet/tests/
--rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/tests/__init__.py
--rw-r--r--   0 munisisazade   (501) staff       (20)      347 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/tests/admin.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1735 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/tests/dashboard.py
--rw-r--r--   0 munisisazade   (501) staff       (20)      661 2023-07-11 00:41:50.000000 django-jet-new-2.3.2/jet/tests/models.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1945 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/tests/settings.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     3085 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/tests/test_dashboard.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     2243 2023-07-11 00:42:46.000000 django-jet-new-2.3.2/jet/tests/test_filters.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     2003 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/tests/test_ordered_set.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     3711 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/tests/test_tags.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     2371 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/tests/test_utils.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     8951 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/tests/test_views.py
--rw-r--r--   0 munisisazade   (501) staff       (20)      858 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/tests/urls.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1030 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/urls.py
--rw-r--r--   0 munisisazade   (501) staff       (20)    16184 2023-07-11 01:14:43.000000 django-jet-new-2.3.2/jet/utils.py
--rw-r--r--   0 munisisazade   (501) staff       (20)     1698 2023-07-11 00:08:01.000000 django-jet-new-2.3.2/jet/views.py
--rw-r--r--   0 munisisazade   (501) staff       (20)       38 2023-07-11 01:17:01.126023 django-jet-new-2.3.2/setup.cfg
--rw-r--r--   0 munisisazade   (501) staff       (20)     2170 2023-07-11 00:23:06.000000 django-jet-new-2.3.2/setup.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     9623 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/PKG-INFO
+-rw-r--r--   0 munisisazade   (501) staff       (20)    34520 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/LICENSE
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/templatetags/
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/templatetags/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     7774 2023-07-11 00:42:46.000000 django-jet-new-2.3.3/jet/templatetags/jet_tags.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/migrations/
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/migrations/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)      317 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/migrations/0002_delete_userdashboardmodule.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2930 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/migrations/0001_initial.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/pl/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1926 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)      751 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/pl/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3852 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      479 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/pl/LC_MESSAGES/djangojs.mo
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/pt_BR/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1197 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1401 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/pt_BR/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1828 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      761 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/pt_BR/LC_MESSAGES/djangojs.mo
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/cs/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1148 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1343 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/cs/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1779 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      703 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/cs/LC_MESSAGES/djangojs.mo
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/ru/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1305 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1427 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/ru/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1936 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      787 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/ru/LC_MESSAGES/djangojs.mo
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/zh_CN/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2005 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3729 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/ar/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1242 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1389 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/ar/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1877 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      739 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/ar/LC_MESSAGES/djangojs.mo
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/de/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/de/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1418 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1347 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/de/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1867 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      622 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/de/LC_MESSAGES/djangojs.mo
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/fr/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1379 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/fr/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1770 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/es/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/es/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1770 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1365 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/es/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2860 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      724 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/es/LC_MESSAGES/djangojs.mo
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/en/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/en/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      495 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1253 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/en/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1592 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      378 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/en/LC_MESSAGES/djangojs.mo
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/fa/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1401 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/fa/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3933 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/locale/fa/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1093 2023-07-11 00:41:50.000000 django-jet-new-2.3.3/jet/models.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/tests/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2371 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/tests/test_utils.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)      661 2023-07-11 00:41:50.000000 django-jet-new-2.3.3/jet/tests/models.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3711 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/tests/test_tags.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3085 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/tests/test_dashboard.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/tests/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     8951 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/tests/test_views.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1735 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/tests/dashboard.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)      347 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/tests/admin.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2003 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/tests/test_ordered_set.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1945 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/tests/settings.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2243 2023-07-11 00:42:46.000000 django-jet-new-2.3.3/jet/tests/test_filters.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)      858 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/tests/urls.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/management/
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/management/__init__.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/management/commands/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1509 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/management/commands/jet_side_menu_items_example.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/management/commands/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1430 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/management/commands/jet_custom_apps_example.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)       18 2023-07-14 22:46:08.000000 django-jet-new-2.3.3/jet/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     5221 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/forms.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/templatetags/
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templatetags/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)      738 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templatetags/jet_dashboard_tags.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/migrations/
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/migrations/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1445 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/migrations/0001_initial.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/pl/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4327 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)    14998 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/cs/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4470 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)      843 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/cs/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)    12226 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      471 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/cs/LC_MESSAGES/djangojs.mo
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/ru/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     6409 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)      857 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/ru/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)    13673 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      485 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/ru/LC_MESSAGES/djangojs.mo
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/zh_cn/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/zh_cn/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3891 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/zh_cn/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)    12159 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/zh_cn/LC_MESSAGES/django.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/ar/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     6102 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)      852 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/ar/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)    13370 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      473 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/ar/LC_MESSAGES/djangojs.mo
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/pt-br/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/pt-br/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     5245 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/pt-br/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)      871 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/pt-br/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)    12513 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/pt-br/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      499 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/pt-br/LC_MESSAGES/djangojs.mo
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/de/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/de/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4947 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)      842 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/de/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)     6200 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      393 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/de/LC_MESSAGES/djangojs.mo
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/fr/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      845 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/fr/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)    12295 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/es/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/es/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     6524 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)      846 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/es/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)    15268 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      474 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/es/LC_MESSAGES/djangojs.mo
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/en/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/en/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      495 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 munisisazade   (501) staff       (20)      827 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/en/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)    10871 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)      378 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/en/LC_MESSAGES/djangojs.mo
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/fa/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      851 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/fa/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 munisisazade   (501) staff       (20)    16058 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/dashboard_modules/
+-rw-r--r--   0 munisisazade   (501) staff       (20)    13655 2023-07-11 01:14:43.000000 django-jet-new-2.3.3/jet/dashboard/dashboard_modules/yandex_metrika.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2423 2023-07-11 00:15:37.000000 django-jet-new-2.3.3/jet/dashboard/dashboard_modules/google_analytics_views.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/dashboard_modules/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2142 2023-07-11 00:15:37.000000 django-jet-new-2.3.3/jet/dashboard/dashboard_modules/yandex_metrika_views.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)    15773 2023-07-11 01:14:54.000000 django-jet-new-2.3.3/jet/dashboard/dashboard_modules/google_analytics.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1972 2023-07-11 00:41:50.000000 django-jet-new-2.3.3/jet/dashboard/models.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     5577 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/forms.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     9833 2023-07-11 00:15:37.000000 django-jet-new-2.3.3/jet/dashboard/dashboard.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)      562 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/utils.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/static/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/static/jet.dashboard/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/static/jet.dashboard/dashboard_modules/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2422 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/static/jet.dashboard/dashboard_modules/yandex_metrika.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2424 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/static/jet.dashboard/dashboard_modules/google_analytics.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/static/jet.dashboard/vendor/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/static/jet.dashboard/vendor/chart.js/
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     1060 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/static/jet.dashboard/vendor/chart.js/LICENSE.md
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)    52091 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/static/jet.dashboard/vendor/chart.js/Chart.min.js
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)   109612 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/static/jet.dashboard/vendor/chart.js/Chart.js
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     1144 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/static/jet.dashboard/vendor/chart.js/README.md
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     2991 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/static/jet.dashboard/vendor/chart.js/CONTRIBUTING.md
+-rw-r--r--   0 munisisazade   (501) staff       (20)      280 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/settings.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/admin/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      938 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/admin/index.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)      949 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/admin/app_index.html
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2163 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/module.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1411 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/dashboard.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4140 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/update_module.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)      950 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/update_module_fieldset.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2060 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/dashboard_tools.html
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      587 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/feed.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1097 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_visitors_chart.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1050 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_period_visitors.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)      597 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_visitors_totals.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)      804 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/model_list.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1667 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/recent_actions.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)      922 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/link_list.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1056 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/google_analytics_period_visitors.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1473 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/app_list.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)      597 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/google_analytics_visitors_totals.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1099 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/google_analytics_visitors_chart.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)    19375 2023-07-11 00:15:37.000000 django-jet-new-2.3.3/jet/dashboard/modules.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/dashboard/south_migrations/
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/south_migrations/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2561 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/south_migrations/0001_initial.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1694 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/dashboard/urls.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     8113 2023-07-11 00:15:37.000000 django-jet-new-2.3.3/jet/dashboard/views.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)      136 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/admin.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)    16231 2023-07-14 22:43:55.000000 django-jet-new-2.3.3/jet/utils.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/range_filter/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/range_filter/css/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      244 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/range_filter/css/style.css
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/css/
+-rw-r--r--   0 munisisazade   (501) staff       (20)    53889 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/vendor.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)     6284 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_variables.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1042 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_object-tools.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2051 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_relatedpopup.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1783 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_delete-confirmation.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1959 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_login.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4119 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_helpers.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     8804 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_dashboard.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)      740 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_modules.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3534 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_forms.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)       67 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_globals.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3249 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_tables.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4029 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_content.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)    17750 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_changeform.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)      880 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_breadcrumbs.scss
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/css/icons/
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)      800 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/icons/_variables.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     2248 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/icons/style.css
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/css/icons/fonts/
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     6240 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/icons/fonts/jet-icons.ttf
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     6412 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/icons/fonts/jet-icons.eot
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)    19664 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/icons/fonts/jet-icons.svg
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     6316 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/icons/fonts/jet-icons.woff
+-rw-r--r--   0 munisisazade   (501) staff       (20)    11150 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_sidebar.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     7749 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_changelist.scss
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/css/select2/
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)      937 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/select2/_single.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     3095 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/select2/_layout.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     1662 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/select2/_multiple.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     5165 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_header.scss
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/green/
+-rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/green/base.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4956 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/green/_variables.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)    23574 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/green/select2.theme.css
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     6760 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/green/jquery-ui.theme.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)    21794 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/green/jquery-ui.theme.css.map
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/green/jquery-ui.theme.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/green/select2.theme.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)   308261 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/green/base.css.map
+-rw-r--r--   0 munisisazade   (501) staff       (20)    49427 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/green/select2.theme.css.map
+-rw-r--r--   0 munisisazade   (501) staff       (20)   178918 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/green/base.css
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-gray/
+-rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-gray/base.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     5310 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-gray/_variables.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)    23569 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-gray/select2.theme.css
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     6769 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-gray/jquery-ui.theme.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)    22166 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-gray/jquery-ui.theme.css.map
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-gray/jquery-ui.theme.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-gray/select2.theme.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)   308599 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-gray/base.css.map
+-rw-r--r--   0 munisisazade   (501) staff       (20)    49791 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-gray/select2.theme.css.map
+-rw-r--r--   0 munisisazade   (501) staff       (20)   178844 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-gray/base.css
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-blue/
+-rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-blue/base.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     5310 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-blue/_variables.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)    23571 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-blue/select2.theme.css
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     6769 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-blue/jquery-ui.theme.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)    22166 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-blue/jquery-ui.theme.css.map
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-blue/jquery-ui.theme.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-blue/select2.theme.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)   308602 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-blue/base.css.map
+-rw-r--r--   0 munisisazade   (501) staff       (20)    49792 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-blue/select2.theme.css.map
+-rw-r--r--   0 munisisazade   (501) staff       (20)   178850 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-blue/base.css
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/default/
+-rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/default/base.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)       66 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/default/_variables.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)    23574 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/default/select2.theme.css
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     6760 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/default/jquery-ui.theme.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)    23121 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/default/jquery-ui.theme.css.map
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/default/jquery-ui.theme.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/default/select2.theme.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)   303057 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/default/base.css.map
+-rw-r--r--   0 munisisazade   (501) staff       (20)    44244 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/default/select2.theme.css.map
+-rw-r--r--   0 munisisazade   (501) staff       (20)   178918 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/default/base.css
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-green/
+-rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-green/base.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     5318 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-green/_variables.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)    23569 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-green/select2.theme.css
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     6769 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-green/jquery-ui.theme.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)    22177 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-green/jquery-ui.theme.css.map
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-green/jquery-ui.theme.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-green/select2.theme.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)   308610 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-green/base.css.map
+-rw-r--r--   0 munisisazade   (501) staff       (20)    49802 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-green/select2.theme.css.map
+-rw-r--r--   0 munisisazade   (501) staff       (20)   178844 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-green/base.css
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-violet/
+-rw-r--r--   0 munisisazade   (501) staff       (20)       42 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-violet/base.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     5310 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-violet/_variables.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)    23573 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-violet/select2.theme.css
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     6769 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-violet/jquery-ui.theme.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)    22172 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-violet/jquery-ui.theme.css.map
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       63 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-violet/jquery-ui.theme.scss
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)       52 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-violet/select2.theme.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)   308556 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-violet/base.css.map
+-rw-r--r--   0 munisisazade   (501) staff       (20)    49799 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-violet/select2.theme.css.map
+-rw-r--r--   0 munisisazade   (501) staff       (20)   178805 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/themes/light-violet/base.css
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/ui-icons_888888_256x240.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)      111 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)      178 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/ui-bg_flat_75_ffffff_40x100.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)      110 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)      105 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)      119 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/ui-icons_222222_256x240.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)      101 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)      120 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4369 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/ui-icons_454545_256x240.png
+-rw-r--r--   0 munisisazade   (501) staff       (20)      180 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)     3192 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/_jquery-ui.theme.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1656 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_messages.scss
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2211 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/css/_base.scss
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/js/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/js/build/
+-rw-r--r--   0 munisisazade   (501) staff       (20)   417084 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/build/bundle.min.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      493 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-es.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      485 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-it.js
+-rwxr-xr-x   0 munisisazade   (501) staff       (20)      503 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-tr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      480 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-cs.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      424 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-nl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      550 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-fr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      468 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-sv.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      458 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-hu.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      462 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-de.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      480 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-pt-BR.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      500 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-ja.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      520 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-ru.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      510 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-mk.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      503 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-hr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      457 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-pl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      492 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-sl.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      859 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/pt.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      801 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/vi.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      872 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/lv.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      800 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/gl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      926 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/pl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      775 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/et.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      773 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/is.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      854 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/ko.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      780 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/hr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      703 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/fi.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      948 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/th.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1127 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/ru.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      844 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/eu.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      979 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/mk.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      894 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/he.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      906 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/bg.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      693 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/id.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      701 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/az.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      876 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/ca.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      723 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/nb.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      769 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/zh-CN.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      708 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/zh-TW.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      853 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/pt-BR.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      816 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/da.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1004 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/fa.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      775 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/de.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      827 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/en.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      786 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/sv.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1125 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/hi.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1117 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/uk.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1236 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/cs.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      823 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/fr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      867 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/nl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      880 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/sr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      727 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/hu.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      878 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/lt.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1184 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/sk.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      876 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/it.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      871 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/es.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      834 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/ro.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      720 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/tr.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1130 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-id.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1168 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-az.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1234 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-CN.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1148 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-en-AU.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1144 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-af.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1422 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-hy.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1356 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ky.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1150 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ja.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1664 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ka.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1228 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-TW.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1196 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-pt-BR.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1264 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-he.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1371 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-bg.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1135 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-sq.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1169 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-nl-BE.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1458 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ar-DZ.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1161 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-fr-CA.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1125 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-en-GB.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1155 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-rm.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1117 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-hr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1139 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ms.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1522 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-th.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1193 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-fi.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1365 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ru.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1091 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-eu.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1305 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-mk.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1137 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-no.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1436 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-el.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1199 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-et.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1194 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-is.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1191 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-sl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1142 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-nn.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1159 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ko.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1116 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-pt.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1342 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-vi.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1190 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-lv.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1365 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-kk.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1169 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-it-CH.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1138 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-gl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1165 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-pl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1141 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-eo.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1237 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ro.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1322 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-tj.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1131 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-tr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1166 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-fo.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1458 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ar.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1099 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-sr-SR.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1153 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-sk.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1160 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-it.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1136 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-es.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1150 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-en-NZ.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1285 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-sr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1140 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-hu.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1209 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-lt.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1684 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ml.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1092 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-bs.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1138 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-sv.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1561 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-hi.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1431 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-uk.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1171 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-cs.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1578 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-km.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1289 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-fr.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1167 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-nl.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1382 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-fa.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1129 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-de.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1138 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-da.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1145 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-nb.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1394 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-be.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1182 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-lb.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1122 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ca.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1744 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ta.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1208 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-fr-CH.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1155 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-cy-GB.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1232 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-HK.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/sidebar/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     7484 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/sidebar/popup.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3391 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/sidebar/main.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4219 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/sidebar/bookmarks.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3652 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/sidebar/application-pinning.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      824 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/scroll-to-bottom-detector.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     8343 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/related-popups.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3803 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/changelist.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1952 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/themes.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      709 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/tooltips.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1117 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/checkboxes.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      895 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/inlines.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2350 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/filters.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      986 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/touchmove-non-scrollable.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     8381 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/selects.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      575 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/siblings.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4309 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/date-time-widgets.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)    11563 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/dashboard.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2852 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/changeform-tabs.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     6694 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/compact-inline.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1354 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/features/changeform.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/utils/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      779 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/utils/window-storage.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      132 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/utils/translate.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      178 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/utils/jquery-slidefade.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      206 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/utils/jquery-icontains.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1199 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/main.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      730 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/icons.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1445 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/user-tools.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1529 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/actions.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      857 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/stacked-inline.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      746 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/branding.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      367 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/object-tools.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1226 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/tabular-inline.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1050 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/breadcrumbs.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2635 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/paginator.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4842 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/toolbar.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      449 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/delete-confirmation.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1187 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/related-widget-wrapper.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2552 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/changeform-tabs.js
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/admin/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/admin/css/
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/admin/css/widgets.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/admin/css/login.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/admin/css/dashboard.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/admin/css/forms.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/admin/css/fonts.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/admin/css/rtl.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/admin/css/base.css
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/admin/css/changelists.css
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/admin/js/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/static/admin/js/admin/
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/admin/js/admin/RelatedObjectLookups.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/admin/js/admin/DateTimeShortcuts.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)       85 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/admin/js/SelectFilter2.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/static/admin/js/related-widget-wrapper.js
+-rw-r--r--   0 munisisazade   (501) staff       (20)      509 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/settings.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/templates/
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/templates/jet/
+-rw-r--r--   0 munisisazade   (501) staff       (20)      450 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/templates/jet/related_field_ajax_list_filter.html
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/templates/admin/
+-rw-r--r--   0 munisisazade   (501) staff       (20)    21995 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/templates/admin/base.html
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/templates/admin/includes/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1808 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/templates/admin/includes/fieldset.html
+-rw-r--r--   0 munisisazade   (501) staff       (20)      379 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/templates/admin/popup_response.html
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/templates/admin/edit_inline/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3630 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/templates/admin/edit_inline/compact.html
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/templates/rangefilter/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1940 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/templates/rangefilter/date_filter.html
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/jet/south_migrations/
+-rw-r--r--   0 munisisazade   (501) staff       (20)        0 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/south_migrations/__init__.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2532 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/south_migrations/0002_auto__del_userdashboardmodule.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     4874 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/south_migrations/0001_initial.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1030 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/urls.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1652 2023-07-11 00:47:03.000000 django-jet-new-2.3.3/jet/ordered_set.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     3097 2023-07-11 00:42:46.000000 django-jet-new-2.3.3/jet/filters.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)     1698 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/jet/views.py
+-rw-r--r--   0 munisisazade   (501) staff       (20)      257 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/MANIFEST.in
+-rw-r--r--   0 munisisazade   (501) staff       (20)     2170 2023-07-11 00:23:06.000000 django-jet-new-2.3.3/setup.py
+drwxr-xr-x   0 munisisazade   (501) staff       (20)        0 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/django_jet_new.egg-info/
+-rw-r--r--   0 munisisazade   (501) staff       (20)     9623 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/django_jet_new.egg-info/PKG-INFO
+-rw-r--r--   0 munisisazade   (501) staff       (20)        1 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/django_jet_new.egg-info/not-zip-safe
+-rw-r--r--   0 munisisazade   (501) staff       (20)    20881 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/django_jet_new.egg-info/SOURCES.txt
+-rw-r--r--   0 munisisazade   (501) staff       (20)        7 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/django_jet_new.egg-info/requires.txt
+-rw-r--r--   0 munisisazade   (501) staff       (20)        4 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/django_jet_new.egg-info/top_level.txt
+-rw-r--r--   0 munisisazade   (501) staff       (20)        1 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/django_jet_new.egg-info/dependency_links.txt
+-rw-r--r--   0 munisisazade   (501) staff       (20)       38 2023-07-14 22:47:01.000000 django-jet-new-2.3.3/setup.cfg
+-rw-r--r--   0 munisisazade   (501) staff       (20)     6613 2023-07-11 00:08:01.000000 django-jet-new-2.3.3/README.rst
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `django-jet-new-2.3.2/LICENSE` & `django-jet-new-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/PKG-INFO` & `django-jet-new-2.3.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,217 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: django-jet-new
-Version: 2.3.2
+Version: 2.3.3
 Summary: Modern template for Django admin interface with improved functionality
 Home-page: https://github.com/geex-arts/django-jet
 Author: Denis Kildishev
 Author-email: support@jet.geex-arts.com
 License: AGPLv3
+Description: ==========
+        Django JET
+        ==========
+        
+        .. image:: https://travis-ci.org/geex-arts/django-jet.svg?branch=master
+            :target: https://travis-ci.org/geex-arts/django-jet
+        
+        **Modern template for Django admin interface with improved functionality**
+        
+        +-----------------------------------------------------------------------------------------------------------------------------------+
+        | Attention! **NEW JET**                                                                                                            |
+        +===================================================================================================================================+
+        | **We are proud to announce completely new Jet. Please check out Live Demo.**                                                      |
+        |                                                                                                                                   |
+        | Developing of new features for Django Jet will be frozen, only critical bugs will be fixed.                                       |
+        +-----------------------------------------------------------------------------------------------------------------------------------+
+        | `Live Demo <https://app.jetadmin.io/demo?utm_source=jet&utm_medium=banner&utm_campaign=github&utm_content=link&utm_term=promo>`_  |
+        +-----------------------------------------------------------------------------------------------------------------------------------+
+        
+        
+        Django JET has two kinds of licenses: open-source (AGPLv3) and commercial. Please note that using AGPLv3
+        code in your programs make them AGPL compatible too. So if you don't want to comply with that we can provide you a commercial
+        license (visit Home page). The commercial license is designed for using Django JET in commercial products
+        and applications without the provisions of the AGPLv3.
+        
+        .. image:: https://raw.githubusercontent.com/geex-arts/jet/static/logo.png
+            :width: 500px
+            :height: 500px
+            :scale: 50%
+            :alt: Logo
+            :align: center
+            
+        * Home page: http://jet.geex-arts.com/
+        * **New Jet**: `Live Demo <https://app.jetadmin.io/demo?utm_source=jet&utm_medium=banner&utm_campaign=github&utm_content=link&utm_term=promo>`_
+        * Live Demo: http://demo.jet.geex-arts.com/admin/
+        * Documentation: http://jet.readthedocs.org/
+        * libi.io http://libi.io/library/1683/django-jet
+        * PyPI: https://pypi.python.org/pypi/django-jet
+        * Support: support@jet.geex-arts.com
+        
+        Why Django JET?
+        ===============
+        
+        * New fresh look
+        * Responsive mobile interface
+        * Useful admin home page
+        * Minimal template overriding
+        * Easy integration
+        * Themes support
+        * Autocompletion
+        * Handy controls
+        
+        Screenshots
+        ===========
+        
+        .. image:: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen1_720.png
+            :alt: Screenshot #1
+            :align: center
+            :target: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen1.png
+            
+        .. image:: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen2_720.png
+            :alt: Screenshot #2
+            :align: center
+            :target: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen2.png
+            
+        .. image:: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen3_720.png
+            :alt: Screenshot #3
+            :align: center
+            :target: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen3.png
+        
+        Installation
+        ============
+        
+        * Download and install latest version of Django JET:
+        
+        .. code:: python
+        
+            pip install django-jet
+            # or
+            easy_install django-jet
+        
+        * Add 'jet' application to the INSTALLED_APPS setting of your Django project settings.py file (note it should be before 'django.contrib.admin'):
+        
+        .. code:: python
+        
+            INSTALLED_APPS = (
+                ...
+                'jet',
+                'django.contrib.admin',
+            )
+                
+        * Make sure ``django.template.context_processors.request`` context processor is enabled in settings.py (Django 1.8+ way):
+        
+        .. code:: python
+        
+            TEMPLATES = [
+                {
+                    'BACKEND': 'django.template.backends.django.DjangoTemplates',
+                    'DIRS': [],
+                    'APP_DIRS': True,
+                    'OPTIONS': {
+                        'context_processors': [
+                            ...
+                            'django.template.context_processors.request',
+                            ...
+                        ],
+                    },
+                },
+            ]
+        
+        .. warning::
+            Before Django 1.8 you should specify context processors different way. Also use ``django.core.context_processors.request`` instead of ``django.template.context_processors.request``.
+        
+            .. code:: python
+        
+                from django.conf import global_settings
+        
+                TEMPLATE_CONTEXT_PROCESSORS = global_settings.TEMPLATE_CONTEXT_PROCESSORS + (
+                    'django.core.context_processors.request',
+                )
+        
+        * Add URL-pattern to the urlpatterns of your Django project urls.py file (they are needed for related–lookups and autocompletes):
+        
+        .. code:: python
+        
+            urlpatterns = patterns(
+                '',
+                url(r'^jet/', include('jet.urls', 'jet')),  # Django JET URLS
+                url(r'^admin/', include(admin.site.urls)),
+                ...
+            )
+        
+        * Create database tables:
+        
+        .. code:: python
+        
+            python manage.py migrate jet
+            # or 
+            python manage.py syncdb
+                
+        * Collect static if you are in production environment:
+        
+        .. code:: python
+        
+                python manage.py collectstatic
+                
+        * Clear your browser cache
+        
+        Dashboard installation
+        ======================
+        
+        .. note:: Dashboard is located into a separate application. So after a typical JET installation it won't be active.
+                  To enable dashboard application follow these steps:
+        
+        * Add 'jet.dashboard' application to the INSTALLED_APPS setting of your Django project settings.py file (note it should be before 'jet'):
+        
+        .. code:: python
+        
+            INSTALLED_APPS = (
+                ...
+                'jet.dashboard',
+                'jet',
+                'django.contrib.admin',
+                ...
+            )
+        
+        * Add URL-pattern to the urlpatterns of your Django project urls.py file (they are needed for related–lookups and autocompletes):
+        
+        .. code:: python
+        
+            urlpatterns = patterns(
+                '',
+                url(r'^jet/', include('jet.urls', 'jet')),  # Django JET URLS
+                url(r'^jet/dashboard/', include('jet.dashboard.urls', 'jet-dashboard')),  # Django JET dashboard URLS
+                url(r'^admin/', include(admin.site.urls)),
+                ...
+            )
+        
+        * **For Google Analytics widgets only** install python package:
+        
+        .. code::
+        
+            pip install google-api-python-client==1.4.1
+        
+        * Create database tables:
+        
+        .. code:: python
+        
+            python manage.py migrate dashboard
+            # or
+            python manage.py syncdb
+        
+        * Collect static if you are in production environment:
+        
+        .. code:: python
+        
+                python manage.py collectstatic
+        
+        
+        
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: Free for non-commercial use
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -24,209 +226,7 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Web Environment
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
-License-File: LICENSE
-
-==========
-Django JET
-==========
-
-.. image:: https://travis-ci.org/geex-arts/django-jet.svg?branch=master
-    :target: https://travis-ci.org/geex-arts/django-jet
-
-**Modern template for Django admin interface with improved functionality**
-
-+-----------------------------------------------------------------------------------------------------------------------------------+
-| Attention! **NEW JET**                                                                                                            |
-+===================================================================================================================================+
-| **We are proud to announce completely new Jet. Please check out Live Demo.**                                                      |
-|                                                                                                                                   |
-| Developing of new features for Django Jet will be frozen, only critical bugs will be fixed.                                       |
-+-----------------------------------------------------------------------------------------------------------------------------------+
-| `Live Demo <https://app.jetadmin.io/demo?utm_source=jet&utm_medium=banner&utm_campaign=github&utm_content=link&utm_term=promo>`_  |
-+-----------------------------------------------------------------------------------------------------------------------------------+
-
-
-Django JET has two kinds of licenses: open-source (AGPLv3) and commercial. Please note that using AGPLv3
-code in your programs make them AGPL compatible too. So if you don't want to comply with that we can provide you a commercial
-license (visit Home page). The commercial license is designed for using Django JET in commercial products
-and applications without the provisions of the AGPLv3.
-
-.. image:: https://raw.githubusercontent.com/geex-arts/jet/static/logo.png
-    :width: 500px
-    :height: 500px
-    :scale: 50%
-    :alt: Logo
-    :align: center
-    
-* Home page: http://jet.geex-arts.com/
-* **New Jet**: `Live Demo <https://app.jetadmin.io/demo?utm_source=jet&utm_medium=banner&utm_campaign=github&utm_content=link&utm_term=promo>`_
-* Live Demo: http://demo.jet.geex-arts.com/admin/
-* Documentation: http://jet.readthedocs.org/
-* libi.io http://libi.io/library/1683/django-jet
-* PyPI: https://pypi.python.org/pypi/django-jet
-* Support: support@jet.geex-arts.com
-
-Why Django JET?
-===============
-
-* New fresh look
-* Responsive mobile interface
-* Useful admin home page
-* Minimal template overriding
-* Easy integration
-* Themes support
-* Autocompletion
-* Handy controls
-
-Screenshots
-===========
-
-.. image:: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen1_720.png
-    :alt: Screenshot #1
-    :align: center
-    :target: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen1.png
-    
-.. image:: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen2_720.png
-    :alt: Screenshot #2
-    :align: center
-    :target: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen2.png
-    
-.. image:: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen3_720.png
-    :alt: Screenshot #3
-    :align: center
-    :target: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen3.png
-
-Installation
-============
-
-* Download and install latest version of Django JET:
-
-.. code:: python
-
-    pip install django-jet
-    # or
-    easy_install django-jet
-
-* Add 'jet' application to the INSTALLED_APPS setting of your Django project settings.py file (note it should be before 'django.contrib.admin'):
-
-.. code:: python
-
-    INSTALLED_APPS = (
-        ...
-        'jet',
-        'django.contrib.admin',
-    )
-        
-* Make sure ``django.template.context_processors.request`` context processor is enabled in settings.py (Django 1.8+ way):
-
-.. code:: python
-
-    TEMPLATES = [
-        {
-            'BACKEND': 'django.template.backends.django.DjangoTemplates',
-            'DIRS': [],
-            'APP_DIRS': True,
-            'OPTIONS': {
-                'context_processors': [
-                    ...
-                    'django.template.context_processors.request',
-                    ...
-                ],
-            },
-        },
-    ]
-
-.. warning::
-    Before Django 1.8 you should specify context processors different way. Also use ``django.core.context_processors.request`` instead of ``django.template.context_processors.request``.
-
-    .. code:: python
-
-        from django.conf import global_settings
-
-        TEMPLATE_CONTEXT_PROCESSORS = global_settings.TEMPLATE_CONTEXT_PROCESSORS + (
-            'django.core.context_processors.request',
-        )
-
-* Add URL-pattern to the urlpatterns of your Django project urls.py file (they are needed for related–lookups and autocompletes):
-
-.. code:: python
-
-    urlpatterns = patterns(
-        '',
-        url(r'^jet/', include('jet.urls', 'jet')),  # Django JET URLS
-        url(r'^admin/', include(admin.site.urls)),
-        ...
-    )
-
-* Create database tables:
-
-.. code:: python
-
-    python manage.py migrate jet
-    # or 
-    python manage.py syncdb
-        
-* Collect static if you are in production environment:
-
-.. code:: python
-
-        python manage.py collectstatic
-        
-* Clear your browser cache
-
-Dashboard installation
-======================
-
-.. note:: Dashboard is located into a separate application. So after a typical JET installation it won't be active.
-          To enable dashboard application follow these steps:
-
-* Add 'jet.dashboard' application to the INSTALLED_APPS setting of your Django project settings.py file (note it should be before 'jet'):
-
-.. code:: python
-
-    INSTALLED_APPS = (
-        ...
-        'jet.dashboard',
-        'jet',
-        'django.contrib.admin',
-        ...
-    )
-
-* Add URL-pattern to the urlpatterns of your Django project urls.py file (they are needed for related–lookups and autocompletes):
-
-.. code:: python
-
-    urlpatterns = patterns(
-        '',
-        url(r'^jet/', include('jet.urls', 'jet')),  # Django JET URLS
-        url(r'^jet/dashboard/', include('jet.dashboard.urls', 'jet-dashboard')),  # Django JET dashboard URLS
-        url(r'^admin/', include(admin.site.urls)),
-        ...
-    )
-
-* **For Google Analytics widgets only** install python package:
-
-.. code::
-
-    pip install google-api-python-client==1.4.1
-
-* Create database tables:
-
-.. code:: python
-
-    python manage.py migrate dashboard
-    # or
-    python manage.py syncdb
-
-* Collect static if you are in production environment:
-
-.. code:: python
-
-        python manage.py collectstatic
-
-
-
```

### Comparing `django-jet-new-2.3.2/README.rst` & `django-jet-new-2.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/django_jet_new.egg-info/PKG-INFO` & `django-jet-new-2.3.3/django_jet_new.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,217 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: django-jet-new
-Version: 2.3.2
+Version: 2.3.3
 Summary: Modern template for Django admin interface with improved functionality
 Home-page: https://github.com/geex-arts/django-jet
 Author: Denis Kildishev
 Author-email: support@jet.geex-arts.com
 License: AGPLv3
+Description: ==========
+        Django JET
+        ==========
+        
+        .. image:: https://travis-ci.org/geex-arts/django-jet.svg?branch=master
+            :target: https://travis-ci.org/geex-arts/django-jet
+        
+        **Modern template for Django admin interface with improved functionality**
+        
+        +-----------------------------------------------------------------------------------------------------------------------------------+
+        | Attention! **NEW JET**                                                                                                            |
+        +===================================================================================================================================+
+        | **We are proud to announce completely new Jet. Please check out Live Demo.**                                                      |
+        |                                                                                                                                   |
+        | Developing of new features for Django Jet will be frozen, only critical bugs will be fixed.                                       |
+        +-----------------------------------------------------------------------------------------------------------------------------------+
+        | `Live Demo <https://app.jetadmin.io/demo?utm_source=jet&utm_medium=banner&utm_campaign=github&utm_content=link&utm_term=promo>`_  |
+        +-----------------------------------------------------------------------------------------------------------------------------------+
+        
+        
+        Django JET has two kinds of licenses: open-source (AGPLv3) and commercial. Please note that using AGPLv3
+        code in your programs make them AGPL compatible too. So if you don't want to comply with that we can provide you a commercial
+        license (visit Home page). The commercial license is designed for using Django JET in commercial products
+        and applications without the provisions of the AGPLv3.
+        
+        .. image:: https://raw.githubusercontent.com/geex-arts/jet/static/logo.png
+            :width: 500px
+            :height: 500px
+            :scale: 50%
+            :alt: Logo
+            :align: center
+            
+        * Home page: http://jet.geex-arts.com/
+        * **New Jet**: `Live Demo <https://app.jetadmin.io/demo?utm_source=jet&utm_medium=banner&utm_campaign=github&utm_content=link&utm_term=promo>`_
+        * Live Demo: http://demo.jet.geex-arts.com/admin/
+        * Documentation: http://jet.readthedocs.org/
+        * libi.io http://libi.io/library/1683/django-jet
+        * PyPI: https://pypi.python.org/pypi/django-jet
+        * Support: support@jet.geex-arts.com
+        
+        Why Django JET?
+        ===============
+        
+        * New fresh look
+        * Responsive mobile interface
+        * Useful admin home page
+        * Minimal template overriding
+        * Easy integration
+        * Themes support
+        * Autocompletion
+        * Handy controls
+        
+        Screenshots
+        ===========
+        
+        .. image:: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen1_720.png
+            :alt: Screenshot #1
+            :align: center
+            :target: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen1.png
+            
+        .. image:: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen2_720.png
+            :alt: Screenshot #2
+            :align: center
+            :target: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen2.png
+            
+        .. image:: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen3_720.png
+            :alt: Screenshot #3
+            :align: center
+            :target: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen3.png
+        
+        Installation
+        ============
+        
+        * Download and install latest version of Django JET:
+        
+        .. code:: python
+        
+            pip install django-jet
+            # or
+            easy_install django-jet
+        
+        * Add 'jet' application to the INSTALLED_APPS setting of your Django project settings.py file (note it should be before 'django.contrib.admin'):
+        
+        .. code:: python
+        
+            INSTALLED_APPS = (
+                ...
+                'jet',
+                'django.contrib.admin',
+            )
+                
+        * Make sure ``django.template.context_processors.request`` context processor is enabled in settings.py (Django 1.8+ way):
+        
+        .. code:: python
+        
+            TEMPLATES = [
+                {
+                    'BACKEND': 'django.template.backends.django.DjangoTemplates',
+                    'DIRS': [],
+                    'APP_DIRS': True,
+                    'OPTIONS': {
+                        'context_processors': [
+                            ...
+                            'django.template.context_processors.request',
+                            ...
+                        ],
+                    },
+                },
+            ]
+        
+        .. warning::
+            Before Django 1.8 you should specify context processors different way. Also use ``django.core.context_processors.request`` instead of ``django.template.context_processors.request``.
+        
+            .. code:: python
+        
+                from django.conf import global_settings
+        
+                TEMPLATE_CONTEXT_PROCESSORS = global_settings.TEMPLATE_CONTEXT_PROCESSORS + (
+                    'django.core.context_processors.request',
+                )
+        
+        * Add URL-pattern to the urlpatterns of your Django project urls.py file (they are needed for related–lookups and autocompletes):
+        
+        .. code:: python
+        
+            urlpatterns = patterns(
+                '',
+                url(r'^jet/', include('jet.urls', 'jet')),  # Django JET URLS
+                url(r'^admin/', include(admin.site.urls)),
+                ...
+            )
+        
+        * Create database tables:
+        
+        .. code:: python
+        
+            python manage.py migrate jet
+            # or 
+            python manage.py syncdb
+                
+        * Collect static if you are in production environment:
+        
+        .. code:: python
+        
+                python manage.py collectstatic
+                
+        * Clear your browser cache
+        
+        Dashboard installation
+        ======================
+        
+        .. note:: Dashboard is located into a separate application. So after a typical JET installation it won't be active.
+                  To enable dashboard application follow these steps:
+        
+        * Add 'jet.dashboard' application to the INSTALLED_APPS setting of your Django project settings.py file (note it should be before 'jet'):
+        
+        .. code:: python
+        
+            INSTALLED_APPS = (
+                ...
+                'jet.dashboard',
+                'jet',
+                'django.contrib.admin',
+                ...
+            )
+        
+        * Add URL-pattern to the urlpatterns of your Django project urls.py file (they are needed for related–lookups and autocompletes):
+        
+        .. code:: python
+        
+            urlpatterns = patterns(
+                '',
+                url(r'^jet/', include('jet.urls', 'jet')),  # Django JET URLS
+                url(r'^jet/dashboard/', include('jet.dashboard.urls', 'jet-dashboard')),  # Django JET dashboard URLS
+                url(r'^admin/', include(admin.site.urls)),
+                ...
+            )
+        
+        * **For Google Analytics widgets only** install python package:
+        
+        .. code::
+        
+            pip install google-api-python-client==1.4.1
+        
+        * Create database tables:
+        
+        .. code:: python
+        
+            python manage.py migrate dashboard
+            # or
+            python manage.py syncdb
+        
+        * Collect static if you are in production environment:
+        
+        .. code:: python
+        
+                python manage.py collectstatic
+        
+        
+        
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 4.2
 Classifier: License :: Free for non-commercial use
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -24,209 +226,7 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Web Environment
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: User Interfaces
-License-File: LICENSE
-
-==========
-Django JET
-==========
-
-.. image:: https://travis-ci.org/geex-arts/django-jet.svg?branch=master
-    :target: https://travis-ci.org/geex-arts/django-jet
-
-**Modern template for Django admin interface with improved functionality**
-
-+-----------------------------------------------------------------------------------------------------------------------------------+
-| Attention! **NEW JET**                                                                                                            |
-+===================================================================================================================================+
-| **We are proud to announce completely new Jet. Please check out Live Demo.**                                                      |
-|                                                                                                                                   |
-| Developing of new features for Django Jet will be frozen, only critical bugs will be fixed.                                       |
-+-----------------------------------------------------------------------------------------------------------------------------------+
-| `Live Demo <https://app.jetadmin.io/demo?utm_source=jet&utm_medium=banner&utm_campaign=github&utm_content=link&utm_term=promo>`_  |
-+-----------------------------------------------------------------------------------------------------------------------------------+
-
-
-Django JET has two kinds of licenses: open-source (AGPLv3) and commercial. Please note that using AGPLv3
-code in your programs make them AGPL compatible too. So if you don't want to comply with that we can provide you a commercial
-license (visit Home page). The commercial license is designed for using Django JET in commercial products
-and applications without the provisions of the AGPLv3.
-
-.. image:: https://raw.githubusercontent.com/geex-arts/jet/static/logo.png
-    :width: 500px
-    :height: 500px
-    :scale: 50%
-    :alt: Logo
-    :align: center
-    
-* Home page: http://jet.geex-arts.com/
-* **New Jet**: `Live Demo <https://app.jetadmin.io/demo?utm_source=jet&utm_medium=banner&utm_campaign=github&utm_content=link&utm_term=promo>`_
-* Live Demo: http://demo.jet.geex-arts.com/admin/
-* Documentation: http://jet.readthedocs.org/
-* libi.io http://libi.io/library/1683/django-jet
-* PyPI: https://pypi.python.org/pypi/django-jet
-* Support: support@jet.geex-arts.com
-
-Why Django JET?
-===============
-
-* New fresh look
-* Responsive mobile interface
-* Useful admin home page
-* Minimal template overriding
-* Easy integration
-* Themes support
-* Autocompletion
-* Handy controls
-
-Screenshots
-===========
-
-.. image:: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen1_720.png
-    :alt: Screenshot #1
-    :align: center
-    :target: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen1.png
-    
-.. image:: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen2_720.png
-    :alt: Screenshot #2
-    :align: center
-    :target: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen2.png
-    
-.. image:: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen3_720.png
-    :alt: Screenshot #3
-    :align: center
-    :target: https://raw.githubusercontent.com/geex-arts/django-jet/static/screen3.png
-
-Installation
-============
-
-* Download and install latest version of Django JET:
-
-.. code:: python
-
-    pip install django-jet
-    # or
-    easy_install django-jet
-
-* Add 'jet' application to the INSTALLED_APPS setting of your Django project settings.py file (note it should be before 'django.contrib.admin'):
-
-.. code:: python
-
-    INSTALLED_APPS = (
-        ...
-        'jet',
-        'django.contrib.admin',
-    )
-        
-* Make sure ``django.template.context_processors.request`` context processor is enabled in settings.py (Django 1.8+ way):
-
-.. code:: python
-
-    TEMPLATES = [
-        {
-            'BACKEND': 'django.template.backends.django.DjangoTemplates',
-            'DIRS': [],
-            'APP_DIRS': True,
-            'OPTIONS': {
-                'context_processors': [
-                    ...
-                    'django.template.context_processors.request',
-                    ...
-                ],
-            },
-        },
-    ]
-
-.. warning::
-    Before Django 1.8 you should specify context processors different way. Also use ``django.core.context_processors.request`` instead of ``django.template.context_processors.request``.
-
-    .. code:: python
-
-        from django.conf import global_settings
-
-        TEMPLATE_CONTEXT_PROCESSORS = global_settings.TEMPLATE_CONTEXT_PROCESSORS + (
-            'django.core.context_processors.request',
-        )
-
-* Add URL-pattern to the urlpatterns of your Django project urls.py file (they are needed for related–lookups and autocompletes):
-
-.. code:: python
-
-    urlpatterns = patterns(
-        '',
-        url(r'^jet/', include('jet.urls', 'jet')),  # Django JET URLS
-        url(r'^admin/', include(admin.site.urls)),
-        ...
-    )
-
-* Create database tables:
-
-.. code:: python
-
-    python manage.py migrate jet
-    # or 
-    python manage.py syncdb
-        
-* Collect static if you are in production environment:
-
-.. code:: python
-
-        python manage.py collectstatic
-        
-* Clear your browser cache
-
-Dashboard installation
-======================
-
-.. note:: Dashboard is located into a separate application. So after a typical JET installation it won't be active.
-          To enable dashboard application follow these steps:
-
-* Add 'jet.dashboard' application to the INSTALLED_APPS setting of your Django project settings.py file (note it should be before 'jet'):
-
-.. code:: python
-
-    INSTALLED_APPS = (
-        ...
-        'jet.dashboard',
-        'jet',
-        'django.contrib.admin',
-        ...
-    )
-
-* Add URL-pattern to the urlpatterns of your Django project urls.py file (they are needed for related–lookups and autocompletes):
-
-.. code:: python
-
-    urlpatterns = patterns(
-        '',
-        url(r'^jet/', include('jet.urls', 'jet')),  # Django JET URLS
-        url(r'^jet/dashboard/', include('jet.dashboard.urls', 'jet-dashboard')),  # Django JET dashboard URLS
-        url(r'^admin/', include(admin.site.urls)),
-        ...
-    )
-
-* **For Google Analytics widgets only** install python package:
-
-.. code::
-
-    pip install google-api-python-client==1.4.1
-
-* Create database tables:
-
-.. code:: python
-
-    python manage.py migrate dashboard
-    # or
-    python manage.py syncdb
-
-* Collect static if you are in production environment:
-
-.. code:: python
-
-        python manage.py collectstatic
-
-
-
```

### Comparing `django-jet-new-2.3.2/django_jet_new.egg-info/SOURCES.txt` & `django-jet-new-2.3.3/django_jet_new.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/dashboard.py` & `django-jet-new-2.3.3/jet/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/dashboard_modules/google_analytics.py` & `django-jet-new-2.3.3/jet/dashboard/dashboard_modules/google_analytics.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/dashboard_modules/google_analytics_views.py` & `django-jet-new-2.3.3/jet/dashboard/dashboard_modules/google_analytics_views.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/dashboard_modules/yandex_metrika.py` & `django-jet-new-2.3.3/jet/dashboard/dashboard_modules/yandex_metrika.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/dashboard_modules/yandex_metrika_views.py` & `django-jet-new-2.3.3/jet/dashboard/dashboard_modules/yandex_metrika_views.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/forms.py` & `django-jet-new-2.3.3/jet/dashboard/forms.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/ar/LC_MESSAGES/django.mo` & `django-jet-new-2.3.3/jet/dashboard/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/ar/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/dashboard/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/ar/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/dashboard/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/cs/LC_MESSAGES/django.mo` & `django-jet-new-2.3.3/jet/dashboard/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/cs/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/dashboard/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/cs/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/dashboard/locale/cs/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/de/LC_MESSAGES/django.mo` & `django-jet-new-2.3.3/jet/dashboard/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/de/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/dashboard/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/de/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/dashboard/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/en/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/dashboard/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/en/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/dashboard/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/es/LC_MESSAGES/django.mo` & `django-jet-new-2.3.3/jet/dashboard/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/es/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/dashboard/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/es/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/dashboard/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/fa/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/dashboard/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/fa/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/dashboard/locale/fa/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/fr/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/dashboard/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/fr/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/dashboard/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/pl/LC_MESSAGES/django.mo` & `django-jet-new-2.3.3/jet/dashboard/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/pl/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/dashboard/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/pt-br/LC_MESSAGES/django.mo` & `django-jet-new-2.3.3/jet/dashboard/locale/pt-br/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/pt-br/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/dashboard/locale/pt-br/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/pt-br/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/dashboard/locale/pt-br/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/ru/LC_MESSAGES/django.mo` & `django-jet-new-2.3.3/jet/dashboard/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/ru/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/dashboard/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/ru/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/dashboard/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/zh_cn/LC_MESSAGES/django.mo` & `django-jet-new-2.3.3/jet/dashboard/locale/zh_cn/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/locale/zh_cn/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/dashboard/locale/zh_cn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/migrations/0001_initial.py` & `django-jet-new-2.3.3/jet/dashboard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/models.py` & `django-jet-new-2.3.3/jet/dashboard/models.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/modules.py` & `django-jet-new-2.3.3/jet/dashboard/modules.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/south_migrations/0001_initial.py` & `django-jet-new-2.3.3/jet/dashboard/south_migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/static/jet.dashboard/dashboard_modules/google_analytics.js` & `django-jet-new-2.3.3/jet/dashboard/static/jet.dashboard/dashboard_modules/google_analytics.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/static/jet.dashboard/dashboard_modules/yandex_metrika.js` & `django-jet-new-2.3.3/jet/dashboard/static/jet.dashboard/dashboard_modules/yandex_metrika.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/static/jet.dashboard/vendor/chart.js/CONTRIBUTING.md` & `django-jet-new-2.3.3/jet/dashboard/static/jet.dashboard/vendor/chart.js/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/static/jet.dashboard/vendor/chart.js/Chart.js` & `django-jet-new-2.3.3/jet/dashboard/static/jet.dashboard/vendor/chart.js/Chart.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/static/jet.dashboard/vendor/chart.js/Chart.min.js` & `django-jet-new-2.3.3/jet/dashboard/static/jet.dashboard/vendor/chart.js/Chart.min.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/static/jet.dashboard/vendor/chart.js/LICENSE.md` & `django-jet-new-2.3.3/jet/dashboard/static/jet.dashboard/vendor/chart.js/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/static/jet.dashboard/vendor/chart.js/README.md` & `django-jet-new-2.3.3/jet/dashboard/static/jet.dashboard/vendor/chart.js/README.md`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templates/admin/app_index.html` & `django-jet-new-2.3.3/jet/dashboard/templates/admin/app_index.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templates/admin/index.html` & `django-jet-new-2.3.3/jet/dashboard/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/dashboard.html` & `django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/dashboard_tools.html` & `django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/dashboard_tools.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/module.html` & `django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/module.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/app_list.html` & `django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/app_list.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/feed.html` & `django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/feed.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/google_analytics_period_visitors.html` & `django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/google_analytics_period_visitors.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/google_analytics_visitors_chart.html` & `django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/google_analytics_visitors_chart.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/google_analytics_visitors_totals.html` & `django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_visitors_totals.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/link_list.html` & `django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/link_list.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/model_list.html` & `django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/model_list.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/recent_actions.html` & `django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/recent_actions.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_period_visitors.html` & `django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_period_visitors.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_visitors_chart.html` & `django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_visitors_chart.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/modules/yandex_metrika_visitors_totals.html` & `django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/modules/google_analytics_visitors_totals.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/update_module.html` & `django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/update_module.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templates/jet.dashboard/update_module_fieldset.html` & `django-jet-new-2.3.3/jet/dashboard/templates/jet.dashboard/update_module_fieldset.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/templatetags/jet_dashboard_tags.py` & `django-jet-new-2.3.3/jet/dashboard/templatetags/jet_dashboard_tags.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/urls.py` & `django-jet-new-2.3.3/jet/dashboard/urls.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/utils.py` & `django-jet-new-2.3.3/jet/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/dashboard/views.py` & `django-jet-new-2.3.3/jet/dashboard/views.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/filters.py` & `django-jet-new-2.3.3/jet/filters.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/forms.py` & `django-jet-new-2.3.3/jet/forms.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/ar/LC_MESSAGES/django.mo` & `django-jet-new-2.3.3/jet/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/ar/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/ar/LC_MESSAGES/djangojs.mo` & `django-jet-new-2.3.3/jet/locale/ar/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/ar/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/cs/LC_MESSAGES/django.mo` & `django-jet-new-2.3.3/jet/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/cs/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/cs/LC_MESSAGES/djangojs.mo` & `django-jet-new-2.3.3/jet/locale/cs/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/cs/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/locale/cs/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/de/LC_MESSAGES/django.mo` & `django-jet-new-2.3.3/jet/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/de/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/de/LC_MESSAGES/djangojs.mo` & `django-jet-new-2.3.3/jet/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/de/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/en/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/en/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/es/LC_MESSAGES/django.mo` & `django-jet-new-2.3.3/jet/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/es/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/es/LC_MESSAGES/djangojs.mo` & `django-jet-new-2.3.3/jet/locale/es/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/es/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/fa/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/fa/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/locale/fa/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/fr/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/fr/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/pl/LC_MESSAGES/django.mo` & `django-jet-new-2.3.3/jet/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/pl/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/pl/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/locale/pl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/pt_BR/LC_MESSAGES/django.mo` & `django-jet-new-2.3.3/jet/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/pt_BR/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `django-jet-new-2.3.3/jet/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/pt_BR/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/ru/LC_MESSAGES/django.mo` & `django-jet-new-2.3.3/jet/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/ru/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/ru/LC_MESSAGES/djangojs.mo` & `django-jet-new-2.3.3/jet/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/ru/LC_MESSAGES/djangojs.po` & `django-jet-new-2.3.3/jet/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/zh_CN/LC_MESSAGES/django.mo` & `django-jet-new-2.3.3/jet/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/locale/zh_CN/LC_MESSAGES/django.po` & `django-jet-new-2.3.3/jet/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/management/commands/jet_custom_apps_example.py` & `django-jet-new-2.3.3/jet/management/commands/jet_custom_apps_example.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/management/commands/jet_side_menu_items_example.py` & `django-jet-new-2.3.3/jet/management/commands/jet_side_menu_items_example.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/migrations/0001_initial.py` & `django-jet-new-2.3.3/jet/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/models.py` & `django-jet-new-2.3.3/jet/models.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/ordered_set.py` & `django-jet-new-2.3.3/jet/ordered_set.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/south_migrations/0001_initial.py` & `django-jet-new-2.3.3/jet/south_migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/south_migrations/0002_auto__del_userdashboardmodule.py` & `django-jet-new-2.3.3/jet/south_migrations/0002_auto__del_userdashboardmodule.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/_base.scss` & `django-jet-new-2.3.3/jet/static/jet/css/_base.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/_breadcrumbs.scss` & `django-jet-new-2.3.3/jet/static/jet/css/_breadcrumbs.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/_changeform.scss` & `django-jet-new-2.3.3/jet/static/jet/css/_changeform.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/_changelist.scss` & `django-jet-new-2.3.3/jet/static/jet/css/_changelist.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/_content.scss` & `django-jet-new-2.3.3/jet/static/jet/css/_content.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/_dashboard.scss` & `django-jet-new-2.3.3/jet/static/jet/css/_dashboard.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/_delete-confirmation.scss` & `django-jet-new-2.3.3/jet/static/jet/css/_delete-confirmation.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/_forms.scss` & `django-jet-new-2.3.3/jet/static/jet/css/_forms.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/_header.scss` & `django-jet-new-2.3.3/jet/static/jet/css/_header.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/_helpers.scss` & `django-jet-new-2.3.3/jet/static/jet/css/_helpers.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/_login.scss` & `django-jet-new-2.3.3/jet/static/jet/css/_login.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/_messages.scss` & `django-jet-new-2.3.3/jet/static/jet/css/_messages.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/_modules.scss` & `django-jet-new-2.3.3/jet/static/jet/css/_modules.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/_object-tools.scss` & `django-jet-new-2.3.3/jet/static/jet/css/_object-tools.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/_relatedpopup.scss` & `django-jet-new-2.3.3/jet/static/jet/css/_relatedpopup.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/_sidebar.scss` & `django-jet-new-2.3.3/jet/static/jet/css/_sidebar.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/_tables.scss` & `django-jet-new-2.3.3/jet/static/jet/css/_tables.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/_variables.scss` & `django-jet-new-2.3.3/jet/static/jet/css/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/icons/_variables.scss` & `django-jet-new-2.3.3/jet/static/jet/css/icons/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/icons/fonts/jet-icons.eot` & `django-jet-new-2.3.3/jet/static/jet/css/icons/fonts/jet-icons.eot`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/icons/fonts/jet-icons.svg` & `django-jet-new-2.3.3/jet/static/jet/css/icons/fonts/jet-icons.svg`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/icons/fonts/jet-icons.ttf` & `django-jet-new-2.3.3/jet/static/jet/css/icons/fonts/jet-icons.ttf`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/icons/fonts/jet-icons.woff` & `django-jet-new-2.3.3/jet/static/jet/css/icons/fonts/jet-icons.woff`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/icons/style.css` & `django-jet-new-2.3.3/jet/static/jet/css/icons/style.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/_jquery-ui.theme.scss` & `django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/_jquery-ui.theme.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/ui-icons_222222_256x240.png` & `django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/ui-icons_2e83ff_256x240.png` & `django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/ui-icons_454545_256x240.png` & `django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/ui-icons_888888_256x240.png` & `django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/jquery-ui/images/ui-icons_cd0a0a_256x240.png` & `django-jet-new-2.3.3/jet/static/jet/css/jquery-ui/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/select2/_layout.scss` & `django-jet-new-2.3.3/jet/static/jet/css/select2/_layout.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/select2/_multiple.scss` & `django-jet-new-2.3.3/jet/static/jet/css/select2/_multiple.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/select2/_single.scss` & `django-jet-new-2.3.3/jet/static/jet/css/select2/_single.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/default/base.css` & `django-jet-new-2.3.3/jet/static/jet/css/themes/default/base.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/default/base.css.map` & `django-jet-new-2.3.3/jet/static/jet/css/themes/default/base.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/default/jquery-ui.theme.css` & `django-jet-new-2.3.3/jet/static/jet/css/themes/default/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/default/jquery-ui.theme.css.map` & `django-jet-new-2.3.3/jet/static/jet/css/themes/default/jquery-ui.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/default/select2.theme.css` & `django-jet-new-2.3.3/jet/static/jet/css/themes/default/select2.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/default/select2.theme.css.map` & `django-jet-new-2.3.3/jet/static/jet/css/themes/default/select2.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/green/_variables.scss` & `django-jet-new-2.3.3/jet/static/jet/css/themes/green/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/green/base.css` & `django-jet-new-2.3.3/jet/static/jet/css/themes/green/base.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/green/base.css.map` & `django-jet-new-2.3.3/jet/static/jet/css/themes/green/base.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/green/jquery-ui.theme.css` & `django-jet-new-2.3.3/jet/static/jet/css/themes/green/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/green/jquery-ui.theme.css.map` & `django-jet-new-2.3.3/jet/static/jet/css/themes/green/jquery-ui.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/green/select2.theme.css` & `django-jet-new-2.3.3/jet/static/jet/css/themes/green/select2.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/green/select2.theme.css.map` & `django-jet-new-2.3.3/jet/static/jet/css/themes/green/select2.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-blue/_variables.scss` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-blue/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-blue/base.css` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-blue/base.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-blue/base.css.map` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-blue/base.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-blue/jquery-ui.theme.css` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-blue/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-blue/jquery-ui.theme.css.map` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-blue/jquery-ui.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-blue/select2.theme.css` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-blue/select2.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-blue/select2.theme.css.map` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-blue/select2.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-gray/_variables.scss` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-gray/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-gray/base.css` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-gray/base.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-gray/base.css.map` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-gray/base.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-gray/jquery-ui.theme.css` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-gray/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-gray/jquery-ui.theme.css.map` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-gray/jquery-ui.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-gray/select2.theme.css` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-gray/select2.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-gray/select2.theme.css.map` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-gray/select2.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-green/_variables.scss` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-green/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-green/base.css` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-green/base.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-green/base.css.map` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-green/base.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-green/jquery-ui.theme.css` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-green/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-green/jquery-ui.theme.css.map` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-green/jquery-ui.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-green/select2.theme.css` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-green/select2.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-green/select2.theme.css.map` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-green/select2.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-violet/_variables.scss` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-violet/_variables.scss`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-violet/base.css` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-violet/base.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-violet/base.css.map` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-violet/base.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-violet/jquery-ui.theme.css` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-violet/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-violet/jquery-ui.theme.css.map` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-violet/jquery-ui.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-violet/select2.theme.css` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-violet/select2.theme.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/themes/light-violet/select2.theme.css.map` & `django-jet-new-2.3.3/jet/static/jet/css/themes/light-violet/select2.theme.css.map`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/css/vendor.css` & `django-jet-new-2.3.3/jet/static/jet/css/vendor.css`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/build/bundle.min.js` & `django-jet-new-2.3.3/jet/static/jet/js/build/bundle.min.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-af.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-af.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ar-DZ.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ar-DZ.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ar.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ar.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-az.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-az.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-be.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-be.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-bg.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-bg.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-bs.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-bs.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ca.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ca.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-cs.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-cs.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-cy-GB.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-cy-GB.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-da.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-da.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-de.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-de.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-el.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-el.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-en-AU.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-en-AU.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-en-GB.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-en-GB.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-en-NZ.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-en-NZ.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-eo.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-eo.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-es.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-es.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-et.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-et.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-eu.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-eu.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-fa.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-fa.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-fi.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-fi.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-fo.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-fo.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-fr-CA.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-fr-CA.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-fr-CH.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-fr-CH.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-fr.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-fr.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-gl.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-gl.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-he.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-he.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-hi.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-hi.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-hr.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-hr.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-hu.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-hu.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-hy.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-hy.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-id.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-id.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-is.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-is.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-it-CH.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-it-CH.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-it.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-it.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ja.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ja.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ka.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ka.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-kk.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-kk.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-km.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-km.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ko.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ko.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ky.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ky.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-lb.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-lb.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-lt.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-lt.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-lv.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-lv.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-mk.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-mk.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ml.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ml.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ms.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ms.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-nb.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-nb.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-nl-BE.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-nl-BE.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-nl.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-nl.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-nn.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-nn.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-no.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-no.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-pl.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-pl.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-pt-BR.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-pt.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-pt.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-rm.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-rm.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ro.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ro.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ru.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ru.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-sk.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-sk.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-sl.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-sl.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-sq.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-sq.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-sr-SR.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-sr-SR.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-sr.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-sr.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-sv.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-sv.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-ta.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-ta.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-th.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-th.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-tj.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-tj.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-tr.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-tr.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-uk.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-uk.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-vi.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-vi.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-CN.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-HK.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-HK.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-TW.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui/datepicker-zh-TW.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-fr.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-fr.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-ru.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/jquery-ui-timepicker/jquery.ui.timepicker-ru.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/az.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/az.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/bg.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/bg.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/ca.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/ca.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/cs.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/cs.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/da.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/da.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/de.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/de.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/en.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/en.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/es.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/es.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/et.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/et.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/eu.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/eu.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/fa.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/fa.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/fi.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/fi.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/fr.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/fr.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/gl.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/gl.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/he.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/he.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/hi.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/hi.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/hr.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/hr.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/hu.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/hu.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/id.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/id.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/is.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/is.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/it.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/it.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/ko.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/ko.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/lt.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/lt.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/lv.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/lv.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/mk.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/mk.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/nb.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/nb.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/nl.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/nl.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/pl.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/pl.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/pt-BR.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/pt.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/pt.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/ro.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/ro.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/ru.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/ru.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/sk.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/sk.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/sr.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/sr.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/sv.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/sv.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/th.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/th.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/tr.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/tr.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/uk.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/uk.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/vi.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/vi.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/zh-CN.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/i18n/select2/zh-TW.js` & `django-jet-new-2.3.3/jet/static/jet/js/i18n/select2/zh-TW.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/changeform-tabs.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/changeform-tabs.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/changeform.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/changeform.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/changelist.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/changelist.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/checkboxes.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/checkboxes.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/compact-inline.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/compact-inline.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/dashboard.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/dashboard.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/date-time-widgets.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/date-time-widgets.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/filters.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/filters.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/inlines.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/inlines.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/related-popups.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/related-popups.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/scroll-to-bottom-detector.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/scroll-to-bottom-detector.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/selects.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/selects.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/siblings.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/siblings.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/sidebar/application-pinning.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/sidebar/application-pinning.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/sidebar/bookmarks.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/sidebar/bookmarks.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/sidebar/main.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/sidebar/main.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/sidebar/popup.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/sidebar/popup.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/themes.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/themes.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/tooltips.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/tooltips.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/features/touchmove-non-scrollable.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/features/touchmove-non-scrollable.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/actions.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/actions.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/branding.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/branding.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/breadcrumbs.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/breadcrumbs.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/changeform-tabs.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/changeform-tabs.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/icons.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/icons.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/paginator.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/paginator.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/related-widget-wrapper.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/related-widget-wrapper.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/stacked-inline.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/stacked-inline.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/tabular-inline.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/tabular-inline.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/toolbar.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/toolbar.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/layout-updaters/user-tools.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/layout-updaters/user-tools.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/main.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/main.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/static/jet/js/src/utils/window-storage.js` & `django-jet-new-2.3.3/jet/static/jet/js/src/utils/window-storage.js`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/templates/admin/base.html` & `django-jet-new-2.3.3/jet/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/templates/admin/edit_inline/compact.html` & `django-jet-new-2.3.3/jet/templates/admin/edit_inline/compact.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/templates/admin/includes/fieldset.html` & `django-jet-new-2.3.3/jet/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/templates/rangefilter/date_filter.html` & `django-jet-new-2.3.3/jet/templates/rangefilter/date_filter.html`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/templatetags/jet_tags.py` & `django-jet-new-2.3.3/jet/templatetags/jet_tags.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/tests/dashboard.py` & `django-jet-new-2.3.3/jet/tests/dashboard.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/tests/models.py` & `django-jet-new-2.3.3/jet/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/tests/settings.py` & `django-jet-new-2.3.3/jet/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/tests/test_dashboard.py` & `django-jet-new-2.3.3/jet/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/tests/test_filters.py` & `django-jet-new-2.3.3/jet/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/tests/test_ordered_set.py` & `django-jet-new-2.3.3/jet/tests/test_ordered_set.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/tests/test_tags.py` & `django-jet-new-2.3.3/jet/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/tests/test_utils.py` & `django-jet-new-2.3.3/jet/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/tests/test_views.py` & `django-jet-new-2.3.3/jet/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/tests/urls.py` & `django-jet-new-2.3.3/jet/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/urls.py` & `django-jet-new-2.3.3/jet/urls.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/jet/utils.py` & `django-jet-new-2.3.3/jet/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,30 +204,32 @@
         queryset = model_admin.get_queryset(request)
     else:
         queryset = model.objects
 
     list_display = model_admin.get_list_display(request)
     list_display_links = model_admin.get_list_display_links(request, list_display)
     list_filter = model_admin.get_list_filter(request)
+
     search_fields = model_admin.get_search_fields(request) \
         if hasattr(model_admin, 'get_search_fields') else model_admin.search_fields
     list_select_related = model_admin.get_list_select_related(request) \
         if hasattr(model_admin, 'get_list_select_related') else model_admin.list_select_related
 
     actions = model_admin.get_actions(request)
     if actions:
         list_display = ['action_checkbox'] + list(list_display)
 
+    search_help_text = None
     ChangeList = model_admin.get_changelist(request)
 
     change_list_args = [
         request, model, list_display, list_display_links, list_filter,
         model_admin.date_hierarchy, search_fields, list_select_related,
         model_admin.list_per_page, model_admin.list_max_show_all,
-        model_admin.list_editable, model_admin]
+        model_admin.list_editable, model_admin, search_help_text]
 
     try:
         sortable_by = model_admin.get_sortable_by(request)
         change_list_args.append(sortable_by)
     except AttributeError:
         # django version < 2.1
         pass
```

### Comparing `django-jet-new-2.3.2/jet/views.py` & `django-jet-new-2.3.3/jet/views.py`

 * *Files identical despite different names*

### Comparing `django-jet-new-2.3.2/setup.py` & `django-jet-new-2.3.3/setup.py`

 * *Files identical despite different names*

