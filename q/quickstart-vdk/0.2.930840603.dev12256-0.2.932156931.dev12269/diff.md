# Comparing `tmp/quickstart-vdk-0.2.930840603.dev12256.tar.gz` & `tmp/quickstart-vdk-0.2.932156931.dev12269.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.930840603.dev12256.tar", last modified: Fri Jul 14 04:25:05 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.932156931.dev12269.tar", last modified: Sat Jul 15 04:24:08 2023, max compression
```

## Comparing `quickstart-vdk-0.2.930840603.dev12256.tar` & `quickstart-vdk-0.2.932156931.dev12269.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 04:25:05.720228 quickstart-vdk-0.2.930840603.dev12256/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-07-14 04:25:05.720228 quickstart-vdk-0.2.930840603.dev12256/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-07-14 04:22:16.000000 quickstart-vdk-0.2.930840603.dev12256/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 04:25:05.720228 quickstart-vdk-0.2.930840603.dev12256/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-07-14 04:25:05.000000 quickstart-vdk-0.2.930840603.dev12256/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-07-14 04:25:05.000000 quickstart-vdk-0.2.930840603.dev12256/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 04:25:05.000000 quickstart-vdk-0.2.930840603.dev12256/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-14 04:25:05.000000 quickstart-vdk-0.2.930840603.dev12256/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-14 04:25:05.000000 quickstart-vdk-0.2.930840603.dev12256/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 04:25:05.720228 quickstart-vdk-0.2.930840603.dev12256/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-07-14 04:24:54.000000 quickstart-vdk-0.2.930840603.dev12256/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 04:25:05.720228 quickstart-vdk-0.2.930840603.dev12256/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-07-14 04:22:16.000000 quickstart-vdk-0.2.930840603.dev12256/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 04:24:08.356281 quickstart-vdk-0.2.932156931.dev12269/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-07-15 04:24:08.356281 quickstart-vdk-0.2.932156931.dev12269/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-07-15 04:21:16.000000 quickstart-vdk-0.2.932156931.dev12269/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 04:24:08.352281 quickstart-vdk-0.2.932156931.dev12269/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-07-15 04:24:08.000000 quickstart-vdk-0.2.932156931.dev12269/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-07-15 04:24:08.000000 quickstart-vdk-0.2.932156931.dev12269/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 04:24:08.000000 quickstart-vdk-0.2.932156931.dev12269/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-15 04:24:08.000000 quickstart-vdk-0.2.932156931.dev12269/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-15 04:24:08.000000 quickstart-vdk-0.2.932156931.dev12269/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-15 04:24:08.356281 quickstart-vdk-0.2.932156931.dev12269/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-07-15 04:23:57.000000 quickstart-vdk-0.2.932156931.dev12269/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 04:24:08.352281 quickstart-vdk-0.2.932156931.dev12269/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-07-15 04:21:16.000000 quickstart-vdk-0.2.932156931.dev12269/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.930840603.dev12256/PKG-INFO` & `quickstart-vdk-0.2.932156931.dev12269/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.930840603.dev12256
+Version: 0.2.932156931.dev12269
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.930840603.dev12256/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.932156931.dev12269/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.930840603.dev12256
+Version: 0.2.932156931.dev12269
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.930840603.dev12256/setup.py` & `quickstart-vdk-0.2.932156931.dev12269/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.930840603.dev12256"
+__version__ = "0.2.932156931.dev12269"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

