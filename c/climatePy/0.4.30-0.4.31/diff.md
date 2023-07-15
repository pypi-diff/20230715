# Comparing `tmp/climatePy-0.4.30.tar.gz` & `tmp/climatePy-0.4.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.4.30.tar", last modified: Sat Jul 15 14:14:50 2023, max compression
+gzip compressed data, was "climatePy-0.4.31.tar", last modified: Sat Jul 15 18:33:19 2023, max compression
```

## Comparing `climatePy-0.4.30.tar` & `climatePy-0.4.31.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:14:50.229277 climatePy-0.4.30/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-15 14:14:46.000000 climatePy-0.4.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-15 14:14:50.229277 climatePy-0.4.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-15 14:14:46.000000 climatePy-0.4.30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:14:50.185278 climatePy-0.4.30/climatePy/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-15 14:14:46.000000 climatePy-0.4.30/climatePy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20018 2023-07-15 14:14:46.000000 climatePy-0.4.30/climatePy/_climatepy_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    61537 2023-07-15 14:14:46.000000 climatePy-0.4.30/climatePy/_dap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-15 14:14:46.000000 climatePy-0.4.30/climatePy/_netrc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    39285 2023-07-15 14:14:46.000000 climatePy-0.4.30/climatePy/_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    26690 2023-07-15 14:14:46.000000 climatePy-0.4.30/climatePy/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:14:50.185278 climatePy-0.4.30/climatePy/data/
--rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-15 14:14:46.000000 climatePy-0.4.30/climatePy/data/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:14:50.185278 climatePy-0.4.30/climatePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-15 14:14:50.000000 climatePy-0.4.30/climatePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-15 14:14:50.000000 climatePy-0.4.30/climatePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 14:14:50.000000 climatePy-0.4.30/climatePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-15 14:14:50.000000 climatePy-0.4.30/climatePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-15 14:14:50.000000 climatePy-0.4.30/climatePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 14:14:50.229277 climatePy-0.4.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-15 14:14:48.000000 climatePy-0.4.30/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:14:50.229277 climatePy-0.4.30/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 14:14:46.000000 climatePy-0.4.30/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-15 14:14:46.000000 climatePy-0.4.30/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-15 14:14:46.000000 climatePy-0.4.30/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:33:19.469154 climatePy-0.4.31/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-15 18:33:16.000000 climatePy-0.4.31/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-15 18:33:19.469154 climatePy-0.4.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-15 18:33:16.000000 climatePy-0.4.31/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:33:19.425153 climatePy-0.4.31/climatePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-07-15 18:33:16.000000 climatePy-0.4.31/climatePy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-15 18:33:16.000000 climatePy-0.4.31/climatePy/_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61682 2023-07-15 18:33:16.000000 climatePy-0.4.31/climatePy/_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-15 18:33:16.000000 climatePy-0.4.31/climatePy/_netrc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39285 2023-07-15 18:33:16.000000 climatePy-0.4.31/climatePy/_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30062 2023-07-15 18:33:16.000000 climatePy-0.4.31/climatePy/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:33:19.425153 climatePy-0.4.31/climatePy/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-15 18:33:16.000000 climatePy-0.4.31/climatePy/data/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:33:19.425153 climatePy-0.4.31/climatePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-15 18:33:19.000000 climatePy-0.4.31/climatePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-15 18:33:19.000000 climatePy-0.4.31/climatePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 18:33:19.000000 climatePy-0.4.31/climatePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-15 18:33:19.000000 climatePy-0.4.31/climatePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-15 18:33:19.000000 climatePy-0.4.31/climatePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 18:33:19.469154 climatePy-0.4.31/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-15 18:33:17.000000 climatePy-0.4.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:33:19.469154 climatePy-0.4.31/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 18:33:16.000000 climatePy-0.4.31/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-15 18:33:16.000000 climatePy-0.4.31/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-15 18:33:16.000000 climatePy-0.4.31/tests/test_utils.py
```

### Comparing `climatePy-0.4.30/LICENSE` & `climatePy-0.4.31/LICENSE`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.30/PKG-INFO` & `climatePy-0.4.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.30
+Version: 0.4.31
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.30/README.md` & `climatePy-0.4.31/README.md`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.30/climatePy/__init__.py` & `climatePy-0.4.31/climatePy/__init__.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.30/climatePy/_climatepy_filter.py` & `climatePy-0.4.31/climatePy/_climatepy_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,59 +51,14 @@
         'miny': [AOI.bounds['miny'].min()],
         'maxx': [AOI.bounds['maxx'].max()],
         'maxy': [AOI.bounds['maxy'].max()]
         })
     
     return max_bbox.iloc[0]
 
-def shapely_to_gpd(AOI):
-
-    """Convert a Shapely object to a GeoDataFrame.
-
-    Args:
-        AOI (shapely.geometry.base.BaseGeometry): The area of interest as a Shapely object.
-
-    Returns:
-        GeoDataFrame: A GeoDataFrame representing the area of interest.
-            The GeoDataFrame has a single geometry column with an automatically assigned CRS (either EPSG:4326 or EPSG:5070)
-
-    Note:
-        The function assumes that the shapely AOI is in either WGS84 (EPSG:4326) or NAD83 (EPSG:5070) coordinate system.
-    """
-
-    # convex hull
-    chull = AOI.convex_hull
-
-    # check if convex hull is a point or a polygon
-    if isinstance(chull, shapely.geometry.point.Point):
-        xx, yy = chull.coords.xy
-    else:
-        xx, yy = chull.exterior.coords.xy
-
-    # bounding box
-    xmax = np.asarray(xx).max()
-    xmin = np.asarray(xx).min()
-    ymax = np.asarray(yy).max()
-    ymin = np.asarray(yy).min()
-
-    # check if AOI is in WGS84 or NAD83
-    if (ymax >= -90 and ymax <= 90
-        and ymin <= 90 and ymin >= -90
-        and xmax >= -180 and xmax <= 180
-        and xmin <= 180 and xmin >= -180):
-        print("Assuming AOI CRS is EPSG:4326 (WGS84)")
-        crs = CRS.from_epsg(4326)
-    else:
-        print("Assuming AOI CRS is EPSG:5070 (NAD83)")
-        crs = CRS.from_epsg(5070)
-
-    out = gpd.GeoDataFrame(geometry = [AOI], crs = crs)
-
-    return out
-
 def find_intersects(catalog, AOI):
     """Check for catalog rows intersecting with the given AOI.
 
     Args:
         catalog (pandas.DataFrame): A DataFrame containing the catalog information.
         AOI (geopandas.GeoDataFrame): A GeoDataFrame representing the Area of Interest.
 
@@ -291,24 +246,27 @@
 
         if scenario is not None:
             if isinstance(scenario, str):
                 catalog = catalog[catalog['scenario'].str.contains(scenario)]
             elif isinstance(scenario, list):
                 catalog = catalog[catalog['scenario'].str.contains('|'.join(scenario))]
 
-    # # If AOI is a shapely geometry, convert AOI into GeoPandas dataframe 
-    if isinstance(AOI, (shapely.geometry.point.Point, 
-            shapely.geometry.multipoint.MultiPoint,
-            shapely.geometry.linestring.LineString, 
-            shapely.geometry.multilinestring.MultiLineString, 
-            shapely.geometry.polygon.Polygon, 
-            shapely.geometry.multipolygon.MultiPolygon)):
+    # # # If AOI is a shapely geometry, convert AOI into GeoPandas dataframe 
+    # if isinstance(AOI, (shapely.geometry.point.Point, 
+    #         shapely.geometry.multipoint.MultiPoint,
+    #         shapely.geometry.linestring.LineString, 
+    #         shapely.geometry.multilinestring.MultiLineString, 
+    #         shapely.geometry.polygon.Polygon, 
+    #         shapely.geometry.multipolygon.MultiPolygon)):
         
-        # convert shapely geometry to geopandas dataframe
-        AOI = shapely_to_gpd(AOI)
+    #     # convert shapely geometry to geopandas dataframe
+    #     AOI = utils.shapely_to_gpd(AOI)
+
+    # check that AOI meets requirements, if a shapely geometry the AOI is transformed into a geodataframe
+    AOI = utils.check_aoi(AOI)
 
     # 5. AOI filter
     if AOI is not None:
         catalog = find_intersects(
             catalog = catalog,
             AOI     = AOI
             )
@@ -527,8 +485,53 @@
 #             catalog = catalog,
 #             AOI     = AOI
 #             )
         
 #     # remove duplicates
 #     catalog = catalog[~catalog.drop(['URL'], axis=1).duplicated()]
 
-#     return catalog
+#     return catalog
+
+# def shapely_to_gpd(AOI):
+
+#     """Convert a Shapely object to a GeoDataFrame.
+
+#     Args:
+#         AOI (shapely.geometry.base.BaseGeometry): The area of interest as a Shapely object.
+
+#     Returns:
+#         GeoDataFrame: A GeoDataFrame representing the area of interest.
+#             The GeoDataFrame has a single geometry column with an automatically assigned CRS (either EPSG:4326 or EPSG:5070)
+
+#     Note:
+#         The function assumes that the shapely AOI is in either WGS84 (EPSG:4326) or NAD83 (EPSG:5070) coordinate system.
+#     """
+
+#     # convex hull
+#     chull = AOI.convex_hull
+
+#     # check if convex hull is a point or a polygon
+#     if isinstance(chull, shapely.geometry.point.Point):
+#         xx, yy = chull.coords.xy
+#     else:
+#         xx, yy = chull.exterior.coords.xy
+
+#     # bounding box
+#     xmax = np.asarray(xx).max()
+#     xmin = np.asarray(xx).min()
+#     ymax = np.asarray(yy).max()
+#     ymin = np.asarray(yy).min()
+
+#     # check if AOI is in WGS84 or NAD83
+#     if (ymax >= -90 and ymax <= 90
+#         and ymin <= 90 and ymin >= -90
+#         and xmax >= -180 and xmax <= 180
+#         and xmin <= 180 and xmin >= -180):
+#         print("Assuming AOI CRS is EPSG:4326 (WGS84)")
+#         crs = CRS.from_epsg(4326)
+#     else:
+#         print("Assuming AOI CRS is EPSG:5070 (NAD83)")
+#         crs = CRS.from_epsg(5070)
+
+#     out = gpd.GeoDataFrame(geometry = [AOI], crs = crs)
+
+#     return out
```

### Comparing `climatePy-0.4.30/climatePy/_dap.py` & `climatePy-0.4.31/climatePy/_dap.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,24 +368,27 @@
 
             # extend list with URL
             url_lst.extend(URL)
 
             # set URL to list of URLS
             URL = url_lst
             
-        # If AOI is a shapely geometry, convert AOI into GeoPandas dataframe 
-        if isinstance(AOI, (shapely.geometry.point.Point, 
-                            shapely.geometry.multipoint.MultiPoint,
-                            shapely.geometry.linestring.LineString, 
-                            shapely.geometry.multilinestring.MultiLineString, 
-                            shapely.geometry.polygon.Polygon, 
-                            shapely.geometry.multipolygon.MultiPolygon)):
+        # # If AOI is a shapely geometry, convert AOI into geodataframe
+        # if isinstance(AOI, (shapely.geometry.point.Point, 
+        #                     shapely.geometry.multipoint.MultiPoint,
+        #                     shapely.geometry.linestring.LineString, 
+        #                     shapely.geometry.multilinestring.MultiLineString, 
+        #                     shapely.geometry.polygon.Polygon, 
+        #                     shapely.geometry.multipolygon.MultiPolygon)):
             
-            # convert shapely geometry to geopandas dataframe
-            AOI = climatepy_filter.shapely_to_gpd(AOI)
+        #     # convert shapely geometry to geopandas dataframe
+        #     AOI = utils.shapely_to_gpd(AOI)
+
+        # check that AOI meets requirements, if a shapely geometry the AOI is transformed into a geodataframe
+        AOI = utils.check_aoi(AOI)
             
         # check if "vrt" or "tif" in URL list, or if "vsi" in all of URL list
         if any([utils.getExtension(i) in ['vrt', "tif"] for i in URL]) or all(["vsi" in i for i in URL]):
 
             if verbose:
                 print("Getting VRT/TIF data")
```

### Comparing `climatePy-0.4.30/climatePy/_netrc_utils.py` & `climatePy-0.4.31/climatePy/_netrc_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.30/climatePy/_shortcuts.py` & `climatePy-0.4.31/climatePy/_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.30/climatePy/_utils.py` & `climatePy-0.4.31/climatePy/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,105 @@
 
 # warnings lib
 import warnings
 
 # suppress warnings
 warnings.filterwarnings('ignore', category=Warning)
 
+def shapely_to_gpd(AOI):
+
+    """Convert a Shapely object to a GeoDataFrame.
+
+    Args:
+        AOI (shapely.geometry.base.BaseGeometry): The area of interest as a Shapely object.
+
+    Returns:
+        GeoDataFrame: A GeoDataFrame representing the area of interest.
+            The GeoDataFrame has a single geometry column with an automatically assigned CRS (either EPSG:4326 or EPSG:5070)
+
+    Note:
+        The function assumes that the shapely AOI is in either WGS84 (EPSG:4326) or NAD83 (EPSG:5070) coordinate system.
+    """
+
+    # convex hull
+    chull = AOI.convex_hull
+
+    # check if convex hull is a point or a polygon
+    if isinstance(chull, shapely.geometry.point.Point):
+        xx, yy = chull.coords.xy
+    else:
+        xx, yy = chull.exterior.coords.xy
+
+    # bounding box
+    xmax = np.asarray(xx).max()
+    xmin = np.asarray(xx).min()
+    ymax = np.asarray(yy).max()
+    ymin = np.asarray(yy).min()
+
+    # check if AOI is in WGS84 or NAD83
+    if (ymax >= -90 and ymax <= 90
+        and ymin <= 90 and ymin >= -90
+        and xmax >= -180 and xmax <= 180
+        and xmin <= 180 and xmin >= -180):
+        print("Assuming AOI CRS is EPSG:4326 (WGS84)")
+        crs = CRS.from_epsg(4326)
+    else:
+        print("Assuming AOI CRS is EPSG:5070 (NAD83)")
+        crs = CRS.from_epsg(5070)
+
+    out = gpd.GeoDataFrame(geometry = [AOI], crs = crs)
+
+    return out
+
+def check_aoi(AOI):
+
+    """Check that the AOI is in a valid format and change if needed.
+
+    If AOI is a GeoDataFrame or GeoSeries with more than 1 geometry, converts AOI to a GeoDataFrame with a 
+    single geometry representing the total bounds of all the geometries in the GeoDataFrame.
+
+    If AOI is a shapely geometry, converts AOI to a GeoDataFrame with a single geometry representing the AOI.
+
+    Args:
+        AOI (GeoDataFrame, GeoSeries, or shapely.geometry.base.BaseGeometry): The area of interest as a GeoDataFrame, GeoSeries, or Shapely object.
+
+    """
+
+    # check if AOI is None
+    if AOI is None:
+        return None
+    
+    # geodataframe check
+    if isinstance(AOI, (gpd.GeoDataFrame, gpd.GeoSeries)):
+
+        if AOI.crs is None:
+            raise ValueError("AOI GeoDataFrame does not have a CRS attribute. Please set a CRS attribute for the AOI GeoDataFrame.")
+
+        # if more than one row/geometry, change geodataframe to be the total bounds of all the shapes in the geodataframe
+        if len(AOI) > 1: 
+            xmin, ymin, xmax, ymax = AOI.geometry.total_bounds
+            AOI = gpd.GeoDataFrame(geometry=[shapely.geometry.box(xmin, ymin, xmax, ymax)], crs=AOI.crs)
+            # bb = AOI.geometry.total_bounds
+            # AOI = gpd.GeoDataFrame(geometry=[shapely.geometry.box(bb[0], bb[1], bb[2], bb[3])], crs=AOI.crs)
+
+            return AOI
+        
+    # If AOI is a shapely geometry, convert AOI into GeoPandas dataframe 
+    if isinstance(AOI, (shapely.geometry.point.Point, 
+                        shapely.geometry.multipoint.MultiPoint,
+                        shapely.geometry.linestring.LineString, 
+                        shapely.geometry.multilinestring.MultiLineString, 
+                        shapely.geometry.polygon.Polygon, 
+                        shapely.geometry.multipolygon.MultiPolygon)):
+            
+            # convert shapely geometry to geopandas dataframe
+            AOI = shapely_to_gpd(AOI)
+    
+    return AOI
+
 def getExtension(x):
     """Extract the file extension from a string"""
 
     dot_pos = x.rfind('.')
     if dot_pos == -1:
         return ''
     else:
```

### Comparing `climatePy-0.4.30/climatePy/data/catalog.csv` & `climatePy-0.4.31/climatePy/data/catalog.csv`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.30/climatePy.egg-info/PKG-INFO` & `climatePy-0.4.31/climatePy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.30
+Version: 0.4.31
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `climatePy-0.4.30/setup.py` & `climatePy-0.4.31/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="climatePy",                         # pkg name
     # version="0.0.4.24",                        # version
-    version='0.4.30',
+    version='0.4.31',
     author="Angus Watters, Mike Johnson",     # authors
     description="A Python package for getting point and gridded climate data by AOI",
     long_description=long_description,      # long description is read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # python modules to install
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `climatePy-0.4.30/tests/test_shortcuts.py` & `climatePy-0.4.31/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.30/tests/test_utils.py` & `climatePy-0.4.31/tests/test_utils.py`

 * *Files identical despite different names*

