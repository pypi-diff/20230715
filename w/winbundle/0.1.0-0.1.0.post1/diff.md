# Comparing `tmp/winbundle-0.1.0.tar.gz` & `tmp/winbundle-0.1.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winbundle-0.1.0.tar", last modified: Sat Jul 15 20:42:04 2023, max compression
+gzip compressed data, was "winbundle-0.1.0.post1.tar", last modified: Sat Jul 15 20:56:31 2023, max compression
```

## Comparing `winbundle-0.1.0.tar` & `winbundle-0.1.0.post1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 20:42:04.315918 winbundle-0.1.0/
--rw-rw-rw-   0        0        0     1095 2023-07-15 14:51:52.000000 winbundle-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       79 2023-07-15 20:42:04.315414 winbundle-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      153 2023-07-15 11:08:53.000000 winbundle-0.1.0/README.md
--rw-rw-rw-   0        0        0      204 2023-07-15 20:39:31.000000 winbundle-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-15 20:42:04.316415 winbundle-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-15 20:42:04.297916 winbundle-0.1.0/winbundle/
--rw-rw-rw-   0        0        0       74 2023-07-15 20:39:31.000000 winbundle-0.1.0/winbundle/__init__.py
--rw-rw-rw-   0        0        0     1882 2023-07-15 20:39:31.000000 winbundle-0.1.0/winbundle/__main__.py
--rw-rw-rw-   0        0        0    10720 2023-07-15 20:40:10.000000 winbundle-0.1.0/winbundle/builder.py
--rw-rw-rw-   0        0        0     3278 2023-07-15 20:39:31.000000 winbundle-0.1.0/winbundle/newconfig.py
--rw-rw-rw-   0        0        0      913 2023-07-15 13:24:35.000000 winbundle-0.1.0/winbundle/util.py
-drwxrwxrwx   0        0        0        0 2023-07-15 20:42:04.314415 winbundle-0.1.0/winbundle.egg-info/
--rw-rw-rw-   0        0        0       79 2023-07-15 20:42:04.000000 winbundle-0.1.0/winbundle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-07-15 20:42:04.000000 winbundle-0.1.0/winbundle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 20:42:04.000000 winbundle-0.1.0/winbundle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-15 20:42:04.000000 winbundle-0.1.0/winbundle.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-15 20:42:04.000000 winbundle-0.1.0/winbundle.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 20:56:31.386338 winbundle-0.1.0.post1/
+-rw-rw-rw-   0        0        0     1095 2023-07-15 14:51:52.000000 winbundle-0.1.0.post1/LICENSE
+-rw-rw-rw-   0        0        0      415 2023-07-15 20:56:31.385338 winbundle-0.1.0.post1/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2023-07-15 20:50:38.000000 winbundle-0.1.0.post1/README.md
+-rw-rw-rw-   0        0        0      412 2023-07-15 20:55:53.000000 winbundle-0.1.0.post1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-15 20:56:31.386338 winbundle-0.1.0.post1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-15 20:56:31.367338 winbundle-0.1.0.post1/winbundle/
+-rw-rw-rw-   0        0        0       74 2023-07-15 20:39:31.000000 winbundle-0.1.0.post1/winbundle/__init__.py
+-rw-rw-rw-   0        0        0     1882 2023-07-15 20:39:31.000000 winbundle-0.1.0.post1/winbundle/__main__.py
+-rw-rw-rw-   0        0        0    10720 2023-07-15 20:40:10.000000 winbundle-0.1.0.post1/winbundle/builder.py
+-rw-rw-rw-   0        0        0     3278 2023-07-15 20:39:31.000000 winbundle-0.1.0.post1/winbundle/newconfig.py
+-rw-rw-rw-   0        0        0      913 2023-07-15 13:24:35.000000 winbundle-0.1.0.post1/winbundle/util.py
+drwxrwxrwx   0        0        0        0 2023-07-15 20:56:31.384340 winbundle-0.1.0.post1/winbundle.egg-info/
+-rw-rw-rw-   0        0        0      415 2023-07-15 20:56:31.000000 winbundle-0.1.0.post1/winbundle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-07-15 20:56:31.000000 winbundle-0.1.0.post1/winbundle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 20:56:31.000000 winbundle-0.1.0.post1/winbundle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-15 20:56:31.000000 winbundle-0.1.0.post1/winbundle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-15 20:56:31.000000 winbundle-0.1.0.post1/winbundle.egg-info/top_level.txt
```

### Comparing `winbundle-0.1.0/LICENSE` & `winbundle-0.1.0.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `winbundle-0.1.0/winbundle/__main__.py` & `winbundle-0.1.0.post1/winbundle/__main__.py`

 * *Files identical despite different names*

### Comparing `winbundle-0.1.0/winbundle/builder.py` & `winbundle-0.1.0.post1/winbundle/builder.py`

 * *Files identical despite different names*

### Comparing `winbundle-0.1.0/winbundle/newconfig.py` & `winbundle-0.1.0.post1/winbundle/newconfig.py`

 * *Files identical despite different names*

### Comparing `winbundle-0.1.0/winbundle/util.py` & `winbundle-0.1.0.post1/winbundle/util.py`

 * *Files identical despite different names*

