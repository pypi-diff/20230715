# Comparing `tmp/wiggler_studiorabota-0.0.3.tar.gz` & `tmp/wiggler_studiorabota-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiggler_studiorabota-0.0.3.tar", last modified: Sat Jul 15 09:27:52 2023, max compression
+gzip compressed data, was "wiggler_studiorabota-0.0.4.tar", last modified: Sat Jul 15 09:40:27 2023, max compression
```

## Comparing `wiggler_studiorabota-0.0.3.tar` & `wiggler_studiorabota-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 09:27:52.914066 wiggler_studiorabota-0.0.3/
--rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-15 09:27:52.913896 wiggler_studiorabota-0.0.3/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)       91 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.3/README.md
--rw-r--r--   0 vincent    (501) staff       (20)      458 2023-07-15 09:27:39.000000 wiggler_studiorabota-0.0.3/pyproject.toml
--rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-15 09:27:52.914108 wiggler_studiorabota-0.0.3/setup.cfg
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 09:27:52.912706 wiggler_studiorabota-0.0.3/wiggler/
--rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.3/wiggler/__init__.py
--rw-r--r--   0 vincent    (501) staff       (20)      318 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.3/wiggler/cli.py
--rw-r--r--   0 vincent    (501) staff       (20)      823 2023-07-15 09:26:59.000000 wiggler_studiorabota-0.0.3/wiggler/main.py
-drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 09:27:52.913588 wiggler_studiorabota-0.0.3/wiggler_studiorabota.egg-info/
--rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-15 09:27:52.000000 wiggler_studiorabota-0.0.3/wiggler_studiorabota.egg-info/PKG-INFO
--rw-r--r--   0 vincent    (501) staff       (20)      298 2023-07-15 09:27:52.000000 wiggler_studiorabota-0.0.3/wiggler_studiorabota.egg-info/SOURCES.txt
--rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-15 09:27:52.000000 wiggler_studiorabota-0.0.3/wiggler_studiorabota.egg-info/dependency_links.txt
--rw-r--r--   0 vincent    (501) staff       (20)       45 2023-07-15 09:27:52.000000 wiggler_studiorabota-0.0.3/wiggler_studiorabota.egg-info/entry_points.txt
--rw-r--r--   0 vincent    (501) staff       (20)        8 2023-07-15 09:27:52.000000 wiggler_studiorabota-0.0.3/wiggler_studiorabota.egg-info/top_level.txt
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 09:40:27.280576 wiggler_studiorabota-0.0.4/
+-rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-15 09:40:27.280414 wiggler_studiorabota-0.0.4/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)       91 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.4/README.md
+-rw-r--r--   0 vincent    (501) staff       (20)      458 2023-07-15 09:40:11.000000 wiggler_studiorabota-0.0.4/pyproject.toml
+-rw-r--r--   0 vincent    (501) staff       (20)       38 2023-07-15 09:40:27.280618 wiggler_studiorabota-0.0.4/setup.cfg
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 09:40:27.278994 wiggler_studiorabota-0.0.4/wiggler/
+-rw-r--r--   0 vincent    (501) staff       (20)        0 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.4/wiggler/__init__.py
+-rw-r--r--   0 vincent    (501) staff       (20)      318 2023-07-15 09:18:49.000000 wiggler_studiorabota-0.0.4/wiggler/cli.py
+-rw-r--r--   0 vincent    (501) staff       (20)      859 2023-07-15 09:39:58.000000 wiggler_studiorabota-0.0.4/wiggler/main.py
+drwxr-xr-x   0 vincent    (501) staff       (20)        0 2023-07-15 09:40:27.280160 wiggler_studiorabota-0.0.4/wiggler_studiorabota.egg-info/
+-rw-r--r--   0 vincent    (501) staff       (20)      483 2023-07-15 09:40:27.000000 wiggler_studiorabota-0.0.4/wiggler_studiorabota.egg-info/PKG-INFO
+-rw-r--r--   0 vincent    (501) staff       (20)      298 2023-07-15 09:40:27.000000 wiggler_studiorabota-0.0.4/wiggler_studiorabota.egg-info/SOURCES.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        1 2023-07-15 09:40:27.000000 wiggler_studiorabota-0.0.4/wiggler_studiorabota.egg-info/dependency_links.txt
+-rw-r--r--   0 vincent    (501) staff       (20)       45 2023-07-15 09:40:27.000000 wiggler_studiorabota-0.0.4/wiggler_studiorabota.egg-info/entry_points.txt
+-rw-r--r--   0 vincent    (501) staff       (20)        8 2023-07-15 09:40:27.000000 wiggler_studiorabota-0.0.4/wiggler_studiorabota.egg-info/top_level.txt
```

