# Comparing `tmp/miauw-base-service-1.0.0.tar.gz` & `tmp/miauw-base-service-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miauw-base-service-1.0.0.tar", last modified: Sat Jul 15 12:56:43 2023, max compression
+gzip compressed data, was "miauw-base-service-1.0.1.tar", last modified: Sat Jul 15 13:06:21 2023, max compression
```

## Comparing `miauw-base-service-1.0.0.tar` & `miauw-base-service-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-15 12:56:43.864951 miauw-base-service-1.0.0/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-15 12:56:43.864951 miauw-base-service-1.0.0/PKG-INFO
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-15 12:56:43.861617 miauw-base-service-1.0.0/base_service/
--rw-r--r--   0 leo       (1000) leo       (1000)       63 2023-07-13 05:13:50.000000 miauw-base-service-1.0.0/base_service/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2091 2023-07-15 12:45:55.000000 miauw-base-service-1.0.0/base_service/service.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1879 2023-07-14 10:06:11.000000 miauw-base-service-1.0.0/base_service/worker.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-15 12:56:43.864951 miauw-base-service-1.0.0/miauw_base_service.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-15 12:56:43.000000 miauw-base-service-1.0.0/miauw_base_service.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-15 12:56:43.000000 miauw-base-service-1.0.0/miauw_base_service.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-15 12:56:43.000000 miauw-base-service-1.0.0/miauw_base_service.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-15 12:56:43.000000 miauw-base-service-1.0.0/miauw_base_service.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-15 12:56:43.000000 miauw-base-service-1.0.0/miauw_base_service.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-15 12:52:38.000000 miauw-base-service-1.0.0/pyproject.toml
--rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-15 12:56:43.864951 miauw-base-service-1.0.0/setup.cfg
--rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-15 12:52:28.000000 miauw-base-service-1.0.0/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-15 13:06:21.114938 miauw-base-service-1.0.1/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-15 13:06:21.111605 miauw-base-service-1.0.1/PKG-INFO
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-15 13:06:21.111605 miauw-base-service-1.0.1/base_service/
+-rw-r--r--   0 leo       (1000) leo       (1000)       67 2023-07-15 13:04:36.000000 miauw-base-service-1.0.1/base_service/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2091 2023-07-15 12:45:55.000000 miauw-base-service-1.0.1/base_service/service.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1879 2023-07-14 10:06:11.000000 miauw-base-service-1.0.1/base_service/worker.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-15 13:06:21.111605 miauw-base-service-1.0.1/miauw_base_service.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-15 13:06:21.000000 miauw-base-service-1.0.1/miauw_base_service.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-15 13:06:21.000000 miauw-base-service-1.0.1/miauw_base_service.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-15 13:06:21.000000 miauw-base-service-1.0.1/miauw_base_service.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-15 13:06:21.000000 miauw-base-service-1.0.1/miauw_base_service.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-15 13:06:21.000000 miauw-base-service-1.0.1/miauw_base_service.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-15 13:05:35.000000 miauw-base-service-1.0.1/pyproject.toml
+-rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-15 13:06:21.114938 miauw-base-service-1.0.1/setup.cfg
+-rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-15 13:05:30.000000 miauw-base-service-1.0.1/setup.py
```

### Comparing `miauw-base-service-1.0.0/base_service/service.py` & `miauw-base-service-1.0.1/base_service/service.py`

 * *Files identical despite different names*

### Comparing `miauw-base-service-1.0.0/base_service/worker.py` & `miauw-base-service-1.0.1/base_service/worker.py`

 * *Files identical despite different names*

