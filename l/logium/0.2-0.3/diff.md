# Comparing `tmp/logium-0.2.tar.gz` & `tmp/logium-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logium-0.2.tar", last modified: Fri Jul 14 19:24:49 2023, max compression
+gzip compressed data, was "logium-0.3.tar", last modified: Sat Jul 15 21:22:22 2023, max compression
```

## Comparing `logium-0.2.tar` & `logium-0.3.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 19:24:48.998425 logium-0.2/
--rw-rw-rw-   0        0        0      157 2023-07-14 19:24:48.998425 logium-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-14 19:24:48.946737 logium-0.2/logium/
--rw-rw-rw-   0        0        0     2785 2023-07-14 19:23:45.000000 logium-0.2/logium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 19:24:48.998425 logium-0.2/logium.egg-info/
--rw-rw-rw-   0        0        0      157 2023-07-14 19:24:48.000000 logium-0.2/logium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2023-07-14 19:24:48.000000 logium-0.2/logium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 19:24:48.000000 logium-0.2/logium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-14 19:24:48.000000 logium-0.2/logium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 19:24:49.006434 logium-0.2/setup.cfg
--rw-rw-rw-   0        0        0      388 2023-07-14 19:24:11.000000 logium-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 21:22:22.658045 logium-0.3/
+-rw-rw-rw-   0        0        0      157 2023-07-15 21:22:22.658045 logium-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-15 21:22:22.621104 logium-0.3/logium/
+-rw-rw-rw-   0        0        0     2301 2023-07-15 21:21:22.000000 logium-0.3/logium/__init__.py
+-rw-rw-rw-   0        0        0      510 2023-07-15 20:34:17.000000 logium-0.3/logium/decorators.py
+-rw-rw-rw-   0        0        0     3545 2023-07-15 21:03:12.000000 logium-0.3/logium/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-15 21:22:22.658045 logium-0.3/logium.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-07-15 21:22:22.000000 logium-0.3/logium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-07-15 21:22:22.000000 logium-0.3/logium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 21:22:22.000000 logium-0.3/logium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-15 21:22:22.000000 logium-0.3/logium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 21:22:22.666027 logium-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      388 2023-07-15 21:20:36.000000 logium-0.3/setup.py
```

