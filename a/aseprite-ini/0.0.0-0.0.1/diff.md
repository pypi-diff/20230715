# Comparing `tmp/aseprite-ini-0.0.0.tar.gz` & `tmp/aseprite-ini-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aseprite-ini-0.0.0.tar", last modified: Sat Jul 15 18:11:46 2023, max compression
+gzip compressed data, was "aseprite-ini-0.0.1.tar", last modified: Sat Jul 15 20:37:03 2023, max compression
```

## Comparing `aseprite-ini-0.0.0.tar` & `aseprite-ini-0.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:11:46.796129 aseprite-ini-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-15 18:11:25.000000 aseprite-ini-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-15 18:11:46.796129 aseprite-ini-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-15 18:11:25.000000 aseprite-ini-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-15 18:11:25.000000 aseprite-ini-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 18:11:46.796129 aseprite-ini-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:11:46.796129 aseprite-ini-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:11:46.796129 aseprite-ini-0.0.0/src/aseprite_ini/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 18:11:25.000000 aseprite-ini-0.0.0/src/aseprite_ini/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:11:46.796129 aseprite-ini-0.0.0/src/aseprite_ini.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-15 18:11:46.000000 aseprite-ini-0.0.0/src/aseprite_ini.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-15 18:11:46.000000 aseprite-ini-0.0.0/src/aseprite_ini.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 18:11:46.000000 aseprite-ini-0.0.0/src/aseprite_ini.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-15 18:11:46.000000 aseprite-ini-0.0.0/src/aseprite_ini.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-15 18:11:46.000000 aseprite-ini-0.0.0/src/aseprite_ini.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:11:46.796129 aseprite-ini-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-15 18:11:25.000000 aseprite-ini-0.0.0/tests/test_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:37:03.313245 aseprite-ini-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-15 20:36:51.000000 aseprite-ini-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-15 20:37:03.313245 aseprite-ini-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-15 20:36:51.000000 aseprite-ini-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-15 20:36:51.000000 aseprite-ini-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 20:37:03.313245 aseprite-ini-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:37:03.313245 aseprite-ini-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:37:03.313245 aseprite-ini-0.0.1/src/aseprite_ini/
+-rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-07-15 20:36:51.000000 aseprite-ini-0.0.1/src/aseprite_ini/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:37:03.313245 aseprite-ini-0.0.1/src/aseprite_ini.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-15 20:37:03.000000 aseprite-ini-0.0.1/src/aseprite_ini.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-15 20:37:03.000000 aseprite-ini-0.0.1/src/aseprite_ini.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 20:37:03.000000 aseprite-ini-0.0.1/src/aseprite_ini.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-15 20:37:03.000000 aseprite-ini-0.0.1/src/aseprite_ini.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-15 20:37:03.000000 aseprite-ini-0.0.1/src/aseprite_ini.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:37:03.313245 aseprite-ini-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-15 20:36:51.000000 aseprite-ini-0.0.1/tests/test_.py
```

### Comparing `aseprite-ini-0.0.0/LICENSE` & `aseprite-ini-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aseprite-ini-0.0.0/pyproject.toml` & `aseprite-ini-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aseprite-ini"
-version = "0.0.0"
+version = "0.0.1"
 description = "A tool to parse Aseprite '.ini' format file."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "Aseprite Quest" },
 ]
```

