# Comparing `tmp/typed-api-framework-0.0.1a5.tar.gz` & `tmp/typed-api-framework-0.2.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typed-api-framework-0.0.1a5.tar", last modified: Sat Jun  3 15:27:04 2023, max compression
+gzip compressed data, was "typed-api-framework-0.2.1a0.tar", last modified: Sat Jul 15 12:34:07 2023, max compression
```

## Comparing `typed-api-framework-0.0.1a5.tar` & `typed-api-framework-0.2.1a0.tar`

### file list

```diff
@@ -1,48 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:27:04.677657 typed-api-framework-0.0.1a5/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-03 15:27:04.677657 typed-api-framework-0.0.1a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 15:27:04.677657 typed-api-framework-0.0.1a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:27:04.673657 typed-api-framework-0.0.1a5/typedAPI/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:27:04.673657 typed-api-framework-0.0.1a5/typedAPI/body/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/body/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/body/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/body/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:27:04.673657 typed-api-framework-0.0.1a5/typedAPI/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/endpoint/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/endpoint/guards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/endpoint/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/endpoint/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:27:04.673657 typed-api-framework-0.0.1a5/typedAPI/headers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/headers/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/headers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/headers/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/headers/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/log_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:27:04.677657 typed-api-framework-0.0.1a5/typedAPI/resource_path/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/resource_path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/resource_path/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/resource_path/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/resource_path/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:27:04.677657 typed-api-framework-0.0.1a5/typedAPI/response/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/response/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/response/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/response/factory_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/response/guards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/response/guards_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/response/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/response/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/response/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/response/service_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-03 15:26:50.000000 typed-api-framework-0.0.1a5/typedAPI/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 15:27:04.677657 typed-api-framework-0.0.1a5/typed_api_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-03 15:27:04.000000 typed-api-framework-0.0.1a5/typed_api_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-03 15:27:04.000000 typed-api-framework-0.0.1a5/typed_api_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 15:27:04.000000 typed-api-framework-0.0.1a5/typed_api_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-03 15:27:04.000000 typed-api-framework-0.0.1a5/typed_api_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-03 15:27:04.000000 typed-api-framework-0.0.1a5/typed_api_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:34:07.487301 typed-api-framework-0.2.1a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-15 12:34:07.487301 typed-api-framework-0.2.1a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 12:34:07.487301 typed-api-framework-0.2.1a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-15 12:33:54.000000 typed-api-framework-0.2.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:34:07.487301 typed-api-framework-0.2.1a0/typed_api_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-15 12:34:07.000000 typed-api-framework-0.2.1a0/typed_api_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-15 12:34:07.000000 typed-api-framework-0.2.1a0/typed_api_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:34:07.000000 typed-api-framework-0.2.1a0/typed_api_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-15 12:34:07.000000 typed-api-framework-0.2.1a0/typed_api_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:34:07.000000 typed-api-framework-0.2.1a0/typed_api_framework.egg-info/top_level.txt
```

### Comparing `typed-api-framework-0.0.1a5/setup.py` & `typed-api-framework-0.2.1a0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from setuptools import setup, find_packages
-
 import os
 
 VERSION = os.getenv('PACKAGE_VERSION', None)
-
 print(f"{VERSION=}")
 
 if VERSION is None:
   raise RuntimeError('`PACKAGE_VERSION` not defined.')
 
 setup(
     name='typed-api-framework',
@@ -21,11 +19,12 @@
     long_description_content_type="text/markdown",
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.11',
     ],
     install_requires=[
-        'starlette>=0.27.0',
-        'pydantic>=1.10.8',
+        'starlette==0.30.0',
+        'pydantic==1.10.8',
+        'uvicorn==0.22.0',
     ],
-)
+)
```

