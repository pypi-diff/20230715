# Comparing `tmp/pysmartapp-0.3.4.tar.gz` & `tmp/pysmartapp-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmartapp-0.3.4.tar", last modified: Thu Nov 18 03:33:12 2021, max compression
+gzip compressed data, was "pysmartapp-0.3.5.tar", last modified: Sat Jul 15 17:30:04 2023, max compression
```

## Comparing `pysmartapp-0.3.4.tar` & `pysmartapp-0.3.5.tar`

### file list

```diff
@@ -1,28 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 03:33:12.281520 pysmartapp-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-11-18 03:32:52.000000 pysmartapp-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1581 2021-11-18 03:33:12.281520 pysmartapp-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      860 2021-11-18 03:32:52.000000 pysmartapp-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 03:33:12.281520 pysmartapp-0.3.4/pysmartapp/
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2021-11-18 03:32:52.000000 pysmartapp-0.3.4/pysmartapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6340 2021-11-18 03:32:52.000000 pysmartapp-0.3.4/pysmartapp/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      477 2021-11-18 03:32:52.000000 pysmartapp-0.3.4/pysmartapp/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     3244 2021-11-18 03:32:52.000000 pysmartapp-0.3.4/pysmartapp/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (121)      697 2021-11-18 03:32:52.000000 pysmartapp-0.3.4/pysmartapp/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     4814 2021-11-18 03:32:52.000000 pysmartapp-0.3.4/pysmartapp/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2021-11-18 03:32:52.000000 pysmartapp-0.3.4/pysmartapp/install.py
--rw-r--r--   0 runner    (1001) docker     (121)      936 2021-11-18 03:32:52.000000 pysmartapp-0.3.4/pysmartapp/oauthcallback.py
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2021-11-18 03:32:52.000000 pysmartapp-0.3.4/pysmartapp/ping.py
--rw-r--r--   0 runner    (1001) docker     (121)     3547 2021-11-18 03:32:52.000000 pysmartapp-0.3.4/pysmartapp/request.py
--rw-r--r--   0 runner    (1001) docker     (121)     7593 2021-11-18 03:32:52.000000 pysmartapp-0.3.4/pysmartapp/smartapp.py
--rw-r--r--   0 runner    (1001) docker     (121)      696 2021-11-18 03:32:52.000000 pysmartapp-0.3.4/pysmartapp/uninstall.py
--rw-r--r--   0 runner    (1001) docker     (121)      996 2021-11-18 03:32:52.000000 pysmartapp-0.3.4/pysmartapp/update.py
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2021-11-18 03:32:52.000000 pysmartapp-0.3.4/pysmartapp/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 03:33:12.281520 pysmartapp-0.3.4/pysmartapp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1581 2021-11-18 03:33:12.000000 pysmartapp-0.3.4/pysmartapp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      539 2021-11-18 03:33:12.000000 pysmartapp-0.3.4/pysmartapp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-18 03:33:12.000000 pysmartapp-0.3.4/pysmartapp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-18 03:33:12.000000 pysmartapp-0.3.4/pysmartapp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-11-18 03:33:12.000000 pysmartapp-0.3.4/pysmartapp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-11-18 03:33:12.000000 pysmartapp-0.3.4/pysmartapp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-18 03:33:12.281520 pysmartapp-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2021-11-18 03:32:52.000000 pysmartapp-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:30:04.234558 pysmartapp-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-15 17:30:04.234558 pysmartapp-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:30:04.234558 pysmartapp-0.3.5/pysmartapp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/pysmartapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/pysmartapp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/pysmartapp/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/pysmartapp/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/pysmartapp/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/pysmartapp/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/pysmartapp/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/pysmartapp/oauthcallback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/pysmartapp/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/pysmartapp/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/pysmartapp/smartapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/pysmartapp/uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/pysmartapp/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/pysmartapp/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:30:04.234558 pysmartapp-0.3.5/pysmartapp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-15 17:30:04.000000 pysmartapp-0.3.5/pysmartapp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-15 17:30:04.000000 pysmartapp-0.3.5/pysmartapp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 17:30:04.000000 pysmartapp-0.3.5/pysmartapp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 17:30:04.000000 pysmartapp-0.3.5/pysmartapp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-15 17:30:04.000000 pysmartapp-0.3.5/pysmartapp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-15 17:30:04.000000 pysmartapp-0.3.5/pysmartapp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 17:30:04.234558 pysmartapp-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:30:04.234558 pysmartapp-0.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/tests/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/tests/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/tests/test_oauthcallback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/tests/test_ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/tests/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/tests/test_smartapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/tests/test_uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-15 17:29:43.000000 pysmartapp-0.3.5/tests/test_utilities.py
```

### Comparing `pysmartapp-0.3.4/LICENSE` & `pysmartapp-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmartapp-0.3.4/PKG-INFO` & `pysmartapp-0.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: pysmartapp
-Version: 0.3.4
+Version: 0.3.5
 Summary: A python library for building a SmartThings SmartApp
 Home-page: https://github.com/andrewsayre/pysmartapp
 Author: Andrew Sayre
 Author-email: andrew@sayre.net
 License: MIT
 Keywords: smartthings,smartapp
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Home Automation
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pysmartapp
 [![CI Status](https://github.com/andrewsayre/pysmartapp/workflows/CI/badge.svg)](https://github.com/andrewsayre/pysmartapp/actions)
 [![codecov](https://codecov.io/gh/andrewsayre/pysmartapp/branch/master/graph/badge.svg?token=VKPQ25JRAY)](https://codecov.io/gh/andrewsayre/pysmartapp)
 [![image](https://img.shields.io/pypi/v/pysmartapp.svg)](https://pypi.org/project/pysmartapp/)
 [![image](https://img.shields.io/pypi/pyversions/pysmartapp.svg)](https://pypi.org/project/pysmartapp/)
 [![image](https://img.shields.io/pypi/l/pysmartapp.svg)](https://pypi.org/project/pysmartapp/)
 
 A python implementation of the WebHook-based [SmartThings SmartApp](https://smartthings.developer.samsung.com/develop/guides/smartapps/basics.html) that uses asyncio and the dispatcher pattern to notify callbacks (coroutines or functions) of SmartApp lifecycle events.
-
```

### Comparing `pysmartapp-0.3.4/README.md` & `pysmartapp-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pysmartapp-0.3.4/pysmartapp/__init__.py` & `pysmartapp-0.3.5/pysmartapp/__init__.py`

 * *Files identical despite different names*

### Comparing `pysmartapp-0.3.4/pysmartapp/config.py` & `pysmartapp-0.3.5/pysmartapp/config.py`

 * *Files identical despite different names*

### Comparing `pysmartapp-0.3.4/pysmartapp/dispatch.py` & `pysmartapp-0.3.5/pysmartapp/dispatch.py`

 * *Files identical despite different names*

### Comparing `pysmartapp-0.3.4/pysmartapp/errors.py` & `pysmartapp-0.3.5/pysmartapp/errors.py`

 * *Files identical despite different names*

### Comparing `pysmartapp-0.3.4/pysmartapp/event.py` & `pysmartapp-0.3.5/pysmartapp/event.py`

 * *Files identical despite different names*

### Comparing `pysmartapp-0.3.4/pysmartapp/install.py` & `pysmartapp-0.3.5/pysmartapp/install.py`

 * *Files identical despite different names*

### Comparing `pysmartapp-0.3.4/pysmartapp/oauthcallback.py` & `pysmartapp-0.3.5/pysmartapp/oauthcallback.py`

 * *Files identical despite different names*

### Comparing `pysmartapp-0.3.4/pysmartapp/ping.py` & `pysmartapp-0.3.5/pysmartapp/ping.py`

 * *Files identical despite different names*

### Comparing `pysmartapp-0.3.4/pysmartapp/request.py` & `pysmartapp-0.3.5/pysmartapp/request.py`

 * *Files identical despite different names*

### Comparing `pysmartapp-0.3.4/pysmartapp/smartapp.py` & `pysmartapp-0.3.5/pysmartapp/smartapp.py`

 * *Files identical despite different names*

### Comparing `pysmartapp-0.3.4/pysmartapp/uninstall.py` & `pysmartapp-0.3.5/pysmartapp/uninstall.py`

 * *Files identical despite different names*

### Comparing `pysmartapp-0.3.4/pysmartapp/update.py` & `pysmartapp-0.3.5/pysmartapp/update.py`

 * *Files identical despite different names*

### Comparing `pysmartapp-0.3.4/pysmartapp/utilities.py` & `pysmartapp-0.3.5/pysmartapp/utilities.py`

 * *Files identical despite different names*

### Comparing `pysmartapp-0.3.4/pysmartapp.egg-info/PKG-INFO` & `pysmartapp-0.3.5/pysmartapp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: pysmartapp
-Version: 0.3.4
+Version: 0.3.5
 Summary: A python library for building a SmartThings SmartApp
 Home-page: https://github.com/andrewsayre/pysmartapp
 Author: Andrew Sayre
 Author-email: andrew@sayre.net
 License: MIT
 Keywords: smartthings,smartapp
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Home Automation
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pysmartapp
 [![CI Status](https://github.com/andrewsayre/pysmartapp/workflows/CI/badge.svg)](https://github.com/andrewsayre/pysmartapp/actions)
 [![codecov](https://codecov.io/gh/andrewsayre/pysmartapp/branch/master/graph/badge.svg?token=VKPQ25JRAY)](https://codecov.io/gh/andrewsayre/pysmartapp)
 [![image](https://img.shields.io/pypi/v/pysmartapp.svg)](https://pypi.org/project/pysmartapp/)
 [![image](https://img.shields.io/pypi/pyversions/pysmartapp.svg)](https://pypi.org/project/pysmartapp/)
 [![image](https://img.shields.io/pypi/l/pysmartapp.svg)](https://pypi.org/project/pysmartapp/)
 
 A python implementation of the WebHook-based [SmartThings SmartApp](https://smartthings.developer.samsung.com/develop/guides/smartapps/basics.html) that uses asyncio and the dispatcher pattern to notify callbacks (coroutines or functions) of SmartApp lifecycle events.
-
```

### Comparing `pysmartapp-0.3.4/setup.py` & `pysmartapp-0.3.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,10 +30,10 @@
       classifiers=[
           "Development Status :: 4 - Beta",
           "Intended Audience :: Developers",
           "License :: OSI Approved :: MIT License",
           "Operating System :: OS Independent",
           "Topic :: Software Development :: Libraries",
           "Topic :: Home Automation",
-          "Programming Language :: Python :: 3.8",
-          "Programming Language :: Python :: 3.9",
+          "Programming Language :: Python :: 3.10",
+          "Programming Language :: Python :: 3.11",
           ])
```

