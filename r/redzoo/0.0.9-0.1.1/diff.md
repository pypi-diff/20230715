# Comparing `tmp/redzoo-0.0.9.tar.gz` & `tmp/redzoo-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redzoo-0.0.9.tar", last modified: Sat Nov 19 12:11:44 2022, max compression
+gzip compressed data, was "redzoo-0.1.1.tar", last modified: Sat Jul 15 08:01:21 2023, max compression
```

## Comparing `redzoo-0.0.9.tar` & `redzoo-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 12:11:44.379693 redzoo-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-19 12:11:33.000000 redzoo-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-11-19 12:11:44.379693 redzoo-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-19 12:11:33.000000 redzoo-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-11-19 12:11:33.000000 redzoo-0.0.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 12:11:44.379693 redzoo-0.0.9/redzoo/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-19 12:11:33.000000 redzoo-0.0.9/redzoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 12:11:44.379693 redzoo-0.0.9/redzoo/database/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-19 12:11:33.000000 redzoo-0.0.9/redzoo/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4069 2022-11-19 12:11:33.000000 redzoo-0.0.9/redzoo/database/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 12:11:44.379693 redzoo-0.0.9/redzoo/math/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-19 12:11:33.000000 redzoo-0.0.9/redzoo/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-11-19 12:11:33.000000 redzoo-0.0.9/redzoo/math/display.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 12:11:44.379693 redzoo-0.0.9/redzoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-11-19 12:11:44.000000 redzoo-0.0.9/redzoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-11-19 12:11:44.000000 redzoo-0.0.9/redzoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-19 12:11:44.000000 redzoo-0.0.9/redzoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-19 12:11:44.000000 redzoo-0.0.9/redzoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-19 12:11:44.000000 redzoo-0.0.9/redzoo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-11-19 12:11:44.379693 redzoo-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 12:11:44.379693 redzoo-0.0.9/test/
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-11-19 12:11:33.000000 redzoo-0.0.9/test/test_display.py
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-11-19 12:11:33.000000 redzoo-0.0.9/test/test_simpledb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:01:21.277086 redzoo-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-15 08:01:09.000000 redzoo-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-15 08:01:21.277086 redzoo-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-15 08:01:09.000000 redzoo-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-15 08:01:09.000000 redzoo-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:01:21.277086 redzoo-0.1.1/redzoo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 08:01:09.000000 redzoo-0.1.1/redzoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:01:21.277086 redzoo-0.1.1/redzoo/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 08:01:09.000000 redzoo-0.1.1/redzoo/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-15 08:01:09.000000 redzoo-0.1.1/redzoo/database/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:01:21.277086 redzoo-0.1.1/redzoo/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 08:01:09.000000 redzoo-0.1.1/redzoo/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-15 08:01:09.000000 redzoo-0.1.1/redzoo/math/display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:01:21.277086 redzoo-0.1.1/redzoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-15 08:01:21.000000 redzoo-0.1.1/redzoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-15 08:01:21.000000 redzoo-0.1.1/redzoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 08:01:21.000000 redzoo-0.1.1/redzoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-15 08:01:21.000000 redzoo-0.1.1/redzoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-15 08:01:21.000000 redzoo-0.1.1/redzoo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-15 08:01:21.277086 redzoo-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 08:01:21.277086 redzoo-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-15 08:01:09.000000 redzoo-0.1.1/test/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-15 08:01:09.000000 redzoo-0.1.1/test/test_simpledb.py
```

### Comparing `redzoo-0.0.9/LICENSE` & `redzoo-0.1.1/LICENSE`

 * *Files identical despite different names*

