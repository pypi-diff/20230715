# Comparing `tmp/django-oscar-newsletter-0.8.8.tar.gz` & `tmp/django-oscar-newsletter-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oscar-newsletter-0.8.8.tar", last modified: Sat Oct 30 08:49:02 2021, max compression
+gzip compressed data, was "django-oscar-newsletter-0.8.9.tar", last modified: Tue Nov  2 22:27:19 2021, max compression
```

## Comparing `django-oscar-newsletter-0.8.8.tar` & `django-oscar-newsletter-0.8.9.tar`

### file list

```diff
@@ -1,222 +1,222 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.034248 django-oscar-newsletter-0.8.8/
--rw-r--r--   0 runner    (1001) docker     (121)      594 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)      926 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-10-30 08:49:02.034248 django-oscar-newsletter-0.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2894 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-10-30 08:48:54.000000 django-oscar-newsletter-0.8.8/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.006248 django-oscar-newsletter-0.8.8/django_oscar_newsletter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-10-30 08:49:01.000000 django-oscar-newsletter-0.8.8/django_oscar_newsletter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7095 2021-10-30 08:49:01.000000 django-oscar-newsletter-0.8.8/django_oscar_newsletter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-30 08:49:01.000000 django-oscar-newsletter-0.8.8/django_oscar_newsletter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       95 2021-10-30 08:49:01.000000 django-oscar-newsletter-0.8.8/django_oscar_newsletter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-10-30 08:49:01.000000 django-oscar-newsletter-0.8.8/django_oscar_newsletter.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.010248 django-oscar-newsletter-0.8.8/newsletter/
--rw-r--r--   0 runner    (1001) docker     (121)      266 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.010248 django-oscar-newsletter-0.8.8/newsletter/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (121)      543 2021-10-30 08:49:01.000000 django-oscar-newsletter-0.8.8/newsletter/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.010248 django-oscar-newsletter-0.8.8/newsletter/addressimport/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/addressimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9581 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/addressimport/parsers.py
--rw-r--r--   0 runner    (1001) docker     (121)    19522 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     6041 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/admin_forms.py
--rw-r--r--   0 runner    (1001) docker     (121)     1690 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/admin_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      364 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/converters.py
--rw-r--r--   0 runner    (1001) docker     (121)      847 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     4455 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.010248 django-oscar-newsletter-0.8.8/newsletter/generator/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      743 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/generator/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      993 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/generator/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)     1167 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/generator/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/generator/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      999 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/generator/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.010248 django-oscar-newsletter-0.8.8/newsletter/jobs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/jobs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.010248 django-oscar-newsletter-0.8.8/newsletter/jobs/daily/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/jobs/daily/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.010248 django-oscar-newsletter-0.8.8/newsletter/jobs/hourly/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/jobs/hourly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      421 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/jobs/hourly/submit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.010248 django-oscar-newsletter-0.8.8/newsletter/jobs/monthly/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/jobs/monthly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.010248 django-oscar-newsletter-0.8.8/newsletter/jobs/weekly/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/jobs/weekly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.002248 django-oscar-newsletter-0.8.8/newsletter/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:01.994248 django-oscar-newsletter-0.8.8/newsletter/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.014248 django-oscar-newsletter-0.8.8/newsletter/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    15804 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    27679 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      916 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/ar/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:01.994248 django-oscar-newsletter-0.8.8/newsletter/locale/cs_CZ/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.014248 django-oscar-newsletter-0.8.8/newsletter/locale/cs_CZ/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    15108 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/cs_CZ/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    26457 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/cs_CZ/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      903 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/cs_CZ/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/cs_CZ/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:01.994248 django-oscar-newsletter-0.8.8/newsletter/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.014248 django-oscar-newsletter-0.8.8/newsletter/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    15968 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    26705 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      765 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/de/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/de/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:01.994248 django-oscar-newsletter-0.8.8/newsletter/locale/el_GR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.014248 django-oscar-newsletter-0.8.8/newsletter/locale/el_GR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    17161 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/el_GR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    28994 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/el_GR/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      994 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/el_GR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/el_GR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:01.998248 django-oscar-newsletter-0.8.8/newsletter/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.014248 django-oscar-newsletter-0.8.8/newsletter/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    15282 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    26219 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      747 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/en/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:01.998248 django-oscar-newsletter-0.8.8/newsletter/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.018248 django-oscar-newsletter-0.8.8/newsletter/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    15820 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    26644 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      792 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/es/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/es/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:01.998248 django-oscar-newsletter-0.8.8/newsletter/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.018248 django-oscar-newsletter-0.8.8/newsletter/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    14351 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    26814 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/fa/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      834 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/fa/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/fa/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:01.998248 django-oscar-newsletter-0.8.8/newsletter/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.018248 django-oscar-newsletter-0.8.8/newsletter/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    16054 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    26804 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      794 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:01.998248 django-oscar-newsletter-0.8.8/newsletter/locale/is_IS/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.018248 django-oscar-newsletter-0.8.8/newsletter/locale/is_IS/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    12225 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/is_IS/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    24447 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/is_IS/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      852 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/is_IS/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/is_IS/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:01.998248 django-oscar-newsletter-0.8.8/newsletter/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.018248 django-oscar-newsletter-0.8.8/newsletter/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    12770 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    24993 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      789 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/it/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/it/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:01.998248 django-oscar-newsletter-0.8.8/newsletter/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.022248 django-oscar-newsletter-0.8.8/newsletter/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    15898 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    26315 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      769 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/nl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/nl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:01.998248 django-oscar-newsletter-0.8.8/newsletter/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.022248 django-oscar-newsletter-0.8.8/newsletter/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    16018 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    26867 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      894 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/pl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/pl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:01.998248 django-oscar-newsletter-0.8.8/newsletter/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.022248 django-oscar-newsletter-0.8.8/newsletter/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    14335 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    25969 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)      784 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:01.998248 django-oscar-newsletter-0.8.8/newsletter/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.022248 django-oscar-newsletter-0.8.8/newsletter/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      767 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/pt_PT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/pt_PT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.002248 django-oscar-newsletter-0.8.8/newsletter/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.022248 django-oscar-newsletter-0.8.8/newsletter/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)    16113 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (121)    28452 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/ru/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.002248 django-oscar-newsletter-0.8.8/newsletter/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.022248 django-oscar-newsletter-0.8.8/newsletter/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)      738 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/zh_CN/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/locale/zh_CN/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.022248 django-oscar-newsletter-0.8.8/newsletter/management/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.026248 django-oscar-newsletter-0.8.8/newsletter/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      958 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/management/commands/submit_newsletter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.026248 django-oscar-newsletter-0.8.8/newsletter/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     7580 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/migrations/0002_auto_20150416_1555.py
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/migrations/0003_auto_20160226_1518.py
--rw-r--r--   0 runner    (1001) docker     (121)      660 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/migrations/0004_auto_20180407_1043.py
--rw-r--r--   0 runner    (1001) docker     (121)      607 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/migrations/0005_auto_20190918_0122.py
--rw-r--r--   0 runner    (1001) docker     (121)      994 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/migrations/0006_attachment.py
--rw-r--r--   0 runner    (1001) docker     (121)      593 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/migrations/0007_switch_from_sorl_imagefield.py
--rw-r--r--   0 runner    (1001) docker     (121)      493 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/migrations/0008_longer_subscription_name.py
--rw-r--r--   0 runner    (1001) docker     (121)     1993 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/migrations/0009_fork_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24562 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     4290 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.002248 django-oscar-newsletter-0.8.8/newsletter/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.002248 django-oscar-newsletter-0.8.8/newsletter/static/newsletter/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.002248 django-oscar-newsletter-0.8.8/newsletter/static/newsletter/admin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.026248 django-oscar-newsletter-0.8.8/newsletter/static/newsletter/admin/img/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/static/newsletter/admin/img/icon-no.gif
--rw-r--r--   0 runner    (1001) docker     (121)      299 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/static/newsletter/admin/img/icon-yes.gif
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/static/newsletter/admin/img/submitting.gif
--rw-r--r--   0 runner    (1001) docker     (121)      100 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/static/newsletter/admin/img/waiting.gif
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.026248 django-oscar-newsletter-0.8.8/newsletter/static/newsletter/admin/js/
--rw-r--r--   0 runner    (1001) docker     (121)      889 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/static/newsletter/admin/js/submit_interface.js
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/static/newsletter/admin/js/subscriber_lookup.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.002248 django-oscar-newsletter-0.8.8/newsletter/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.002248 django-oscar-newsletter-0.8.8/newsletter/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.002248 django-oscar-newsletter-0.8.8/newsletter/templates/admin/newsletter/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.026248 django-oscar-newsletter-0.8.8/newsletter/templates/admin/newsletter/message/
--rw-r--r--   0 runner    (1001) docker     (121)      407 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/admin/newsletter/message/change_form.html
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/admin/newsletter/message/preview.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.026248 django-oscar-newsletter-0.8.8/newsletter/templates/admin/newsletter/submission/
--rw-r--r--   0 runner    (1001) docker     (121)      909 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/admin/newsletter/submission/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.030248 django-oscar-newsletter-0.8.8/newsletter/templates/admin/newsletter/subscription/
--rw-r--r--   0 runner    (1001) docker     (121)      218 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/admin/newsletter/subscription/change_list.html
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/admin/newsletter/subscription/confirmimportform.html
--rw-r--r--   0 runner    (1001) docker     (121)      938 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/admin/newsletter/subscription/importform.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.030248 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/common.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.034248 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/
--rw-r--r--   0 runner    (1001) docker     (121)     2255 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/default_footer.html
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/default_footer.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/message.html
--rw-r--r--   0 runner    (1001) docker     (121)      374 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/message.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/message_subject.txt
--rw-r--r--   0 runner    (1001) docker     (121)      624 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/subscribe.html
--rw-r--r--   0 runner    (1001) docker     (121)      424 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/subscribe.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/subscribe_subject.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.034248 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/thumbnail/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/thumbnail/easy_thumbnails.html
--rw-r--r--   0 runner    (1001) docker     (121)      176 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/thumbnail/sorl_thumbnail.html
--rw-r--r--   0 runner    (1001) docker     (121)      633 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/unsubscribe.html
--rw-r--r--   0 runner    (1001) docker     (121)      430 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/unsubscribe.txt
--rw-r--r--   0 runner    (1001) docker     (121)       77 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/unsubscribe_subject.txt
--rw-r--r--   0 runner    (1001) docker     (121)      656 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/update.html
--rw-r--r--   0 runner    (1001) docker     (121)      447 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/update.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/update_subject.txt
--rw-r--r--   0 runner    (1001) docker     (121)      891 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/newsletter_detail.html
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/newsletter_list.html
--rw-r--r--   0 runner    (1001) docker     (121)      508 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/submission_archive.html
--rw-r--r--   0 runner    (1001) docker     (121)      540 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/subscription_activate.html
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/subscription_subscribe.html
--rw-r--r--   0 runner    (1001) docker     (121)      390 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/subscription_subscribe_activated.html
--rw-r--r--   0 runner    (1001) docker     (121)      462 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/subscription_subscribe_email_sent.html
--rw-r--r--   0 runner    (1001) docker     (121)      695 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/subscription_subscribe_user.html
--rw-r--r--   0 runner    (1001) docker     (121)     1008 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/subscription_unsubscribe.html
--rw-r--r--   0 runner    (1001) docker     (121)      380 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/subscription_unsubscribe_activated.html
--rw-r--r--   0 runner    (1001) docker     (121)      430 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/subscription_unsubscribe_email_sent.html
--rw-r--r--   0 runner    (1001) docker     (121)      709 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/subscription_unsubscribe_user.html
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/subscription_update.html
--rw-r--r--   0 runner    (1001) docker     (121)      388 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/subscription_update_activated.html
--rw-r--r--   0 runner    (1001) docker     (121)      448 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/subscription_update_email_sent.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-30 08:49:02.034248 django-oscar-newsletter-0.8.8/newsletter/templates/widget/
--rwxr-xr-x   0 runner    (1001) docker     (121)      372 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/templates/widget/image.html
--rw-r--r--   0 runner    (1001) docker     (121)     2795 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1011 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      640 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)    19110 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/newsletter/views.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-30 08:49:02.034248 django-oscar-newsletter-0.8.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2585 2021-10-30 08:48:47.000000 django-oscar-newsletter-0.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.954638 django-oscar-newsletter-0.8.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      594 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      926 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (121)    34523 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-11-02 22:27:19.954638 django-oscar-newsletter-0.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2894 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2021-11-02 22:27:12.000000 django-oscar-newsletter-0.8.9/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.926638 django-oscar-newsletter-0.8.9/django_oscar_newsletter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-11-02 22:27:19.000000 django-oscar-newsletter-0.8.9/django_oscar_newsletter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7095 2021-11-02 22:27:19.000000 django-oscar-newsletter-0.8.9/django_oscar_newsletter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-02 22:27:19.000000 django-oscar-newsletter-0.8.9/django_oscar_newsletter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2021-11-02 22:27:19.000000 django-oscar-newsletter-0.8.9/django_oscar_newsletter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-11-02 22:27:19.000000 django-oscar-newsletter-0.8.9/django_oscar_newsletter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.926638 django-oscar-newsletter-0.8.9/newsletter/
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.926638 django-oscar-newsletter-0.8.9/newsletter/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (121)      543 2021-11-02 22:27:19.000000 django-oscar-newsletter-0.8.9/newsletter/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.926638 django-oscar-newsletter-0.8.9/newsletter/addressimport/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/addressimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9581 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/addressimport/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19569 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6065 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/admin_forms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1690 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/admin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/converters.py
+-rw-r--r--   0 runner    (1001) docker     (121)      847 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4455 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.930638 django-oscar-newsletter-0.8.9/newsletter/generator/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      743 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/generator/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      993 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/generator/forms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1167 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/generator/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1789 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/generator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      999 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/generator/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.930638 django-oscar-newsletter-0.8.9/newsletter/jobs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/jobs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.930638 django-oscar-newsletter-0.8.9/newsletter/jobs/daily/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/jobs/daily/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.930638 django-oscar-newsletter-0.8.9/newsletter/jobs/hourly/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/jobs/hourly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      421 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/jobs/hourly/submit.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.930638 django-oscar-newsletter-0.8.9/newsletter/jobs/monthly/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/jobs/monthly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.930638 django-oscar-newsletter-0.8.9/newsletter/jobs/weekly/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/jobs/weekly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.922638 django-oscar-newsletter-0.8.9/newsletter/locale/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.914638 django-oscar-newsletter-0.8.9/newsletter/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.930638 django-oscar-newsletter-0.8.9/newsletter/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    15804 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    27679 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      916 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1256 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/ar/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.914638 django-oscar-newsletter-0.8.9/newsletter/locale/cs_CZ/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.930638 django-oscar-newsletter-0.8.9/newsletter/locale/cs_CZ/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    15108 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/cs_CZ/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    26457 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/cs_CZ/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      903 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/cs_CZ/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1220 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/cs_CZ/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.914638 django-oscar-newsletter-0.8.9/newsletter/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.930638 django-oscar-newsletter-0.8.9/newsletter/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    15968 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    26705 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      765 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/de/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/de/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.914638 django-oscar-newsletter-0.8.9/newsletter/locale/el_GR/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.934638 django-oscar-newsletter-0.8.9/newsletter/locale/el_GR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    17161 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/el_GR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    28994 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/el_GR/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/el_GR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1336 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/el_GR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.918638 django-oscar-newsletter-0.8.9/newsletter/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.934638 django-oscar-newsletter-0.8.9/newsletter/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    15282 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    26219 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      747 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/en/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1016 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/en/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.918638 django-oscar-newsletter-0.8.9/newsletter/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.934638 django-oscar-newsletter-0.8.9/newsletter/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    15820 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    26644 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      792 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/es/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1122 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/es/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.918638 django-oscar-newsletter-0.8.9/newsletter/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.934638 django-oscar-newsletter-0.8.9/newsletter/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    14351 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    26814 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/fa/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      834 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/fa/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1158 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/fa/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.918638 django-oscar-newsletter-0.8.9/newsletter/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.934638 django-oscar-newsletter-0.8.9/newsletter/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16054 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    26804 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      794 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1121 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/fr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.918638 django-oscar-newsletter-0.8.9/newsletter/locale/is_IS/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.938638 django-oscar-newsletter-0.8.9/newsletter/locale/is_IS/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    12225 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/is_IS/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    24447 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/is_IS/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      852 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/is_IS/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1179 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/is_IS/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.918638 django-oscar-newsletter-0.8.9/newsletter/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.938638 django-oscar-newsletter-0.8.9/newsletter/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    12770 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    24993 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      789 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/it/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1119 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/it/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.918638 django-oscar-newsletter-0.8.9/newsletter/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.938638 django-oscar-newsletter-0.8.9/newsletter/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    15898 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    26315 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      769 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/nl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1053 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/nl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.922638 django-oscar-newsletter-0.8.9/newsletter/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.938638 django-oscar-newsletter-0.8.9/newsletter/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16018 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    26867 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      894 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/pl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1206 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/pl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.922638 django-oscar-newsletter-0.8.9/newsletter/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.938638 django-oscar-newsletter-0.8.9/newsletter/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    14335 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    25969 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)      784 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/pt_BR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1117 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/pt_BR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.922638 django-oscar-newsletter-0.8.9/newsletter/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.938638 django-oscar-newsletter-0.8.9/newsletter/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      767 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/pt_PT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1093 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/pt_PT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.922638 django-oscar-newsletter-0.8.9/newsletter/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.942638 django-oscar-newsletter-0.8.9/newsletter/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16113 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (121)    28452 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (121)     1003 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/ru/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.922638 django-oscar-newsletter-0.8.9/newsletter/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.942638 django-oscar-newsletter-0.8.9/newsletter/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/zh_CN/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (121)     1073 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/locale/zh_CN/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.942638 django-oscar-newsletter-0.8.9/newsletter/management/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.942638 django-oscar-newsletter-0.8.9/newsletter/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      958 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/management/commands/submit_newsletter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.942638 django-oscar-newsletter-0.8.9/newsletter/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     7580 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1458 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/migrations/0002_auto_20150416_1555.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1233 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/migrations/0003_auto_20160226_1518.py
+-rw-r--r--   0 runner    (1001) docker     (121)      660 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/migrations/0004_auto_20180407_1043.py
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/migrations/0005_auto_20190918_0122.py
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/migrations/0006_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (121)      593 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/migrations/0007_switch_from_sorl_imagefield.py
+-rw-r--r--   0 runner    (1001) docker     (121)      493 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/migrations/0008_longer_subscription_name.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1993 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/migrations/0009_fork_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24562 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4290 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.922638 django-oscar-newsletter-0.8.9/newsletter/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.922638 django-oscar-newsletter-0.8.9/newsletter/static/newsletter/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.922638 django-oscar-newsletter-0.8.9/newsletter/static/newsletter/admin/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.946638 django-oscar-newsletter-0.8.9/newsletter/static/newsletter/admin/img/
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/static/newsletter/admin/img/icon-no.gif
+-rw-r--r--   0 runner    (1001) docker     (121)      299 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/static/newsletter/admin/img/icon-yes.gif
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/static/newsletter/admin/img/submitting.gif
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/static/newsletter/admin/img/waiting.gif
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.946638 django-oscar-newsletter-0.8.9/newsletter/static/newsletter/admin/js/
+-rw-r--r--   0 runner    (1001) docker     (121)      889 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/static/newsletter/admin/js/submit_interface.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1336 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/static/newsletter/admin/js/subscriber_lookup.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.922638 django-oscar-newsletter-0.8.9/newsletter/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.922638 django-oscar-newsletter-0.8.9/newsletter/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.922638 django-oscar-newsletter-0.8.9/newsletter/templates/admin/newsletter/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.946638 django-oscar-newsletter-0.8.9/newsletter/templates/admin/newsletter/message/
+-rw-r--r--   0 runner    (1001) docker     (121)      407 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/admin/newsletter/message/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1443 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/admin/newsletter/message/preview.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.946638 django-oscar-newsletter-0.8.9/newsletter/templates/admin/newsletter/submission/
+-rw-r--r--   0 runner    (1001) docker     (121)      909 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/admin/newsletter/submission/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.946638 django-oscar-newsletter-0.8.9/newsletter/templates/admin/newsletter/subscription/
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/admin/newsletter/subscription/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1017 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/admin/newsletter/subscription/confirmimportform.html
+-rw-r--r--   0 runner    (1001) docker     (121)      938 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/admin/newsletter/subscription/importform.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.950638 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/common.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.950638 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/
+-rw-r--r--   0 runner    (1001) docker     (121)     2357 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/default_footer.html
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/default_footer.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1971 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/message.html
+-rw-r--r--   0 runner    (1001) docker     (121)      374 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/message.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/message_subject.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/subscribe.html
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/subscribe.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/subscribe_subject.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.950638 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/thumbnail/
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/thumbnail/easy_thumbnails.html
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/thumbnail/sorl_thumbnail.html
+-rw-r--r--   0 runner    (1001) docker     (121)      633 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/unsubscribe.html
+-rw-r--r--   0 runner    (1001) docker     (121)      430 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/unsubscribe.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/unsubscribe_subject.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/update.html
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/update.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/update_subject.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      891 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/newsletter_detail.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/newsletter_list.html
+-rw-r--r--   0 runner    (1001) docker     (121)      508 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/submission_archive.html
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/subscription_activate.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1002 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/subscription_subscribe.html
+-rw-r--r--   0 runner    (1001) docker     (121)      390 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/subscription_subscribe_activated.html
+-rw-r--r--   0 runner    (1001) docker     (121)      462 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/subscription_subscribe_email_sent.html
+-rw-r--r--   0 runner    (1001) docker     (121)      695 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/subscription_subscribe_user.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1008 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/subscription_unsubscribe.html
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/subscription_unsubscribe_activated.html
+-rw-r--r--   0 runner    (1001) docker     (121)      430 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/subscription_unsubscribe_email_sent.html
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/subscription_unsubscribe_user.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1006 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/subscription_update.html
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/subscription_update_activated.html
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/subscription_update_email_sent.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-02 22:27:19.954638 django-oscar-newsletter-0.8.9/newsletter/templates/widget/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      372 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/templates/widget/image.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2795 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1011 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      640 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19110 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/newsletter/views.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-02 22:27:19.954638 django-oscar-newsletter-0.8.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2585 2021-11-02 22:27:09.000000 django-oscar-newsletter-0.8.9/setup.py
```

### Comparing `django-oscar-newsletter-0.8.8/AUTHORS.rst` & `django-oscar-newsletter-0.8.9/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/COPYRIGHT` & `django-oscar-newsletter-0.8.9/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/LICENSE.txt` & `django-oscar-newsletter-0.8.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/PKG-INFO` & `django-oscar-newsletter-0.8.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscar-newsletter
-Version: 0.8.8
+Version: 0.8.9
 Summary: Django app for managing multiple mass-mailing lists with both plaintext as well as HTML templates (and pluggable WYSIWYG editors for messages), images and a smart queueing system all right from the admin interface.
 Home-page: https://github.com/snake-soft/django-oscar-newsletter
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
```

### Comparing `django-oscar-newsletter-0.8.8/README.rst` & `django-oscar-newsletter-0.8.9/README.rst`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/django_oscar_newsletter.egg-info/PKG-INFO` & `django-oscar-newsletter-0.8.9/django_oscar_newsletter.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscar-newsletter
-Version: 0.8.8
+Version: 0.8.9
 Summary: Django app for managing multiple mass-mailing lists with both plaintext as well as HTML templates (and pluggable WYSIWYG editors for messages), images and a smart queueing system all right from the admin interface.
 Home-page: https://github.com/snake-soft/django-oscar-newsletter
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
```

### Comparing `django-oscar-newsletter-0.8.8/django_oscar_newsletter.egg-info/SOURCES.txt` & `django-oscar-newsletter-0.8.9/django_oscar_newsletter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/__pycache__/__init__.cpython-310.pyc` & `django-oscar-newsletter-0.8.9/newsletter/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Oct 30 08:48:47 2021 UTC, .py size: 266 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 ef06 7d61 0a01 0000  o.........}a....
+00000000: 6f0d 0d0a 0000 0000 3dbb 8161 0a01 0000  o.......=..a....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 8400 5a03 6503 8300 5a04  ..d.d...Z.e...Z.
 00000050: 6401 5300 2905 e900 0000 004e 2901 da04  d.S.)......N)...
 00000060: 5061 7468 6300 0000 0000 0000 0000 0000  Pathc...........
 00000070: 0002 0000 0008 0000 0043 0000 0073 5e00  .........C...s^.
```

### Comparing `django-oscar-newsletter-0.8.8/newsletter/addressimport/parsers.py` & `django-oscar-newsletter-0.8.9/newsletter/addressimport/parsers.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/admin.py` & `django-oscar-newsletter-0.8.9/newsletter/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 }
 
 
 class NewsletterAdmin(admin.ModelAdmin):
     list_display = (
         'title', 'admin_subscriptions', 'admin_messages', 'admin_submissions'
     )
-    fields = ('title', 'slug', 'email', 'sender', 'visible', 'send_html',
+    fields = ('title', 'slug', 'email', 'sender', 'visible',
               'footer_template_html', 'footer_template_text')
     prepopulated_fields = {'slug': ('title',)}
 
     """ List extensions """
     def _admin_url(self, obj, model, text):
         url = reverse('admin:%s_%s_changelist' %
                       (model._meta.app_label, model._meta.model_name),
@@ -108,15 +108,15 @@
     admin_newsletter.short_description = _('newsletter')
 
 
 class SubmissionAdmin(NewsletterAdminLinkMixin, ExtendibleModelAdminMixin,
                       admin.ModelAdmin):
     form = SubmissionAdminForm
     list_display = (
-        'admin_message', 'admin_newsletter', 'admin_publish_date', 'publish',
+        'admin_message', 'admin_newsletter', 'admin_publish_date', #'publish',
         'admin_status_text', 'admin_status'
     )
     date_hierarchy = 'publish_date'
     list_filter = ('newsletter', 'publish', 'sent')
     save_as = True
     filter_horizontal = ('subscriptions',)
 
@@ -241,23 +241,26 @@
 
 BaseArticleInline = type('BaseArticleInline', ArticleInlineClassTuple, {})
 
 class ArticleInline(BaseArticleInline):
     model = Article
     extra = 0
     formset = ArticleFormSet
+    fields = ('image', 'url', 'sortorder')
+    '''
     fieldsets = (
         (_('Optional'), {
             'fields': ('sortorder', 'title', 'text'),
             'classes': ('collapse', 'mb-5')
         }),
         (None, {
             'fields': ('image', 'url')
         }),
     )
+    '''
 
 
     # Perform any formfield overrides depending on specified settings
     formfield_overrides = {}
 
     if newsletter_settings.RICHTEXT_WIDGET:
         formfield_overrides[models.TextField] = {
```

### Comparing `django-oscar-newsletter-0.8.8/newsletter/admin_forms.py` & `django-oscar-newsletter-0.8.9/newsletter/admin_forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,10 +175,12 @@
         super().__init__(*args, **kwargs)
 
         assert self.instance
         next_sortorder = self.instance.get_next_article_sortorder()
         for index, form in enumerate(self.extra_forms):
             form.initial['sortorder'] = next_sortorder + index * 10
 
+        '''
         for form in self.forms:
             form.fields['text'].required = False
             form.fields['title'].required = False
+        '''
```

### Comparing `django-oscar-newsletter-0.8.8/newsletter/admin_utils.py` & `django-oscar-newsletter-0.8.9/newsletter/admin_utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/fields.py` & `django-oscar-newsletter-0.8.9/newsletter/fields.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/forms.py` & `django-oscar-newsletter-0.8.9/newsletter/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/generator/admin.py` & `django-oscar-newsletter-0.8.9/newsletter/generator/admin.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/generator/forms.py` & `django-oscar-newsletter-0.8.9/newsletter/generator/forms.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/generator/models.py` & `django-oscar-newsletter-0.8.9/newsletter/generator/models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/generator/utils.py` & `django-oscar-newsletter-0.8.9/newsletter/generator/utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/generator/views.py` & `django-oscar-newsletter-0.8.9/newsletter/generator/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/ar/LC_MESSAGES/django.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/ar/LC_MESSAGES/django.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/ar/LC_MESSAGES/djangojs.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/ar/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/ar/LC_MESSAGES/djangojs.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/cs_CZ/LC_MESSAGES/django.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/cs_CZ/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/cs_CZ/LC_MESSAGES/django.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/cs_CZ/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/cs_CZ/LC_MESSAGES/djangojs.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/cs_CZ/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/cs_CZ/LC_MESSAGES/djangojs.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/cs_CZ/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/de/LC_MESSAGES/django.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/de/LC_MESSAGES/django.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/de/LC_MESSAGES/djangojs.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/de/LC_MESSAGES/djangojs.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/el_GR/LC_MESSAGES/django.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/el_GR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/el_GR/LC_MESSAGES/django.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/el_GR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/el_GR/LC_MESSAGES/djangojs.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/el_GR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/el_GR/LC_MESSAGES/djangojs.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/el_GR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/en/LC_MESSAGES/django.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/en/LC_MESSAGES/django.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/en/LC_MESSAGES/djangojs.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/en/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/en/LC_MESSAGES/djangojs.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/es/LC_MESSAGES/django.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/es/LC_MESSAGES/django.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/es/LC_MESSAGES/djangojs.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/es/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/es/LC_MESSAGES/djangojs.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/fa/LC_MESSAGES/django.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/fa/LC_MESSAGES/django.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/fa/LC_MESSAGES/djangojs.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/fa/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/fa/LC_MESSAGES/djangojs.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/fa/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/fr/LC_MESSAGES/django.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/fr/LC_MESSAGES/django.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/fr/LC_MESSAGES/djangojs.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/fr/LC_MESSAGES/djangojs.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/is_IS/LC_MESSAGES/django.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/is_IS/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/is_IS/LC_MESSAGES/django.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/is_IS/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/is_IS/LC_MESSAGES/djangojs.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/is_IS/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/is_IS/LC_MESSAGES/djangojs.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/is_IS/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/it/LC_MESSAGES/django.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/it/LC_MESSAGES/django.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/it/LC_MESSAGES/djangojs.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/it/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/it/LC_MESSAGES/djangojs.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/it/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/nl/LC_MESSAGES/django.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/nl/LC_MESSAGES/django.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/nl/LC_MESSAGES/djangojs.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/nl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/nl/LC_MESSAGES/djangojs.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/nl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/pl/LC_MESSAGES/django.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/pl/LC_MESSAGES/django.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/pl/LC_MESSAGES/djangojs.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/pl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/pl/LC_MESSAGES/djangojs.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/pl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/pt_BR/LC_MESSAGES/django.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/pt_BR/LC_MESSAGES/django.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/pt_BR/LC_MESSAGES/djangojs.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/pt_PT/LC_MESSAGES/djangojs.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/pt_PT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/pt_PT/LC_MESSAGES/djangojs.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/pt_PT/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/ru/LC_MESSAGES/django.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/ru/LC_MESSAGES/django.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/ru/LC_MESSAGES/djangojs.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/ru/LC_MESSAGES/djangojs.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/zh_CN/LC_MESSAGES/djangojs.mo` & `django-oscar-newsletter-0.8.9/newsletter/locale/zh_CN/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/locale/zh_CN/LC_MESSAGES/djangojs.po` & `django-oscar-newsletter-0.8.9/newsletter/locale/zh_CN/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/management/commands/submit_newsletter.py` & `django-oscar-newsletter-0.8.9/newsletter/management/commands/submit_newsletter.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/migrations/0001_initial.py` & `django-oscar-newsletter-0.8.9/newsletter/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/migrations/0002_auto_20150416_1555.py` & `django-oscar-newsletter-0.8.9/newsletter/migrations/0002_auto_20150416_1555.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/migrations/0003_auto_20160226_1518.py` & `django-oscar-newsletter-0.8.9/newsletter/migrations/0003_auto_20160226_1518.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/migrations/0004_auto_20180407_1043.py` & `django-oscar-newsletter-0.8.9/newsletter/migrations/0004_auto_20180407_1043.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/migrations/0005_auto_20190918_0122.py` & `django-oscar-newsletter-0.8.9/newsletter/migrations/0005_auto_20190918_0122.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/migrations/0006_attachment.py` & `django-oscar-newsletter-0.8.9/newsletter/migrations/0006_attachment.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/migrations/0007_switch_from_sorl_imagefield.py` & `django-oscar-newsletter-0.8.9/newsletter/migrations/0007_switch_from_sorl_imagefield.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/migrations/0009_fork_initial.py` & `django-oscar-newsletter-0.8.9/newsletter/migrations/0009_fork_initial.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/models.py` & `django-oscar-newsletter-0.8.9/newsletter/models.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/settings.py` & `django-oscar-newsletter-0.8.9/newsletter/settings.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/static/newsletter/admin/img/submitting.gif` & `django-oscar-newsletter-0.8.9/newsletter/static/newsletter/admin/img/submitting.gif`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/static/newsletter/admin/js/submit_interface.js` & `django-oscar-newsletter-0.8.9/newsletter/static/newsletter/admin/js/submit_interface.js`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/static/newsletter/admin/js/subscriber_lookup.js` & `django-oscar-newsletter-0.8.9/newsletter/static/newsletter/admin/js/subscriber_lookup.js`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/templates/admin/newsletter/message/preview.html` & `django-oscar-newsletter-0.8.9/newsletter/templates/admin/newsletter/message/preview.html`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/templates/admin/newsletter/submission/change_form.html` & `django-oscar-newsletter-0.8.9/newsletter/templates/admin/newsletter/submission/change_form.html`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/templates/admin/newsletter/subscription/confirmimportform.html` & `django-oscar-newsletter-0.8.9/newsletter/templates/admin/newsletter/subscription/confirmimportform.html`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/templates/admin/newsletter/subscription/importform.html` & `django-oscar-newsletter-0.8.9/newsletter/templates/admin/newsletter/subscription/importform.html`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/default_footer.html` & `django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/default_footer.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 {% load thumbnail i18n %}
 
 <table class="row" width="100%" cellspacing="0" cellpadding="0">
 	<tbody>
         <tr>
             <td class="wrapper last" valign="top">
-                <table class="twelve columns" width="100%" cellspacing="0" cellpadding="0">
+              <table class="twelve columns" width="100%" cellspacing="0" cellpadding="0">
                 <tbody>
                     <tr>
                         <td style="padding:5px" class="text" valign="top">
                             <p>* Angebote gültig für diesen Monat</p>
                             <p>* Solange der Vorrat reicht&nbsp;</p>
                         </td>
                     </tr>
                 </tbody>
-                </table>
+              </table>
             </td>
         </tr>
         <tr>
             <td height="2px"align="center" style="padding: 20px; background: {{ CONFIG.color_1 }};"></td>
         </tr>
         <tr>
-            <td height="2px" bgcolor="{{ CONFIG.color_background }}" align="center">
+            <td style="background-color:white;" height="2px" bgcolor="{{ CONFIG.color_background }}" align="center">
                 <a href="{{ BASE_URL }}">
                   <img src="{{ BASE_URL }}{% thumbnail CONFIG.logo 400x120 crop %}" alt="logo" data-unique-identifier="">
                 </a>
             </td>
         </tr>
         <tr>
-        <td style="color: #000; background: {{ CONFIG.color_1 }}; font-size: 24px; padding: 20px 0;" align="center">
+        <td style="color: #000; background-color:{{ CONFIG.color_1 }}; font-size: 24px; padding: 20px 0;" align="center">
           <p>
             <strong>Preise gelten nur bei online Bestellung!</strong>
-            <br> Infos unter Tel.: {{ CONFIG.company_support_phone }}
           </p>
         </td>
         </tr>
         <tr>
             <td style="color: #000; background: {{ CONFIG.color_1 }}; font-size: 13px; padding-bottom: 10px;" align="center">
-              {{ CONFIG.company_name }} | {{ CONFIG.company_street }} | {{ CONFIG.company_postcode }} {{ CONFIG.company_city }} <br> Telefon: {{ CONFIG.company_support_phone }}
-              <br> <a href="{{ BASE_URL }}{{ impressum_url }}">Impressum</a> | <a href="{{ BASE_URL }}{{ delivery_times_url }}">Liefergebiete</a></td>
+              {{ CONFIG.company_name }} | {{ CONFIG.company_street }} | {{ CONFIG.company_postcode }} {{ CONFIG.company_city }} <br> Telefon: <a href="tel:{{ CONFIG.company_support_phone }}">{{ CONFIG.company_support_phone }}</a> | E-Mail: <a href="mailto:{{ CONFIG.company_support_email }}">{{ CONFIG.company_support_email }}</a><br> <a href="{{ BASE_URL }}{{ impressum_url }}">Impressum</a> | <a href="{{ BASE_URL }}{{ delivery_times_url }}">Liefergebiete</a></td>
         </tr>
         <tr>
             <td style="color: #333; font-size: 10px; padding: 5px;" align="center">Sie möchten unseren Newsletter nicht länger erhalten.&nbsp; <!--#link#--><a href="{{ BASE_URL }}{% url 'newsletter_unsubscribe_request' newsletter.slug %}">{% trans "Unsubscribe" %}</a><!--#/link#--></td>
         </tr>
     </tbody>
 </table>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% load thumbnail i18n %}
 * Angebote gÃ¼ltig fÃ¼r diesen Monat
 * Solange der Vorrat reicht 
                                                           [logo]
-                             Preise gelten nur bei online Bestellung!
-                        Infos unter Tel.: {{ CONFIG.company_support_phone }}
+                                 Preise gelten nur bei online Bestellung!
 {{ CONFIG.company_name }} | {{ CONFIG.company_street }} | {{ CONFIG.company_postcode
                            }} {{ CONFIG.company_city }}
-                    Telefon: {{ CONFIG.company_support_phone }}
+              Telefon: {{_CONFIG.company_support_phone_}} | E-Mail: {
+                         {_CONFIG.company_support_email_}}
                              Impressum | Liefergebiete
  Sie mÃ¶chten unseren Newsletter nicht lÃ¤nger erhalten.  {%_trans_"Unsubscribe"_%}
```

### Comparing `django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/message.html` & `django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/message.html`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,17 @@
   <title>{{ newsletter.title }}: {{ message.title }}</title>
   <style>
     @import url(http://fonts.googleapis.com/css?family=Roboto);
     /* The rest of your CSS here */
     *{ font-family: Roboto, Arial, sans-serif;}
   </style>
 </head>
-<body>
+<body style="margin:0;">
+  <div style="width:100%;background-color:{{ CONFIG.color_1 }};height:25px;"></div>
+  <div style="width:100%;background-color:#f9f8f8;height:5px;"></div>
   <div dir="ltr">
     <center>
       <table cellspacing=20>
         <tbody>
           {% for article in message.articles.all %}
             <tr>
               <td valign="top" align="center">
```

### Comparing `django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/subscribe.html` & `django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/subscribe.html`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/unsubscribe.html` & `django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/unsubscribe.html`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/message/update.html` & `django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/message/update.html`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/newsletter_detail.html` & `django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/newsletter_detail.html`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/newsletter_list.html` & `django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/newsletter_list.html`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/subscription_activate.html` & `django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/subscription_activate.html`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/subscription_subscribe.html` & `django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/subscription_subscribe.html`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/subscription_subscribe_user.html` & `django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/subscription_subscribe_user.html`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/subscription_unsubscribe.html` & `django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/subscription_unsubscribe.html`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/subscription_unsubscribe_user.html` & `django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/subscription_unsubscribe_user.html`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/templates/newsletter/subscription_update.html` & `django-oscar-newsletter-0.8.9/newsletter/templates/newsletter/subscription_update.html`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/urls.py` & `django-oscar-newsletter-0.8.9/newsletter/urls.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/utils.py` & `django-oscar-newsletter-0.8.9/newsletter/utils.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/validators.py` & `django-oscar-newsletter-0.8.9/newsletter/validators.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/newsletter/views.py` & `django-oscar-newsletter-0.8.9/newsletter/views.py`

 * *Files identical despite different names*

### Comparing `django-oscar-newsletter-0.8.8/setup.py` & `django-oscar-newsletter-0.8.9/setup.py`

 * *Files identical despite different names*

