# Comparing `tmp/streamlit-binary-tree-0.2.1.tar.gz` & `tmp/streamlit-binary-tree-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-binary-tree-0.2.1.tar", last modified: Sat Jul 15 08:44:45 2023, max compression
+gzip compressed data, was "streamlit-binary-tree-0.2.2.tar", last modified: Sat Jul 15 08:55:05 2023, max compression
```

## Comparing `streamlit-binary-tree-0.2.1.tar` & `streamlit-binary-tree-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 08:44:45.775781 streamlit-binary-tree-0.2.1/
--rw-rw-rw-   0        0        0     3577 2023-07-09 22:12:58.000000 streamlit-binary-tree-0.2.1/LICENSE
--rw-rw-rw-   0        0        0       57 2023-07-05 06:03:11.000000 streamlit-binary-tree-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      346 2023-07-15 08:44:45.775781 streamlit-binary-tree-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-07-09 22:09:53.000000 streamlit-binary-tree-0.2.1/README.md
--rw-rw-rw-   0        0        0       86 2023-07-15 08:44:45.777782 streamlit-binary-tree-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      755 2023-07-15 08:44:05.000000 streamlit-binary-tree-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 08:44:45.551126 streamlit-binary-tree-0.2.1/streamlit_binary_tree/
--rw-rw-rw-   0        0        0    17412 2023-07-15 08:38:58.000000 streamlit-binary-tree-0.2.1/streamlit_binary_tree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 08:44:45.518582 streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/
-drwxrwxrwx   0        0        0        0 2023-07-15 08:44:45.589264 streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/
--rw-rw-rw-   0        0        0      879 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0     2186 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/index.html
-drwxrwxrwx   0        0        0        0 2023-07-15 08:44:45.520582 streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2023-07-15 08:44:45.600054 streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/css/
--rw-rw-rw-   0        0        0     8091 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css
--rw-rw-rw-   0        0        0    15517 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map
-drwxrwxrwx   0        0        0        0 2023-07-15 08:44:45.774781 streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/js/
--rw-rw-rw-   0        0        0   667302 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js
--rw-rw-rw-   0        0        0     3049 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  2405682 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map
--rw-rw-rw-   0        0        0     5066 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js
--rw-rw-rw-   0        0        0    16890 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js.map
--rw-rw-rw-   0        0        0     1598 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
--rw-rw-rw-   0        0        0     8383 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
-drwxrwxrwx   0        0        0        0 2023-07-15 08:44:45.581855 streamlit-binary-tree-0.2.1/streamlit_binary_tree.egg-info/
--rw-rw-rw-   0        0        0      346 2023-07-15 08:44:45.000000 streamlit-binary-tree-0.2.1/streamlit_binary_tree.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1068 2023-07-15 08:44:45.000000 streamlit-binary-tree-0.2.1/streamlit_binary_tree.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 08:44:45.000000 streamlit-binary-tree-0.2.1/streamlit_binary_tree.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 08:44:45.000000 streamlit-binary-tree-0.2.1/streamlit_binary_tree.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-15 08:44:45.000000 streamlit-binary-tree-0.2.1/streamlit_binary_tree.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 08:55:05.864080 streamlit-binary-tree-0.2.2/
+-rw-rw-rw-   0        0        0     3577 2023-07-09 22:12:58.000000 streamlit-binary-tree-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-07-05 06:03:11.000000 streamlit-binary-tree-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      346 2023-07-15 08:55:05.864080 streamlit-binary-tree-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2023-07-09 22:09:53.000000 streamlit-binary-tree-0.2.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-15 08:55:05.871082 streamlit-binary-tree-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-07-15 08:55:01.000000 streamlit-binary-tree-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 08:55:05.827540 streamlit-binary-tree-0.2.2/streamlit_binary_tree/
+-rw-rw-rw-   0        0        0    17411 2023-07-15 08:54:37.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 08:55:05.806593 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/
+drwxrwxrwx   0        0        0        0 2023-07-15 08:55:05.847508 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/
+-rw-rw-rw-   0        0        0      879 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0     2186 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/index.html
+drwxrwxrwx   0        0        0        0 2023-07-15 08:55:05.808593 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-15 08:55:05.849508 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/css/
+-rw-rw-rw-   0        0        0     8091 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css
+-rw-rw-rw-   0        0        0    15517 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map
+drwxrwxrwx   0        0        0        0 2023-07-15 08:55:05.863081 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   667302 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js
+-rw-rw-rw-   0        0        0     3049 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  2405682 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map
+-rw-rw-rw-   0        0        0     5066 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js
+-rw-rw-rw-   0        0        0    16890 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js.map
+-rw-rw-rw-   0        0        0     1598 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js
+-rw-rw-rw-   0        0        0     8383 2023-07-15 08:39:23.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map
+drwxrwxrwx   0        0        0        0 2023-07-15 08:55:05.846509 streamlit-binary-tree-0.2.2/streamlit_binary_tree.egg-info/
+-rw-rw-rw-   0        0        0      346 2023-07-15 08:55:05.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1068 2023-07-15 08:55:05.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 08:55:05.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 08:55:05.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-15 08:55:05.000000 streamlit-binary-tree-0.2.2/streamlit_binary_tree.egg-info/top_level.txt
```

### Comparing `streamlit-binary-tree-0.2.1/LICENSE` & `streamlit-binary-tree-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.1/streamlit_binary_tree/__init__.py` & `streamlit-binary-tree-0.2.2/streamlit_binary_tree/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 from typing import List
 import streamlit as st
 import streamlit.components.v1 as components
 from sklearn.tree import _tree
 from sklearn.tree._classes import DecisionTreeClassifier as DCTClass
 
-_RELEASE = False
+_RELEASE = True
 _DEBUG = True
 _NAME = "streamlit_binary_tree"
 
 if _RELEASE:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _component_func = components.declare_component(_NAME, path=build_dir)
```

### Comparing `streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/asset-manifest.json` & `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/index.html` & `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css` & `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map` & `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/css/main.3a4c9b92.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js` & `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt` & `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map` & `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/2.41f15472.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js` & `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js.map` & `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/main.50b0a73e.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js` & `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.1/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map` & `streamlit-binary-tree-0.2.2/streamlit_binary_tree/frontend/build/static/js/runtime-main.624f085e.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-binary-tree-0.2.1/streamlit_binary_tree.egg-info/SOURCES.txt` & `streamlit-binary-tree-0.2.2/streamlit_binary_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

