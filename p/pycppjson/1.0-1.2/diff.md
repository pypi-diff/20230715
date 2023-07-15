# Comparing `tmp/pycppjson-1.0.tar.gz` & `tmp/pycppjson-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycppjson-1.0.tar", last modified: Fri Mar 31 05:44:12 2023, max compression
+gzip compressed data, was "pycppjson-1.2.tar", last modified: Sat Jul 15 05:58:57 2023, max compression
```

## Comparing `pycppjson-1.0.tar` & `pycppjson-1.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 05:44:12.508557 pycppjson-1.0/
--rw-rw-rw-   0        0        0     1091 2023-01-20 14:48:20.000000 pycppjson-1.0/LICENSE
--rw-rw-rw-   0        0        0      600 2023-03-31 05:44:12.508557 pycppjson-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      451 2023-02-23 06:34:00.000000 pycppjson-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-31 05:44:12.503559 pycppjson-1.0/pycppjson/
--rw-rw-rw-   0        0        0       87 2023-02-23 06:04:22.000000 pycppjson-1.0/pycppjson/__init__.py
--rw-rw-rw-   0        0        0      278 2023-02-23 06:02:06.000000 pycppjson-1.0/pycppjson/dumper.py
--rw-rw-rw-   0        0        0      301 2023-02-23 06:02:04.000000 pycppjson-1.0/pycppjson/loader.py
-drwxrwxrwx   0        0        0        0 2023-03-31 05:44:12.508557 pycppjson-1.0/pycppjson.egg-info/
--rw-rw-rw-   0        0        0      600 2023-03-31 05:44:12.000000 pycppjson-1.0/pycppjson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-03-31 05:44:12.000000 pycppjson-1.0/pycppjson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 05:44:12.000000 pycppjson-1.0/pycppjson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-03-31 05:44:12.000000 pycppjson-1.0/pycppjson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      718 2023-03-31 05:43:01.000000 pycppjson-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-31 05:44:12.508557 pycppjson-1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-15 05:58:57.994303 pycppjson-1.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-15 05:27:13.000000 pycppjson-1.2/LICENSE
+-rw-rw-rw-   0        0        0      154 2023-07-15 05:58:57.994303 pycppjson-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      557 2023-07-15 05:56:03.000000 pycppjson-1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 05:58:57.980303 pycppjson-1.2/pycppjson/
+-rw-rw-rw-   0        0        0      388 2023-07-15 05:42:40.000000 pycppjson-1.2/pycppjson/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 05:58:57.994303 pycppjson-1.2/pycppjson.egg-info/
+-rw-rw-rw-   0        0        0      154 2023-07-15 05:58:57.000000 pycppjson-1.2/pycppjson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-07-15 05:58:57.000000 pycppjson-1.2/pycppjson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 05:58:57.000000 pycppjson-1.2/pycppjson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-15 05:58:57.000000 pycppjson-1.2/pycppjson.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       24 2023-07-15 05:58:57.000000 pycppjson-1.2/pycppjson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 05:58:57.996304 pycppjson-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      391 2023-07-15 05:58:55.000000 pycppjson-1.2/setup.py
```

### Comparing `pycppjson-1.0/LICENSE` & `pycppjson-1.2/LICENSE`

 * *Files identical despite different names*

