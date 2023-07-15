# Comparing `tmp/srai-core-0.2.0.tar.gz` & `tmp/srai-core-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srai-core-0.2.0.tar", last modified: Sat Jul 15 08:03:44 2023, max compression
+gzip compressed data, was "srai-core-0.3.0.tar", last modified: Sat Jul 15 08:26:33 2023, max compression
```

## Comparing `srai-core-0.2.0.tar` & `srai-core-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 08:03:44.046131 srai-core-0.2.0/
--rw-rw-rw-   0        0        0     1092 2023-07-15 07:11:37.000000 srai-core-0.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0      788 2023-07-15 08:03:44.046131 srai-core-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-07-15 07:11:37.000000 srai-core-0.2.0/README.md
--rw-rw-rw-   0        0        0       86 2023-07-15 08:03:44.048132 srai-core-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1221 2023-07-15 07:53:40.000000 srai-core-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 08:03:44.034183 srai-core-0.2.0/srai_core/
--rw-rw-rw-   0        0        0        0 2023-07-15 06:16:01.000000 srai-core-0.2.0/srai_core/__init__.py
--rw-rw-rw-   0        0        0      356 2023-07-15 07:48:15.000000 srai-core-0.2.0/srai_core/file_store_disk.py
--rw-rw-rw-   0        0        0     1238 2023-07-15 07:46:28.000000 srai-core-0.2.0/srai_core/jsondict_store.py
-drwxrwxrwx   0        0        0        0 2023-07-15 08:03:44.044133 srai-core-0.2.0/srai_core.egg-info/
--rw-rw-rw-   0        0        0      788 2023-07-15 08:03:43.000000 srai-core-0.2.0/srai_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-07-15 08:03:43.000000 srai-core-0.2.0/srai_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 08:03:43.000000 srai-core-0.2.0/srai_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-15 08:03:43.000000 srai-core-0.2.0/srai_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-15 08:03:43.000000 srai-core-0.2.0/srai_core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 08:26:33.804980 srai-core-0.3.0/
+-rw-rw-rw-   0        0        0     1092 2023-07-15 07:11:37.000000 srai-core-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       24 2023-07-15 08:05:50.000000 srai-core-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      767 2023-07-15 08:26:33.805985 srai-core-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-07-15 07:11:37.000000 srai-core-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-15 07:25:20.000000 srai-core-0.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-07-15 08:26:33.807980 srai-core-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1221 2023-07-15 08:06:27.000000 srai-core-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 08:26:33.794984 srai-core-0.3.0/srai_core/
+-rw-rw-rw-   0        0        0        0 2023-07-15 06:16:01.000000 srai-core-0.3.0/srai_core/__init__.py
+-rw-rw-rw-   0        0        0      356 2023-07-15 07:48:15.000000 srai-core-0.3.0/srai_core/file_store_disk.py
+-rw-rw-rw-   0        0        0     1238 2023-07-15 07:46:28.000000 srai-core-0.3.0/srai_core/jsondict_store.py
+drwxrwxrwx   0        0        0        0 2023-07-15 08:26:33.803981 srai-core-0.3.0/srai_core.egg-info/
+-rw-rw-rw-   0        0        0      767 2023-07-15 08:26:33.000000 srai-core-0.3.0/srai_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-15 08:26:33.000000 srai-core-0.3.0/srai_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 08:26:33.000000 srai-core-0.3.0/srai_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-15 08:26:33.000000 srai-core-0.3.0/srai_core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-15 08:26:33.000000 srai-core-0.3.0/srai_core.egg-info/top_level.txt
```

### Comparing `srai-core-0.2.0/LICENSE.txt` & `srai-core-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srai-core-0.2.0/setup.py` & `srai-core-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="srai-core",
     packages=find_packages(),
-    version="0.2.0",
+    version="0.3.0",
     license='MIT',
     package_data={},
     python_requires=">=3.5",
     install_requires=requirements,
     author="Jaap Oosterbroek",
     author_email="jaap.oosterbroek@southriverai.com",
     description="A library core functions used in other SRAI libraries.",
```

### Comparing `srai-core-0.2.0/srai_core/jsondict_store.py` & `srai-core-0.3.0/srai_core/jsondict_store.py`

 * *Files identical despite different names*

