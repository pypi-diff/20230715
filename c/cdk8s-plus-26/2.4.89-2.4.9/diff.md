# Comparing `tmp/cdk8s-plus-26-2.4.89.tar.gz` & `tmp/cdk8s-plus-26-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-plus-26-2.4.89.tar", last modified: Sat Jul 15 00:40:34 2023, max compression
+gzip compressed data, was "cdk8s-plus-26-2.4.9.tar", last modified: Fri Jun  2 02:39:56 2023, max compression
```

## Comparing `cdk8s-plus-26-2.4.89.tar` & `cdk8s-plus-26-2.4.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:40:34.130288 cdk8s-plus-26-2.4.89/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-15 00:40:18.000000 cdk8s-plus-26-2.4.89/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 00:40:18.000000 cdk8s-plus-26-2.4.89/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-15 00:40:18.000000 cdk8s-plus-26-2.4.89/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-15 00:40:34.130288 cdk8s-plus-26-2.4.89/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-15 00:40:18.000000 cdk8s-plus-26-2.4.89/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-15 00:40:18.000000 cdk8s-plus-26-2.4.89/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 00:40:34.130288 cdk8s-plus-26-2.4.89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-15 00:40:18.000000 cdk8s-plus-26-2.4.89/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:40:34.122288 cdk8s-plus-26-2.4.89/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:40:34.122288 cdk8s-plus-26-2.4.89/src/cdk8s_plus_26/
--rw-r--r--   0 runner    (1001) docker     (123)  1161508 2023-07-15 00:40:18.000000 cdk8s-plus-26-2.4.89/src/cdk8s_plus_26/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:40:34.126288 cdk8s-plus-26-2.4.89/src/cdk8s_plus_26/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-15 00:40:18.000000 cdk8s-plus-26-2.4.89/src/cdk8s_plus_26/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1287698 2023-07-15 00:40:18.000000 cdk8s-plus-26-2.4.89/src/cdk8s_plus_26/_jsii/cdk8s-plus-26@2.4.89.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:40:34.126288 cdk8s-plus-26-2.4.89/src/cdk8s_plus_26/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)  2771385 2023-07-15 00:40:18.000000 cdk8s-plus-26-2.4.89/src/cdk8s_plus_26/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 00:40:18.000000 cdk8s-plus-26-2.4.89/src/cdk8s_plus_26/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:40:34.126288 cdk8s-plus-26-2.4.89/src/cdk8s_plus_26.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-07-15 00:40:34.000000 cdk8s-plus-26-2.4.89/src/cdk8s_plus_26.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-15 00:40:34.000000 cdk8s-plus-26-2.4.89/src/cdk8s_plus_26.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 00:40:34.000000 cdk8s-plus-26-2.4.89/src/cdk8s_plus_26.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-15 00:40:34.000000 cdk8s-plus-26-2.4.89/src/cdk8s_plus_26.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-15 00:40:34.000000 cdk8s-plus-26-2.4.89/src/cdk8s_plus_26.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:39:56.353091 cdk8s-plus-26-2.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-02 02:39:44.000000 cdk8s-plus-26-2.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 02:39:44.000000 cdk8s-plus-26-2.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-02 02:39:44.000000 cdk8s-plus-26-2.4.9/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-02 02:39:56.353091 cdk8s-plus-26-2.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-02 02:39:44.000000 cdk8s-plus-26-2.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-02 02:39:44.000000 cdk8s-plus-26-2.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 02:39:56.353091 cdk8s-plus-26-2.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-02 02:39:44.000000 cdk8s-plus-26-2.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:39:56.345091 cdk8s-plus-26-2.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:39:56.345091 cdk8s-plus-26-2.4.9/src/cdk8s_plus_26/
+-rw-r--r--   0 runner    (1001) docker     (123)  1161508 2023-06-02 02:39:44.000000 cdk8s-plus-26-2.4.9/src/cdk8s_plus_26/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:39:56.345091 cdk8s-plus-26-2.4.9/src/cdk8s_plus_26/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-02 02:39:44.000000 cdk8s-plus-26-2.4.9/src/cdk8s_plus_26/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1287683 2023-06-02 02:39:44.000000 cdk8s-plus-26-2.4.9/src/cdk8s_plus_26/_jsii/cdk8s-plus-26@2.4.9.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:39:56.349091 cdk8s-plus-26-2.4.9/src/cdk8s_plus_26/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)  2771385 2023-06-02 02:39:44.000000 cdk8s-plus-26-2.4.9/src/cdk8s_plus_26/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 02:39:44.000000 cdk8s-plus-26-2.4.9/src/cdk8s_plus_26/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:39:56.345091 cdk8s-plus-26-2.4.9/src/cdk8s_plus_26.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-02 02:39:56.000000 cdk8s-plus-26-2.4.9/src/cdk8s_plus_26.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-02 02:39:56.000000 cdk8s-plus-26-2.4.9/src/cdk8s_plus_26.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 02:39:56.000000 cdk8s-plus-26-2.4.9/src/cdk8s_plus_26.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-02 02:39:56.000000 cdk8s-plus-26-2.4.9/src/cdk8s_plus_26.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 02:39:56.000000 cdk8s-plus-26-2.4.9/src/cdk8s_plus_26.egg-info/top_level.txt
```

### Comparing `cdk8s-plus-26-2.4.89/LICENSE` & `cdk8s-plus-26-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-26-2.4.89/PKG-INFO` & `cdk8s-plus-26-2.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-26
-Version: 2.4.89
+Version: 2.4.9
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-26 synthesizes Kubernetes manifests for Kubernetes 1.26.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-plus-26-2.4.89/README.md` & `cdk8s-plus-26-2.4.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-26-2.4.89/setup.py` & `cdk8s-plus-26-2.4.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-plus-26",
-    "version": "2.4.89",
+    "version": "2.4.9",
     "description": "cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-26 synthesizes Kubernetes manifests for Kubernetes 1.26.0",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-plus.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -23,25 +23,25 @@
     "packages": [
         "cdk8s_plus_26",
         "cdk8s_plus_26._jsii",
         "cdk8s_plus_26.k8s"
     ],
     "package_data": {
         "cdk8s_plus_26._jsii": [
-            "cdk8s-plus-26@2.4.89.jsii.tgz"
+            "cdk8s-plus-26@2.4.9.jsii.tgz"
         ],
         "cdk8s_plus_26": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdk8s>=2.7.106, <3.0.0",
-        "constructs>=10.2.69, <11.0.0",
-        "jsii>=1.84.0, <2.0.0",
+        "cdk8s>=2.7.77, <3.0.0",
+        "constructs>=10.2.40, <11.0.0",
+        "jsii>=1.82.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk8s-plus-26-2.4.89/src/cdk8s_plus_26/__init__.py` & `cdk8s-plus-26-2.4.9/src/cdk8s_plus_26/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-26-2.4.89/src/cdk8s_plus_26/k8s/__init__.py` & `cdk8s-plus-26-2.4.9/src/cdk8s_plus_26/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-26-2.4.89/src/cdk8s_plus_26.egg-info/PKG-INFO` & `cdk8s-plus-26-2.4.9/src/cdk8s_plus_26.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-26
-Version: 2.4.89
+Version: 2.4.9
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-26 synthesizes Kubernetes manifests for Kubernetes 1.26.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

