# Comparing `tmp/mcemtools-0.6.0.tar.gz` & `tmp/mcemtools-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcemtools-0.6.0.tar", last modified: Fri Jul 14 12:18:42 2023, max compression
+gzip compressed data, was "mcemtools-0.7.0.tar", last modified: Sat Jul 15 12:00:28 2023, max compression
```

## Comparing `mcemtools-0.6.0.tar` & `mcemtools-0.7.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:18:42.402227 mcemtools-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-14 12:18:32.000000 mcemtools-0.6.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-14 12:18:32.000000 mcemtools-0.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-14 12:18:32.000000 mcemtools-0.6.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-14 12:18:32.000000 mcemtools-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-14 12:18:32.000000 mcemtools-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-14 12:18:42.402227 mcemtools-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-14 12:18:32.000000 mcemtools-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:18:42.398227 mcemtools-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/mcemtools.denoise.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/mcemtools.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-14 12:18:32.000000 mcemtools-0.6.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:18:42.402227 mcemtools-0.6.0/mcemtools/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-14 12:18:32.000000 mcemtools-0.6.0/mcemtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-14 12:18:32.000000 mcemtools-0.6.0/mcemtools/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-14 12:18:32.000000 mcemtools-0.6.0/mcemtools/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-07-14 12:18:32.000000 mcemtools-0.6.0/mcemtools/masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-14 12:18:32.000000 mcemtools-0.6.0/mcemtools/mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-07-14 12:18:32.000000 mcemtools-0.6.0/mcemtools/tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-14 12:18:32.000000 mcemtools-0.6.0/mcemtools/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:18:42.402227 mcemtools-0.6.0/mcemtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-14 12:18:42.000000 mcemtools-0.6.0/mcemtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-14 12:18:42.000000 mcemtools-0.6.0/mcemtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:18:42.000000 mcemtools-0.6.0/mcemtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 12:18:42.000000 mcemtools-0.6.0/mcemtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:18:42.000000 mcemtools-0.6.0/mcemtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-14 12:18:42.000000 mcemtools-0.6.0/mcemtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 12:18:42.000000 mcemtools-0.6.0/mcemtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 12:18:32.000000 mcemtools-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-14 12:18:42.402227 mcemtools-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-14 12:18:32.000000 mcemtools-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:18:42.402227 mcemtools-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-14 12:18:32.000000 mcemtools-0.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-14 12:18:32.000000 mcemtools-0.6.0/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-14 12:18:32.000000 mcemtools-0.6.0/tests/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-14 12:18:32.000000 mcemtools-0.6.0/tests/test_mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-14 12:18:32.000000 mcemtools-0.6.0/tests/test_tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-14 12:18:32.000000 mcemtools-0.6.0/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:00:28.195562 mcemtools-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-15 12:00:16.000000 mcemtools-0.7.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-15 12:00:16.000000 mcemtools-0.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-15 12:00:16.000000 mcemtools-0.7.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-15 12:00:16.000000 mcemtools-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-15 12:00:16.000000 mcemtools-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-15 12:00:28.195562 mcemtools-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-15 12:00:16.000000 mcemtools-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:00:28.191562 mcemtools-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/mcemtools.denoise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/mcemtools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-15 12:00:16.000000 mcemtools-0.7.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:00:28.195562 mcemtools-0.7.0/mcemtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-15 12:00:16.000000 mcemtools-0.7.0/mcemtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-15 12:00:16.000000 mcemtools-0.7.0/mcemtools/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-15 12:00:16.000000 mcemtools-0.7.0/mcemtools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-15 12:00:16.000000 mcemtools-0.7.0/mcemtools/masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-15 12:00:16.000000 mcemtools-0.7.0/mcemtools/mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-07-15 12:00:16.000000 mcemtools-0.7.0/mcemtools/tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-15 12:00:16.000000 mcemtools-0.7.0/mcemtools/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:00:28.195562 mcemtools-0.7.0/mcemtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-07-15 12:00:28.000000 mcemtools-0.7.0/mcemtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-15 12:00:28.000000 mcemtools-0.7.0/mcemtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:00:28.000000 mcemtools-0.7.0/mcemtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-15 12:00:28.000000 mcemtools-0.7.0/mcemtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:00:28.000000 mcemtools-0.7.0/mcemtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-15 12:00:28.000000 mcemtools-0.7.0/mcemtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-15 12:00:28.000000 mcemtools-0.7.0/mcemtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-15 12:00:16.000000 mcemtools-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-15 12:00:28.195562 mcemtools-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-15 12:00:16.000000 mcemtools-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:00:28.195562 mcemtools-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-15 12:00:16.000000 mcemtools-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-15 12:00:16.000000 mcemtools-0.7.0/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-15 12:00:16.000000 mcemtools-0.7.0/tests/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-15 12:00:16.000000 mcemtools-0.7.0/tests/test_mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-15 12:00:16.000000 mcemtools-0.7.0/tests/test_tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-15 12:00:16.000000 mcemtools-0.7.0/tests/test_transforms.py
```

### Comparing `mcemtools-0.6.0/CONTRIBUTING.rst` & `mcemtools-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.6.0/LICENSE` & `mcemtools-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcemtools-0.6.0/PKG-INFO` & `mcemtools-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.6.0
+Version: 0.7.0
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -90,11 +90,15 @@
 
 * Many small bugs are fixed
 
 0.5.0 (2023-07-12)
 ------------------
 * Added binning to transforms
 
-0.6.0 (2023-07-15)
+0.6.0 (2023-07-14)
 ------------------
 * More tests are added
 * Names are consistant accross the package.
+
+0.7.0 (2023-07-15)
+------------------
+* markimage bug is fixed
```

### Comparing `mcemtools-0.6.0/README.rst` & `mcemtools-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.6.0/docs/Makefile` & `mcemtools-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcemtools-0.6.0/docs/conf.py` & `mcemtools-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.6.0/docs/installation.rst` & `mcemtools-0.7.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.6.0/docs/make.bat` & `mcemtools-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcemtools-0.6.0/mcemtools/__init__.py` & `mcemtools-0.7.0/mcemtools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for mcemtools."""
 
 __author__ = """Alireza Sadri"""
 __email__ = 'Alireza.Sadri@monash.edu'
-__version__ = '0.6.0'
+__version__ = '0.7.0'
 
 from .analysis import pyMSSE, cross_correlation_4D, SymmSTEM
 from .analysis import centre_of_mass_4D, sum_4D
 
 from .masking import annular_mask, image_by_windows, markimage, mask2D_to_4D
 
 from .tensor_svd import svd_fit, svd_eval
```

### Comparing `mcemtools-0.6.0/mcemtools/analysis.py` & `mcemtools-0.7.0/mcemtools/analysis.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.6.0/mcemtools/masking.py` & `mcemtools-0.7.0/mcemtools/masking.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         
         if(self.mark_shape == 'circle'):
             cx, cy = in_image.shape
             cx = cx / 2
             cy = cy / 2
             circle_radius = cx if cx < cy else cy
             sl1 = plt.axes([0.25, 0.15, 0.6, 0.03])
-            sl2 = plt.axes([0.25, 0.1, 0.6, 0.03])
+            sl2 = plt.axes([0.25, 0.1,  0.6, 0.03])
             sl3 = plt.axes([0.25, 0.05, 0.6, 0.03])
             self.markshape = plt.Circle((cy,cx), circle_radius, ec="k", fc = 'None')
             axs[0].add_patch(self.markshape)
             self.slider_r = Slider(sl1, 
                 'radius', 0.0, self.im.get_array().shape[0]/2, valinit = circle_radius)
             self.slider_cx = Slider(sl2,
                 'centre_x', 0.0, self.im.get_array().shape[0], valinit = cx)
@@ -250,25 +250,25 @@
         self.fig.canvas.draw_idle()
 
     def update2(self, val):
         if(self.mark_shape == 'circle'):
             r = self.slider_r.val
             cx = self.slider_cx.val
             cy  = self.slider_cy.val
-            self.markshape.centre = (cy, cx)
+            self.markshape.set_centre((cy, cx))
             self.markshape.set_radius(r)
             
         if(self.mark_shape == 'rectangle'):
             self.slider_top_left_r.val
             self.slider_top_left_c.val
             self.slider_bot_right_r.val
             self.slider_s_bot_right_c.val
 
-            self.markshape.xy = (
+            self.markshape.set_xy = ((
                 self.slider_top_left_r.val,
-                self.slider_top_left_c.val)
+                self.slider_top_left_c.val))
             self.markshape.set_width(
                 self.slider_bot_right_r.val - self.slider_top_left_r.val)
             self.markshape.set_height(
                 self.slider_s_bot_right_c.val - self.slider_top_left_c.val)
 
         self.fig.canvas.draw_idle()
```

### Comparing `mcemtools-0.6.0/mcemtools/mcemtools.py` & `mcemtools-0.7.0/mcemtools/mcemtools.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.6.0/mcemtools/tensor_svd.py` & `mcemtools-0.7.0/mcemtools/tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.6.0/mcemtools/transforms.py` & `mcemtools-0.7.0/mcemtools/transforms.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.6.0/mcemtools.egg-info/PKG-INFO` & `mcemtools-0.7.0/mcemtools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.6.0
+Version: 0.7.0
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -90,11 +90,15 @@
 
 * Many small bugs are fixed
 
 0.5.0 (2023-07-12)
 ------------------
 * Added binning to transforms
 
-0.6.0 (2023-07-15)
+0.6.0 (2023-07-14)
 ------------------
 * More tests are added
 * Names are consistant accross the package.
+
+0.7.0 (2023-07-15)
+------------------
+* markimage bug is fixed
```

### Comparing `mcemtools-0.6.0/mcemtools.egg-info/SOURCES.txt` & `mcemtools-0.7.0/mcemtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcemtools-0.6.0/setup.py` & `mcemtools-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-__version__ = '0.6.0'
+__version__ = '0.7.0'
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
```

### Comparing `mcemtools-0.6.0/tests/test_analysis.py` & `mcemtools-0.7.0/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.6.0/tests/test_masking.py` & `mcemtools-0.7.0/tests/test_masking.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.6.0/tests/test_mcemtools.py` & `mcemtools-0.7.0/tests/test_mcemtools.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.6.0/tests/test_tensor_svd.py` & `mcemtools-0.7.0/tests/test_tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.6.0/tests/test_transforms.py` & `mcemtools-0.7.0/tests/test_transforms.py`

 * *Files identical despite different names*

