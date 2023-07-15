# Comparing `tmp/terrainman-0.0.26.tar.gz` & `tmp/terrainman-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terrainman-0.0.26.tar", max compression
+gzip compressed data, was "terrainman-0.0.9.tar", max compression
```

## Comparing `terrainman-0.0.26.tar` & `terrainman-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-05-10 17:44:29.464943 terrainman-0.0.26/LICENSE
--rw-r--r--   0        0        0        4 2023-05-10 17:38:08.409616 terrainman-0.0.26/README.md
--rw-r--r--   0        0        0      828 2023-07-15 21:18:46.010049 terrainman-0.0.26/pyproject.toml
--rw-r--r--   0        0        0      661 2023-07-15 21:04:50.613763 terrainman-0.0.26/src/terrainman/__init__.py
--rw-r--r--   0        0        0   235704 2023-07-15 20:24:19.297877 terrainman-0.0.26/src/terrainman/data/LAADS_query.2023-05-08T19_09.csv
--rw-r--r--   0        0        0     7112 2023-07-15 20:32:47.154826 terrainman-0.0.26/src/terrainman/data/tsi_daily.csv
--rw-r--r--   0        0        0   188622 2023-05-08 19:14:49.435284 terrainman-0.0.26/src/terrainman/data/viirs_aerosol_daily.csv
--rw-r--r--   0        0        0    23654 2023-05-08 19:15:56.452272 terrainman-0.0.26/src/terrainman/data/viirs_aerosol_monthly.csv
--rw-r--r--   0        0        0    13073 2023-07-15 21:14:00.642915 terrainman-0.0.26/src/terrainman/tile_io.py
--rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 terrainman-0.0.26/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-10 17:44:29.464943 terrainman-0.0.9/LICENSE
+-rw-r--r--   0        0        0        4 2023-05-10 17:38:08.409616 terrainman-0.0.9/README.md
+-rw-r--r--   0        0        0      969 2023-05-10 17:54:37.102852 terrainman-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-05-08 00:34:50.893087 terrainman-0.0.9/src/__init__.py
+-rw-r--r--   0        0        0     9650 2023-05-09 02:23:25.027650 terrainman-0.0.9/src/tile_io.py
+-rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 terrainman-0.0.9/PKG-INFO
```

### Comparing `terrainman-0.0.26/LICENSE` & `terrainman-0.0.9/LICENSE`

 * *Files identical despite different names*

