# Comparing `tmp/lolcatt-0.1.4.tar.gz` & `tmp/lolcatt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lolcatt-0.1.4.tar", last modified: Sat Jul 15 14:32:32 2023, max compression
+gzip compressed data, was "lolcatt-0.1.5.tar", last modified: Sat Jul 15 16:24:39 2023, max compression
```

## Comparing `lolcatt-0.1.4.tar` & `lolcatt-0.1.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.413197 lolcatt-0.1.4/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1074 2023-06-30 16:54:52.000000 lolcatt-0.1.4/LICENSE
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      239 2023-06-30 20:26:17.000000 lolcatt-0.1.4/MANIFEST.in
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1987 2023-07-15 14:32:32.413197 lolcatt-0.1.4/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1308 2023-07-07 17:09:03.000000 lolcatt-0.1.4/README.rst
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.409197 lolcatt-0.1.4/docs/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      608 2023-06-30 16:54:52.000000 lolcatt-0.1.4/docs/Makefile
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.405197 lolcatt-0.1.4/docs/_build/
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.405197 lolcatt-0.1.4/docs/_build/html/
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.409197 lolcatt-0.1.4/docs/_build/html/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    14813 2023-07-15 14:28:35.000000 lolcatt-0.1.4/docs/_build/html/_static/basic.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.1.4/docs/_build/html/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      286 2023-05-12 22:36:26.000000 lolcatt-0.1.4/docs/_build/html/_static/file.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.1.4/docs/_build/html/_static/minus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4208 2023-07-15 14:28:35.000000 lolcatt-0.1.4/docs/_build/html/_static/nature.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.1.4/docs/_build/html/_static/plus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4956 2023-07-15 14:28:35.000000 lolcatt-0.1.4/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    17073 2023-07-07 17:09:03.000000 lolcatt-0.1.4/docs/_build/html/_static/screenshot.png
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.409197 lolcatt-0.1.4/docs/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.1.4/docs/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    17073 2023-07-07 17:09:03.000000 lolcatt-0.1.4/docs/_static/screenshot.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4983 2023-06-30 21:18:35.000000 lolcatt-0.1.4/docs/conf.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      264 2023-06-30 16:54:52.000000 lolcatt-0.1.4/docs/index.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1138 2023-06-30 16:54:52.000000 lolcatt-0.1.4/docs/installation.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      346 2023-07-07 17:09:03.000000 lolcatt-0.1.4/docs/lolcatt.casting.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      517 2023-07-15 14:28:33.000000 lolcatt-0.1.4/docs/lolcatt.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1232 2023-07-07 17:09:03.000000 lolcatt-0.1.4/docs/lolcatt.ui.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      331 2023-07-07 17:09:03.000000 lolcatt-0.1.4/docs/lolcatt.utils.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      805 2023-06-30 16:54:52.000000 lolcatt-0.1.4/docs/make.bat
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       58 2023-07-15 14:28:33.000000 lolcatt-0.1.4/docs/modules.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       27 2023-06-30 16:54:52.000000 lolcatt-0.1.4/docs/readme.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       69 2023-06-30 16:54:52.000000 lolcatt-0.1.4/docs/usage.rst
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.409197 lolcatt-0.1.4/lolcatt/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      125 2023-07-15 14:30:25.000000 lolcatt-0.1.4/lolcatt/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1288 2023-07-15 14:24:48.000000 lolcatt-0.1.4/lolcatt/app.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.409197 lolcatt-0.1.4/lolcatt/casting/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.1.4/lolcatt/casting/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     5421 2023-07-15 14:12:20.000000 lolcatt-0.1.4/lolcatt/casting/caster.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1079 2023-07-15 14:12:20.000000 lolcatt-0.1.4/lolcatt/cli.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.413197 lolcatt-0.1.4/lolcatt/ui/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.1.4/lolcatt/ui/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1480 2023-07-15 14:12:20.000000 lolcatt-0.1.4/lolcatt/ui/lolcatt.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3857 2023-07-15 14:16:18.000000 lolcatt-0.1.4/lolcatt/ui/lolcatt_controls.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1265 2023-07-07 17:09:03.000000 lolcatt-0.1.4/lolcatt/ui/lolcatt_device_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1561 2023-07-15 14:12:20.000000 lolcatt-0.1.4/lolcatt/ui/lolcatt_playback_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2646 2023-07-15 14:07:42.000000 lolcatt-0.1.4/lolcatt/ui/lolcatt_progress.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      894 2023-07-15 14:27:50.000000 lolcatt-0.1.4/lolcatt/ui/lolcatt_url_input.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.413197 lolcatt-0.1.4/lolcatt/utils/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-07 17:09:03.000000 lolcatt-0.1.4/lolcatt/utils/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1472 2023-07-07 17:09:03.000000 lolcatt-0.1.4/lolcatt/utils/utils.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.409197 lolcatt-0.1.4/lolcatt.egg-info/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1987 2023-07-15 14:32:32.000000 lolcatt-0.1.4/lolcatt.egg-info/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1236 2023-07-15 14:32:32.000000 lolcatt-0.1.4/lolcatt.egg-info/SOURCES.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-15 14:32:32.000000 lolcatt-0.1.4/lolcatt.egg-info/dependency_links.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       45 2023-07-15 14:32:32.000000 lolcatt-0.1.4/lolcatt.egg-info/entry_points.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-15 14:32:29.000000 lolcatt-0.1.4/lolcatt.egg-info/not-zip-safe
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       49 2023-07-15 14:32:32.000000 lolcatt-0.1.4/lolcatt.egg-info/requires.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        8 2023-07-15 14:32:32.000000 lolcatt-0.1.4/lolcatt.egg-info/top_level.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      558 2023-07-15 14:30:25.000000 lolcatt-0.1.4/pyproject.toml
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      354 2023-07-15 14:32:32.413197 lolcatt-0.1.4/setup.cfg
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1556 2023-07-15 14:30:25.000000 lolcatt-0.1.4/setup.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.413197 lolcatt-0.1.4/tests/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       37 2023-06-30 16:54:52.000000 lolcatt-0.1.4/tests/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      211 2023-07-15 14:12:20.000000 lolcatt-0.1.4/tests/test_lolcatt.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.580939 lolcatt-0.1.5/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1074 2023-06-30 16:54:52.000000 lolcatt-0.1.5/LICENSE
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      239 2023-06-30 20:26:17.000000 lolcatt-0.1.5/MANIFEST.in
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1987 2023-07-15 16:24:39.580939 lolcatt-0.1.5/PKG-INFO
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1308 2023-07-07 17:09:03.000000 lolcatt-0.1.5/README.rst
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.576939 lolcatt-0.1.5/docs/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      608 2023-06-30 16:54:52.000000 lolcatt-0.1.5/docs/Makefile
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.576939 lolcatt-0.1.5/docs/_build/
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.576939 lolcatt-0.1.5/docs/_build/html/
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.580939 lolcatt-0.1.5/docs/_build/html/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    14813 2023-07-15 14:28:35.000000 lolcatt-0.1.5/docs/_build/html/_static/basic.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.1.5/docs/_build/html/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      286 2023-05-12 22:36:26.000000 lolcatt-0.1.5/docs/_build/html/_static/file.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.1.5/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4208 2023-07-15 14:28:35.000000 lolcatt-0.1.5/docs/_build/html/_static/nature.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.1.5/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4956 2023-07-15 14:28:35.000000 lolcatt-0.1.5/docs/_build/html/_static/pygments.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    17073 2023-07-07 17:09:03.000000 lolcatt-0.1.5/docs/_build/html/_static/screenshot.png
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.580939 lolcatt-0.1.5/docs/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.1.5/docs/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    17073 2023-07-07 17:09:03.000000 lolcatt-0.1.5/docs/_static/screenshot.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4983 2023-06-30 21:18:35.000000 lolcatt-0.1.5/docs/conf.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      264 2023-06-30 16:54:52.000000 lolcatt-0.1.5/docs/index.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1138 2023-06-30 16:54:52.000000 lolcatt-0.1.5/docs/installation.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      346 2023-07-07 17:09:03.000000 lolcatt-0.1.5/docs/lolcatt.casting.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      517 2023-07-15 14:28:33.000000 lolcatt-0.1.5/docs/lolcatt.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1232 2023-07-07 17:09:03.000000 lolcatt-0.1.5/docs/lolcatt.ui.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      331 2023-07-07 17:09:03.000000 lolcatt-0.1.5/docs/lolcatt.utils.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      805 2023-06-30 16:54:52.000000 lolcatt-0.1.5/docs/make.bat
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       58 2023-07-15 14:28:33.000000 lolcatt-0.1.5/docs/modules.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       27 2023-06-30 16:54:52.000000 lolcatt-0.1.5/docs/readme.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       69 2023-06-30 16:54:52.000000 lolcatt-0.1.5/docs/usage.rst
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.580939 lolcatt-0.1.5/lolcatt/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      125 2023-07-15 16:24:08.000000 lolcatt-0.1.5/lolcatt/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1288 2023-07-15 16:19:10.000000 lolcatt-0.1.5/lolcatt/app.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.580939 lolcatt-0.1.5/lolcatt/casting/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.1.5/lolcatt/casting/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     5421 2023-07-15 16:19:10.000000 lolcatt-0.1.5/lolcatt/casting/caster.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1079 2023-07-15 16:19:10.000000 lolcatt-0.1.5/lolcatt/cli.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.580939 lolcatt-0.1.5/lolcatt/ui/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.1.5/lolcatt/ui/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1480 2023-07-15 16:19:10.000000 lolcatt-0.1.5/lolcatt/ui/lolcatt.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3861 2023-07-15 16:19:23.000000 lolcatt-0.1.5/lolcatt/ui/lolcatt_controls.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1265 2023-07-07 17:09:03.000000 lolcatt-0.1.5/lolcatt/ui/lolcatt_device_info.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1561 2023-07-15 16:19:10.000000 lolcatt-0.1.5/lolcatt/ui/lolcatt_playback_info.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2646 2023-07-15 14:07:42.000000 lolcatt-0.1.5/lolcatt/ui/lolcatt_progress.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      894 2023-07-15 16:19:10.000000 lolcatt-0.1.5/lolcatt/ui/lolcatt_url_input.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.580939 lolcatt-0.1.5/lolcatt/utils/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-07 17:09:03.000000 lolcatt-0.1.5/lolcatt/utils/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1472 2023-07-07 17:09:03.000000 lolcatt-0.1.5/lolcatt/utils/utils.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.580939 lolcatt-0.1.5/lolcatt.egg-info/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1987 2023-07-15 16:24:39.000000 lolcatt-0.1.5/lolcatt.egg-info/PKG-INFO
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1236 2023-07-15 16:24:39.000000 lolcatt-0.1.5/lolcatt.egg-info/SOURCES.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-15 16:24:39.000000 lolcatt-0.1.5/lolcatt.egg-info/dependency_links.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       45 2023-07-15 16:24:39.000000 lolcatt-0.1.5/lolcatt.egg-info/entry_points.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-15 16:24:39.000000 lolcatt-0.1.5/lolcatt.egg-info/not-zip-safe
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       49 2023-07-15 16:24:39.000000 lolcatt-0.1.5/lolcatt.egg-info/requires.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        8 2023-07-15 16:24:39.000000 lolcatt-0.1.5/lolcatt.egg-info/top_level.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      558 2023-07-15 16:24:08.000000 lolcatt-0.1.5/pyproject.toml
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      354 2023-07-15 16:24:39.584939 lolcatt-0.1.5/setup.cfg
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1556 2023-07-15 16:24:08.000000 lolcatt-0.1.5/setup.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 16:24:39.580939 lolcatt-0.1.5/tests/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       37 2023-06-30 16:54:52.000000 lolcatt-0.1.5/tests/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      211 2023-07-15 16:19:10.000000 lolcatt-0.1.5/tests/test_lolcatt.py
```

### Comparing `lolcatt-0.1.4/LICENSE` & `lolcatt-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/PKG-INFO` & `lolcatt-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.1.4
+Version: 0.1.5
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `lolcatt-0.1.4/README.rst` & `lolcatt-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/docs/Makefile` & `lolcatt-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/docs/_build/html/_static/basic.css` & `lolcatt-0.1.5/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/docs/_build/html/_static/nature.css` & `lolcatt-0.1.5/docs/_build/html/_static/nature.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/docs/_build/html/_static/pygments.css` & `lolcatt-0.1.5/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/docs/_build/html/_static/screenshot.png` & `lolcatt-0.1.5/docs/_build/html/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/docs/_static/screenshot.png` & `lolcatt-0.1.5/docs/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/docs/conf.py` & `lolcatt-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/docs/installation.rst` & `lolcatt-0.1.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/docs/lolcatt.rst` & `lolcatt-0.1.5/docs/lolcatt.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/docs/lolcatt.ui.rst` & `lolcatt-0.1.5/docs/lolcatt.ui.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/docs/make.bat` & `lolcatt-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/lolcatt/app.py` & `lolcatt-0.1.5/lolcatt/app.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/lolcatt/casting/caster.py` & `lolcatt-0.1.5/lolcatt/casting/caster.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/lolcatt/cli.py` & `lolcatt-0.1.5/lolcatt/cli.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/lolcatt/ui/lolcatt.css` & `lolcatt-0.1.5/lolcatt/ui/lolcatt.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/lolcatt/ui/lolcatt_controls.py` & `lolcatt-0.1.5/lolcatt/ui/lolcatt_controls.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,14 +106,14 @@
         except CastError:
             pass
 
     def on_key(self, event: Key) -> None:
         if event.key == 'space':
             self.toggle_play_pause()
         elif event.key == ('q'):
-            self.stop()
+            self.app.exit()
         elif event.key in ('h', 'left'):
             self.rewind()
         elif event.key in ('l', 'right'):
             self.ffwd()
         else:
             pass
```

### Comparing `lolcatt-0.1.4/lolcatt/ui/lolcatt_device_info.py` & `lolcatt-0.1.5/lolcatt/ui/lolcatt_device_info.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/lolcatt/ui/lolcatt_playback_info.py` & `lolcatt-0.1.5/lolcatt/ui/lolcatt_playback_info.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/lolcatt/ui/lolcatt_progress.py` & `lolcatt-0.1.5/lolcatt/ui/lolcatt_progress.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/lolcatt/ui/lolcatt_url_input.py` & `lolcatt-0.1.5/lolcatt/ui/lolcatt_url_input.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/lolcatt/utils/utils.py` & `lolcatt-0.1.5/lolcatt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/lolcatt.egg-info/PKG-INFO` & `lolcatt-0.1.5/lolcatt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.1.4
+Version: 0.1.5
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `lolcatt-0.1.4/lolcatt.egg-info/SOURCES.txt` & `lolcatt-0.1.5/lolcatt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.4/pyproject.toml` & `lolcatt-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   | buck-out
   | build
   | dist
 )/
 '''
 
 [tool.bumpver]
-current_version = "0.1.4"
+current_version = "0.1.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `lolcatt-0.1.4/setup.py` & `lolcatt-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='lolcatt',
     name='lolcatt',
     packages=find_packages(include=['lolcatt', 'lolcatt.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/LokiLuciferase/lolcatt',
-    version='0.1.4',
+    version='0.1.5',
     zip_safe=False,
 )
```

