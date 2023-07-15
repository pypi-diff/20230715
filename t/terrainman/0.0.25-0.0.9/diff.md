# Comparing `tmp/terrainman-0.0.25.tar.gz` & `tmp/terrainman-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terrainman-0.0.25.tar", max compression
+gzip compressed data, was "terrainman-0.0.9.tar", max compression
```

## Comparing `terrainman-0.0.25.tar` & `terrainman-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1070 2023-05-10 17:44:29.464943 terrainman-0.0.25/LICENSE
--rw-r--r--   0        0        0        4 2023-05-10 17:38:08.409616 terrainman-0.0.25/README.md
--rw-r--r--   0        0        0      851 2023-07-15 21:15:48.661776 terrainman-0.0.25/pyproject.toml
--rw-r--r--   0        0        0      661 2023-07-15 21:04:50.613763 terrainman-0.0.25/src/terrainman/__init__.py
--rw-r--r--   0        0        0    13073 2023-07-15 21:14:00.642915 terrainman-0.0.25/src/terrainman/tile_io.py
--rw-r--r--   0        0        0     1103 1970-01-01 00:00:00.000000 terrainman-0.0.25/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-10 17:44:29.464943 terrainman-0.0.9/LICENSE
+-rw-r--r--   0        0        0        4 2023-05-10 17:38:08.409616 terrainman-0.0.9/README.md
+-rw-r--r--   0        0        0      969 2023-05-10 17:54:37.102852 terrainman-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-05-08 00:34:50.893087 terrainman-0.0.9/src/__init__.py
+-rw-r--r--   0        0        0     9650 2023-05-09 02:23:25.027650 terrainman-0.0.9/src/tile_io.py
+-rw-r--r--   0        0        0     1038 1970-01-01 00:00:00.000000 terrainman-0.0.9/PKG-INFO
```

### Comparing `terrainman-0.0.25/LICENSE` & `terrainman-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `terrainman-0.0.25/pyproject.toml` & `terrainman-0.0.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 [tool.poetry]
 name = "terrainman"
-version = "0.0.25"
+version = "0.0.9"
 description = "A package for downloading and managing high-fidelity terrain files"
 authors = ["Liam Robinson <robin502@purdue.edu>"]
 readme = "README.md"
-packages = [{include = "terrainman", from = "src"}]
-exclude = ['src/terrainman/data', 'src/terrainman/__pycache']
+packages = [{include = "src"}]
+include = [{path = "src", format = "sdist"}]
 documentation = "https://python-poetry.org/docs/"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: MacOS",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-numpy = "^1.24.2"
-scipy = "^1.10.1"
-pyvista = "^0.38.5"
-python-dotenv = "^1.0.0"
-trimesh = "^3.21.5"
-rtree = "^1.0.1"
-pyembree = "^0.1.12"
-rasterio = "^1.3.6"
-netCDF4 = "^1.6.3"
+numpy = "==1.24.2"
+scipy = "==1.10.1"
+pyvista = "==0.38.5"
+python-dotenv = "1.0.0"
+trimesh = "==3.21.5"
+rtree = "==1.0.1"
+pyembree = "==0.1.12"
+rasterio = "==1.3.6"
+netCDF4 = "==1.6.3"
+
+[project.urls]
+"Homepage" = "https://github.com/liamrobinson1/PyLightCurves"
+"Bug Tracker" = "https://github.com/liamrobinson1/PyLightCurves/issues"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

