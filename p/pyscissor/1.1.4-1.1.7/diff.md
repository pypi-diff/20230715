# Comparing `tmp/pyscissor-1.1.4.tar.gz` & `tmp/pyscissor-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscissor-1.1.4.tar", last modified: Wed Sep 22 17:56:23 2021, max compression
+gzip compressed data, was "pyscissor-1.1.7.tar", last modified: Sat Jul 15 13:52:53 2023, max compression
```

## Comparing `pyscissor-1.1.4.tar` & `pyscissor-1.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 17:56:23.483105 pyscissor-1.1.4/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1070 2021-09-22 17:56:00.000000 pyscissor-1.1.4/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (121)       33 2021-09-22 17:56:00.000000 pyscissor-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3502 2021-09-22 17:56:23.483105 pyscissor-1.1.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 17:56:23.483105 pyscissor-1.1.4/pyscissor/
--rwxr-xr-x   0 runner    (1001) docker     (121)      117 2021-09-22 17:56:00.000000 pyscissor-1.1.4/pyscissor/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      530 2021-09-22 17:56:00.000000 pyscissor-1.1.4/pyscissor/helper.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3313 2021-09-22 17:56:00.000000 pyscissor-1.1.4/pyscissor/pinpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11973 2021-09-22 17:56:00.000000 pyscissor-1.1.4/pyscissor/scissor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 17:56:23.483105 pyscissor-1.1.4/pyscissor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3502 2021-09-22 17:56:23.000000 pyscissor-1.1.4/pyscissor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      407 2021-09-22 17:56:23.000000 pyscissor-1.1.4/pyscissor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-22 17:56:23.000000 pyscissor-1.1.4/pyscissor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-22 17:56:23.000000 pyscissor-1.1.4/pyscissor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-09-22 17:56:23.000000 pyscissor-1.1.4/pyscissor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-09-22 17:56:23.000000 pyscissor-1.1.4/pyscissor.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)       79 2021-09-22 17:56:23.483105 pyscissor-1.1.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1035 2021-09-22 17:56:00.000000 pyscissor-1.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-22 17:56:23.483105 pyscissor-1.1.4/tools/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-09-22 17:56:00.000000 pyscissor-1.1.4/tools/nc2ts_by_shp.cmd
--rwxr-xr-x   0 runner    (1001) docker     (121)     7658 2021-09-22 17:56:00.000000 pyscissor-1.1.4/tools/nc2ts_by_shp.py
--rw-r--r--   0 runner    (1001) docker     (121)       45 2021-09-22 17:56:00.000000 pyscissor-1.1.4/tools/nc2ts_by_xy.cmd
--rwxr-xr-x   0 runner    (1001) docker     (121)     3975 2021-09-22 17:56:00.000000 pyscissor-1.1.4/tools/nc2ts_by_xy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:52:53.223504 pyscissor-1.1.7/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1070 2023-07-15 13:52:22.000000 pyscissor-1.1.7/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-07-15 13:52:22.000000 pyscissor-1.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-15 13:52:53.223504 pyscissor-1.1.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:52:53.219504 pyscissor-1.1.7/pyscissor/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      104 2023-07-15 13:52:22.000000 pyscissor-1.1.7/pyscissor/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      530 2023-07-15 13:52:22.000000 pyscissor-1.1.7/pyscissor/helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3313 2023-07-15 13:52:22.000000 pyscissor-1.1.7/pyscissor/pinpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12183 2023-07-15 13:52:22.000000 pyscissor-1.1.7/pyscissor/scissor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:52:53.219504 pyscissor-1.1.7/pyscissor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-15 13:52:53.000000 pyscissor-1.1.7/pyscissor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-15 13:52:53.000000 pyscissor-1.1.7/pyscissor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 13:52:53.000000 pyscissor-1.1.7/pyscissor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 13:52:53.000000 pyscissor-1.1.7/pyscissor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-15 13:52:53.000000 pyscissor-1.1.7/pyscissor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-15 13:52:53.000000 pyscissor-1.1.7/pyscissor.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       79 2023-07-15 13:52:53.223504 pyscissor-1.1.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1035 2023-07-15 13:52:22.000000 pyscissor-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:52:53.223504 pyscissor-1.1.7/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-15 13:52:22.000000 pyscissor-1.1.7/tools/nc2ts_by_shp.cmd
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7658 2023-07-15 13:52:22.000000 pyscissor-1.1.7/tools/nc2ts_by_shp.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-15 13:52:22.000000 pyscissor-1.1.7/tools/nc2ts_by_xy.cmd
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3975 2023-07-15 13:52:22.000000 pyscissor-1.1.7/tools/nc2ts_by_xy.py
```

### Comparing `pyscissor-1.1.4/LICENSE` & `pyscissor-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscissor-1.1.4/PKG-INFO` & `pyscissor-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyscissor
-Version: 1.1.4
+Version: 1.1.7
 Summary: A python module for obtaining reduced(min,max,avg) value from netCDF file under a polygon region
 Home-page: https://github.com/nzahasan/pyscissor
 Author: nzahasan
 Author-email: nzahasan@gmail.com
 License: MIT
 Keywords: netcdf,crop,shapefile
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyscissor
 ![Supported Version](https://img.shields.io/badge/python-3.6|3.7|3.8-blue.svg) 
 ![Action: Build](https://github.com/nzahasan/pyscissor/workflows/build/badge.svg)
@@ -114,8 +113,7 @@
 	-o   = output file name
 
 
 ### Causes of Erroneous output
 
 	- when shapefile and netcdf file have different projection
 	- shapefile dosen't fully reside within netcdf bounds 
-
```

#### html2text {}

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1 Name: pyscissor Version: 1.1.4 Summary: A python module
+Metadata-Version: 2.1 Name: pyscissor Version: 1.1.7 Summary: A python module
 for obtaining reduced(min,max,avg) value from netCDF file under a polygon
 region Home-page: https://github.com/nzahasan/pyscissor Author: nzahasan
 Author-email: nzahasan@gmail.com License: MIT Keywords: netcdf,crop,shapefile
-Platform: UNKNOWN Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE # pyscissor ![Supported Version](https://
-img.shields.io/badge/python-3.6|3.7|3.8-blue.svg) ![Action: Build](https://
-github.com/nzahasan/pyscissor/workflows/build/badge.svg) ![publish](https://
-github.com/nzahasan/pyscissor/workflows/publish/badge.svg) [![License: MIT]
-(https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/
-licenses/MIT) A Python3 module for extracting data from netcdf file under a
-shapefile region. [data/sample.png] ### Installation pyscissor can be installed
-using the following commands ```bash $ git clone https://github.com/nzahasan/
-pyscissor.git $ cd pyscissor $ python3 setup.py install ``` or using pip
-```bash $ pip install pyscissor ``` ### Using pyscissor ```python import fiona
-import numpy as np from netCDF4 import Dataset from shapely.geometry import
-shape from pyscissor import scissor # read shapefile sf = fiona.open('data/
-shape.geojson') shapely_shp =shape(sf.get(0)['geometry']) # read netcdf nf =
-Dataset('data/sample_2.nc','r') lats = nf.variables['lat'][:] lons =
-nf.variables['lon'][:] # create scissor object pys = scissor
-(shapely_shp,lats,lons) weight_grid = pys.get_masked_weight() #=> returns a
-masked array containing weights # get weighted average avg = np.average
-(var,weights=weight_grid) # if only intersection mask with shape is needed use
-`weight_grid.mask` ``` A detailed use case can be found in the following
-jupyter notebooks - example_01.ipynb - example_02.ipynb - example_03.ipynb -
-example_04.ipynb ### Using nc2ts_by_shp.py this package contains a
-`nc2ts_by_shp.py` script. A command line tool that can be used to quickly
-extract reduced(min/max/average/weighted average) time-series form netcdf file
-with shapefile ```bash # with 3d array [data/sample_2.nc] generel case $
-nc2ts_by_shp.py -nc=sample_2.nc -nci='Y=lat;X=lon;T=time;V=tmin;' -
-s=shape_esri.zip \ -sp='ADM2_EN;ADM3_EN' -r=avg -o=test2.csv # with 4d array
-[data/sample_1.nc] $ nc2ts_by_shp.py -nc=sample_1.nc -
-nci='Y=lat;X=lon;T=time;V=temperature;slicer=[:,0,:,:]' -sf=shape_esri.zip \ -
-sfp='ADM2_EN;ADM3_EN' -r=wavg -o=test1.csv ``` Options: -nc = netcdf file -nci
-= netcdf variable and dimension information available options: X = x dimension
-variable name, Y = y dimension variable name, T = time dimension variable name,
-V = variable name, slicer = slicing index for obtaining 3d array [optional]
-note: `slicer` is required if variable has more than three dimension -sf =
-shape file ( can be zipped shapefile, shapefile or geojson ) -sfp = shapefile
-properties only required when shapefile contains multiple records -r = reducer,
-default is average Available options: min,max,avg,wavg -o = output file name
-### Causes of Erroneous output - when shapefile and netcdf file have different
-projection - shapefile dosen't fully reside within netcdf bounds
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE # pyscissor ![Supported Version](https://img.shields.io/badge/python-
+3.6|3.7|3.8-blue.svg) ![Action: Build](https://github.com/nzahasan/pyscissor/
+workflows/build/badge.svg) ![publish](https://github.com/nzahasan/pyscissor/
+workflows/publish/badge.svg) [![License: MIT](https://img.shields.io/badge/
+License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) A Python3 module
+for extracting data from netcdf file under a shapefile region. [data/
+sample.png] ### Installation pyscissor can be installed using the following
+commands ```bash $ git clone https://github.com/nzahasan/pyscissor.git $ cd
+pyscissor $ python3 setup.py install ``` or using pip ```bash $ pip install
+pyscissor ``` ### Using pyscissor ```python import fiona import numpy as np
+from netCDF4 import Dataset from shapely.geometry import shape from pyscissor
+import scissor # read shapefile sf = fiona.open('data/shape.geojson')
+shapely_shp =shape(sf.get(0)['geometry']) # read netcdf nf = Dataset('data/
+sample_2.nc','r') lats = nf.variables['lat'][:] lons = nf.variables['lon'][:] #
+create scissor object pys = scissor(shapely_shp,lats,lons) weight_grid =
+pys.get_masked_weight() #=> returns a masked array containing weights # get
+weighted average avg = np.average(var,weights=weight_grid) # if only
+intersection mask with shape is needed use `weight_grid.mask` ``` A detailed
+use case can be found in the following jupyter notebooks - example_01.ipynb -
+example_02.ipynb - example_03.ipynb - example_04.ipynb ### Using
+nc2ts_by_shp.py this package contains a `nc2ts_by_shp.py` script. A command
+line tool that can be used to quickly extract reduced(min/max/average/weighted
+average) time-series form netcdf file with shapefile ```bash # with 3d array
+[data/sample_2.nc] generel case $ nc2ts_by_shp.py -nc=sample_2.nc -
+nci='Y=lat;X=lon;T=time;V=tmin;' -s=shape_esri.zip \ -sp='ADM2_EN;ADM3_EN' -
+r=avg -o=test2.csv # with 4d array [data/sample_1.nc] $ nc2ts_by_shp.py -
+nc=sample_1.nc -nci='Y=lat;X=lon;T=time;V=temperature;slicer=[:,0,:,:]' -
+sf=shape_esri.zip \ -sfp='ADM2_EN;ADM3_EN' -r=wavg -o=test1.csv ``` Options: -
+nc = netcdf file -nci = netcdf variable and dimension information available
+options: X = x dimension variable name, Y = y dimension variable name, T = time
+dimension variable name, V = variable name, slicer = slicing index for
+obtaining 3d array [optional] note: `slicer` is required if variable has more
+than three dimension -sf = shape file ( can be zipped shapefile, shapefile or
+geojson ) -sfp = shapefile properties only required when shapefile contains
+multiple records -r = reducer, default is average Available options:
+min,max,avg,wavg -o = output file name ### Causes of Erroneous output - when
+shapefile and netcdf file have different projection - shapefile dosen't fully
+reside within netcdf bounds
```

### Comparing `pyscissor-1.1.4/pyscissor/helper.py` & `pyscissor-1.1.7/pyscissor/helper.py`

 * *Files identical despite different names*

### Comparing `pyscissor-1.1.4/pyscissor/pinpoint.py` & `pyscissor-1.1.7/pyscissor/pinpoint.py`

 * *Files identical despite different names*

### Comparing `pyscissor-1.1.4/pyscissor/scissor.py` & `pyscissor-1.1.7/pyscissor/scissor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 import numpy as np
 from shapely.geometry import Polygon,MultiPolygon
 
 class scissor():    
 
-    def __init__(self, shape_obj,lattitude_array,longitude_array):
+    def __init__(self, shape_obj, lattitude_array,longitude_array):
         
         self.lats  = lattitude_array
         self.nlats = self.lats.shape[0]
         
 
         self.lons  = longitude_array
         self.nlons = self.lons.shape[0]
@@ -17,31 +17,31 @@
         
         # check for shapely polygon
         if isinstance(shape_obj,Polygon) or isinstance(shape_obj,MultiPolygon):
             self.shape_obj = shape_obj
         else:
             raise Exception('Invalid object, Must be a shapely Polygon or MultiPolygon.')
 
-        # find nearest neighbours for lat and lons
+        # find nearest neighbors for lat and lons
         min_lon_idx = np.abs(self.lons - self.shape_obj.bounds[0]).argmin()
         max_lon_idx = np.abs(self.lons - self.shape_obj.bounds[2]).argmin()
 
         min_lat_idx = np.abs(self.lats - self.shape_obj.bounds[1]).argmin()
         max_lat_idx = np.abs(self.lats - self.shape_obj.bounds[3]).argmin()
 
         # expand lat lon index by 1 cell 
         # only search/operate within these bounds
         self.lon_idx_range = np.arange( 
             (min_lon_idx-1) if min_lon_idx>0 else 0,
             (max_lon_idx+1)+1 if (max_lon_idx+1)<self.nlons else max_lon_idx+1
         )
 
         # lat can be laid in 2 ways:
-        #   - lat deceases with index[generel case] / Lat reversed
-        #   - lat inceases with index[odd case]  
+        #   - lat deceases with index[general case] / Lat reversed
+        #   - lat increases with index[odd case]  
 
         # shape bound sample (90.53, 20.74, 92.68, 24.26)
 
         self.lat_reversed = True
 
         if self.lats[1]>self.lats[0]:
             self.lat_reversed = False
@@ -59,20 +59,27 @@
                 (max_lat_idx+1)+1 if (max_lat_idx+1)< self.nlats else max_lat_idx+1
             )
 
     def __repr__(self):
         return '<pyscissor_instance>'        
 
 
+    def get_masked_weight(self, recursive=True):
+        
+        if recursive == False:
+            return self.get_masked_weight_iter()
+        
+        return self.get_masked_weight_recursive()
+        
     
-    def get_masked_weight(self):
+    def get_masked_weight_iter(self):
         
         ''' 
 
-        # generel case
+        # general case
                 
                                        r-1,c 
                                          |
                                          |
                                          |
                       [1,0]---------[r+(r-1)]/2--------[1,1]
                         |                |               |
@@ -161,16 +168,16 @@
                      |
                      |
                      |
                   r+1,c
         '''
 
 
-        weight_grid = np.zeros((self.nlats,self.nlons))
-        mask_grid   = np.ones((self.nlats,self.nlons),dtype=np.bool)
+        weight_grid = np.zeros((self.nlats, self.nlons))
+        mask_grid   = np.ones((self.nlats, self.nlons), dtype=bool)
 
         for ry in self.lat_idx_range:
             
             for cx in self.lon_idx_range:
             
                 # edge cases
 
@@ -251,15 +258,15 @@
 
         # root func call
         if root==True:
             lat_ids       = self.lat_idx_range.copy()
             lon_ids       = self.lon_idx_range.copy()
             masked_weight = np.ma.masked_array(
                                 np.zeros((self.nlats,self.nlons)),
-                                mask = np.ones((self.nlats,self.nlons),dtype=np.bool)
+                                mask = np.ones((self.nlats,self.nlons), dtype=bool)
                             )
 
         gx0,gx1= lon_ids[0],lon_ids[-1]
         gy0,gy1= lat_ids[-1],lat_ids[0]
 
         if gx0==0:
             x0 = self.lons[gx0] - abs( self.lons[gx0+1] - self.lons[gx0])/2
```

### Comparing `pyscissor-1.1.4/pyscissor.egg-info/PKG-INFO` & `pyscissor-1.1.7/pyscissor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyscissor
-Version: 1.1.4
+Version: 1.1.7
 Summary: A python module for obtaining reduced(min,max,avg) value from netCDF file under a polygon region
 Home-page: https://github.com/nzahasan/pyscissor
 Author: nzahasan
 Author-email: nzahasan@gmail.com
 License: MIT
 Keywords: netcdf,crop,shapefile
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyscissor
 ![Supported Version](https://img.shields.io/badge/python-3.6|3.7|3.8-blue.svg) 
 ![Action: Build](https://github.com/nzahasan/pyscissor/workflows/build/badge.svg)
@@ -114,8 +113,7 @@
 	-o   = output file name
 
 
 ### Causes of Erroneous output
 
 	- when shapefile and netcdf file have different projection
 	- shapefile dosen't fully reside within netcdf bounds 
-
```

#### html2text {}

```diff
@@ -1,43 +1,43 @@
-Metadata-Version: 2.1 Name: pyscissor Version: 1.1.4 Summary: A python module
+Metadata-Version: 2.1 Name: pyscissor Version: 1.1.7 Summary: A python module
 for obtaining reduced(min,max,avg) value from netCDF file under a polygon
 region Home-page: https://github.com/nzahasan/pyscissor Author: nzahasan
 Author-email: nzahasan@gmail.com License: MIT Keywords: netcdf,crop,shapefile
-Platform: UNKNOWN Requires-Python: >=3.6 Description-Content-Type: text/
-markdown License-File: LICENSE # pyscissor ![Supported Version](https://
-img.shields.io/badge/python-3.6|3.7|3.8-blue.svg) ![Action: Build](https://
-github.com/nzahasan/pyscissor/workflows/build/badge.svg) ![publish](https://
-github.com/nzahasan/pyscissor/workflows/publish/badge.svg) [![License: MIT]
-(https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/
-licenses/MIT) A Python3 module for extracting data from netcdf file under a
-shapefile region. [data/sample.png] ### Installation pyscissor can be installed
-using the following commands ```bash $ git clone https://github.com/nzahasan/
-pyscissor.git $ cd pyscissor $ python3 setup.py install ``` or using pip
-```bash $ pip install pyscissor ``` ### Using pyscissor ```python import fiona
-import numpy as np from netCDF4 import Dataset from shapely.geometry import
-shape from pyscissor import scissor # read shapefile sf = fiona.open('data/
-shape.geojson') shapely_shp =shape(sf.get(0)['geometry']) # read netcdf nf =
-Dataset('data/sample_2.nc','r') lats = nf.variables['lat'][:] lons =
-nf.variables['lon'][:] # create scissor object pys = scissor
-(shapely_shp,lats,lons) weight_grid = pys.get_masked_weight() #=> returns a
-masked array containing weights # get weighted average avg = np.average
-(var,weights=weight_grid) # if only intersection mask with shape is needed use
-`weight_grid.mask` ``` A detailed use case can be found in the following
-jupyter notebooks - example_01.ipynb - example_02.ipynb - example_03.ipynb -
-example_04.ipynb ### Using nc2ts_by_shp.py this package contains a
-`nc2ts_by_shp.py` script. A command line tool that can be used to quickly
-extract reduced(min/max/average/weighted average) time-series form netcdf file
-with shapefile ```bash # with 3d array [data/sample_2.nc] generel case $
-nc2ts_by_shp.py -nc=sample_2.nc -nci='Y=lat;X=lon;T=time;V=tmin;' -
-s=shape_esri.zip \ -sp='ADM2_EN;ADM3_EN' -r=avg -o=test2.csv # with 4d array
-[data/sample_1.nc] $ nc2ts_by_shp.py -nc=sample_1.nc -
-nci='Y=lat;X=lon;T=time;V=temperature;slicer=[:,0,:,:]' -sf=shape_esri.zip \ -
-sfp='ADM2_EN;ADM3_EN' -r=wavg -o=test1.csv ``` Options: -nc = netcdf file -nci
-= netcdf variable and dimension information available options: X = x dimension
-variable name, Y = y dimension variable name, T = time dimension variable name,
-V = variable name, slicer = slicing index for obtaining 3d array [optional]
-note: `slicer` is required if variable has more than three dimension -sf =
-shape file ( can be zipped shapefile, shapefile or geojson ) -sfp = shapefile
-properties only required when shapefile contains multiple records -r = reducer,
-default is average Available options: min,max,avg,wavg -o = output file name
-### Causes of Erroneous output - when shapefile and netcdf file have different
-projection - shapefile dosen't fully reside within netcdf bounds
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE # pyscissor ![Supported Version](https://img.shields.io/badge/python-
+3.6|3.7|3.8-blue.svg) ![Action: Build](https://github.com/nzahasan/pyscissor/
+workflows/build/badge.svg) ![publish](https://github.com/nzahasan/pyscissor/
+workflows/publish/badge.svg) [![License: MIT](https://img.shields.io/badge/
+License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) A Python3 module
+for extracting data from netcdf file under a shapefile region. [data/
+sample.png] ### Installation pyscissor can be installed using the following
+commands ```bash $ git clone https://github.com/nzahasan/pyscissor.git $ cd
+pyscissor $ python3 setup.py install ``` or using pip ```bash $ pip install
+pyscissor ``` ### Using pyscissor ```python import fiona import numpy as np
+from netCDF4 import Dataset from shapely.geometry import shape from pyscissor
+import scissor # read shapefile sf = fiona.open('data/shape.geojson')
+shapely_shp =shape(sf.get(0)['geometry']) # read netcdf nf = Dataset('data/
+sample_2.nc','r') lats = nf.variables['lat'][:] lons = nf.variables['lon'][:] #
+create scissor object pys = scissor(shapely_shp,lats,lons) weight_grid =
+pys.get_masked_weight() #=> returns a masked array containing weights # get
+weighted average avg = np.average(var,weights=weight_grid) # if only
+intersection mask with shape is needed use `weight_grid.mask` ``` A detailed
+use case can be found in the following jupyter notebooks - example_01.ipynb -
+example_02.ipynb - example_03.ipynb - example_04.ipynb ### Using
+nc2ts_by_shp.py this package contains a `nc2ts_by_shp.py` script. A command
+line tool that can be used to quickly extract reduced(min/max/average/weighted
+average) time-series form netcdf file with shapefile ```bash # with 3d array
+[data/sample_2.nc] generel case $ nc2ts_by_shp.py -nc=sample_2.nc -
+nci='Y=lat;X=lon;T=time;V=tmin;' -s=shape_esri.zip \ -sp='ADM2_EN;ADM3_EN' -
+r=avg -o=test2.csv # with 4d array [data/sample_1.nc] $ nc2ts_by_shp.py -
+nc=sample_1.nc -nci='Y=lat;X=lon;T=time;V=temperature;slicer=[:,0,:,:]' -
+sf=shape_esri.zip \ -sfp='ADM2_EN;ADM3_EN' -r=wavg -o=test1.csv ``` Options: -
+nc = netcdf file -nci = netcdf variable and dimension information available
+options: X = x dimension variable name, Y = y dimension variable name, T = time
+dimension variable name, V = variable name, slicer = slicing index for
+obtaining 3d array [optional] note: `slicer` is required if variable has more
+than three dimension -sf = shape file ( can be zipped shapefile, shapefile or
+geojson ) -sfp = shapefile properties only required when shapefile contains
+multiple records -r = reducer, default is average Available options:
+min,max,avg,wavg -o = output file name ### Causes of Erroneous output - when
+shapefile and netcdf file have different projection - shapefile dosen't fully
+reside within netcdf bounds
```

### Comparing `pyscissor-1.1.4/setup.py` & `pyscissor-1.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `pyscissor-1.1.4/tools/nc2ts_by_shp.py` & `pyscissor-1.1.7/tools/nc2ts_by_shp.py`

 * *Files identical despite different names*

### Comparing `pyscissor-1.1.4/tools/nc2ts_by_xy.py` & `pyscissor-1.1.7/tools/nc2ts_by_xy.py`

 * *Files identical despite different names*

