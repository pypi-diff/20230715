# Comparing `tmp/climatePy-0.4.29.tar.gz` & `tmp/climatePy-0.4.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.4.29.tar", last modified: Tue Jul 11 19:37:08 2023, max compression
+gzip compressed data, was "climatePy-0.4.30.tar", last modified: Sat Jul 15 14:14:50 2023, max compression
```

## Comparing `climatePy-0.4.29.tar` & `climatePy-0.4.30.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:37:08.620567 climatePy-0.4.29/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-11 19:37:04.000000 climatePy-0.4.29/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-11 19:37:08.620567 climatePy-0.4.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-11 19:37:04.000000 climatePy-0.4.29/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:37:08.564567 climatePy-0.4.29/climatePy/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-11 19:37:04.000000 climatePy-0.4.29/climatePy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20018 2023-07-11 19:37:04.000000 climatePy-0.4.29/climatePy/_climatepy_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    60892 2023-07-11 19:37:04.000000 climatePy-0.4.29/climatePy/_dap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-11 19:37:04.000000 climatePy-0.4.29/climatePy/_netrc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    39285 2023-07-11 19:37:04.000000 climatePy-0.4.29/climatePy/_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    26690 2023-07-11 19:37:04.000000 climatePy-0.4.29/climatePy/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:37:08.568568 climatePy-0.4.29/climatePy/data/
--rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-11 19:37:04.000000 climatePy-0.4.29/climatePy/data/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:37:08.568568 climatePy-0.4.29/climatePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-11 19:37:08.000000 climatePy-0.4.29/climatePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-11 19:37:08.000000 climatePy-0.4.29/climatePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:37:08.000000 climatePy-0.4.29/climatePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-11 19:37:08.000000 climatePy-0.4.29/climatePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 19:37:08.000000 climatePy-0.4.29/climatePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 19:37:08.620567 climatePy-0.4.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-11 19:37:06.000000 climatePy-0.4.29/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:37:08.620567 climatePy-0.4.29/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:37:04.000000 climatePy-0.4.29/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-11 19:37:04.000000 climatePy-0.4.29/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-11 19:37:04.000000 climatePy-0.4.29/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:14:50.229277 climatePy-0.4.30/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-15 14:14:46.000000 climatePy-0.4.30/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-15 14:14:50.229277 climatePy-0.4.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-15 14:14:46.000000 climatePy-0.4.30/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:14:50.185278 climatePy-0.4.30/climatePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-15 14:14:46.000000 climatePy-0.4.30/climatePy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20018 2023-07-15 14:14:46.000000 climatePy-0.4.30/climatePy/_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61537 2023-07-15 14:14:46.000000 climatePy-0.4.30/climatePy/_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-15 14:14:46.000000 climatePy-0.4.30/climatePy/_netrc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39285 2023-07-15 14:14:46.000000 climatePy-0.4.30/climatePy/_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26690 2023-07-15 14:14:46.000000 climatePy-0.4.30/climatePy/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:14:50.185278 climatePy-0.4.30/climatePy/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-15 14:14:46.000000 climatePy-0.4.30/climatePy/data/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:14:50.185278 climatePy-0.4.30/climatePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-15 14:14:50.000000 climatePy-0.4.30/climatePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-15 14:14:50.000000 climatePy-0.4.30/climatePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 14:14:50.000000 climatePy-0.4.30/climatePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-15 14:14:50.000000 climatePy-0.4.30/climatePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-15 14:14:50.000000 climatePy-0.4.30/climatePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 14:14:50.229277 climatePy-0.4.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-15 14:14:48.000000 climatePy-0.4.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:14:50.229277 climatePy-0.4.30/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 14:14:46.000000 climatePy-0.4.30/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-15 14:14:46.000000 climatePy-0.4.30/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-15 14:14:46.000000 climatePy-0.4.30/tests/test_utils.py
```

### Comparing `climatePy-0.4.29/LICENSE` & `climatePy-0.4.30/LICENSE`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.29/PKG-INFO` & `climatePy-0.4.30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.29
+Version: 0.4.30
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.29/README.md` & `climatePy-0.4.30/README.md`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.29/climatePy/__init__.py` & `climatePy-0.4.30/climatePy/__init__.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.29/climatePy/_climatepy_filter.py` & `climatePy-0.4.30/climatePy/_climatepy_filter.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.29/climatePy/_dap.py` & `climatePy-0.4.30/climatePy/_dap.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,26 @@
             url_lst = catalog.URL.values.tolist()
 
             # extend list with URL
             url_lst.extend(URL)
 
             # set URL to list of URLS
             URL = url_lst
-
+            
+        # If AOI is a shapely geometry, convert AOI into GeoPandas dataframe 
+        if isinstance(AOI, (shapely.geometry.point.Point, 
+                            shapely.geometry.multipoint.MultiPoint,
+                            shapely.geometry.linestring.LineString, 
+                            shapely.geometry.multilinestring.MultiLineString, 
+                            shapely.geometry.polygon.Polygon, 
+                            shapely.geometry.multipolygon.MultiPolygon)):
+            
+            # convert shapely geometry to geopandas dataframe
+            AOI = climatepy_filter.shapely_to_gpd(AOI)
+            
         # check if "vrt" or "tif" in URL list, or if "vsi" in all of URL list
         if any([utils.getExtension(i) in ['vrt', "tif"] for i in URL]) or all(["vsi" in i for i in URL]):
 
             if verbose:
                 print("Getting VRT/TIF data")
                 
             # get the vrt catalog features for each URL
```

### Comparing `climatePy-0.4.29/climatePy/_netrc_utils.py` & `climatePy-0.4.30/climatePy/_netrc_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.29/climatePy/_shortcuts.py` & `climatePy-0.4.30/climatePy/_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.29/climatePy/_utils.py` & `climatePy-0.4.30/climatePy/_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.29/climatePy/data/catalog.csv` & `climatePy-0.4.30/climatePy/data/catalog.csv`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.29/climatePy.egg-info/PKG-INFO` & `climatePy-0.4.30/climatePy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.29
+Version: 0.4.30
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.29/setup.py` & `climatePy-0.4.30/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="climatePy",                         # pkg name
     # version="0.0.4.24",                        # version
-    version='0.4.29',
+    version='0.4.30',
     author="Angus Watters, Mike Johnson",     # authors
     description="A Python package for getting point and gridded climate data by AOI",
     long_description=long_description,      # long description is read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # python modules to install
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `climatePy-0.4.29/tests/test_shortcuts.py` & `climatePy-0.4.30/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.29/tests/test_utils.py` & `climatePy-0.4.30/tests/test_utils.py`

 * *Files identical despite different names*

