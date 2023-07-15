# Comparing `tmp/ContactApi-0.0.2.tar.gz` & `tmp/ContactApi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ContactApi-0.0.2.tar", last modified: Sat Jul 15 15:09:58 2023, max compression
+gzip compressed data, was "ContactApi-0.0.3.tar", last modified: Sat Jul 15 15:12:12 2023, max compression
```

## Comparing `ContactApi-0.0.2.tar` & `ContactApi-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:09:58.593755 ContactApi-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-15 15:09:58.593755 ContactApi-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-15 15:09:46.000000 ContactApi-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-15 15:09:46.000000 ContactApi-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 15:09:58.593755 ContactApi-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:09:58.589755 ContactApi-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:09:58.593755 ContactApi-0.0.2/src/ContactApi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-15 15:09:58.000000 ContactApi-0.0.2/src/ContactApi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-15 15:09:58.000000 ContactApi-0.0.2/src/ContactApi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 15:09:58.000000 ContactApi-0.0.2/src/ContactApi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-15 15:09:58.000000 ContactApi-0.0.2/src/ContactApi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-15 15:09:58.000000 ContactApi-0.0.2/src/ContactApi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-15 15:09:58.000000 ContactApi-0.0.2/src/ContactApi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 15:09:46.000000 ContactApi-0.0.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-15 15:09:46.000000 ContactApi-0.0.2/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-15 15:09:46.000000 ContactApi-0.0.2/src/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-15 15:09:46.000000 ContactApi-0.0.2/src/crud.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-15 15:09:46.000000 ContactApi-0.0.2/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-15 15:09:46.000000 ContactApi-0.0.2/src/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-15 15:09:46.000000 ContactApi-0.0.2/src/router.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-15 15:09:46.000000 ContactApi-0.0.2/src/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:12:12.273049 ContactApi-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-15 15:12:12.269049 ContactApi-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-15 15:11:56.000000 ContactApi-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-15 15:11:57.000000 ContactApi-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 15:12:12.273049 ContactApi-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:12:12.269049 ContactApi-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:12:12.269049 ContactApi-0.0.3/src/ContactApi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-15 15:12:12.000000 ContactApi-0.0.3/src/ContactApi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-15 15:12:12.000000 ContactApi-0.0.3/src/ContactApi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 15:12:12.000000 ContactApi-0.0.3/src/ContactApi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-15 15:12:12.000000 ContactApi-0.0.3/src/ContactApi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-15 15:12:12.000000 ContactApi-0.0.3/src/ContactApi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-15 15:12:12.000000 ContactApi-0.0.3/src/ContactApi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 15:11:56.000000 ContactApi-0.0.3/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-15 15:11:56.000000 ContactApi-0.0.3/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-15 15:11:56.000000 ContactApi-0.0.3/src/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-15 15:11:56.000000 ContactApi-0.0.3/src/crud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-15 15:11:56.000000 ContactApi-0.0.3/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-15 15:11:56.000000 ContactApi-0.0.3/src/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-15 15:11:56.000000 ContactApi-0.0.3/src/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-15 15:11:56.000000 ContactApi-0.0.3/src/schemas.py
```

### Comparing `ContactApi-0.0.2/PKG-INFO` & `ContactApi-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: ContactApi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Just a demo project
 Keywords: flask,project
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # fastapi
 
-# Runing app
+# Runing app with docker
+
+export DB_PASS="password"
 
-export  DB_PASS="password"
 export DATABASE_URL="postgresql://postgres:$DB_PASS@localhost:5432"
 
 podman create network contactapi
 
 podman pull docker.io/library/postgres
+
 podman pull ghcr.io/yulai202020/contactapi
 
 podman images
 
 podman run --network contactapi -e POSTGRES_PASSWORD=$DB_PASS -d --name postgresdb docker.io/library/postgres
 
 podman run --network contactapi -e DATABASE_URL=$DATABASE_URL -p 8000:8000 -d ghcr.io/yulai202020/contactapi
```

### Comparing `ContactApi-0.0.2/src/ContactApi.egg-info/PKG-INFO` & `ContactApi-0.0.3/src/ContactApi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: ContactApi
-Version: 0.0.2
+Version: 0.0.3
 Summary: Just a demo project
 Keywords: flask,project
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # fastapi
 
-# Runing app
+# Runing app with docker
+
+export DB_PASS="password"
 
-export  DB_PASS="password"
 export DATABASE_URL="postgresql://postgres:$DB_PASS@localhost:5432"
 
 podman create network contactapi
 
 podman pull docker.io/library/postgres
+
 podman pull ghcr.io/yulai202020/contactapi
 
 podman images
 
 podman run --network contactapi -e POSTGRES_PASSWORD=$DB_PASS -d --name postgresdb docker.io/library/postgres
 
 podman run --network contactapi -e DATABASE_URL=$DATABASE_URL -p 8000:8000 -d ghcr.io/yulai202020/contactapi
```

### Comparing `ContactApi-0.0.2/src/config.py` & `ContactApi-0.0.3/src/config.py`

 * *Files identical despite different names*

### Comparing `ContactApi-0.0.2/src/crud.py` & `ContactApi-0.0.3/src/crud.py`

 * *Files identical despite different names*

### Comparing `ContactApi-0.0.2/src/router.py` & `ContactApi-0.0.3/src/router.py`

 * *Files identical despite different names*

