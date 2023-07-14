# Comparing `tmp/PyMenus-0.2.0.tar.gz` & `tmp/PyMenus-66.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMenus-0.2.0.tar", last modified: Fri Jul 14 22:24:56 2023, max compression
+gzip compressed data, was "PyMenus-66.0.0.tar", last modified: Wed Feb  8 15:28:24 2023, max compression
```

## Comparing `PyMenus-0.2.0.tar` & `PyMenus-66.0.0.tar`

### file list

```diff
@@ -1,21 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 22:24:56.446378 PyMenus-0.2.0/
--rw-rw-rw-   0        0        0       66 2023-07-10 08:42:05.000000 PyMenus-0.2.0/.gitattributes
--rw-rw-rw-   0        0        0     2940 2023-07-13 23:55:54.000000 PyMenus-0.2.0/.gitignore
--rw-rw-rw-   0        0        0    27011 2023-07-10 08:42:05.000000 PyMenus-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       18 2023-07-14 22:23:28.000000 PyMenus-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2642 2023-07-14 22:24:56.443372 PyMenus-0.2.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-14 22:24:56.413371 PyMenus-0.2.0/PyMenus.egg-info/
--rw-rw-rw-   0        0        0     2642 2023-07-14 22:24:56.000000 PyMenus-0.2.0/PyMenus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-07-14 22:24:56.000000 PyMenus-0.2.0/PyMenus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 22:24:56.000000 PyMenus-0.2.0/PyMenus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-14 22:24:56.000000 PyMenus-0.2.0/PyMenus.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-14 22:24:56.000000 PyMenus-0.2.0/PyMenus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2143 2023-07-13 23:55:54.000000 PyMenus-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 22:24:56.438370 PyMenus-0.2.0/pymenus/
--rw-rw-rw-   0        0        0      118 2023-07-14 22:11:59.000000 PyMenus-0.2.0/pymenus/__init__.py
--rw-rw-rw-   0        0        0     3601 2023-07-14 22:07:50.000000 PyMenus-0.2.0/pymenus/base.py
--rw-rw-rw-   0        0        0     4141 2023-07-14 22:10:44.000000 PyMenus-0.2.0/pymenus/menu.py
--rw-rw-rw-   0        0        0      335 2023-07-14 22:07:37.000000 PyMenus-0.2.0/pymenus/option.py
--rw-rw-rw-   0        0        0     3821 2023-07-14 22:09:41.000000 PyMenus-0.2.0/pymenus/structual_menu.py
--rw-rw-rw-   0        0        0      776 2023-07-14 22:22:38.000000 PyMenus-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-14 22:24:56.447372 PyMenus-0.2.0/setup.cfg
+drwxrwxr-x   0 ezzer     (1000) ezzer     (1001)        0 2023-02-08 15:28:24.608459 PyMenus-66.0.0/
+-rw-rw-r--   0 ezzer     (1000) ezzer     (1001)      482 2023-02-08 15:28:24.608459 PyMenus-66.0.0/PKG-INFO
+drwxrwxr-x   0 ezzer     (1000) ezzer     (1001)        0 2023-02-08 15:28:24.608459 PyMenus-66.0.0/PyMenus.egg-info/
+-rw-rw-r--   0 ezzer     (1000) ezzer     (1001)      482 2023-02-08 15:28:24.000000 PyMenus-66.0.0/PyMenus.egg-info/PKG-INFO
+-rw-rw-r--   0 ezzer     (1000) ezzer     (1001)      142 2023-02-08 15:28:24.000000 PyMenus-66.0.0/PyMenus.egg-info/SOURCES.txt
+-rw-rw-r--   0 ezzer     (1000) ezzer     (1001)        1 2023-02-08 15:28:24.000000 PyMenus-66.0.0/PyMenus.egg-info/dependency_links.txt
+-rw-rw-r--   0 ezzer     (1000) ezzer     (1001)        1 2023-02-08 15:28:24.000000 PyMenus-66.0.0/PyMenus.egg-info/top_level.txt
+-rw-r--r--   0 ezzer     (1000) ezzer     (1001)      172 2023-02-08 15:28:24.000000 PyMenus-66.0.0/README.md
+-rw-rw-r--   0 ezzer     (1000) ezzer     (1001)       38 2023-02-08 15:28:24.608459 PyMenus-66.0.0/setup.cfg
+-rw-r--r--   0 ezzer     (1000) ezzer     (1001)      526 2023-02-08 15:28:24.000000 PyMenus-66.0.0/setup.py
```

