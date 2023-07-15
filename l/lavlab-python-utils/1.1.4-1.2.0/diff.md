# Comparing `tmp/lavlab-python-utils-1.1.4.tar.gz` & `tmp/lavlab-python-utils-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavlab-python-utils-1.1.4.tar", last modified: Tue Jul 11 16:09:15 2023, max compression
+gzip compressed data, was "lavlab-python-utils-1.2.0.tar", last modified: Sat Jul 15 18:30:10 2023, max compression
```

## Comparing `lavlab-python-utils-1.1.4.tar` & `lavlab-python-utils-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:09:15.492064 lavlab-python-utils-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-11 16:09:15.492064 lavlab-python-utils-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-11 16:08:58.000000 lavlab-python-utils-1.1.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-11 16:08:58.000000 lavlab-python-utils-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 16:09:15.492064 lavlab-python-utils-1.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:09:15.492064 lavlab-python-utils-1.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:09:15.492064 lavlab-python-utils-1.1.4/src/lavlab/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-11 16:08:58.000000 lavlab-python-utils-1.1.4/src/lavlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-11 16:08:58.000000 lavlab-python-utils-1.1.4/src/lavlab/omero_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    27605 2023-07-11 16:08:58.000000 lavlab-python-utils-1.1.4/src/lavlab/omero_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-11 16:08:58.000000 lavlab-python-utils-1.1.4/src/lavlab/python_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:09:15.492064 lavlab-python-utils-1.1.4/src/lavlab_python_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-11 16:09:15.000000 lavlab-python-utils-1.1.4/src/lavlab_python_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-11 16:09:15.000000 lavlab-python-utils-1.1.4/src/lavlab_python_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:09:15.000000 lavlab-python-utils-1.1.4/src/lavlab_python_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 16:09:15.000000 lavlab-python-utils-1.1.4/src/lavlab_python_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 16:09:15.000000 lavlab-python-utils-1.1.4/src/lavlab_python_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:09:15.492064 lavlab-python-utils-1.1.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-11 16:08:58.000000 lavlab-python-utils-1.1.4/test/test_omero_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-11 16:08:58.000000 lavlab-python-utils-1.1.4/test/test_python_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:30:10.783745 lavlab-python-utils-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-15 18:30:10.783745 lavlab-python-utils-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-15 18:29:59.000000 lavlab-python-utils-1.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-15 18:29:59.000000 lavlab-python-utils-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 18:30:10.783745 lavlab-python-utils-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:30:10.783745 lavlab-python-utils-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:30:10.783745 lavlab-python-utils-1.2.0/src/lavlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-15 18:29:59.000000 lavlab-python-utils-1.2.0/src/lavlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-15 18:29:59.000000 lavlab-python-utils-1.2.0/src/lavlab/omero_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30893 2023-07-15 18:29:59.000000 lavlab-python-utils-1.2.0/src/lavlab/omero_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10553 2023-07-15 18:29:59.000000 lavlab-python-utils-1.2.0/src/lavlab/python_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:30:10.783745 lavlab-python-utils-1.2.0/src/lavlab_python_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-15 18:30:10.000000 lavlab-python-utils-1.2.0/src/lavlab_python_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-15 18:30:10.000000 lavlab-python-utils-1.2.0/src/lavlab_python_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 18:30:10.000000 lavlab-python-utils-1.2.0/src/lavlab_python_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-15 18:30:10.000000 lavlab-python-utils-1.2.0/src/lavlab_python_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-15 18:30:10.000000 lavlab-python-utils-1.2.0/src/lavlab_python_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:30:10.783745 lavlab-python-utils-1.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-15 18:29:59.000000 lavlab-python-utils-1.2.0/test/test_omero_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-15 18:29:59.000000 lavlab-python-utils-1.2.0/test/test_python_utils.py
```

### Comparing `lavlab-python-utils-1.1.4/PKG-INFO` & `lavlab-python-utils-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: lavlab-python-utils
-Version: 1.1.4
+Version: 1.2.0
 Summary: LaViolette Lab utility package
 Author-email: Michael Barrett <mjbarrett@mcw.edu>
 Project-URL: Homepage, https://github.com/laviolette-lab/lavlab-python-utils
 Project-URL: Bug Tracker, https://github.com/laviolette-lab/lavlab-python-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 
 TODO: this readme
 =================
 for more info goto: https://lavlab-python-utils.readthedocs.io/en/latest/
 python3 -m unittest
```

### Comparing `lavlab-python-utils-1.1.4/pyproject.toml` & `lavlab-python-utils-1.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [project]
 name = "lavlab-python-utils"
 description = "LaViolette Lab utility package"
-version = "1.1.4"
+version = "1.2.0"
 
 authors = [
   { name="Michael Barrett", email="mjbarrett@mcw.edu" },
 ]
 
 readme = "README.rst"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 dependencies = [
   'omero-py >= 5.13.1',
-  'omero-scripts >= 5.7.1',
-  'scikit-image >= 0.19.3'
+  'tiatoolbox >= 1.4.0'
 ]
 
 [project.optional-dependencies]
 docs = ["sphinx>=6.2.1","docutils >= 0.18.1"]
 
 [project.urls]
 "Homepage" = "https://github.com/laviolette-lab/lavlab-python-utils"
```

### Comparing `lavlab-python-utils-1.1.4/src/lavlab/omero_asyncio.py` & `lavlab-python-utils-1.2.0/src/lavlab/omero_asyncio.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.1.4/src/lavlab/omero_util.py` & `lavlab-python-utils-1.2.0/src/lavlab/omero_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,33 +2,38 @@
 """
 Helper functions that handle high-level operations and translating asynchronous requests for easy development.
 """
 import os
 import asyncio
 import tempfile
 
+from io import BytesIO
+from collections.abc import AsyncGenerator
+
 import numpy as np
 from PIL import Image
-from skimage import draw
 
-from collections.abc import AsyncGenerator
+import scipy.ndimage
+from skimage import draw, morphology 
+
+from tiatoolbox.tools import tissuemask 
 
 from omero.gateway import _BlitzGateway, ImageWrapper, FileAnnotationWrapper, ShapeWrapper
 import omero.model.enums as omero_enums
 from omero.rtypes import rint, rstring
 
 from omero_model_RoiI import RoiI
 from omero_model_PolygonI import PolygonI
 from omero_model_EllipseI import EllipseI
 from omero_model_PolygonI import PolygonI
 from omero_model_RectangleI import RectangleI
 from omero_model_FileAnnotationI import FileAnnotationI
 
 from lavlab import omero_asyncio
-from lavlab.python_util import chunkify, merge_async_iters, interlace_lists, lookup_filetype_by_name, FILETYPE_DICTIONARY, rgba_to_uint, uint_to_rgba
+from lavlab.python_util import chunkify, merge_async_iters, interlace_lists, lookup_filetype_by_name, FILETYPE_DICTIONARY, rgba_to_uint, uint_to_rgba, create_array
 
 PARALLEL_STORE_COUNT=4
 """Number of pixel stores to be created for an image."""
 
 OMERO_DICTIONARY = {
     # TODO add real pixeltype support
     "PIXEL_TYPES": {
@@ -145,18 +150,18 @@
             if i == tile_len: await rps.close()
             else: i+=1
             yield rv, (z,c,t,tile)
 
 
     # force async client
     session =  omero_asyncio.AsyncSession(img._conn.c.sf)
-
+    session.setSecurityContext(img.details.group)
     # create parallel raw pixels stores
     jobs=[]
-    for chunk in chunkify(tiles, int(len(tiles)/PARALLEL_STORE_COUNT)):
+    for chunk in chunkify(tiles, PARALLEL_STORE_COUNT):
         jobs.append(work(img.getPrimaryPixels().getId(), chunk, resLvl))
     return merge_async_iters(*jobs)
 
 def getDownsampledXYDimensions(img: ImageWrapper, downsample_factor: int) -> tuple[int,int]:
     """
 Returns XY (rows,columns) dimensions of given image at the downsample.
 
@@ -256,18 +261,14 @@
 
 
 
 def getChannelsAtResolution(img: ImageWrapper, xy_dim: tuple[int,int], channels:list[int]=None) -> Image.Image:
     """
 Gathers tiles and scales down to desired resolution.
 
-Warns
--------
-Out of Memory issues ahead! Request a reasonable resolution!
-
 Parameters
 ----------
 img: omero.gateway.ImageWrapper
     Omero Image object from conn.getObjects().
 xy_dim: tuple(x,y)
     Tuple of desired dimensions (x,y)
 channels: tuple(int,...), default: all channels
@@ -280,37 +281,37 @@
     Python Image Object
     """
     async def work(img, xy, channels):
         res_lvl, xy_info = getClosestResolutionLevel(img, xy)
         images = []
         for channel in channels:
             tiles = createTileList2D(0,channel,0,*xy_info)
-            arr = np.zeros((xy_info[1], xy_info[0]), np.uint8)
+            arr = create_array((xy_info[1], xy_info[0]), np.uint8)
             async for tile, (z,c,t,coord) in getTiles(img,tiles,res_lvl):
                 arr [
                     coord[1]:coord[1]+coord[3],
                     coord[0]:coord[0]+coord[2],
                     c ] = tile
             image = Image.fromarray(arr)
             if image.size != xy:
                 del arr # just to be safe
                 image = image.resize(xy)
             images.append(image)
         return images
-
-    return asyncio.run(work(img, xy_dim, channels))
+    
+    event_loop = asyncio.get_running_loop()
+    if event_loop is None:
+        return asyncio.run(work(img, xy_dim, channels))
+    else:
+        return work(img,xy_dim,channels)
 
 def getImageAtResolution(img: ImageWrapper, xy_dim: tuple[int,int]) -> Image.Image:
     """
 Gathers tiles of full rgb image and scales down to desired resolution.
 
-Warns
--------
-Out of Memory issues ahead! Request a reasonable resolution!
-
 Parameters
 ----------
 img: omero.gateway.ImageWrapper
     Omero Image object from conn.getObjects().
 xy_dim: tuple(x,y)
     Tuple of desired dimensions (x,y)
 
@@ -319,30 +320,33 @@
 PIL.Image.Image
     Python Image Object
     """
     async def work(img, xy):
         res_lvl, xy_info = getClosestResolutionLevel(img, xy)
         tiles = createFullTileList([0,],range(3),[0,], xy_info[0],xy_info[1], xy_info[2:])# rgb tile list
 
-        arr = np.zeros((xy_info[1], xy_info[0], 3), np.uint8)
+        arr = create_array((xy_info[1], xy_info[0], 3), np.uint8)
         async for tile, (z,c,t,coord) in getTiles(img,tiles,res_lvl):
             arr [
                 coord[1]:coord[1]+coord[3],
                 coord[0]:coord[0]+coord[2],
                 c ] = tile
 
         image = Image.fromarray(arr)
         if image.size != xy:
             del arr # just to be safe
             image = image.resize(xy)
 
         return image
 
-    return asyncio.run(work(img, xy_dim))
-
+    event_loop = asyncio.get_running_loop()
+    if event_loop is None:
+        return asyncio.run(work(img, xy_dim))
+    else:
+        return work(img, xy_dim)
 
 def getLargeRecon(img:ImageWrapper, downsample_factor:int = 10, workdir='./', skip_upload=False):
     """
 Checks OMERO for a pregenerated large recon, if none are found, it will generate and upload one.
 
 Parameters
 ----------
@@ -386,14 +390,96 @@
                     img.linkAnnotation(recon)
     else:
         reconPath = downloadFileAnnotation(recon, workdir)
         recon_img = Image.open(reconPath)
 
     return recon, recon_img
 
+
+def loadFullImageSmart(img_obj: ImageWrapper):
+    """
+Attempts to only request tiles with tissue, with the rest being filled in by white space.
+    """
+    
+    async def work(img, mask):
+        # Overall image dimensions
+        image_width, image_height = img_obj.getSizeX(), img_obj.getSizeY()
+
+        # Scaling factors
+        scale_x = mask.shape[1] / image_width
+        scale_y = mask.shape[0] / image_height
+
+        tiles = createTileListFromImage(img)
+        arr = create_array((image_height, image_width, img.getSizeC()), np.uint8)
+        # Empty list to store tiles that land on the mask
+        tiles_on_land = []
+
+        for z,c,t,tile in tiles:
+            x, y, width, height = tile
+
+            # Calculate downscaled coordinates and dimensions
+            x_ds, y_ds = int(x * scale_x), int(y * scale_y)
+            width_ds, height_ds = int(width * scale_x), int(height * scale_y)
+
+            # Check if any pixel in the corresponding mask area is True (assuming binary mask)
+            if np.any(mask[y_ds:(y_ds+height_ds), x_ds:(x_ds+width_ds)]):
+                tiles_on_land.append((z,c,t,tile))
+        async for tile, (z,c,t,coord) in getTiles(img,tiles_on_land):
+            arr [
+                coord[1]:coord[1]+coord[3],
+                coord[0]:coord[0]+coord[2],
+                c ] = tile
+        return Image.fromarray(arr)
+    
+    mask = maskTissueLoose(img_obj)
+
+    event_loop = asyncio.get_running_loop()
+    if event_loop is None:
+        return asyncio.run(work(img_obj, mask))
+    else:
+        return work(img_obj, mask)
+
+
+#
+## MASKING
+#
+
+def maskTissueLoose(img_obj:ImageWrapper, mpp=728):
+    phys_w = img_obj.getPixelSizeX()
+    downsample_factor = mpp / phys_w
+    scaled_dims = getDownsampledXYDimensions(img_obj, downsample_factor)
+
+    # get img ( at super low res )
+    img = Image.open(BytesIO(img_obj.getThumbnail(scaled_dims)))
+    arr = np.array(img)
+    
+    # # tia tissue masker (too fine for our purposes)
+    mask = tissuemask.MorphologicalMasker(mpp=mpp).fit_transform([arr])[0]
+
+    # clean up mask
+    mask = morphology.remove_small_holes(mask)
+    mask = morphology.remove_small_objects(mask)
+
+    # increase resolution
+    scale = 32/mpp 
+    mask_img=Image.fromarray(mask)
+    full_mask_img = mask_img.resize((int(mask_img.size[0]/scale), int(mask_img.size[1]/scale)))
+    mask_img.close()
+    mask = np.array(full_mask_img)
+    full_mask_img.close()
+    
+    # smooth up mask
+    mask = scipy.ndimage.binary_dilation(mask, iterations=16)
+    mask = scipy.ndimage.gaussian_filter(mask.astype(float), sigma=24)
+    mask = mask > 0.5
+
+    # invert mask
+    return ~mask
+
+
 #
 ## TILES
 #
 def createTileList2D(z:int, c:int, t:int, size_x:int, size_y:int,
         tile_size:tuple[int,int]) -> list[tuple[int,int,int,tuple[int,int,int,int]]]:
     """
 Creates a list of tile coords for a given 2D plane (z,c,t)
@@ -536,14 +622,39 @@
 
     return createFullTileList(z_indexes,channels,timepoints,width,height,tile_size, rgb)
 
 
 #
 ## ROIS
 #
+
+def getRois(img: ImageWrapper, roi_service=None):
+    """
+Gathers OMERO RoiI objects.
+
+Parameters
+----------
+img: omero.gateway.ImageWrapper
+    Omero Image object from conn.getObjects()
+roi_service: omero.RoiService, optional
+    Allows roiservice passthrough for performance
+    """
+    if roi_service is None:
+        roi_service = img._conn.getRoiService()
+        close_roi = True
+    else:
+        close_roi = False
+
+    rois = roi_service.findByImage(img.getId(), None, img._conn.SERVICE_OPTS).rois
+
+    if close_roi:
+        roi_service.close()
+
+    return rois
+
 def getShapesAsPoints(img: ImageWrapper, point_downsample=4, img_downsample=1,
                       roi_service=None) -> list[tuple[int, tuple[int,int,int], list[tuple[float, float]]]]:
     """
 Gathers Rectangles, Polygons, and Ellipses as a tuple containing the shapeId, its rgb val, and a tuple of yx points of its bounds.
 
 Parameters
 ----------
@@ -557,26 +668,21 @@
     Allows roiservice passthrough for performance.
 
 Returns
 -------
 returns: list[ shape.id, (r,g,b), list[tuple(x,y)] ]
     list of tuples containing a shape's id, rgb value, and a tuple of row and column points
     """
-    if roi_service is None:
-        roi_service=img._conn.getRoiService()
-        close_roi=True
 
     sizeX = img.getSizeX() / img_downsample
     sizeY = img.getSizeY() / img_downsample
     yx_shape = (sizeY,sizeX)
 
-    result = roi_service.findByImage(img.getId(), None)
-
     shapes=[]
-    for roi in result.rois:
+    for roi in getRois(img, roi_service):
         points= None
         for shape in roi.copyShapes():
 
             if type(shape) == RectangleI:
                 x = float(shape.getX().getValue()) / img_downsample
                 y = float(shape.getY().getValue()) / img_downsample
                 w = float(shape.getWidth().getValue()) / img_downsample
@@ -609,16 +715,14 @@
                 points=(points[0][::point_downsample], points[1][::point_downsample])
 
                 shapes.append((shape.getId()._val, rgb, points))
 
     if not shapes : # if no shapes in shapes return none
         return None
 
-    if close_roi: roi_service.close()
-
     # make sure is in correct order
     return sorted(shapes)
 
 
 def createPolygon(points:list[tuple[float, float]], stride=1, x_offset=0, y_offset=0, z=None, t=None, comment=None, rgb=(0,0,0)) -> PolygonI:
     """
 Creates a local omero polygon obj from a list of points, and parameters.
```

### Comparing `lavlab-python-utils-1.1.4/src/lavlab/python_util.py` & `lavlab-python-utils-1.2.0/src/lavlab/python_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from __future__ import annotations
 """
 Contains general utilities for lavlab's python scripts.
 """
 import os
+import psutil
 import asyncio
+import tempfile
+from math import ceil
 
 import numpy as np
+import dask.array as da
+
 from PIL import Image, ImageDraw
 from skimage import measure
 
 #
 ## Utility Dictionary
 #
 FILETYPE_DICTIONARY = {
@@ -117,16 +122,19 @@
         Number of lists to make
 
     Returns
     -------
     list[list*n]
         lst split into n chunks.
     """
-    return [lst[i : i + n] for i in range(0, len(lst), n)]
-
+    size = ceil(len(lst) / n)
+    return list(
+        map(lambda x: lst[x * size:x * size + size],
+        list(range(n)))
+    )
 
 def interlace_lists(*lists: list[list]) -> list:
     """
     Interlaces a list of lists. Useful for combining tileLists of different channels.
 
     Parameters
     ----------
@@ -231,14 +239,49 @@
     for x in it:
         yield x
 
 
 #
 ## Image Array Utilities
 #
+
+def create_array(shape, dtype=np.float64, use_dask=False, chunksize=1e6):
+    """
+Creates a numpy array, a dask array or a memmap array based on the available system memory.
+
+Parameters
+----------
+dtype : np.dtype
+    Data-type of the array’s elements.
+shape : tuple
+    Shape of the array.
+chunksize : int, optional
+    Size of chunks for dask array, by default 1e6.
+use_dask : bool, optional
+    Whether to use dask arrays for large datasets. If False, memmap is used, by default False.
+
+Returns
+-------
+array
+    Numpy array, Dask array or memmap array based on the available system memory.
+    """
+    size = np.prod(shape) * np.dtype(dtype).itemsize
+    free_memory = psutil.virtual_memory().available
+
+    if size < free_memory:
+        return np.zeros(shape, dtype)
+    else:
+        if use_dask:
+            chunks = tuple(max(1, x // chunksize) for x in shape)
+            return da.zeros(shape, dtype, chunks=chunks)
+        else:
+            _, path = tempfile.mkstemp()
+            return np.memmap(path, dtype=dtype, mode='w+', shape=shape)
+
+
 def rgba_to_uint(red: int, green: int, blue: int, alpha=255) -> int:
     """
     Return the color as an Integer in RGBA encoding.
 
     Parameters
     ----------
     red: int
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lavlab-python-utils-1.1.4/src/lavlab_python_utils.egg-info/PKG-INFO` & `lavlab-python-utils-1.2.0/src/lavlab_python_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: lavlab-python-utils
-Version: 1.1.4
+Version: 1.2.0
 Summary: LaViolette Lab utility package
 Author-email: Michael Barrett <mjbarrett@mcw.edu>
 Project-URL: Homepage, https://github.com/laviolette-lab/lavlab-python-utils
 Project-URL: Bug Tracker, https://github.com/laviolette-lab/lavlab-python-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: docs
 
 TODO: this readme
 =================
 for more info goto: https://lavlab-python-utils.readthedocs.io/en/latest/
 python3 -m unittest
```

### Comparing `lavlab-python-utils-1.1.4/test/test_omero_util.py` & `lavlab-python-utils-1.2.0/test/test_omero_util.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.1.4/test/test_python_utils.py` & `lavlab-python-utils-1.2.0/test/test_python_utils.py`

 * *Files identical despite different names*

