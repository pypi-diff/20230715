# Comparing `tmp/waterfly-15.7.2023.tar.gz` & `tmp/waterfly-8.7.2023.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waterfly-15.7.2023.tar", last modified: Sat Jul 15 17:51:50 2023, max compression
+gzip compressed data, was "waterfly-8.7.2023.tar", last modified: Sat Jul  8 18:40:09 2023, max compression
```

## Comparing `waterfly-15.7.2023.tar` & `waterfly-8.7.2023.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 17:51:50.236295 waterfly-15.7.2023/
--rw-rw-rw-   0        0        0     3923 2023-07-15 17:51:50.236295 waterfly-15.7.2023/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-15 17:51:50.236295 waterfly-15.7.2023/setup.cfg
--rw-rw-rw-   0        0        0     4206 2023-07-15 17:09:18.000000 waterfly-15.7.2023/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 17:51:50.220674 waterfly-15.7.2023/waterfly/
--rw-rw-rw-   0        0        0    36600 2023-07-15 17:03:08.000000 waterfly-15.7.2023/waterfly/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 17:51:50.236295 waterfly-15.7.2023/waterfly.egg-info/
--rw-rw-rw-   0        0        0     3923 2023-07-15 17:51:50.000000 waterfly-15.7.2023/waterfly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-07-15 17:51:50.000000 waterfly-15.7.2023/waterfly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 17:51:50.000000 waterfly-15.7.2023/waterfly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-15 17:51:50.000000 waterfly-15.7.2023/waterfly.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-15 17:51:50.000000 waterfly-15.7.2023/waterfly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 18:40:09.640290 waterfly-8.7.2023/
+-rw-rw-rw-   0        0        0     1822 2023-07-08 18:40:09.640290 waterfly-8.7.2023/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-08 18:40:09.640290 waterfly-8.7.2023/setup.cfg
+-rw-rw-rw-   0        0        0     2173 2023-07-08 18:34:35.000000 waterfly-8.7.2023/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:40:09.593429 waterfly-8.7.2023/waterfly/
+-rw-rw-rw-   0        0        0     7887 2023-07-08 17:40:07.000000 waterfly-8.7.2023/waterfly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:40:09.640290 waterfly-8.7.2023/waterfly.egg-info/
+-rw-rw-rw-   0        0        0     1822 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/top_level.txt
```

