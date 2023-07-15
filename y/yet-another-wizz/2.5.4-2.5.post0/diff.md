# Comparing `tmp/yet_another_wizz-2.5.4.tar.gz` & `tmp/yet_another_wizz-2.5.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yet_another_wizz-2.5.4.tar", last modified: Sat Jul 15 14:11:16 2023, max compression
+gzip compressed data, was "yet_another_wizz-2.5.post0.tar", last modified: Mon Jul 10 08:18:48 2023, max compression
```

## Comparing `yet_another_wizz-2.5.4.tar` & `yet_another_wizz-2.5.post0.tar`

### file list

```diff
@@ -1,64 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:11:16.836363 yet_another_wizz-2.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-15 14:11:16.836363 yet_another_wizz-2.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 14:11:16.836363 yet_another_wizz-2.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:11:16.828363 yet_another_wizz-2.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:11:16.828363 yet_another_wizz-2.5.4/src/yaw/
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:11:16.828363 yet_another_wizz-2.5.4/src/yaw/catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/catalogs/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/catalogs/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/catalogs/linkage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:11:16.828363 yet_another_wizz-2.5.4/src/yaw/catalogs/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/catalogs/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/catalogs/scipy/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/catalogs/scipy/kdtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/catalogs/scipy/patches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:11:16.828363 yet_another_wizz-2.5.4/src/yaw/catalogs/treecorr/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/catalogs/treecorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15092 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/catalogs/treecorr/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:11:16.832363 yet_another_wizz-2.5.4/src/yaw/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/config/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/config/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)    15324 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/config/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/config/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/config/resampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/config/scales.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:11:16.832363 yet_another_wizz-2.5.4/src/yaw/core/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9840 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/core/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16139 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/core/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/core/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/core/cosmology.py
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/core/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/core/math.c
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/core/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/core/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:11:16.832363 yet_another_wizz-2.5.4/src/yaw/correlation/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/correlation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40339 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/correlation/corrfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/correlation/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)    41097 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/correlation/paircounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/deprecated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:11:16.836363 yet_another_wizz-2.5.4/src/yaw/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   129479 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/examples/auto_reference.hdf
--rw-r--r--   0 runner    (1001) docker     (123)   123032 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/examples/auto_unknown_1.hdf
--rw-r--r--   0 runner    (1001) docker     (123)   100475 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/examples/cross_1.hdf
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/randoms.py
--rw-r--r--   0 runner    (1001) docker     (123)    22167 2023-07-15 14:09:23.000000 yet_another_wizz-2.5.4/src/yaw/redshifts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:11:16.836363 yet_another_wizz-2.5.4/src/yet_another_wizz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-07-15 14:11:16.000000 yet_another_wizz-2.5.4/src/yet_another_wizz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-15 14:11:16.000000 yet_another_wizz-2.5.4/src/yet_another_wizz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 14:11:16.000000 yet_another_wizz-2.5.4/src/yet_another_wizz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-15 14:11:16.000000 yet_another_wizz-2.5.4/src/yet_another_wizz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-15 14:11:16.000000 yet_another_wizz-2.5.4/src/yet_another_wizz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.342015 yet_another_wizz-2.5.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-10 08:18:48.342015 yet_another_wizz-2.5.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 08:18:48.342015 yet_another_wizz-2.5.post0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.318014 yet_another_wizz-2.5.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.322014 yet_another_wizz-2.5.post0/src/yaw/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.322014 yet_another_wizz-2.5.post0/src/yaw/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/linkage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.326015 yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/patches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.326015 yet_another_wizz-2.5.post0/src/yaw/catalogs/treecorr/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/treecorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15092 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/catalogs/treecorr/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.330015 yet_another_wizz-2.5.post0/src/yaw/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14829 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/resampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/scales.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.334015 yet_another_wizz-2.5.post0/src/yaw/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16139 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/cosmology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/math.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.334015 yet_another_wizz-2.5.post0/src/yaw/correlation/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/correlation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40475 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/correlation/corrfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/correlation/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41424 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/correlation/paircounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/deprecated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.334015 yet_another_wizz-2.5.post0/src/yaw/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129479 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/examples/auto_reference.hdf
+-rw-r--r--   0 runner    (1001) docker     (123)   123032 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/examples/auto_unknown_1.hdf
+-rw-r--r--   0 runner    (1001) docker     (123)   100475 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/examples/cross_1.hdf
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/randoms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22413 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw/redshifts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.338015 yet_another_wizz-2.5.post0/src/yaw_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.338015 yet_another_wizz-2.5.post0/src/yaw_cli/commandline/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/commandline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/commandline/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17458 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/commandline/subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/commandline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.338015 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17790 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/default_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18945 2023-07-10 08:16:37.000000 yet_another_wizz-2.5.post0/src/yaw_cli/pipeline/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:18:48.342015 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-10 08:18:48.000000 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-10 08:18:48.000000 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:18:48.000000 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 08:18:48.000000 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-10 08:18:48.000000 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 08:18:48.000000 yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/top_level.txt
```

### Comparing `yet_another_wizz-2.5.4/LICENSE` & `yet_another_wizz-2.5.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/PKG-INFO` & `yet_another_wizz-2.5.post0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 Metadata-Version: 2.1
 Name: yet_another_wizz
-Version: 2.5.4
-Summary: Implementation of the Schmidt et al. (2013) clustering redshift method.
+Version: 2.5.post0
+Summary: Implementation of the Schmidt et al. (2013) clustering redshift method and wrapper scripts to produce cross-correlation (CC) redshifts.
 Home-page: https://github.com/jlvdb/yet_another_wizz.git
 Author-email: Jan Luca van den Busch <jlvdb@astro.ruhr-uni-bochum.de>
 License: GPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: cli
 Provides-Extra: plot
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: style
 Provides-Extra: dev
 License-File: LICENSE
 
-.. image:: https://raw.githubusercontent.com/jlvdb/yet_another_wizz/main/docs/source/_static/logo-dark.png
-    :width: 1000
-    :alt: yet_another_wizz
+yet_another_wizz
+================
 
-|
-
-.. image:: https://img.shields.io/pypi/v/yet_another_wizz?logo=pypi&logoColor=blue
-    :target: https://pypi.org/project/yet_another_wizz/
+.. image:: https://badge.fury.io/py/yet-another-wizz.svg
+    :target: https://badge.fury.io/py/yet-another-wizz
 .. image:: https://readthedocs.org/projects/yet-another-wizz/badge/?version=latest
     :target: https://yet-another-wizz.readthedocs.io/en/latest/?badge=latest
 .. image:: https://github.com/jlvdb/yet_another_wizz/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/jlvdb/yet_another_wizz/actions/workflows/run-tests.yml
 .. image:: https://codecov.io/gh/jlvdb/yet_another_wizz/branch/main/graph/badge.svg?token=PC41ME2AR8
     :target: https://codecov.io/gh/jlvdb/yet_another_wizz
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
     :target: https://pycqa.github.io/isort/
 
-|
 
 *yet_another_wizz* is a python package to efficiently compute cross-correlation
 redshifts, also know as clustering redshifts and is hosted on github:
 
 - code: https://github.com/jlvdb/yet_another_wizz.git
 - docs: https://yet-another-wizz.readthedocs.io/
 - PyPI: https://pypi.org/project/yet_another_wizz/
@@ -62,38 +57,29 @@
 Installation
 ------------
 
 The yet_another_wizz package can be installed directly with pip::
 
     pip install yet_another_wizz
 
-This will install the python library ``yaw``.
-
-Commandline tool
-~~~~~~~~~~~~~~~~
-
-There also exists a separate command line tool called
-`yet_another_wizz_cli <https://github.com/jlvdb/yet_another_wizz_cli>`_
-(``yaw_cli``) that is available at PyPI and github. To install it alongside the
-python library, type::
-
-    pip install yet_another_wizz[cli]
+This will install the python package ``yaw``, as well as the ``yaw_cli``
+executable command line tool.
 
 
 Usage
 -----
 
 There are two main ways to use yet_another_wizz,
 
-- the python library ``yaw`` itself and
-- the (separate) ``yaw_cli`` commmand line tool.
+- the ``yaw_cli`` commmand line tool and
+- the python package ``yaw`` directly.
 
 Most people will probably get started with the command line tool, which should
 cover all necessary tasks for a standard clustering redshift calibration. For
-custom solutions, use the python library. A basic example as well as the API
+custom solutions, use the python package. A basic example as well as the API
 reference can be found in the official documentation.
 
 
 Reporting bugs and requesting features
 --------------------------------------
 
 For bug reports or requesting new features, please use the github issue page:
```

### Comparing `yet_another_wizz-2.5.4/README.rst` & `yet_another_wizz-2.5.post0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,23 @@
-.. image:: https://raw.githubusercontent.com/jlvdb/yet_another_wizz/main/docs/source/_static/logo-dark.png
-    :width: 1000
-    :alt: yet_another_wizz
+yet_another_wizz
+================
 
-|
-
-.. image:: https://img.shields.io/pypi/v/yet_another_wizz?logo=pypi&logoColor=blue
-    :target: https://pypi.org/project/yet_another_wizz/
+.. image:: https://badge.fury.io/py/yet-another-wizz.svg
+    :target: https://badge.fury.io/py/yet-another-wizz
 .. image:: https://readthedocs.org/projects/yet-another-wizz/badge/?version=latest
     :target: https://yet-another-wizz.readthedocs.io/en/latest/?badge=latest
 .. image:: https://github.com/jlvdb/yet_another_wizz/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/jlvdb/yet_another_wizz/actions/workflows/run-tests.yml
 .. image:: https://codecov.io/gh/jlvdb/yet_another_wizz/branch/main/graph/badge.svg?token=PC41ME2AR8
     :target: https://codecov.io/gh/jlvdb/yet_another_wizz
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
     :target: https://pycqa.github.io/isort/
 
-|
 
 *yet_another_wizz* is a python package to efficiently compute cross-correlation
 redshifts, also know as clustering redshifts and is hosted on github:
 
 - code: https://github.com/jlvdb/yet_another_wizz.git
 - docs: https://yet-another-wizz.readthedocs.io/
 - PyPI: https://pypi.org/project/yet_another_wizz/
@@ -41,38 +37,29 @@
 Installation
 ------------
 
 The yet_another_wizz package can be installed directly with pip::
 
     pip install yet_another_wizz
 
-This will install the python library ``yaw``.
-
-Commandline tool
-~~~~~~~~~~~~~~~~
-
-There also exists a separate command line tool called
-`yet_another_wizz_cli <https://github.com/jlvdb/yet_another_wizz_cli>`_
-(``yaw_cli``) that is available at PyPI and github. To install it alongside the
-python library, type::
-
-    pip install yet_another_wizz[cli]
+This will install the python package ``yaw``, as well as the ``yaw_cli``
+executable command line tool.
 
 
 Usage
 -----
 
 There are two main ways to use yet_another_wizz,
 
-- the python library ``yaw`` itself and
-- the (separate) ``yaw_cli`` commmand line tool.
+- the ``yaw_cli`` commmand line tool and
+- the python package ``yaw`` directly.
 
 Most people will probably get started with the command line tool, which should
 cover all necessary tasks for a standard clustering redshift calibration. For
-custom solutions, use the python library. A basic example as well as the API
+custom solutions, use the python package. A basic example as well as the API
 reference can be found in the official documentation.
 
 
 Reporting bugs and requesting features
 --------------------------------------
 
 For bug reports or requesting new features, please use the github issue page:
```

### Comparing `yet_another_wizz-2.5.4/pyproject.toml` & `yet_another_wizz-2.5.post0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,51 +4,51 @@
 
 [project]
 name = "yet_another_wizz"
 dynamic = ["version"]
 authors = [
     {name = "Jan Luca van den Busch", email = "jlvdb@astro.ruhr-uni-bochum.de"},
 ]
-description = "Implementation of the Schmidt et al. (2013) clustering redshift method."
+description = "Implementation of the Schmidt et al. (2013) clustering redshift method and wrapper scripts to produce cross-correlation (CC) redshifts."
 readme = "README.rst"
 license = {text = "GPL-3.0-or-later"}
 classifiers = [
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Astronomy",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"
 ]
 requires-python = ">=3.8"
 dependencies = [
     "typing_extensions;python_version<'3.10'",
     "more_itertools;python_version<'3.10'",
     "deprecated",
-    "tqdm",
     "numpy",
+    "pyarrow",
+    "tqdm",
+    "h5py",
     "pandas",
     "astropandas>=1.2.1",
     "scipy",
     "astropy",
-    "pyarrow",
-    "h5py",
-    "pyyaml",
     "treecorr>=4.3",
+    "emcee",
     "matplotlib",
 ]
 
+[project.scripts]
+yaw_cli = "yaw_cli:Commandline.main"
+
 [project.optional-dependencies]
-cli = ["yet_another_wizz_cli>=1.2.1"]
 plot = ["matplotlib"]
-# note that yaw_cli is currently necessary to generate the joint docs
 docs = [
     "sphinx",
     "sphinx-design",
     "sphinx-copybutton",
     "pydata-sphinx-theme",
-    "yet_another_wizz[cli]",
 ]
 test = [
     "typing_extensions",
     "more_itertools",
     "coverage",
     "pytest",
     "pytest-cov",
@@ -77,21 +77,17 @@
     "examples/*.hdf",
     "examples/*.dat",
     "examples/*.cov",
     "examples/*.smp",
 ]
 
 [tool.pytest.ini_options]
-testpaths = [
-    "tests",
-]
-addopts = [
-    "--cov=yaw",
-    "--cov-report=xml",
-]
+minversion = "6.0"
+addopts = "-ra -q"
+testpaths = ["tests"]
 
 [tool.isort]
 profile = "black"
 
 [tool.black]
 include = ".pyi?$"
 exclude = """
```

### Comparing `yet_another_wizz-2.5.4/src/yaw/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     CorrelationFunction,
     HistogramData,
     PairCountResult,
 )
 from yaw.randoms import UniformRandoms
 from yaw.redshifts import HistData, RedshiftData
 
+__version__ = "2.5.post0"
+
 __all__ = [
     "NewCatalog",
     "Configuration",
     "ResamplingConfig",
     "Scale",
     "global_covariance",
     "CorrData",
@@ -52,8 +54,7 @@
     "RedshiftData",
     # deprecated
     "CorrelationData",
     "CorrelationFunction",
     "HistogramData",
     "PairCountResult",
 ]
-__version__ = "2.5.4"
```

### Comparing `yet_another_wizz-2.5.4/src/yaw/catalogs/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/catalogs/catalog.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/catalog.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/catalogs/factory.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/factory.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/catalogs/linkage.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/linkage.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/catalogs/scipy/catalog.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/catalog.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/catalogs/scipy/kdtree.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/kdtree.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/catalogs/scipy/patches.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/scipy/patches.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/catalogs/treecorr/catalog.py` & `yet_another_wizz-2.5.post0/src/yaw/catalogs/treecorr/catalog.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/config/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/config/backend.py` & `yet_another_wizz-2.5.post0/src/yaw/config/backend.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,22 +59,18 @@
     def __post_init__(self) -> None:
         if self.thread_num is None:
             object.__setattr__(self, "thread_num", os.cpu_count())
 
     def get_threads(self, max=None) -> int:
         """Get the number of threads for parallel processing.
 
-        The value is capped at an optional maximum value.
-
-        Args:
-            max (:obj:`int`, optional):
-                Maximum number to return.
-
-        Returns:
-            :obj:`int`
+        The value is capped at the number of logical cores available.
         """
-        thread_num = self.thread_num
+        if self.thread_num is None:
+            thread_num = os.cpu_count()
+        else:
+            thread_num = self.thread_num
         if max is not None:
             if max < 1:
                 raise ValueError("'max' must be positive")
             thread_num = min(max, thread_num)
         return thread_num
```

### Comparing `yet_another_wizz-2.5.4/src/yaw/config/binning.py` & `yet_another_wizz-2.5.post0/src/yaw/config/binning.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-import warnings
+import logging
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any
 
 import numpy as np
 
 from yaw.config import OPTIONS
 from yaw.config import default as DEFAULT
@@ -16,14 +16,17 @@
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
 
 __all__ = ["AutoBinningConfig", "ManualBinningConfig", "make_binning_config"]
 
 
+logger = logging.getLogger(__name__)
+
+
 class BaseBinningConfig(DictRepresentation):
     """Base class for redshift binning configuration."""
 
     zbins: NDArray[np.float_]
     """Edges of redshift bins."""
     method: str
     """Method used to create redshift binning, ``manual`` or either of
@@ -46,15 +49,16 @@
             Edges of redshift bins, must increase monotonically.
     """
 
     zbins: NDArray[np.float_] = field(
         metadata=Parameter(
             type=float,
             nargs="*",
-            help="list of custom redshift bin edges, if method is set to 'manual'",
+            help="list of custom redshift bin edges, if provided, other "
+            "binning parameters are omitted, method is set to 'manual'",
         )
     )
 
     def __post_init__(self) -> None:
         if len(self.zbins) < 2:
             raise ConfigError("'zbins' must have at least two edges")
         BinFactory.check(self.zbins)
@@ -83,17 +87,15 @@
     @property
     def zbin_num(self) -> int:
         """Number of redshift bins."""
         return len(self.zbins) - 1
 
     @classmethod
     def from_dict(cls, the_dict: dict[str, Any], **kwargs) -> ManualBinningConfig:
-        new_dict = {key: val for key, val in the_dict.items()}
-        zbins = new_dict.pop("zbins")
-        return cls(np.asarray(zbins), **new_dict)
+        return cls(np.asarray(the_dict["zbins"]))
 
     def to_dict(self) -> dict[str, Any]:
         return dict(method=self.method, zbins=self.zbins.tolist())
 
 
 @dataclass(frozen=True, repr=False)
 class AutoBinningConfig(BaseBinningConfig):
@@ -183,24 +185,22 @@
             cosmology (:obj:`astropy.cosmology.FLRW`, :obj:`~yaw.core.cosmology.CustomCosmology`, optional):
                 Cosmological model used for distance calculations. For a custom
                 model, refer to :mod:`yaw.core.cosmology`.
 
         Returns:
             :obj:`AutoBinningConfig`
         """
-        if not isinstance(method, str):
-            raise ValueError("'method' must a string")
         zbins = BinFactory(zmin, zmax, zbin_num, cosmology).get(method)
         return cls(zbins, method)
 
     def __eq__(self, other: ManualBinningConfig) -> bool:
-        if self.method != other.method:
-            return False
         if not array_equal(self.zbins, other.zbins):
             return False
+        if self.method != other.method:
+            return False
         return True
 
     @classmethod
     def from_dict(
         cls, the_dict: dict[str, Any], cosmology: TypeCosmology | None = None
     ) -> AutoBinningConfig:
         """Create a class instance from a dictionary representation of the
@@ -217,38 +217,43 @@
 
     def to_dict(self) -> dict[str, Any]:
         return dict(
             zmin=self.zmin, zmax=self.zmax, zbin_num=self.zbin_num, method=self.method
         )
 
 
+def warn_binning_args_ignored(
+    zmin: bool | float | None, zmax: bool | float | None, zbin_num: bool | int | None
+) -> None:
+    """Issue a warning that values are ignored, if any of the arguments is
+    set."""
+    # NOTE: NotSet is also False
+    if zmin or zmax or zbin_num:
+        logger.warn("'zmin', 'zmax', 'nbins' are ignored if 'zbins' is provided")
+
+
 def make_binning_config(
-    *,
-    cosmology: TypeCosmology | str | None = None,
+    cosmology: TypeCosmology | str | None,
     zmin: float | None = None,
     zmax: float | None = None,
-    zbin_num: int = DEFAULT.AutoBinning.zbin_num,
-    method: str = DEFAULT.AutoBinning.method,
+    zbin_num: int | None = None,
+    method: str | None = None,
     zbins: NDArray[np.float_] | None = None,
 ) -> ManualBinningConfig | AutoBinningConfig:
     """
     Helper function to construct a binning configuration.
 
     The ``cosmology`` argument is always required. If redshift bins (``zbins``)
     are provided, a :obj:`ManualBinningConfig` is returned, otherwise an
     :obj:`AutoBinningConfig`. Issues a warning if any argument is set but
     ignored by the returned configuration instance.
     """
-    auto_args_set = (zmin is not None, zmax is not None)
-    manual_args_set = (zbins is not None,)
-    if not all(manual_args_set) and not all(auto_args_set):
-        raise ConfigError("either 'zbins' or 'zmin' and 'zmax' are required")
+    auto_args_set = (zmin is not None, zmax is not None, zbin_num is not None)
+    if zbins is None and not all(auto_args_set):
+        raise ConfigError("either 'zbins' or 'zmin', 'zmax', 'zbin_num' are required")
     elif all(auto_args_set):
-        if all(manual_args_set):
-            warnings.warn(
-                "'zbins' set but ignored since 'zmin' and 'zmax' are provided"
-            )
         return AutoBinningConfig.generate(
             zmin=zmin, zmax=zmax, zbin_num=zbin_num, method=method, cosmology=cosmology
         )
     else:
+        warn_binning_args_ignored(*auto_args_set)
         return ManualBinningConfig(zbins)
```

### Comparing `yet_another_wizz-2.5.4/src/yaw/config/config.py` & `yet_another_wizz-2.5.post0/src/yaw/config/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 import logging
 from dataclasses import asdict, dataclass, field
 from typing import TYPE_CHECKING, Any, get_args
 
 import numpy as np
 import yaml
-from deprecated import deprecated
 
 from yaw.config import OPTIONS
 from yaw.config import default as DEFAULT
 from yaw.config import utils
 from yaw.config.backend import BackendConfig
 from yaw.config.binning import (
     AutoBinningConfig,
     ManualBinningConfig,
     make_binning_config,
+    warn_binning_args_ignored,
 )
 from yaw.config.scales import ScalesConfig
 from yaw.core.abc import DictRepresentation
 from yaw.core.cosmology import TypeCosmology, get_default_cosmology, r_kpc_to_angle
 from yaw.core.docs import Parameter
 
 if TYPE_CHECKING:  # pragma: no cover
@@ -31,32 +31,14 @@
 
 __all__ = ["Configuration"]
 
 
 logger = logging.getLogger(__name__)
 
 
-def update_if_set(the_dict: dict, key: str, value: Any | DEFAULT.NotSet) -> None:
-    if value is not DEFAULT.NotSet:
-        the_dict[key] = value
-
-
-def update_auto_binning_if_set(
-    the_dict: dict,
-    zmin: float | None = DEFAULT.NotSet,
-    zmax: float | None = DEFAULT.NotSet,
-    zbin_num: int | None = DEFAULT.NotSet,
-    method: str | None = DEFAULT.NotSet,
-) -> None:
-    update_if_set(the_dict, "zmin", zmin)
-    update_if_set(the_dict, "zmax", zmax)
-    update_if_set(the_dict, "zbin_num", zbin_num)
-    update_if_set(the_dict, "method", method)
-
-
 @dataclass(frozen=True)
 class Configuration(DictRepresentation):
     """The central configration for correlation measurements.
 
     Bundles the configuration of measurement scales, redshift binning, and
     backend parameters in a single, hierarchical configuration class.
     Additionally holds the cosmological model used for distance calculations.
@@ -110,15 +92,15 @@
     def __post_init__(self) -> None:
         # parse cosmology
         if self.cosmology is None:
             cosmology = get_default_cosmology()
         elif isinstance(self.cosmology, str):
             cosmology = utils.yaml_to_cosmology(self.cosmology)
         elif not isinstance(self.cosmology, get_args(TypeCosmology)):
-            which = ", ".join(str(c) for c in get_args(TypeCosmology))
+            which = ", ".join(get_args(TypeCosmology))
             raise utils.ConfigError(f"'cosmology' must be instance of: {which}")
         else:
             cosmology = self.cosmology
         cosmology = utils.parse_cosmology(self.cosmology)
         object.__setattr__(self, "cosmology", cosmology)
 
     @classmethod
@@ -234,61 +216,54 @@
         values.
 
         The method arguments are identical to :meth:`create`. Values that should
         not be modified are by default represented by the special value
         :obj:`~yaw.config.default.NotSet`.
         """
         config = self.to_dict()
-
-        # cosmology
         if cosmology is not DEFAULT.NotSet:
             if isinstance(cosmology, str):
                 cosmology = utils.yaml_to_cosmology(cosmology)
             config["cosmology"] = utils.cosmology_to_yaml(cosmology)
-
         # ScalesConfig
-        update_if_set(config["scales"], "rmin", rmin)
-        update_if_set(config["scales"], "rmax", rmax)
-        update_if_set(config["scales"], "rweight", rweight)
-        update_if_set(config["scales"], "rbin_num", rbin_num)
-
-        # AutoBinningConfig / ManualBinningConfig
-        if isinstance(self.binning, AutoBinningConfig):
-            if zbins is not DEFAULT.NotSet:
-                config["binning"] = dict(zbins=zbins)  # remove other params
-            else:
-                update_auto_binning_if_set(
-                    config["binning"], zmin, zmax, zbin_num, method
-                )
-        else:  # is ManualBinningConfig
-            if zbins is not DEFAULT.NotSet:
-                config["binning"]["zbins"] = zbins
-            else:
-                config["binning"] = dict()  # clear the binning parameters
-                update_auto_binning_if_set(
-                    config["binning"], zmin, zmax, zbin_num, method
-                )
-
+        if rmin is not DEFAULT.NotSet:
+            config["scales"]["rmin"] = rmin
+        if rmax is not DEFAULT.NotSet:
+            config["scales"]["rmax"] = rmax
+        if rweight is not DEFAULT.NotSet:
+            config["scales"]["rweight"] = rweight
+        if rbin_num is not DEFAULT.NotSet:
+            config["scales"]["rbin_num"] = rbin_num
+        # AutoBinningConfig /  ManualBinningConfig
+        if zbins is not DEFAULT.NotSet:
+            warn_binning_args_ignored(zmin, zmax, zbin_num)
+            config["binning"]["zbins"] = zbins
+        else:
+            if zmin is not DEFAULT.NotSet:
+                config["binning"]["zmin"] = zmin
+            if zmax is not DEFAULT.NotSet:
+                config["binning"]["zmax"] = zmax
+            if zbin_num is not DEFAULT.NotSet:
+                config["binning"]["zbin_num"] = zbin_num
+            if method is not DEFAULT.NotSet:
+                config["binning"]["method"] = method
         # BackendConfig
-        update_if_set(config["backend"], "thread_num", thread_num)
-        update_if_set(config["backend"], "crosspatch", crosspatch)
-        update_if_set(config["backend"], "rbin_slop", rbin_slop)
-
+        if thread_num is not DEFAULT.NotSet:
+            config["backend"]["thread_num"] = thread_num
+        if crosspatch is not DEFAULT.NotSet:
+            config["backend"]["crosspatch"] = crosspatch
+        if rbin_slop is not DEFAULT.NotSet:
+            config["backend"]["rbin_slop"] = rbin_slop
         return self.__class__.from_dict(config)
 
-    @deprecated(reason="no longer maintained", version="2.5.3")
     def plot_scales(
         self, catalog: BaseCatalog, log: bool = True, legend: bool = True
-    ) -> Figure:  # pragma: no cover
+    ) -> Figure:
         """Plot the configured correlation scales at different redshifts in
-        comparison to the size of patches in a data catalogue.
-
-        .. deprecated:: 2.5.3
-            No longer maintained.
-        """
+        comparison to the size of patches in a data catalogue."""
         import matplotlib.pyplot as plt
 
         fig, ax_scale = plt.subplots(1, 1)
         # plot scale of annulus
         for r_min, r_max in self.scales.as_array():
             ang_min, ang_max = np.transpose(
                 [
@@ -333,15 +308,20 @@
         # parse the required subgroups
         try:
             scales = ScalesConfig.from_dict(config.pop("scales"))
         except (TypeError, KeyError) as e:
             utils.parse_section_error(e, "scales")
         try:
             binning_conf = config.pop("binning")
-            binning = make_binning_config(cosmology=cosmology, **binning_conf)
+            if "zbins" in binning_conf:
+                binning = ManualBinningConfig(binning_conf["zbins"])
+            else:
+                binning = AutoBinningConfig.generate(
+                    cosmology=cosmology, **binning_conf
+                )
         except (TypeError, KeyError) as e:
             utils.parse_section_error(e, "binning")
         # parse the optional subgroups
         try:
             backend = BackendConfig.from_dict(config.pop("backend"))
         except KeyError:
             backend = BackendConfig()
```

### Comparing `yet_another_wizz-2.5.4/src/yaw/config/default.py` & `yet_another_wizz-2.5.post0/src/yaw/config/default.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/config/options.py` & `yet_another_wizz-2.5.post0/src/yaw/config/options.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/config/resampling.py` & `yet_another_wizz-2.5.post0/src/yaw/config/resampling.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from dataclasses import asdict, dataclass, field
+from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any
 
 import numpy as np
 
 from yaw.config import OPTIONS
 from yaw.config import default as DEFAULT
 from yaw.config.utils import ConfigError
@@ -69,18 +69,16 @@
         Available only after generating samples with :meth:`get_samples`.
 
         Returns:
             int if samples have been generated, else None.
         """
         if self._resampling_idx is None:
             return None
-        elif self.method == "bootstrap":
-            return self._resampling_idx.shape[1]
         else:
-            return self._resampling_idx.shape[0]
+            return self._resampling_idx.shape[1]
 
     def _generate_bootstrap(self, n_patches: int) -> NDArray[np.int_]:
         """Generate samples for the bootstrap resampling method.
 
         For N patches, draw M realisations each containing N randomly chosen
         patches.
         """
@@ -132,16 +130,10 @@
     def reset(self) -> None:
         """Reset the internally stored patch indices generated by
         :meth:`get_samples`."""
         object.__setattr__(self, "_resampling_idx", None)
 
     def to_dict(self) -> dict[str, Any]:
         if self.method == "jackknife":
-            return dict(
-                method=self.method,
-                crosspatch=self.crosspatch,
-                global_norm=self.global_norm,
-            )
+            return dict(method=self.method, crosspatch=self.crosspatch)
         else:
-            the_dict = asdict(self)
-            the_dict.pop("_resampling_idx")
-            return the_dict
+            return super().to_dict()
```

### Comparing `yet_another_wizz-2.5.4/src/yaw/config/scales.py` & `yet_another_wizz-2.5.post0/src/yaw/config/scales.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,37 +33,37 @@
     :math:`r^\\alpha` if a power-law exponent is provided through ``rweight``.
     The weighting is applied logarithmically spaced bins of separation (based
     on the logarithmic bin centers). This is an approximation to actually
     weighting each pair individually and the resolution of this approximation
     can be controlled by setting the number of bins.
 
     Args:
-        rmin (:obj:`float`, :obj:`list[float]`):
+        rmin (:obj:`float`, :obj:`Sequence[float]`):
             Single or multiple lower scale limits in kpc (angular diameter
             distance).
-        rmax (:obj:`float`, :obj:`list[float]`):
+        rmax (:obj:`float`, :obj:`Sequence[float]`):
             Single or multiple upper scale limits in kpc (angular diameter
             distance).
         rweight (:obj:`float`, optional):
             Power-law exponent used to weight pairs by their separation.
         rbin_num (:obj:`int`, optional):
             Number of radial logarithmic bin used to approximate the weighting
             by separation.
     """
 
-    rmin: list[float] | float = field(
+    rmin: Sequence[float] | float = field(
         metadata=Parameter(
             type=float,
             nargs="*",
             required=True,
             help="(list of) lower scale limit in kpc (pyhsical)",
         )
     )
     """Lower scale limit(s) in kpc (angular diameter distance)."""
-    rmax: list[float] | float = field(
+    rmax: Sequence[float] | float = field(
         metadata=Parameter(
             type=float,
             nargs="*",
             required=True,
             help="(list of) upper scale limit in kpc (pyhsical)",
         )
     )
```

### Comparing `yet_another_wizz-2.5.4/src/yaw/config/utils.py` & `yet_another_wizz-2.5.post0/src/yaw/config/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import NoReturn, get_args
 
 import astropy.cosmology
 
-from yaw.core.cosmology import CustomCosmology, TypeCosmology, get_default_cosmology
+from yaw.core.cosmology import TypeCosmology, get_default_cosmology
 
 __all__ = [
     "cosmology_to_yaml",
     "yaml_to_cosmology",
     "parse_cosmology",
     "parse_section_error",
 ]
@@ -19,18 +19,16 @@
 
 
 def cosmology_to_yaml(cosmology: TypeCosmology) -> str:
     """Try to represent the cosmological model in a YAML-friendly way.
 
     If it is one of the names :obj:`astropy` cosmologies, returns the name,
     otherwise raises an :exc:`ConfigError`."""
-    if isinstance(cosmology, CustomCosmology):
+    if not isinstance(cosmology, astropy.cosmology.FLRW):
         raise ConfigError("cannot serialise custom cosmoligies to YAML")
-    elif not isinstance(cosmology, astropy.cosmology.FLRW):
-        raise TypeError(f"invalid type '{type(cosmology)}' for cosmology")
     if cosmology.name not in astropy.cosmology.available:
         raise ConfigError("can only serialise predefined astropy cosmologies to YAML")
     return cosmology.name
 
 
 def yaml_to_cosmology(cosmo_name: str) -> TypeCosmology:
     """Reinstantiate the cosmological model from its name representation."""
@@ -50,39 +48,35 @@
     :obj:`astropy` cosmologies or subclass of
     :obj:`yaw.core.cosmology.CustomCosmology`."""
     if cosmology is None:
         cosmology = get_default_cosmology()
     elif isinstance(cosmology, str):
         cosmology = yaml_to_cosmology(cosmology)
     elif not isinstance(cosmology, get_args(TypeCosmology)):
-        which = ", ".join(str(c) for c in get_args(TypeCosmology))
+        which = ", ".join(get_args(TypeCosmology))
         raise ConfigError(f"'cosmology' must be instance of: {which}")
     return cosmology
 
 
 def parse_section_error(
     exception: Exception, section: str, reraise: Exception = ConfigError
 ) -> NoReturn:
     """Reraises are a more descriptive exception from an existing exception when
     parsing a YAML configuration.
 
     Covered cases are undefined key names, missing required key names or
     entirely missing subsection in the configuration.
     """
-    if len(exception.args) > 0:
-        msg = exception.args[0]
-        try:
-            item = msg.split("'")[1]
-        except IndexError:
-            item = msg
-        if isinstance(exception, TypeError):
-            if "got an unexpected keyword argument" in msg:
-                raise reraise(
-                    f"encountered unknown option '{item}' in section '{section}'"
-                ) from exception
-            elif "missing" in msg:
-                raise reraise(
-                    f"missing option '{item}' in section '{section}'"
-                ) from exception
-        elif isinstance(exception, KeyError):
-            raise reraise(f"missing section '{section}'") from exception
+    msg = exception.args[0]
+    item = msg.split("'")[1]
+    if isinstance(exception, TypeError):
+        if "__init__() got an unexpected keyword argument" in msg:
+            raise reraise(
+                f"encountered unknown option '{item}' in section '{section}'"
+            ) from exception
+        elif "missing" in msg:
+            raise reraise(
+                f"missing option '{item}' in section '{section}'"
+            ) from exception
+    elif isinstance(exception, KeyError):
+        raise reraise(f"missing section '{section}'") from exception
     raise
```

### Comparing `yet_another_wizz-2.5.4/src/yaw/core/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/core/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/core/abc.py` & `yet_another_wizz-2.5.post0/src/yaw/core/abc.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
         .. Note::
             Indexing rules for a one-dimensional numpy array apply.
 
         Returns:
             :obj:`yaw.core.containers.Indexer`
         """
-        pass
+        raise NotImplementedError
 
     @abstractmethod
     def concatenate_patches(self: _Tpatched, *data: _Tpatched) -> _Tpatched:
         """Concatenate pair count data containers with equal redshift binning.
 
         The data is merged by extending the dimension of the patch axes. The
         resulting data array will be a block matrix of the input data arrays,
@@ -73,31 +73,30 @@
             *data:
                 Containers of same type that are appended to the patch dimension
                 of this container.
 
         Returns:
             New instance of this container with combined data.
         """
-        pass
+        raise NotImplementedError
 
 
 _Tbinned = TypeVar("_Tbinned", bound="BinnedQuantity")
 
 
 class BinnedQuantity(ABC):
     """Base class for an object that has data organised in redshift bins."""
 
-    @abstractmethod
     def get_binning(self) -> IntervalIndex:
         """Get the underlying, exact redshift bin intervals.
 
         Returns:
             :obj:`pandas.IntervalIndex`
         """
-        pass
+        raise NotImplementedError
 
     def __repr__(self) -> str:
         name = self.__class__.__name__
         n_bins = self.n_bins
         binning = self.get_binning()
         z = f"{binning[0].left:.3f}...{binning[-1].right:.3f}"
         return f"{name}({n_bins=}, {z=})"
@@ -141,15 +140,15 @@
             Indexing rules for a one-dimensional numpy array apply, however if
             the resulting binning is not contiguous or contains repeated bins,
             some operations on the returned container may fail.
 
         Returns:
             :obj:`yaw.core.containers.Indexer`
         """
-        pass
+        raise NotImplementedError
 
     def is_compatible(self: _Tbinned, other: _Tbinned, require: bool = False) -> bool:
         """Check whether this instance is compatible with another instance.
 
         Ensures that both objects are instances of the same class and that the
         redshift binning is identical.
 
@@ -194,15 +193,15 @@
             *data:
                 Containers of same type that are appended to the patch dimension
                 of this container.
 
         Returns:
             New instance of this container with combined data.
         """
-        pass
+        raise NotImplementedError
 
 
 def concatenate_bin_edges(*patched: BinnedQuantity) -> IntervalIndex:
     """Concatenate the binning a set of data containers.
 
     The input containers are automatically sorted by the lowest edge of the
     redshift binning. Necessary condidtions for mergning are are that the patch
@@ -234,25 +233,25 @@
         Args:
             source (:obj:`h5py.Group`):
                 Group in an opened HDF5 file that contains the serialised data.
 
         Returns:
             :obj:`HDFSerializablep`
         """
-        pass
+        raise NotImplementedError
 
     @abstractmethod
     def to_hdf(self, dest: h5py.Group) -> None:
         """Serialise the class instance into an existing HDF5 group.
 
         Args:
             dest (:obj:`h5py.Group`):
                 Group in which the serialised data structures are created.
         """
-        pass
+        raise NotImplementedError
 
     @classmethod
     def from_file(cls: Type[_Thdf], path: TypePathStr) -> _Thdf:
         """Create a class instance by deserialising data from a HDF5 file.
 
         Args:
             path (:obj:`pathlib.Path`, :obj:`str`):
```

### Comparing `yet_another_wizz-2.5.4/src/yaw/core/containers.py` & `yet_another_wizz-2.5.post0/src/yaw/core/containers.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/core/coordinates.py` & `yet_another_wizz-2.5.post0/src/yaw/core/coordinates.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/core/cosmology.py` & `yet_another_wizz-2.5.post0/src/yaw/core/cosmology.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             z (Quantity-like ``redshift``, :obj:`NDArray`, or scalar number):
                 Input redshift.
 
         Returns:
             :obj:`astropy.units.Quantity`:
                 Comoving distance in Mpc to each input redshift.
         """
-        pass
+        NotImplemented
 
     @abstractmethod
     def comoving_transverse_distance(self, z: ArrayLike) -> ArrayLike:
         """Comoving transverse distance in Mpc at a given redshift.
 
         This value is the transverse comoving distance at redshift :math:`z`
         corresponding to an angular separation of 1 radian. This is the same as
@@ -71,15 +71,15 @@
             z (Quantity-like ``redshift``, :obj:`NDArray`, or scalar number):
                 Input redshift.
 
         Returns:
             :obj:`astropy.units.Quantity`:
                 Comoving transverse distance in Mpc at each input redshift.
         """
-        pass
+        NotImplemented
 
 
 TypeCosmology: TypeAlias = Union[FLRW, CustomCosmology]
 
 
 def r_kpc_to_angle(
     r_kpc: NDArray[np.float_] | Sequence[float], z: float, cosmology: TypeCosmology
```

### Comparing `yet_another_wizz-2.5.4/src/yaw/core/docs.py` & `yet_another_wizz-2.5.post0/src/yaw/core/docs.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/core/math.c` & `yet_another_wizz-2.5.post0/src/yaw/core/math.c`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/core/math.py` & `yet_another_wizz-2.5.post0/src/yaw/core/math.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/core/parallel.py` & `yet_another_wizz-2.5.post0/src/yaw/core/parallel.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/core/utils.py` & `yet_another_wizz-2.5.post0/src/yaw/core/utils.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/correlation/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/correlation/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/correlation/corrfuncs.py` & `yet_another_wizz-2.5.post0/src/yaw/correlation/corrfuncs.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import pandas as pd
 from deprecated import deprecated
 
 from yaw.catalogs import PatchLinkage
 from yaw.config import OPTIONS, ResamplingConfig
 from yaw.core.abc import BinnedQuantity, HDFSerializable, PatchedQuantity
 from yaw.core.containers import Indexer, SampledData
-from yaw.core.logging import TimedLog
+from yaw.core.logging import LogCustomWarning, TimedLog
 from yaw.core.utils import TypePathStr
 from yaw.core.utils import format_float_fixed_width as fmt_num
 from yaw.correlation.estimators import (
     CorrelationEstimator,
     CtsMix,
     EstimatorError,
     cts_from_code,
@@ -102,15 +102,18 @@
             by :func:`CorrData.to_files`.
     """
 
     info: str | None = None
     """Optional descriptive text for the contained data."""
 
     def __post_init__(self) -> None:
-        super().__post_init__()
+        with LogCustomWarning(
+            logger, "invalid values encountered in correlation samples"
+        ):
+            super().__post_init__()
 
     @classmethod
     def from_files(cls: Type[_Tdata], path_prefix: TypePathStr) -> _Tdata:
         """Create a new instance by loading the data from ASCII files.
 
         The data is restored from a set of three input files produced by
         :meth:`to_files`.
```

### Comparing `yet_another_wizz-2.5.4/src/yaw/correlation/estimators.py` & `yet_another_wizz-2.5.post0/src/yaw/correlation/estimators.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 True
 >>> CtsMix() == CtsRD()
 True
 """
 
 from __future__ import annotations
 
-import warnings
+import logging
 from abc import ABC, abstractclassmethod, abstractproperty
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
@@ -36,14 +36,17 @@
     "PeeblesHauser",
     "DavisPeebles",
     "Hamilton",
     "LandySzalay",
 ]
 
 
+logger = logging.getLogger(__name__)
+
+
 class EstimatorError(Exception):
     pass
 
 
 class Cts(ABC):
     """Base class to symbolically represent pair counts."""
 
@@ -152,25 +155,25 @@
         super().__init_subclass__(**kwargs)
         cls.variants.append(cls)
 
     @classmethod
     def _warn_enum_zero(cls, counts: NDArray):
         """Raise a warning if any value in the expression enumerator is zero"""
         if np.any(counts == 0.0):
-            warnings.warn(f"estimator {cls.short} encontered zeros in enumerator")
+            logger.warn(f"estimator {cls.short} encontered zeros in enumerator")
 
     @abstractclassmethod
     def eval(
         cls, *, dd: NDArray, dr: NDArray, rr: NDArray, rd: NDArray | None = None
     ) -> NDArray:
         """Method that implements the estimator.
 
         Should call :meth:`_warn_enum_zero` to raise warnings on zero-division.
         """
-        pass
+        NotImplemented
 
 
 class PeeblesHauser(CorrelationEstimator):
     """Implementation of the Peebles-Hauser correlation estimator
     :math:`\\frac{DD}{RR} - 1`.
     """
```

### Comparing `yet_another_wizz-2.5.4/src/yaw/correlation/paircounts.py` & `yet_another_wizz-2.5.post0/src/yaw/correlation/paircounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 both a :obj:`PatchedCount` and :obj:`PatchedTotal` container. Its
 :meth:`NormalisedCounts.sample` method computes the ratio of
 counts-to-total-objects and samples thereof.
 """
 
 from __future__ import annotations
 
+import logging
 from abc import abstractmethod
 from collections.abc import Iterable, Sequence
 from dataclasses import dataclass
 from itertools import accumulate
 from typing import TYPE_CHECKING, NoReturn, Union
 
 try:  # pragma: no cover
@@ -33,22 +34,26 @@
 from yaw.core.abc import (
     BinnedQuantity,
     HDFSerializable,
     PatchedQuantity,
     concatenate_bin_edges,
 )
 from yaw.core.containers import Indexer, PatchIDs, SampledData
+from yaw.core.logging import LogCustomWarning
 from yaw.core.math import apply_slice_ndim, outer_triu_sum
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import DTypeLike, NDArray
     from pandas import IntervalIndex
 
 __all__ = ["PatchedTotal", "PatchedCount", "NormalisedCounts"]
 
+
+logger = logging.getLogger(__name__)
+
 _compression = dict(fletcher32=True, compression="gzip", shuffle=True)
 """default compression settings for :obj:`h5py.Dataset`."""
 
 
 TypeSlice: TypeAlias = Union[slice, int, None]
 TypeIndex: TypeAlias = Union[int, slice, Sequence]
 
@@ -157,39 +162,39 @@
 
     @abstractmethod
     def as_array(self) -> NDArray:
         """Get the underlying data as contiguous array.
 
         The array 3-dimensional with shape (N, N, K), where N is the number of
         spatial patches, and K is the number of redshift bins."""
-        pass
+        raise NotImplementedError
 
     @abstractmethod
     def _sum(self, config: ResamplingConfig) -> NDArray:
         """Method that implements the sum over all patches."""
-        pass
+        raise NotImplementedError
 
     @abstractmethod
     def _jackknife(self, config: ResamplingConfig, signal: NDArray) -> NDArray:
         """Method that implements generating jackknife samples of the sum over
         all patches.
 
         For N patches, draw N realisations by leaving out one of the N patches.
         """
-        pass
+        raise NotImplementedError
 
     @abstractmethod
     def _bootstrap(self, config: ResamplingConfig) -> NDArray:
         """Method that implements generating bootstrap samples of the sum over
         all patches.
 
         For N patches, draw M realisations each containing N randomly chosen
         patches.
         """
-        pass
+        raise NotImplementedError
 
     @deprecated(reason="renamed to CorrFunc.sample_sum", version="2.3.1")
     def get_sum(self, *args, **kwargs):
         """
         .. deprecated:: 2.3.1
             Renamed to :meth:`sample_sum`.
         """
@@ -1029,20 +1034,23 @@
                 parameters.
 
         Returns:
             :obj:`~yaw.core.SampledData`
         """
         counts = self.count.sample_sum(config)
         totals = self.total.sample_sum(config)
-        samples = SampledData(
-            binning=self.get_binning(),
-            data=(counts.data / totals.data),
-            samples=(counts.samples / totals.samples),
-            method=config.method,
-        )
+        with LogCustomWarning(
+            logger, "some patches contain no data after binning by redshift"
+        ):
+            samples = SampledData(
+                binning=self.get_binning(),
+                data=(counts.data / totals.data),
+                samples=(counts.samples / totals.samples),
+                method=config.method,
+            )
         return samples
 
     @classmethod
     def from_hdf(cls, source: h5py.Group) -> NormalisedCounts:
         count = PatchedCount.from_hdf(source["count"])
         total = PatchedTotal.from_hdf(source["total"])
         return cls(count=count, total=total)
```

### Comparing `yet_another_wizz-2.5.4/src/yaw/deprecated.py` & `yet_another_wizz-2.5.post0/src/yaw/deprecated.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/examples/__init__.py` & `yet_another_wizz-2.5.post0/src/yaw/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/examples/auto_reference.hdf` & `yet_another_wizz-2.5.post0/src/yaw/examples/auto_reference.hdf`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/examples/auto_unknown_1.hdf` & `yet_another_wizz-2.5.post0/src/yaw/examples/auto_unknown_1.hdf`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/examples/cross_1.hdf` & `yet_another_wizz-2.5.post0/src/yaw/examples/cross_1.hdf`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/randoms.py` & `yet_another_wizz-2.5.post0/src/yaw/randoms.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz-2.5.4/src/yaw/redshifts.py` & `yet_another_wizz-2.5.post0/src/yaw/redshifts.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,26 @@
 corresponding autocorrelation functions (e.g. of the reference sample) are
 known.
 """
 
 from __future__ import annotations
 
 import logging
+import warnings
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 import scipy.optimize
 from deprecated import deprecated
 
 from yaw.config import ResamplingConfig
 from yaw.core.containers import SampledValue
-from yaw.core.logging import TimedLog
+from yaw.core.logging import LogCustomWarning, TimedLog
 from yaw.core.math import rebin, shift_histogram
 from yaw.core.utils import TypePathStr
 from yaw.correlation import CorrData
 
 if TYPE_CHECKING:  # pragma: no cover
     from numpy.typing import NDArray
 
@@ -200,16 +201,21 @@
             mitigate.append("unknown")
 
         if len(mitigate) > 0:
             logger.debug(f"mitigating {' and '.join(mitigate)} sample bias")
         N = cross_data.n_samples
         dzsq_data = cross_data.dz**2
         dzsq_samp = np.tile(dzsq_data, N).reshape((N, -1))
-        nz_data = w_sp_data / np.sqrt(dzsq_data * w_ss_data * w_pp_data)
-        nz_samp = w_sp_samp / np.sqrt(dzsq_samp * w_ss_samp * w_pp_samp)
+        with LogCustomWarning(
+            logger, "invalid values encountered in redshift estimate"
+        ):
+            nz_data = w_sp_data / np.sqrt(dzsq_data * w_ss_data * w_pp_data)
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+            nz_samp = w_sp_samp / np.sqrt(dzsq_samp * w_ss_samp * w_pp_samp)
         return cls(
             binning=cross_data.binning,
             data=nz_data,
             samples=nz_samp,
             method=cross_data.method,
             info=info,
         )
@@ -284,15 +290,15 @@
                 ref_data = ref_corr.sample(config, estimator=ref_est)
             else:
                 ref_data = None
             if unk_corr is not None:
                 unk_data = unk_corr.sample(config, estimator=unk_est)
             else:
                 unk_data = None
-            return cls.from_corrdata(
+            return cls.from_correlation_data(
                 cross_data=cross_data, ref_data=ref_data, unk_data=unk_data, info=info
             )
 
     @property
     def _dat_desc(self) -> str:
         return "# n(z) estimate with symmetric 68% percentile confidence"
```

### Comparing `yet_another_wizz-2.5.4/src/yet_another_wizz.egg-info/PKG-INFO` & `yet_another_wizz-2.5.post0/src/yet_another_wizz.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 Metadata-Version: 2.1
 Name: yet-another-wizz
-Version: 2.5.4
-Summary: Implementation of the Schmidt et al. (2013) clustering redshift method.
+Version: 2.5.post0
+Summary: Implementation of the Schmidt et al. (2013) clustering redshift method and wrapper scripts to produce cross-correlation (CC) redshifts.
 Home-page: https://github.com/jlvdb/yet_another_wizz.git
 Author-email: Jan Luca van den Busch <jlvdb@astro.ruhr-uni-bochum.de>
 License: GPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
-Provides-Extra: cli
 Provides-Extra: plot
 Provides-Extra: docs
 Provides-Extra: test
 Provides-Extra: style
 Provides-Extra: dev
 License-File: LICENSE
 
-.. image:: https://raw.githubusercontent.com/jlvdb/yet_another_wizz/main/docs/source/_static/logo-dark.png
-    :width: 1000
-    :alt: yet_another_wizz
+yet_another_wizz
+================
 
-|
-
-.. image:: https://img.shields.io/pypi/v/yet_another_wizz?logo=pypi&logoColor=blue
-    :target: https://pypi.org/project/yet_another_wizz/
+.. image:: https://badge.fury.io/py/yet-another-wizz.svg
+    :target: https://badge.fury.io/py/yet-another-wizz
 .. image:: https://readthedocs.org/projects/yet-another-wizz/badge/?version=latest
     :target: https://yet-another-wizz.readthedocs.io/en/latest/?badge=latest
 .. image:: https://github.com/jlvdb/yet_another_wizz/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/jlvdb/yet_another_wizz/actions/workflows/run-tests.yml
 .. image:: https://codecov.io/gh/jlvdb/yet_another_wizz/branch/main/graph/badge.svg?token=PC41ME2AR8
     :target: https://codecov.io/gh/jlvdb/yet_another_wizz
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
     :target: https://pycqa.github.io/isort/
 
-|
 
 *yet_another_wizz* is a python package to efficiently compute cross-correlation
 redshifts, also know as clustering redshifts and is hosted on github:
 
 - code: https://github.com/jlvdb/yet_another_wizz.git
 - docs: https://yet-another-wizz.readthedocs.io/
 - PyPI: https://pypi.org/project/yet_another_wizz/
@@ -62,38 +57,29 @@
 Installation
 ------------
 
 The yet_another_wizz package can be installed directly with pip::
 
     pip install yet_another_wizz
 
-This will install the python library ``yaw``.
-
-Commandline tool
-~~~~~~~~~~~~~~~~
-
-There also exists a separate command line tool called
-`yet_another_wizz_cli <https://github.com/jlvdb/yet_another_wizz_cli>`_
-(``yaw_cli``) that is available at PyPI and github. To install it alongside the
-python library, type::
-
-    pip install yet_another_wizz[cli]
+This will install the python package ``yaw``, as well as the ``yaw_cli``
+executable command line tool.
 
 
 Usage
 -----
 
 There are two main ways to use yet_another_wizz,
 
-- the python library ``yaw`` itself and
-- the (separate) ``yaw_cli`` commmand line tool.
+- the ``yaw_cli`` commmand line tool and
+- the python package ``yaw`` directly.
 
 Most people will probably get started with the command line tool, which should
 cover all necessary tasks for a standard clustering redshift calibration. For
-custom solutions, use the python library. A basic example as well as the API
+custom solutions, use the python package. A basic example as well as the API
 reference can be found in the official documentation.
 
 
 Reporting bugs and requesting features
 --------------------------------------
 
 For bug reports or requesting new features, please use the github issue page:
```

