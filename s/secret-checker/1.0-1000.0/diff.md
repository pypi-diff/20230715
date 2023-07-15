# Comparing `tmp/secret_checker-1.0.tar.gz` & `tmp/secret_checker-1000.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secret_checker-1.0.tar", last modified: Sat Jul 15 01:40:50 2023, max compression
+gzip compressed data, was "secret_checker-1000.0.tar", last modified: Sat Jul 15 15:14:07 2023, max compression
```

## Comparing `secret_checker-1.0.tar` & `secret_checker-1000.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 01:40:50.792290 secret_checker-1.0/
--rw-rw-rw-   0        0        0      240 2023-07-15 01:40:50.792290 secret_checker-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-07-15 01:11:16.000000 secret_checker-1.0/README.md
--rw-rw-rw-   0        0        0        0 2023-07-15 01:37:29.000000 secret_checker-1.0/__init__.py
--rw-rw-rw-   0        0        0     3533 2023-07-15 01:11:16.000000 secret_checker-1.0/detect_prod_env.py
-drwxrwxrwx   0        0        0        0 2023-07-15 01:40:50.776683 secret_checker-1.0/secret_checker.egg-info/
--rw-rw-rw-   0        0        0      240 2023-07-15 01:40:50.000000 secret_checker-1.0/secret_checker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-07-15 01:40:50.000000 secret_checker-1.0/secret_checker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 01:40:50.000000 secret_checker-1.0/secret_checker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 01:40:50.000000 secret_checker-1.0/secret_checker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 01:40:50.792290 secret_checker-1.0/setup.cfg
--rw-rw-rw-   0        0        0      340 2023-07-15 01:40:35.000000 secret_checker-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 15:14:07.969776 secret_checker-1000.0/
+-rw-rw-rw-   0        0        0      243 2023-07-15 15:14:07.969776 secret_checker-1000.0/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-07-15 01:11:16.000000 secret_checker-1000.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 15:14:07.954652 secret_checker-1000.0/secret_checker/
+-rw-rw-rw-   0        0        0      111 2023-07-15 15:09:30.000000 secret_checker-1000.0/secret_checker/__init__.py
+-rw-rw-rw-   0        0        0     3533 2023-07-15 14:46:22.000000 secret_checker-1000.0/secret_checker/check_var.py
+drwxrwxrwx   0        0        0        0 2023-07-15 15:14:07.969776 secret_checker-1000.0/secret_checker.egg-info/
+-rw-rw-rw-   0        0        0      243 2023-07-15 15:14:07.000000 secret_checker-1000.0/secret_checker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-15 15:14:07.000000 secret_checker-1000.0/secret_checker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 15:14:07.000000 secret_checker-1000.0/secret_checker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-15 15:14:07.000000 secret_checker-1000.0/secret_checker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 15:14:07.969776 secret_checker-1000.0/setup.cfg
+-rw-rw-rw-   0        0        0      357 2023-07-15 15:13:31.000000 secret_checker-1000.0/setup.py
```

### Comparing `secret_checker-1.0/detect_prod_env.py` & `secret_checker-1000.0/secret_checker/check_var.py`

 * *Files identical despite different names*

