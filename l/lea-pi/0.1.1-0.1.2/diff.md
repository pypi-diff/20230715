# Comparing `tmp/lea_pi-0.1.1.tar.gz` & `tmp/lea_pi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lea_pi-0.1.1.tar", max compression
+gzip compressed data, was "lea_pi-0.1.2.tar", max compression
```

## Comparing `lea_pi-0.1.1.tar` & `lea_pi-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       59 2023-07-15 07:22:18.737195 lea_pi-0.1.1/README.md
--rw-r--r--   0        0        0      325 2023-07-15 07:28:15.158768 lea_pi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      204 2023-07-15 07:24:20.551627 lea_pi-0.1.1/src/k.py
--rw-r--r--   0        0        0        0 2023-07-15 07:16:57.650801 lea_pi-0.1.1/src/lea_pi/__init__.py
--rw-r--r--   0        0        0      205 2023-07-15 07:23:53.678430 lea_pi-0.1.1/src/lea_pi/main.py
--rw-r--r--   0        0        0      455 1970-01-01 00:00:00.000000 lea_pi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-07-15 07:22:18.737195 lea_pi-0.1.2/README.md
+-rw-r--r--   0        0        0      325 2023-07-15 07:42:26.747069 lea_pi-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      204 2023-07-15 07:24:20.551627 lea_pi-0.1.2/src/k.py
+-rw-r--r--   0        0        0        0 2023-07-15 07:16:57.650801 lea_pi-0.1.2/src/lea_pi/__init__.py
+-rw-r--r--   0        0        0      205 2023-07-15 07:23:53.678430 lea_pi-0.1.2/src/lea_pi/main.py
+-rw-r--r--   0        0        0      455 1970-01-01 00:00:00.000000 lea_pi-0.1.2/PKG-INFO
```

