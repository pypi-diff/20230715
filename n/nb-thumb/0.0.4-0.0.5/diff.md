# Comparing `tmp/nb-thumb-0.0.4.tar.gz` & `tmp/nb-thumb-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb-thumb-0.0.4.tar", last modified: Sat Jul 15 06:01:13 2023, max compression
+gzip compressed data, was "nb-thumb-0.0.5.tar", last modified: Sat Jul 15 06:02:21 2023, max compression
```

## Comparing `nb-thumb-0.0.4.tar` & `nb-thumb-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-15 06:01:13.157323 nb-thumb-0.0.4/
--rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 nb-thumb-0.0.4/LICENSE
--rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 nb-thumb-0.0.4/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     2415 2023-07-15 06:01:13.157170 nb-thumb-0.0.4/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)     1614 2023-07-15 06:00:58.000000 nb-thumb-0.0.4/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-15 06:01:13.155963 nb-thumb-0.0.4/nb_thumb/
--rw-r--r--   0 hamel      (501) staff       (20)       96 2023-07-15 06:01:07.000000 nb-thumb-0.0.4/nb_thumb/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)     1014 2023-07-15 06:01:07.000000 nb-thumb-0.0.4/nb_thumb/_modidx.py
--rw-r--r--   0 hamel      (501) staff       (20)      142 2023-07-14 03:45:28.000000 nb-thumb-0.0.4/nb_thumb/core.py
--rw-r--r--   0 hamel      (501) staff       (20)     1466 2023-07-15 06:01:07.000000 nb-thumb-0.0.4/nb_thumb/gallery.py
--rw-r--r--   0 hamel      (501) staff       (20)     1948 2023-07-15 06:01:07.000000 nb-thumb-0.0.4/nb_thumb/thumb.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-15 06:01:13.156973 nb-thumb-0.0.4/nb_thumb.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     2415 2023-07-15 06:01:12.000000 nb-thumb-0.0.4/nb_thumb.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      372 2023-07-15 06:01:13.000000 nb-thumb-0.0.4/nb_thumb.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-07-15 06:01:12.000000 nb-thumb-0.0.4/nb_thumb.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-07-15 06:01:12.000000 nb-thumb-0.0.4/nb_thumb.egg-info/entry_points.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-07-14 05:34:35.000000 nb-thumb-0.0.4/nb_thumb.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       46 2023-07-15 06:01:12.000000 nb-thumb-0.0.4/nb_thumb.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)        9 2023-07-15 06:01:13.000000 nb-thumb-0.0.4/nb_thumb.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)      850 2023-07-15 06:01:07.000000 nb-thumb-0.0.4/settings.ini
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-07-15 06:01:13.157366 nb-thumb-0.0.4/setup.cfg
--rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 nb-thumb-0.0.4/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-15 06:02:21.318692 nb-thumb-0.0.5/
+-rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 nb-thumb-0.0.5/LICENSE
+-rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 nb-thumb-0.0.5/MANIFEST.in
+-rw-r--r--   0 hamel      (501) staff       (20)     2424 2023-07-15 06:02:21.318534 nb-thumb-0.0.5/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)     1623 2023-07-15 06:02:09.000000 nb-thumb-0.0.5/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-15 06:02:21.316984 nb-thumb-0.0.5/nb_thumb/
+-rw-r--r--   0 hamel      (501) staff       (20)       96 2023-07-15 06:02:16.000000 nb-thumb-0.0.5/nb_thumb/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1014 2023-07-15 06:02:16.000000 nb-thumb-0.0.5/nb_thumb/_modidx.py
+-rw-r--r--   0 hamel      (501) staff       (20)      142 2023-07-14 03:45:28.000000 nb-thumb-0.0.5/nb_thumb/core.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1466 2023-07-15 06:02:16.000000 nb-thumb-0.0.5/nb_thumb/gallery.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1948 2023-07-15 06:02:16.000000 nb-thumb-0.0.5/nb_thumb/thumb.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-07-15 06:02:21.318338 nb-thumb-0.0.5/nb_thumb.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)     2424 2023-07-15 06:02:20.000000 nb-thumb-0.0.5/nb_thumb.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      372 2023-07-15 06:02:21.000000 nb-thumb-0.0.5/nb_thumb.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-07-15 06:02:20.000000 nb-thumb-0.0.5/nb_thumb.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2023-07-15 06:02:21.000000 nb-thumb-0.0.5/nb_thumb.egg-info/entry_points.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-07-14 05:34:35.000000 nb-thumb-0.0.5/nb_thumb.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       46 2023-07-15 06:02:21.000000 nb-thumb-0.0.5/nb_thumb.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        9 2023-07-15 06:02:21.000000 nb-thumb-0.0.5/nb_thumb.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)      850 2023-07-15 06:02:16.000000 nb-thumb-0.0.5/settings.ini
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2023-07-15 06:02:21.318740 nb-thumb-0.0.5/setup.cfg
+-rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 nb-thumb-0.0.5/setup.py
```

### Comparing `nb-thumb-0.0.4/LICENSE` & `nb-thumb-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nb-thumb-0.0.4/PKG-INFO` & `nb-thumb-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-thumb
-Version: 0.0.4
+Version: 0.0.5
 Summary: Extract thumbnails from Jupyter notebooks
 Home-page: https://github.com/fastai/nb-thumb
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
@@ -91,10 +91,10 @@
 ```
 
 ![image.png](index_files/figure-commonmark/cell-13-1-f2854a9b-19e7-4f38-ae0b-894462a88e09.png)
 
 ## Usage
 
 For more information and examples, see [the
-docs](https://fastai.github.io/).
+docs](https://fastai.github.io/nb-thumb/).
```

### Comparing `nb-thumb-0.0.4/README.md` & `nb-thumb-0.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -68,8 +68,8 @@
 ```
 
 ![image.png](index_files/figure-commonmark/cell-13-1-f2854a9b-19e7-4f38-ae0b-894462a88e09.png)
 
 ## Usage
 
 For more information and examples, see [the
-docs](https://fastai.github.io/).
+docs](https://fastai.github.io/nb-thumb/).
```

### Comparing `nb-thumb-0.0.4/nb_thumb/_modidx.py` & `nb-thumb-0.0.5/nb_thumb/_modidx.py`

 * *Files identical despite different names*

### Comparing `nb-thumb-0.0.4/nb_thumb/gallery.py` & `nb-thumb-0.0.5/nb_thumb/gallery.py`

 * *Files identical despite different names*

### Comparing `nb-thumb-0.0.4/nb_thumb/thumb.py` & `nb-thumb-0.0.5/nb_thumb/thumb.py`

 * *Files identical despite different names*

### Comparing `nb-thumb-0.0.4/nb_thumb.egg-info/PKG-INFO` & `nb-thumb-0.0.5/nb_thumb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-thumb
-Version: 0.0.4
+Version: 0.0.5
 Summary: Extract thumbnails from Jupyter notebooks
 Home-page: https://github.com/fastai/nb-thumb
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
@@ -91,10 +91,10 @@
 ```
 
 ![image.png](index_files/figure-commonmark/cell-13-1-f2854a9b-19e7-4f38-ae0b-894462a88e09.png)
 
 ## Usage
 
 For more information and examples, see [the
-docs](https://fastai.github.io/).
+docs](https://fastai.github.io/nb-thumb/).
```

### Comparing `nb-thumb-0.0.4/settings.ini` & `nb-thumb-0.0.5/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = nb-thumb
 lib_name = nb-thumb
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = nb_thumb
 nbs_path = nbs
 recursive = True
```

### Comparing `nb-thumb-0.0.4/setup.py` & `nb-thumb-0.0.5/setup.py`

 * *Files identical despite different names*

