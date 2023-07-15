# Comparing `tmp/revealjs-0.0.1.tar.gz` & `tmp/revealjs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revealjs-0.0.1.tar", last modified: Sat Jul 15 17:27:16 2023, max compression
+gzip compressed data, was "revealjs-0.0.2.tar", last modified: Sat Jul 15 18:03:45 2023, max compression
```

## Comparing `revealjs-0.0.1.tar` & `revealjs-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 guna      (1001) guna      (1001)        0 2023-07-15 17:27:11.522643 revealjs-0.0.1/
--rw-rw-r--   0 guna      (1001) guna      (1001)     1429 2023-07-15 17:27:16.821444 revealjs-0.0.1/PKG-INFO
--rw-rw-r--   0 guna      (1001) guna      (1001)      898 2023-07-15 16:22:37.000000 revealjs-0.0.1/README.md
-drwxrwxr-x   0 guna      (1001) guna      (1001)        0 2023-07-15 17:27:11.522643 revealjs-0.0.1/revealjs/
--rw-rw-r--   0 guna      (1001) guna      (1001)        0 2023-07-15 17:23:21.000000 revealjs-0.0.1/revealjs/__init__.py
--rw-rw-r--   0 guna      (1001) guna      (1001)    15520 2023-07-15 16:40:05.000000 revealjs-0.0.1/revealjs/reveal_js.py
-drwxrwxr-x   0 guna      (1001) guna      (1001)        0 2023-07-15 17:27:16.821444 revealjs-0.0.1/revealjs.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     1429 2023-07-15 17:27:16.000000 revealjs-0.0.1/revealjs.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      255 2023-07-15 17:27:16.000000 revealjs-0.0.1/revealjs.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-07-15 17:27:16.000000 revealjs-0.0.1/revealjs.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       55 2023-07-15 17:27:16.000000 revealjs-0.0.1/revealjs.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)       22 2023-07-15 17:27:16.000000 revealjs-0.0.1/revealjs.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        9 2023-07-15 17:27:16.000000 revealjs-0.0.1/revealjs.egg-info/top_level.txt
--rw-rw-r--   0 guna      (1001) guna      (1001)       38 2023-07-15 17:27:16.821444 revealjs-0.0.1/setup.cfg
--rw-rw-r--   0 guna      (1001) guna      (1001)      652 2023-07-15 17:26:10.000000 revealjs-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 18:03:45.106750 revealjs-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-07-15 18:03:45.106750 revealjs-0.0.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      898 2023-07-15 16:22:37.000000 revealjs-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 18:03:45.106750 revealjs-0.0.2/revealjs/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-15 17:47:50.000000 revealjs-0.0.2/revealjs/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    15520 2023-07-15 17:47:50.000000 revealjs-0.0.2/revealjs/reveal_js.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 18:03:45.106750 revealjs-0.0.2/revealjs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-07-15 18:03:45.000000 revealjs-0.0.2/revealjs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      255 2023-07-15 18:03:45.000000 revealjs-0.0.2/revealjs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 18:03:45.000000 revealjs-0.0.2/revealjs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-07-15 18:03:45.000000 revealjs-0.0.2/revealjs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-15 18:03:45.000000 revealjs-0.0.2/revealjs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-15 18:03:45.000000 revealjs-0.0.2/revealjs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-15 18:03:45.106750 revealjs-0.0.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      482 2023-07-15 18:00:50.000000 revealjs-0.0.2/setup.py
```

### Comparing `revealjs-0.0.1/PKG-INFO` & `revealjs-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revealjs
-Version: 0.0.1
+Version: 0.0.2
 Summary: Reveal.js Presentation
 Home-page: https://github.com/gunaNeelamegam/revealjs-presentation.git
 Author: guna
 Author-email: gunag5127@gmail.com
 License: UNKNOWN
 Description: ### Docker image for reveal js
```

### Comparing `revealjs-0.0.1/README.md` & `revealjs-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `revealjs-0.0.1/revealjs/reveal_js.py` & `revealjs-0.0.2/revealjs/reveal_js.py`

 * *Files identical despite different names*

### Comparing `revealjs-0.0.1/revealjs.egg-info/PKG-INFO` & `revealjs-0.0.2/revealjs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revealjs
-Version: 0.0.1
+Version: 0.0.2
 Summary: Reveal.js Presentation
 Home-page: https://github.com/gunaNeelamegam/revealjs-presentation.git
 Author: guna
 Author-email: gunag5127@gmail.com
 License: UNKNOWN
 Description: ### Docker image for reveal js
```

