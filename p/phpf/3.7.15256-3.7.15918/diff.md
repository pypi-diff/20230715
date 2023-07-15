# Comparing `tmp/phpf-3.7.15256.tar.gz` & `tmp/phpf-3.7.15918.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phpf-3.7.15256.tar", last modified: Sat Jul 15 02:56:41 2023, max compression
+gzip compressed data, was "phpf-3.7.15918.tar", last modified: Sat Jul 15 09:19:17 2023, max compression
```

## Comparing `phpf-3.7.15256.tar` & `phpf-3.7.15918.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 02:56:41.490992 phpf-3.7.15256/
--rw-rw-rw-   0        0        0      829 2023-07-15 02:56:38.000000 phpf-3.7.15256/LICENSE
--rw-rw-rw-   0        0        0      204 2023-07-15 02:56:41.490992 phpf-3.7.15256/PKG-INFO
--rw-rw-rw-   0        0        0       81 2023-07-15 02:56:38.000000 phpf-3.7.15256/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 02:56:41.475362 phpf-3.7.15256/phpf/
--rw-rw-rw-   0        0        0    18184 2023-07-15 02:56:38.000000 phpf-3.7.15256/phpf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 02:56:41.490992 phpf-3.7.15256/phpf.egg-info/
--rw-rw-rw-   0        0        0      204 2023-07-15 02:56:41.000000 phpf-3.7.15256/phpf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      155 2023-07-15 02:56:41.000000 phpf-3.7.15256/phpf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 02:56:41.000000 phpf-3.7.15256/phpf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-07-15 02:56:41.000000 phpf-3.7.15256/phpf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 02:56:41.490992 phpf-3.7.15256/setup.cfg
--rw-rw-rw-   0        0        0      376 2023-07-15 02:56:38.000000 phpf-3.7.15256/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:19:17.085143 phpf-3.7.15918/
+-rw-rw-rw-   0        0        0      829 2023-07-15 09:18:31.000000 phpf-3.7.15918/LICENSE
+-rw-rw-rw-   0        0        0      204 2023-07-15 09:19:17.084275 phpf-3.7.15918/PKG-INFO
+-rw-rw-rw-   0        0        0       81 2023-07-15 09:18:31.000000 phpf-3.7.15918/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 09:19:17.062277 phpf-3.7.15918/phpf/
+-rw-rw-rw-   0        0        0    23611 2023-07-15 09:18:31.000000 phpf-3.7.15918/phpf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:19:17.081276 phpf-3.7.15918/phpf.egg-info/
+-rw-rw-rw-   0        0        0      204 2023-07-15 09:19:16.000000 phpf-3.7.15918/phpf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      155 2023-07-15 09:19:16.000000 phpf-3.7.15918/phpf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 09:19:16.000000 phpf-3.7.15918/phpf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-07-15 09:19:16.000000 phpf-3.7.15918/phpf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 09:19:17.085143 phpf-3.7.15918/setup.cfg
+-rw-rw-rw-   0        0        0      376 2023-07-15 09:18:31.000000 phpf-3.7.15918/setup.py
```

### Comparing `phpf-3.7.15256/LICENSE` & `phpf-3.7.15918/LICENSE`

 * *Files identical despite different names*

