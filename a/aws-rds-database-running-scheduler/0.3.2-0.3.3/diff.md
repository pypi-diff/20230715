# Comparing `tmp/aws-rds-database-running-scheduler-0.3.2.tar.gz` & `tmp/aws-rds-database-running-scheduler-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-rds-database-running-scheduler-0.3.2.tar", last modified: Fri Jul 14 19:15:58 2023, max compression
+gzip compressed data, was "aws-rds-database-running-scheduler-0.3.3.tar", last modified: Sat Jul 15 19:14:57 2023, max compression
```

## Comparing `aws-rds-database-running-scheduler-0.3.2.tar` & `aws-rds-database-running-scheduler-0.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:15:58.196821 aws-rds-database-running-scheduler-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-14 19:15:40.000000 aws-rds-database-running-scheduler-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 19:15:40.000000 aws-rds-database-running-scheduler-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-14 19:15:58.196821 aws-rds-database-running-scheduler-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-14 19:15:40.000000 aws-rds-database-running-scheduler-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-14 19:15:40.000000 aws-rds-database-running-scheduler-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 19:15:58.196821 aws-rds-database-running-scheduler-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-14 19:15:40.000000 aws-rds-database-running-scheduler-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:15:58.192821 aws-rds-database-running-scheduler-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:15:58.192821 aws-rds-database-running-scheduler-0.3.2/src/aws_rds_database_running_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-07-14 19:15:40.000000 aws-rds-database-running-scheduler-0.3.2/src/aws_rds_database_running_scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:15:58.196821 aws-rds-database-running-scheduler-0.3.2/src/aws_rds_database_running_scheduler/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-14 19:15:40.000000 aws-rds-database-running-scheduler-0.3.2/src/aws_rds_database_running_scheduler/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22198 2023-07-14 19:15:40.000000 aws-rds-database-running-scheduler-0.3.2/src/aws_rds_database_running_scheduler/_jsii/aws-rds-database-running-scheduler@0.3.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:15:40.000000 aws-rds-database-running-scheduler-0.3.2/src/aws_rds_database_running_scheduler/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:15:58.196821 aws-rds-database-running-scheduler-0.3.2/src/aws_rds_database_running_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-14 19:15:58.000000 aws-rds-database-running-scheduler-0.3.2/src/aws_rds_database_running_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-14 19:15:58.000000 aws-rds-database-running-scheduler-0.3.2/src/aws_rds_database_running_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:15:58.000000 aws-rds-database-running-scheduler-0.3.2/src/aws_rds_database_running_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-14 19:15:58.000000 aws-rds-database-running-scheduler-0.3.2/src/aws_rds_database_running_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-14 19:15:58.000000 aws-rds-database-running-scheduler-0.3.2/src/aws_rds_database_running_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:57.591251 aws-rds-database-running-scheduler-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-15 19:14:46.000000 aws-rds-database-running-scheduler-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 19:14:46.000000 aws-rds-database-running-scheduler-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-15 19:14:57.591251 aws-rds-database-running-scheduler-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-15 19:14:46.000000 aws-rds-database-running-scheduler-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-15 19:14:46.000000 aws-rds-database-running-scheduler-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 19:14:57.591251 aws-rds-database-running-scheduler-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-15 19:14:46.000000 aws-rds-database-running-scheduler-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:57.587251 aws-rds-database-running-scheduler-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:57.591251 aws-rds-database-running-scheduler-0.3.3/src/aws_rds_database_running_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-07-15 19:14:46.000000 aws-rds-database-running-scheduler-0.3.3/src/aws_rds_database_running_scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:57.591251 aws-rds-database-running-scheduler-0.3.3/src/aws_rds_database_running_scheduler/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-15 19:14:46.000000 aws-rds-database-running-scheduler-0.3.3/src/aws_rds_database_running_scheduler/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22198 2023-07-15 19:14:46.000000 aws-rds-database-running-scheduler-0.3.3/src/aws_rds_database_running_scheduler/_jsii/aws-rds-database-running-scheduler@0.3.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 19:14:46.000000 aws-rds-database-running-scheduler-0.3.3/src/aws_rds_database_running_scheduler/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 19:14:57.591251 aws-rds-database-running-scheduler-0.3.3/src/aws_rds_database_running_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-15 19:14:57.000000 aws-rds-database-running-scheduler-0.3.3/src/aws_rds_database_running_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-15 19:14:57.000000 aws-rds-database-running-scheduler-0.3.3/src/aws_rds_database_running_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 19:14:57.000000 aws-rds-database-running-scheduler-0.3.3/src/aws_rds_database_running_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-15 19:14:57.000000 aws-rds-database-running-scheduler-0.3.3/src/aws_rds_database_running_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-15 19:14:57.000000 aws-rds-database-running-scheduler-0.3.3/src/aws_rds_database_running_scheduler.egg-info/top_level.txt
```

### Comparing `aws-rds-database-running-scheduler-0.3.2/LICENSE` & `aws-rds-database-running-scheduler-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-rds-database-running-scheduler-0.3.2/PKG-INFO` & `aws-rds-database-running-scheduler-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-rds-database-running-scheduler
-Version: 0.3.2
+Version: 0.3.3
 Summary: AWS RDS Database Running Scheduler
 Home-page: https://github.com/yicr/aws-rds-database-running-scheduler.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-rds-database-running-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-rds-database-running-scheduler-0.3.2/README.md` & `aws-rds-database-running-scheduler-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `aws-rds-database-running-scheduler-0.3.2/setup.py` & `aws-rds-database-running-scheduler-0.3.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-rds-database-running-scheduler",
-    "version": "0.3.2",
+    "version": "0.3.3",
     "description": "AWS RDS Database Running Scheduler",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-rds-database-running-scheduler.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_rds_database_running_scheduler",
         "aws_rds_database_running_scheduler._jsii"
     ],
     "package_data": {
         "aws_rds_database_running_scheduler._jsii": [
-            "aws-rds-database-running-scheduler@0.3.2.jsii.tgz"
+            "aws-rds-database-running-scheduler@0.3.3.jsii.tgz"
         ],
         "aws_rds_database_running_scheduler": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws-rds-database-running-scheduler-0.3.2/src/aws_rds_database_running_scheduler/__init__.py` & `aws-rds-database-running-scheduler-0.3.3/src/aws_rds_database_running_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-rds-database-running-scheduler-0.3.2/src/aws_rds_database_running_scheduler.egg-info/PKG-INFO` & `aws-rds-database-running-scheduler-0.3.3/src/aws_rds_database_running_scheduler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-rds-database-running-scheduler
-Version: 0.3.2
+Version: 0.3.3
 Summary: AWS RDS Database Running Scheduler
 Home-page: https://github.com/yicr/aws-rds-database-running-scheduler.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-rds-database-running-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-rds-database-running-scheduler-0.3.2/src/aws_rds_database_running_scheduler.egg-info/SOURCES.txt` & `aws-rds-database-running-scheduler-0.3.3/src/aws_rds_database_running_scheduler.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/aws_rds_database_running_scheduler/py.typed
 src/aws_rds_database_running_scheduler.egg-info/PKG-INFO
 src/aws_rds_database_running_scheduler.egg-info/SOURCES.txt
 src/aws_rds_database_running_scheduler.egg-info/dependency_links.txt
 src/aws_rds_database_running_scheduler.egg-info/requires.txt
 src/aws_rds_database_running_scheduler.egg-info/top_level.txt
 src/aws_rds_database_running_scheduler/_jsii/__init__.py
-src/aws_rds_database_running_scheduler/_jsii/aws-rds-database-running-scheduler@0.3.2.jsii.tgz
+src/aws_rds_database_running_scheduler/_jsii/aws-rds-database-running-scheduler@0.3.3.jsii.tgz
```

