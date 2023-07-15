# Comparing `tmp/runpandarun-0.1rc4.tar.gz` & `tmp/runpandarun-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/runpandarun-0.1rc4.tar", last modified: Wed Apr  8 13:04:09 2020, max compression
+gzip compressed data, was "runpandarun-0.2.1.tar", max compression
```

## Comparing `runpandarun-0.1rc4.tar` & `runpandarun-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-04-08 13:04:09.047204 runpandarun-0.1rc4/
--rw-r--r--   0 runner    (1001) docker     (115)       19 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (115)    18443 2020-04-08 13:04:09.047204 runpandarun-0.1rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)    13565 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-04-08 13:04:09.043203 runpandarun-0.1rc4/runpandarun/
--rw-r--r--   0 runner    (1001) docker     (115)      527 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     3043 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/cli.py
--rw-r--r--   0 runner    (1001) docker     (115)      702 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/columns.py
--rw-r--r--   0 runner    (1001) docker     (115)      625 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/combine.py
--rw-r--r--   0 runner    (1001) docker     (115)     2761 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/config.py
--rw-r--r--   0 runner    (1001) docker     (115)     3840 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/dataset.py
--rw-r--r--   0 runner    (1001) docker     (115)       79 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (115)      802 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/index.py
--rw-r--r--   0 runner    (1001) docker     (115)      776 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/load.py
--rw-r--r--   0 runner    (1001) docker     (115)      994 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/ops.py
--rw-r--r--   0 runner    (1001) docker     (115)     2480 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/publish.py
--rw-r--r--   0 runner    (1001) docker     (115)     1139 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/revisions.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-04-08 13:04:09.047204 runpandarun-0.1rc4/runpandarun/storage/
--rw-r--r--   0 runner    (1001) docker     (115)     1242 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     1808 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/storage/backend.py
--rw-r--r--   0 runner    (1001) docker     (115)      947 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/storage/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (115)     2045 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/storage/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (115)     6504 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (115)     3222 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/store.py
--rw-r--r--   0 runner    (1001) docker     (115)     4863 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/runpandarun/util.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-04-08 13:04:09.043203 runpandarun-0.1rc4/runpandarun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)    18443 2020-04-08 13:04:08.000000 runpandarun-0.1rc4/runpandarun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)      744 2020-04-08 13:04:08.000000 runpandarun-0.1rc4/runpandarun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-04-08 13:04:08.000000 runpandarun-0.1rc4/runpandarun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)       54 2020-04-08 13:04:08.000000 runpandarun-0.1rc4/runpandarun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-04-08 13:04:08.000000 runpandarun-0.1rc4/runpandarun.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (115)       82 2020-04-08 13:04:08.000000 runpandarun-0.1rc4/runpandarun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)       12 2020-04-08 13:04:08.000000 runpandarun-0.1rc4/runpandarun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (115)       38 2020-04-08 13:04:09.047204 runpandarun-0.1rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)     1109 2020-04-08 13:03:58.000000 runpandarun-0.1rc4/setup.py
+-rw-r--r--   0        0        0     1070 2023-07-15 09:47:01.438078 runpandarun-0.2.1/LICENSE
+-rw-r--r--   0        0        0     9271 2023-07-15 09:47:01.438078 runpandarun-0.2.1/README.md
+-rw-r--r--   0        0        0     1345 2023-07-15 09:55:53.530736 runpandarun-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-07-15 09:55:53.530736 runpandarun-0.2.1/runpandarun/__init__.py
+-rw-r--r--   0        0        0      618 2023-07-15 09:47:01.438078 runpandarun-0.2.1/runpandarun/cli.py
+-rw-r--r--   0        0        0       37 2023-07-15 09:47:01.438078 runpandarun-0.2.1/runpandarun/exceptions.py
+-rw-r--r--   0        0        0     1853 2023-07-15 09:47:01.438078 runpandarun-0.2.1/runpandarun/io.py
+-rw-r--r--   0        0        0     2304 2023-07-15 09:47:01.438078 runpandarun-0.2.1/runpandarun/playbook.py
+-rw-r--r--   0        0        0     1770 2023-07-15 09:47:01.438078 runpandarun-0.2.1/runpandarun/util.py
+-rw-r--r--   0        0        0    10496 1970-01-01 00:00:00.000000 runpandarun-0.2.1/PKG-INFO
```

