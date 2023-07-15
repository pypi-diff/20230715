# Comparing `tmp/lolcatt-0.1.3.tar.gz` & `tmp/lolcatt-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lolcatt-0.1.3.tar", last modified: Sat Jul  8 19:44:58 2023, max compression
+gzip compressed data, was "lolcatt-0.1.4.tar", last modified: Sat Jul 15 14:32:32 2023, max compression
```

## Comparing `lolcatt-0.1.3.tar` & `lolcatt-0.1.4.tar`

### file list

```diff
@@ -1,63 +1,64 @@
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.191541 lolcatt-0.1.3/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1074 2023-06-30 16:54:52.000000 lolcatt-0.1.3/LICENSE
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      239 2023-06-30 20:26:17.000000 lolcatt-0.1.3/MANIFEST.in
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1987 2023-07-08 19:44:58.191541 lolcatt-0.1.3/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1308 2023-07-07 17:09:03.000000 lolcatt-0.1.3/README.rst
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.135541 lolcatt-0.1.3/docs/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      608 2023-06-30 16:54:52.000000 lolcatt-0.1.3/docs/Makefile
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.075541 lolcatt-0.1.3/docs/_build/
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.075541 lolcatt-0.1.3/docs/_build/html/
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.151541 lolcatt-0.1.3/docs/_build/html/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    14813 2023-07-04 00:19:31.000000 lolcatt-0.1.3/docs/_build/html/_static/basic.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.1.3/docs/_build/html/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      286 2023-05-12 22:36:26.000000 lolcatt-0.1.3/docs/_build/html/_static/file.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.1.3/docs/_build/html/_static/minus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4208 2023-07-04 00:19:31.000000 lolcatt-0.1.3/docs/_build/html/_static/nature.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.1.3/docs/_build/html/_static/plus.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4956 2023-07-04 00:19:31.000000 lolcatt-0.1.3/docs/_build/html/_static/pygments.css
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.159541 lolcatt-0.1.3/docs/_static/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.1.3/docs/_static/custom.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    17073 2023-07-07 17:09:03.000000 lolcatt-0.1.3/docs/_static/screenshot.png
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4983 2023-06-30 21:18:35.000000 lolcatt-0.1.3/docs/conf.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      264 2023-06-30 16:54:52.000000 lolcatt-0.1.3/docs/index.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1138 2023-06-30 16:54:52.000000 lolcatt-0.1.3/docs/installation.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      346 2023-07-07 17:09:03.000000 lolcatt-0.1.3/docs/lolcatt.casting.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      517 2023-07-07 17:09:03.000000 lolcatt-0.1.3/docs/lolcatt.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1232 2023-07-07 17:09:03.000000 lolcatt-0.1.3/docs/lolcatt.ui.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      331 2023-07-07 17:09:03.000000 lolcatt-0.1.3/docs/lolcatt.utils.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      805 2023-06-30 16:54:52.000000 lolcatt-0.1.3/docs/make.bat
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       58 2023-07-04 00:19:25.000000 lolcatt-0.1.3/docs/modules.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       27 2023-06-30 16:54:52.000000 lolcatt-0.1.3/docs/readme.rst
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       69 2023-06-30 16:54:52.000000 lolcatt-0.1.3/docs/usage.rst
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.183541 lolcatt-0.1.3/lolcatt/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      125 2023-07-08 19:38:10.000000 lolcatt-0.1.3/lolcatt/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1206 2023-07-08 19:31:59.000000 lolcatt-0.1.3/lolcatt/app.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.187541 lolcatt-0.1.3/lolcatt/casting/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.1.3/lolcatt/casting/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     5421 2023-07-08 19:31:59.000000 lolcatt-0.1.3/lolcatt/casting/caster.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1079 2023-07-08 19:35:39.000000 lolcatt-0.1.3/lolcatt/cli.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.191541 lolcatt-0.1.3/lolcatt/ui/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.1.3/lolcatt/ui/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1442 2023-07-08 19:31:59.000000 lolcatt-0.1.3/lolcatt/ui/lolcatt.css
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3492 2023-07-07 17:09:03.000000 lolcatt-0.1.3/lolcatt/ui/lolcatt_controls.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1265 2023-07-07 17:09:03.000000 lolcatt-0.1.3/lolcatt/ui/lolcatt_device_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1561 2023-07-08 19:31:59.000000 lolcatt-0.1.3/lolcatt/ui/lolcatt_playback_info.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2368 2023-07-07 17:09:03.000000 lolcatt-0.1.3/lolcatt/ui/lolcatt_progress.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      746 2023-07-08 19:31:59.000000 lolcatt-0.1.3/lolcatt/ui/lolcatt_url_input.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.191541 lolcatt-0.1.3/lolcatt/utils/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-07 17:09:03.000000 lolcatt-0.1.3/lolcatt/utils/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1472 2023-07-07 17:09:03.000000 lolcatt-0.1.3/lolcatt/utils/utils.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.187541 lolcatt-0.1.3/lolcatt.egg-info/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1987 2023-07-08 19:44:57.000000 lolcatt-0.1.3/lolcatt.egg-info/PKG-INFO
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1196 2023-07-08 19:44:58.000000 lolcatt-0.1.3/lolcatt.egg-info/SOURCES.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-08 19:44:57.000000 lolcatt-0.1.3/lolcatt.egg-info/dependency_links.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       45 2023-07-08 19:44:57.000000 lolcatt-0.1.3/lolcatt.egg-info/entry_points.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-07 17:15:34.000000 lolcatt-0.1.3/lolcatt.egg-info/not-zip-safe
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       49 2023-07-08 19:44:57.000000 lolcatt-0.1.3/lolcatt.egg-info/requires.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        8 2023-07-08 19:44:57.000000 lolcatt-0.1.3/lolcatt.egg-info/top_level.txt
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      558 2023-07-08 19:38:10.000000 lolcatt-0.1.3/pyproject.toml
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      354 2023-07-08 19:44:58.191541 lolcatt-0.1.3/setup.cfg
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1556 2023-07-08 19:38:10.000000 lolcatt-0.1.3/setup.py
-drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-08 19:44:58.191541 lolcatt-0.1.3/tests/
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       37 2023-06-30 16:54:52.000000 lolcatt-0.1.3/tests/__init__.py
--rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      211 2023-07-07 17:09:03.000000 lolcatt-0.1.3/tests/test_lolcatt.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.413197 lolcatt-0.1.4/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1074 2023-06-30 16:54:52.000000 lolcatt-0.1.4/LICENSE
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      239 2023-06-30 20:26:17.000000 lolcatt-0.1.4/MANIFEST.in
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1987 2023-07-15 14:32:32.413197 lolcatt-0.1.4/PKG-INFO
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1308 2023-07-07 17:09:03.000000 lolcatt-0.1.4/README.rst
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.409197 lolcatt-0.1.4/docs/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      608 2023-06-30 16:54:52.000000 lolcatt-0.1.4/docs/Makefile
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.405197 lolcatt-0.1.4/docs/_build/
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.405197 lolcatt-0.1.4/docs/_build/html/
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.409197 lolcatt-0.1.4/docs/_build/html/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    14813 2023-07-15 14:28:35.000000 lolcatt-0.1.4/docs/_build/html/_static/basic.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.1.4/docs/_build/html/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      286 2023-05-12 22:36:26.000000 lolcatt-0.1.4/docs/_build/html/_static/file.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.1.4/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4208 2023-07-15 14:28:35.000000 lolcatt-0.1.4/docs/_build/html/_static/nature.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       90 2023-05-12 22:36:26.000000 lolcatt-0.1.4/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4956 2023-07-15 14:28:35.000000 lolcatt-0.1.4/docs/_build/html/_static/pygments.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    17073 2023-07-07 17:09:03.000000 lolcatt-0.1.4/docs/_build/html/_static/screenshot.png
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.409197 lolcatt-0.1.4/docs/_static/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       84 2023-06-30 16:54:52.000000 lolcatt-0.1.4/docs/_static/custom.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)    17073 2023-07-07 17:09:03.000000 lolcatt-0.1.4/docs/_static/screenshot.png
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     4983 2023-06-30 21:18:35.000000 lolcatt-0.1.4/docs/conf.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      264 2023-06-30 16:54:52.000000 lolcatt-0.1.4/docs/index.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1138 2023-06-30 16:54:52.000000 lolcatt-0.1.4/docs/installation.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      346 2023-07-07 17:09:03.000000 lolcatt-0.1.4/docs/lolcatt.casting.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      517 2023-07-15 14:28:33.000000 lolcatt-0.1.4/docs/lolcatt.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1232 2023-07-07 17:09:03.000000 lolcatt-0.1.4/docs/lolcatt.ui.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      331 2023-07-07 17:09:03.000000 lolcatt-0.1.4/docs/lolcatt.utils.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      805 2023-06-30 16:54:52.000000 lolcatt-0.1.4/docs/make.bat
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       58 2023-07-15 14:28:33.000000 lolcatt-0.1.4/docs/modules.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       27 2023-06-30 16:54:52.000000 lolcatt-0.1.4/docs/readme.rst
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       69 2023-06-30 16:54:52.000000 lolcatt-0.1.4/docs/usage.rst
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.409197 lolcatt-0.1.4/lolcatt/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      125 2023-07-15 14:30:25.000000 lolcatt-0.1.4/lolcatt/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1288 2023-07-15 14:24:48.000000 lolcatt-0.1.4/lolcatt/app.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.409197 lolcatt-0.1.4/lolcatt/casting/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.1.4/lolcatt/casting/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     5421 2023-07-15 14:12:20.000000 lolcatt-0.1.4/lolcatt/casting/caster.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1079 2023-07-15 14:12:20.000000 lolcatt-0.1.4/lolcatt/cli.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.413197 lolcatt-0.1.4/lolcatt/ui/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-03 23:40:52.000000 lolcatt-0.1.4/lolcatt/ui/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1480 2023-07-15 14:12:20.000000 lolcatt-0.1.4/lolcatt/ui/lolcatt.css
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     3857 2023-07-15 14:16:18.000000 lolcatt-0.1.4/lolcatt/ui/lolcatt_controls.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1265 2023-07-07 17:09:03.000000 lolcatt-0.1.4/lolcatt/ui/lolcatt_device_info.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1561 2023-07-15 14:12:20.000000 lolcatt-0.1.4/lolcatt/ui/lolcatt_playback_info.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     2646 2023-07-15 14:07:42.000000 lolcatt-0.1.4/lolcatt/ui/lolcatt_progress.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      894 2023-07-15 14:27:50.000000 lolcatt-0.1.4/lolcatt/ui/lolcatt_url_input.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.413197 lolcatt-0.1.4/lolcatt/utils/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        0 2023-07-07 17:09:03.000000 lolcatt-0.1.4/lolcatt/utils/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1472 2023-07-07 17:09:03.000000 lolcatt-0.1.4/lolcatt/utils/utils.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.409197 lolcatt-0.1.4/lolcatt.egg-info/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1987 2023-07-15 14:32:32.000000 lolcatt-0.1.4/lolcatt.egg-info/PKG-INFO
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1236 2023-07-15 14:32:32.000000 lolcatt-0.1.4/lolcatt.egg-info/SOURCES.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-15 14:32:32.000000 lolcatt-0.1.4/lolcatt.egg-info/dependency_links.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       45 2023-07-15 14:32:32.000000 lolcatt-0.1.4/lolcatt.egg-info/entry_points.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        1 2023-07-15 14:32:29.000000 lolcatt-0.1.4/lolcatt.egg-info/not-zip-safe
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       49 2023-07-15 14:32:32.000000 lolcatt-0.1.4/lolcatt.egg-info/requires.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)        8 2023-07-15 14:32:32.000000 lolcatt-0.1.4/lolcatt.egg-info/top_level.txt
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      558 2023-07-15 14:30:25.000000 lolcatt-0.1.4/pyproject.toml
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      354 2023-07-15 14:32:32.413197 lolcatt-0.1.4/setup.cfg
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)     1556 2023-07-15 14:30:25.000000 lolcatt-0.1.4/setup.py
+drwxrwxr-x   0 atav1st   (1000) atav1st   (1000)        0 2023-07-15 14:32:32.413197 lolcatt-0.1.4/tests/
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)       37 2023-06-30 16:54:52.000000 lolcatt-0.1.4/tests/__init__.py
+-rw-rw-r--   0 atav1st   (1000) atav1st   (1000)      211 2023-07-15 14:12:20.000000 lolcatt-0.1.4/tests/test_lolcatt.py
```

### Comparing `lolcatt-0.1.3/LICENSE` & `lolcatt-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.3/PKG-INFO` & `lolcatt-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.1.3
+Version: 0.1.4
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `lolcatt-0.1.3/README.rst` & `lolcatt-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.3/docs/Makefile` & `lolcatt-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.3/docs/_build/html/_static/basic.css` & `lolcatt-0.1.4/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.3/docs/_build/html/_static/nature.css` & `lolcatt-0.1.4/docs/_build/html/_static/nature.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.3/docs/_build/html/_static/pygments.css` & `lolcatt-0.1.4/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.3/docs/_static/screenshot.png` & `lolcatt-0.1.4/docs/_build/html/_static/screenshot.png`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.3/docs/conf.py` & `lolcatt-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.3/docs/installation.rst` & `lolcatt-0.1.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.3/docs/lolcatt.rst` & `lolcatt-0.1.4/docs/lolcatt.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.3/docs/lolcatt.ui.rst` & `lolcatt-0.1.4/docs/lolcatt.ui.rst`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.3/docs/make.bat` & `lolcatt-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.3/lolcatt/app.py` & `lolcatt-0.1.4/lolcatt/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,17 +27,19 @@
 class LolCatt(App):
     """The main application class for lolcatt."""
 
     CSS_PATH = 'ui/lolcatt.css'
 
     def __init__(self, device_name: str = None, *args, **kwargs):
         self.caster = Caster(device_name)
+        self.remote_screen = None
         super().__init__(*args, **kwargs)
 
     def on_mount(self):
-        self.install_screen(RemoteScreen(), name='remote')
+        self.remote_screen = RemoteScreen()
+        self.install_screen(self.remote_screen, name='remote')
         self.push_screen('remote')
 
 
 if __name__ == '__main__':
     app = LolCatt('default')
     app.run()
```

### Comparing `lolcatt-0.1.3/lolcatt/casting/caster.py` & `lolcatt-0.1.4/lolcatt/casting/caster.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.3/lolcatt/cli.py` & `lolcatt-0.1.4/lolcatt/cli.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.3/lolcatt/ui/lolcatt.css` & `lolcatt-0.1.4/lolcatt/ui/lolcatt.css`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 #stop_button {
     border-bottom: tall $error;
 }
 
 Bar > .bar--bar {
     color: $accent;
+    background: $background-lighten-3;
 }
 
 #volume_buttons,
 #playback_buttons,
 #wind_buttons {
     layout: horizontal;
     align: center middle;
@@ -49,19 +50,19 @@
     align: center middle;
     width: 100%;
     margin-left: 1;
     margin-right: 1;
     padding: 0;
     height: 4;
     border: grey;
+    text-style: bold;
 }
 
 #progress_label {
-    margin-left: 10;
-    text-style: bold;
+    margin-left: 7;
 }
 
 #device_info,
 #playback_info {
     height: 3;
     width: 100%;
     align: center middle;
```

### Comparing `lolcatt-0.1.3/lolcatt/ui/lolcatt_controls.py` & `lolcatt-0.1.4/lolcatt/ui/lolcatt_controls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from dataclasses import dataclass
 
 from catt.cli import get_config_as_dict
 from catt.error import CastError
 from textual import on
 from textual.app import DEFAULT_COLORS
 from textual.containers import Container
+from textual.events import Key
 from textual.widgets import Button
 from textual.widgets import Static
 
 
 @dataclass
 class ControlsConfig:
     ffwd_secs: int = 30
@@ -100,7 +101,19 @@
 
     @on(Button.Pressed, "#rewind_button")
     def rewind(self):
         try:
             self.app.caster.get_device().rewind(self._config.rewind_secs)
         except CastError:
             pass
+
+    def on_key(self, event: Key) -> None:
+        if event.key == 'space':
+            self.toggle_play_pause()
+        elif event.key == ('q'):
+            self.stop()
+        elif event.key in ('h', 'left'):
+            self.rewind()
+        elif event.key in ('l', 'right'):
+            self.ffwd()
+        else:
+            pass
```

### Comparing `lolcatt-0.1.3/lolcatt/ui/lolcatt_device_info.py` & `lolcatt-0.1.4/lolcatt/ui/lolcatt_device_info.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.3/lolcatt/ui/lolcatt_playback_info.py` & `lolcatt-0.1.4/lolcatt/ui/lolcatt_playback_info.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.3/lolcatt/ui/lolcatt_progress.py` & `lolcatt-0.1.4/lolcatt/ui/lolcatt_progress.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,29 +21,35 @@
         percent_complete = current / duration * 100 if duration else 0.0
         return current, duration, percent_complete
 
     def _format_time(self, seconds: float) -> str:
         if seconds is None:
             return '--:--'
         minutes, seconds = divmod(seconds, 60)
+        hours, minutes = divmod(minutes, 60)
+        if hours:
+            return f'{hours:02.0f}:{minutes:02.0f}:{seconds:02.0f}'
         return f'{minutes:02.0f}:{seconds:02.0f}'
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.pb = ProgressBar(total=100, show_percentage=False, show_eta=False, id='progress_bar')
-        self.pblabel = Label('(00:00/00:00)', id='progress_label')
+        self.pblabel = Label('', id='progress_label')
+        self._needed_width = 16  # FIXME: learn CSS
 
     def update_progress(self) -> int:
         self.current, self.duration, self.percent_complete = self._extract_progress(
             self.app.caster.get_cast_state().cast_info
         )
         self.pb.update(progress=self.percent_complete)
         current_fmt = self._format_time(self.current)
         duration_fmt = self._format_time(self.duration)
-        self.pblabel.update(f'({current_fmt}/{duration_fmt})')
+        upd_str = f'({current_fmt}/{duration_fmt})'
+        padding = ' ' * max(0, (self._needed_width - len(upd_str)))
+        self.pblabel.update(f'{padding}{upd_str}')
 
     def on_mount(self):
         self.update_progress()
         self.set_interval(
             interval=self.app.caster.get_update_interval(), callback=self.update_progress
         )
```

### Comparing `lolcatt-0.1.3/lolcatt/ui/lolcatt_url_input.py` & `lolcatt-0.1.4/lolcatt/ui/lolcatt_url_input.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from textual import on
 from textual.containers import Container
+from textual.events import Key
 from textual.widgets import Input
 from textual.widgets import Static
 
 
 class LolCattUrlInput(Static):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -17,9 +18,13 @@
         if self._input.value:
             self.app.caster.cast(self._input.value)
             self._input.value = ''
 
     def compose(self):
         yield Container(self._input, id='url_input_container')
 
+    def on_key(self, event: Key):
+        if event.key == 'escape':
+            self.app.remote_screen.focus_next()
+
     def on_mount(self):
         self._input.focus()
```

### Comparing `lolcatt-0.1.3/lolcatt/utils/utils.py` & `lolcatt-0.1.4/lolcatt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lolcatt-0.1.3/lolcatt.egg-info/PKG-INFO` & `lolcatt-0.1.4/lolcatt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lolcatt
-Version: 0.1.3
+Version: 0.1.4
 Summary: A TUI wrapper around `catt`.
 Home-page: https://github.com/LokiLuciferase/lolcatt
 Author: Lukas Lüftinger
 Author-email: lukas.lueftinger@outlook.com
 License: MIT license
 Keywords: lolcatt
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `lolcatt-0.1.3/lolcatt.egg-info/SOURCES.txt` & `lolcatt-0.1.4/lolcatt.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 docs/_build/html/_static/basic.css
 docs/_build/html/_static/custom.css
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/nature.css
 docs/_build/html/_static/plus.png
 docs/_build/html/_static/pygments.css
+docs/_build/html/_static/screenshot.png
 docs/_static/custom.css
 docs/_static/screenshot.png
 lolcatt/__init__.py
 lolcatt/app.py
 lolcatt/cli.py
 lolcatt.egg-info/PKG-INFO
 lolcatt.egg-info/SOURCES.txt
```

### Comparing `lolcatt-0.1.3/pyproject.toml` & `lolcatt-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   | buck-out
   | build
   | dist
 )/
 '''
 
 [tool.bumpver]
-current_version = "0.1.3"
+current_version = "0.1.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `lolcatt-0.1.3/setup.py` & `lolcatt-0.1.4/setup.py`

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
-    version='0.1.3',
+    version='0.1.4',
     zip_safe=False,
 )
```

