# Comparing `tmp/wiggler_studiorabota-0.0.2.tar.gz` & `tmp/wiggler_studiorabota-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiggler_studiorabota-0.0.2.tar", last modified: Mon Jul 10 20:16:21 2023, max compression
+gzip compressed data, was "wiggler_studiorabota-0.0.3.tar", last modified: Sat Jul 15 09:27:52 2023, max compression
```

## Comparing `wiggler_studiorabota-0.0.2.tar` & `wiggler_studiorabota-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-10 20:16:21.864207 wiggler_studiorabota-0.0.2/
--rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-10 20:16:21.864062 wiggler_studiorabota-0.0.2/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)       91 2023-07-10 20:08:40.000000 wiggler_studiorabota-0.0.2/README.md
--rw-r--r--   0 vincent    (501) staff       (20)      458 2023-07-10 20:16:15.000000 wiggler_studiorabota-0.0.2/pyproject.toml
--rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-10 20:16:21.864241 wiggler_studiorabota-0.0.2/setup.cfg
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-10 20:16:21.862861 wiggler_studiorabota-0.0.2/wiggler/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-09 16:41:51.000000 wiggler_studiorabota-0.0.2/wiggler/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      318 2023-07-10 20:15:53.000000 wiggler_studiorabota-0.0.2/wiggler/cli.py
--rw-r--r--   0 vincent    (501) staff       (20)      709 2023-07-10 19:47:45.000000 wiggler_studiorabota-0.0.2/wiggler/main.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-10 20:16:21.863877 wiggler_studiorabota-0.0.2/wiggler_studiorabota.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-10 20:16:21.000000 wiggler_studiorabota-0.0.2/wiggler_studiorabota.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      298 2023-07-10 20:16:21.000000 wiggler_studiorabota-0.0.2/wiggler_studiorabota.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-10 20:16:21.000000 wiggler_studiorabota-0.0.2/wiggler_studiorabota.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)       45 2023-07-10 20:16:21.000000 wiggler_studiorabota-0.0.2/wiggler_studiorabota.egg-info/entry_points.txt
--rw-r--r--   0 vincent    (501) staff       (20)        8 2023-07-10 20:16:21.000000 wiggler_studiorabota-0.0.2/wiggler_studiorabota.egg-info/top_level.txt
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 09:27:52.914066 wiggler_studiorabota-0.0.3/
+-rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-15 09:27:52.913896 wiggler_studiorabota-0.0.3/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)       91 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.3/README.md
+-rw-r--r--   0 vincent    (501) staff       (20)      458 2023-07-15 09:27:39.000000 wiggler_studiorabota-0.0.3/pyproject.toml
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-15 09:27:52.914108 wiggler_studiorabota-0.0.3/setup.cfg
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 09:27:52.912706 wiggler_studiorabota-0.0.3/wiggler/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.3/wiggler/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      318 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.3/wiggler/cli.py
+-rw-r--r--   0 vincent    (501) staff       (20)      823 2023-07-15 09:26:59.000000 wiggler_studiorabota-0.0.3/wiggler/main.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 09:27:52.913588 wiggler_studiorabota-0.0.3/wiggler_studiorabota.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-15 09:27:52.000000 wiggler_studiorabota-0.0.3/wiggler_studiorabota.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      298 2023-07-15 09:27:52.000000 wiggler_studiorabota-0.0.3/wiggler_studiorabota.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-15 09:27:52.000000 wiggler_studiorabota-0.0.3/wiggler_studiorabota.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       45 2023-07-15 09:27:52.000000 wiggler_studiorabota-0.0.3/wiggler_studiorabota.egg-info/entry_points.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        8 2023-07-15 09:27:52.000000 wiggler_studiorabota-0.0.3/wiggler_studiorabota.egg-info/top_level.txt
```

### Comparing `wiggler_studiorabota-0.0.2/wiggler/main.py` & `wiggler_studiorabota-0.0.3/wiggler/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from fastapi import FastAPI
+from fastapi.staticfiles import StaticFiles
 from datetime import datetime
 import os
 
 app = FastAPI()
 
+app.mount("/image", StaticFiles(directory="./images"), name="image")
+
 @app.get("/")
 def read_root():
     return {"Hello": "Worm"}
 
 @app.get("/images")
 def images():
     out = []
```

