# Comparing `tmp/nb-thumb-0.0.6.tar.gz` & `tmp/nb-thumb-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb-thumb-0.0.6.tar", last modified: Sat Jul 15 06:06:21 2023, max compression
+gzip compressed data, was "nb-thumb-0.0.7.tar", last modified: Sat Jul 15 06:12:55 2023, max compression
```

## Comparing `nb-thumb-0.0.6.tar` & `nb-thumb-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-15 06:06:21.735539 nb-thumb-0.0.6/
--rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 nb-thumb-0.0.6/LICENSE
--rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 nb-thumb-0.0.6/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     2424 2023-07-15 06:06:21.735377 nb-thumb-0.0.6/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)     1623 2023-07-15 06:02:09.000000 nb-thumb-0.0.6/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-15 06:06:21.734176 nb-thumb-0.0.6/nb_thumb/
--rw-r--r--   0 hamel      (501) staff       (20)       96 2023-07-15 06:06:09.000000 nb-thumb-0.0.6/nb_thumb/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)     1014 2023-07-15 06:06:09.000000 nb-thumb-0.0.6/nb_thumb/_modidx.py
--rw-r--r--   0 hamel      (501) staff       (20)      142 2023-07-14 03:45:28.000000 nb-thumb-0.0.6/nb_thumb/core.py
--rw-r--r--   0 hamel      (501) staff       (20)     1497 2023-07-15 06:06:09.000000 nb-thumb-0.0.6/nb_thumb/gallery.py
--rw-r--r--   0 hamel      (501) staff       (20)     1948 2023-07-15 06:06:09.000000 nb-thumb-0.0.6/nb_thumb/thumb.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-15 06:06:21.735149 nb-thumb-0.0.6/nb_thumb.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     2424 2023-07-15 06:06:21.000000 nb-thumb-0.0.6/nb_thumb.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      372 2023-07-15 06:06:21.000000 nb-thumb-0.0.6/nb_thumb.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-07-15 06:06:21.000000 nb-thumb-0.0.6/nb_thumb.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-07-15 06:06:21.000000 nb-thumb-0.0.6/nb_thumb.egg-info/entry_points.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-07-14 05:34:35.000000 nb-thumb-0.0.6/nb_thumb.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       46 2023-07-15 06:06:21.000000 nb-thumb-0.0.6/nb_thumb.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)        9 2023-07-15 06:06:21.000000 nb-thumb-0.0.6/nb_thumb.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)      850 2023-07-15 06:06:09.000000 nb-thumb-0.0.6/settings.ini
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-07-15 06:06:21.735585 nb-thumb-0.0.6/setup.cfg
--rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 nb-thumb-0.0.6/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-15 06:12:55.671821 nb-thumb-0.0.7/
+-rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 nb-thumb-0.0.7/LICENSE
+-rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 nb-thumb-0.0.7/MANIFEST.in
+-rw-r--r--   0 hamel      (501) staff       (20)     2424 2023-07-15 06:12:55.671654 nb-thumb-0.0.7/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)     1623 2023-07-15 06:02:09.000000 nb-thumb-0.0.7/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-15 06:12:55.670226 nb-thumb-0.0.7/nb_thumb/
+-rw-r--r--   0 hamel      (501) staff       (20)       96 2023-07-15 06:12:46.000000 nb-thumb-0.0.7/nb_thumb/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1014 2023-07-15 06:12:46.000000 nb-thumb-0.0.7/nb_thumb/_modidx.py
+-rw-r--r--   0 hamel      (501) staff       (20)      142 2023-07-14 03:45:28.000000 nb-thumb-0.0.7/nb_thumb/core.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1572 2023-07-15 06:12:46.000000 nb-thumb-0.0.7/nb_thumb/gallery.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1948 2023-07-15 06:12:46.000000 nb-thumb-0.0.7/nb_thumb/thumb.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-15 06:12:55.671437 nb-thumb-0.0.7/nb_thumb.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)     2424 2023-07-15 06:12:55.000000 nb-thumb-0.0.7/nb_thumb.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      372 2023-07-15 06:12:55.000000 nb-thumb-0.0.7/nb_thumb.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-07-15 06:12:55.000000 nb-thumb-0.0.7/nb_thumb.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2023-07-15 06:12:55.000000 nb-thumb-0.0.7/nb_thumb.egg-info/entry_points.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-07-14 05:34:35.000000 nb-thumb-0.0.7/nb_thumb.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       46 2023-07-15 06:12:55.000000 nb-thumb-0.0.7/nb_thumb.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        9 2023-07-15 06:12:55.000000 nb-thumb-0.0.7/nb_thumb.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)      850 2023-07-15 06:12:46.000000 nb-thumb-0.0.7/settings.ini
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2023-07-15 06:12:55.671869 nb-thumb-0.0.7/setup.cfg
+-rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 nb-thumb-0.0.7/setup.py
```

### Comparing `nb-thumb-0.0.6/LICENSE` & `nb-thumb-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nb-thumb-0.0.6/PKG-INFO` & `nb-thumb-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-thumb
-Version: 0.0.6
+Version: 0.0.7
 Summary: Extract thumbnails from Jupyter notebooks
 Home-page: https://github.com/fastai/nb-thumb
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `nb-thumb-0.0.6/README.md` & `nb-thumb-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `nb-thumb-0.0.6/nb_thumb/_modidx.py` & `nb-thumb-0.0.7/nb_thumb/_modidx.py`

 * *Files identical despite different names*

### Comparing `nb-thumb-0.0.6/nb_thumb/gallery.py` & `nb-thumb-0.0.7/nb_thumb/gallery.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from fastcore.utils import mkdir
 from fastcore.test import test_eq
 
 # %% ../nbs/01_gallery.ipynb 3
 def emb_img(nb_path:str, # the path to the notebook
             label:str, # the label indicating the cell where the plot is
             caption:str='', # the caption, will be inferred from label if not specified.
-            anchor='#example', # anchor tag in source page
+            anchor='#example', # anchor tag in source page, this defaults to `#example` for plotnine: https://plotnine.readthedocs.io
            size=(150,150) # size of the thumbnail
            ) -> str:
     "Embed a thumbnail image as a markdown cell."
     if not caption: caption = label.replace('_', ' ').title()
     d = mkdir(f'{Path(nb_path).stem}_data', exist_ok=True)
     img = nb2thumb(nb_path, label=label, size=size)
     outfile = d/f'{label}.png'
```

### Comparing `nb-thumb-0.0.6/nb_thumb/thumb.py` & `nb-thumb-0.0.7/nb_thumb/thumb.py`

 * *Files identical despite different names*

### Comparing `nb-thumb-0.0.6/nb_thumb.egg-info/PKG-INFO` & `nb-thumb-0.0.7/nb_thumb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-thumb
-Version: 0.0.6
+Version: 0.0.7
 Summary: Extract thumbnails from Jupyter notebooks
 Home-page: https://github.com/fastai/nb-thumb
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `nb-thumb-0.0.6/settings.ini` & `nb-thumb-0.0.7/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = nb-thumb
 lib_name = nb-thumb
-version = 0.0.6
+version = 0.0.7
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = nb_thumb
 nbs_path = nbs
 recursive = True
```

### Comparing `nb-thumb-0.0.6/setup.py` & `nb-thumb-0.0.7/setup.py`

 * *Files identical despite different names*

