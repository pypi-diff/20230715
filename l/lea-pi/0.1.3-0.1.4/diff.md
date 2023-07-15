# Comparing `tmp/lea_pi-0.1.3.tar.gz` & `tmp/lea_pi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lea_pi-0.1.3.tar", max compression
+gzip compressed data, was "lea_pi-0.1.4.tar", max compression
```

## Comparing `lea_pi-0.1.3.tar` & `lea_pi-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0       59 2023-07-15 07:22:18.737195 lea_pi-0.1.3/README.md
--rw-r--r--   0        0        0      368 2023-07-15 07:50:05.923452 lea_pi-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      204 2023-07-15 07:24:20.551627 lea_pi-0.1.3/src/k.py
--rw-r--r--   0        0        0        0 2023-07-15 07:16:57.650801 lea_pi-0.1.3/src/lea_pi/__init__.py
--rw-r--r--   0        0        0      205 2023-07-15 07:23:53.678430 lea_pi-0.1.3/src/lea_pi/main.py
--rw-r--r--   0        0        0      455 1970-01-01 00:00:00.000000 lea_pi-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       59 2023-07-15 07:22:18.737195 lea_pi-0.1.4/README.md
+-rw-r--r--   0        0        0      330 2023-07-15 07:52:16.442210 lea_pi-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-15 07:16:57.650801 lea_pi-0.1.4/src/lea_pi/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-15 07:52:07.455074 lea_pi-0.1.4/src/lea_pi/main.py
+-rw-r--r--   0        0        0      455 1970-01-01 00:00:00.000000 lea_pi-0.1.4/PKG-INFO
```

