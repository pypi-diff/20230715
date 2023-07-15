# Comparing `tmp/graph_cordinates-0.0.1.tar.gz` & `tmp/graph_cordinates-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_cordinates-0.0.1.tar", last modified: Thu Jul 13 06:23:52 2023, max compression
+gzip compressed data, was "graph_cordinates-0.0.2.tar", last modified: Sat Jul 15 13:55:07 2023, max compression
```

## Comparing `graph_cordinates-0.0.1.tar` & `graph_cordinates-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 06:23:52.580534 graph_cordinates-0.0.1/
--rw-rw-rw-   0        0        0     1365 2023-07-13 06:23:52.580534 graph_cordinates-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-13 06:23:52.554508 graph_cordinates-0.0.1/graph_cordinates/
--rw-rw-rw-   0        0        0        0 2023-07-11 19:14:02.000000 graph_cordinates-0.0.1/graph_cordinates/__init__.py
--rw-rw-rw-   0        0        0     1295 2023-07-13 05:58:11.000000 graph_cordinates-0.0.1/graph_cordinates/graph_cordinates.py
-drwxrwxrwx   0        0        0        0 2023-07-13 06:23:52.580534 graph_cordinates-0.0.1/graph_cordinates.egg-info/
--rw-rw-rw-   0        0        0     1365 2023-07-13 06:23:52.000000 graph_cordinates-0.0.1/graph_cordinates.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-13 06:23:52.000000 graph_cordinates-0.0.1/graph_cordinates.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 06:23:52.000000 graph_cordinates-0.0.1/graph_cordinates.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-13 06:23:52.000000 graph_cordinates-0.0.1/graph_cordinates.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 06:23:52.587871 graph_cordinates-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1692 2023-07-13 06:23:30.000000 graph_cordinates-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 13:55:07.406964 graph_cordinates-0.0.2/
+-rw-rw-rw-   0        0        0     1419 2023-07-15 13:55:07.406964 graph_cordinates-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-15 13:55:07.376026 graph_cordinates-0.0.2/graph_cordinates/
+-rw-rw-rw-   0        0        0        0 2023-07-11 19:14:02.000000 graph_cordinates-0.0.2/graph_cordinates/__init__.py
+-rw-rw-rw-   0        0        0     1295 2023-07-13 05:58:11.000000 graph_cordinates-0.0.2/graph_cordinates/graph_cordinates.py
+drwxrwxrwx   0        0        0        0 2023-07-15 13:55:07.405738 graph_cordinates-0.0.2/graph_cordinates.egg-info/
+-rw-rw-rw-   0        0        0     1419 2023-07-15 13:55:06.000000 graph_cordinates-0.0.2/graph_cordinates.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-07-15 13:55:07.000000 graph_cordinates-0.0.2/graph_cordinates.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 13:55:06.000000 graph_cordinates-0.0.2/graph_cordinates.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-15 13:55:06.000000 graph_cordinates-0.0.2/graph_cordinates.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 13:55:07.406964 graph_cordinates-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1746 2023-07-15 13:53:59.000000 graph_cordinates-0.0.2/setup.py
```

### Comparing `graph_cordinates-0.0.1/PKG-INFO` & `graph_cordinates-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: graph_cordinates
-Version: 0.0.1
+Version: 0.0.2
 Summary: From Image of a curve/graph, extract and store the cordinates pairs in a 2D array, Github link (https://github.com/kumarUjjawal3621/mypython_lib)
 Author: Ujjawal Kumar (India)
 Author-email: <kumarujjawal3621@gmail.com>
 Keywords: stock price,Python,Cordinates,Image,2D Curve
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
  
-Library-
-1. graph_cordinates.graph_cordinates.get_graphcordinates(image_path,x_range,y_range,background_value)
-
+How to use:
+    1. import graph_cordinates.graph_cordinates as gc
+    2. gc.get_graphcordinates(image_path,x_range,y_range,background_value)
+    3. Will return an array of 2D cordinates: [[x1,y1], [x2,y2], .......n-points] ; n=pixel width of Image
+    
 How to pass arguments-
-1. image_path ==path to a graph image
-2. x_range ==[Value of left most point on graph's x-axis, Value of right most point on graph's x-axis]
-3.y_range ==[Value of bottom most point on graph's y-axis, Value of top most point on graph's y-axis]
-4.background_value ==0 or 1 , 0: When the graph's background color is relatively darker than the curve, 1: Otherwise
-
-Caution- 
-Try to pass the Image by erasing the axes
+    1. image_path == path to a graph image
+    2. x_range == [Value of left most point on graph's x-axis, Value of right most point on graph's x-axis]
+    3. y_range == [Value of bottom most point on graph's y-axis, Value of top most point on graph's y-axis]
+    4. background_value == 0 or 1 
+        0: When the graph's background color is relatively darker than the curve 
+        1: Otherwise
 
-Return value- Will return a numpy array of structure- array = [[x1,y1], [x2,y2], .......n-points] ; n=pixel width of Image
+Caution- Try to pass the Image by erasing the axes
```

### Comparing `graph_cordinates-0.0.1/graph_cordinates/graph_cordinates.py` & `graph_cordinates-0.0.2/graph_cordinates/graph_cordinates.py`

 * *Files identical despite different names*

### Comparing `graph_cordinates-0.0.1/graph_cordinates.egg-info/PKG-INFO` & `graph_cordinates-0.0.2/graph_cordinates.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: graph-cordinates
-Version: 0.0.1
+Version: 0.0.2
 Summary: From Image of a curve/graph, extract and store the cordinates pairs in a 2D array, Github link (https://github.com/kumarUjjawal3621/mypython_lib)
 Author: Ujjawal Kumar (India)
 Author-email: <kumarujjawal3621@gmail.com>
 Keywords: stock price,Python,Cordinates,Image,2D Curve
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
  
-Library-
-1. graph_cordinates.graph_cordinates.get_graphcordinates(image_path,x_range,y_range,background_value)
-
+How to use:
+    1. import graph_cordinates.graph_cordinates as gc
+    2. gc.get_graphcordinates(image_path,x_range,y_range,background_value)
+    3. Will return an array of 2D cordinates: [[x1,y1], [x2,y2], .......n-points] ; n=pixel width of Image
+    
 How to pass arguments-
-1. image_path ==path to a graph image
-2. x_range ==[Value of left most point on graph's x-axis, Value of right most point on graph's x-axis]
-3.y_range ==[Value of bottom most point on graph's y-axis, Value of top most point on graph's y-axis]
-4.background_value ==0 or 1 , 0: When the graph's background color is relatively darker than the curve, 1: Otherwise
-
-Caution- 
-Try to pass the Image by erasing the axes
+    1. image_path == path to a graph image
+    2. x_range == [Value of left most point on graph's x-axis, Value of right most point on graph's x-axis]
+    3. y_range == [Value of bottom most point on graph's y-axis, Value of top most point on graph's y-axis]
+    4. background_value == 0 or 1 
+        0: When the graph's background color is relatively darker than the curve 
+        1: Otherwise
 
-Return value- Will return a numpy array of structure- array = [[x1,y1], [x2,y2], .......n-points] ; n=pixel width of Image
+Caution- Try to pass the Image by erasing the axes
```

### Comparing `graph_cordinates-0.0.1/setup.py` & `graph_cordinates-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'From Image of a curve/graph, extract and store the cordinates pairs in a 2D array, Github link (https://github.com/kumarUjjawal3621/mypython_lib)'
 LONG_DESCRIPTION = """ 
-Library-
-1. graph_cordinates.graph_cordinates.get_graphcordinates(image_path,x_range,y_range,background_value)
-
+How to use:
+    1. import graph_cordinates.graph_cordinates as gc
+    2. gc.get_graphcordinates(image_path,x_range,y_range,background_value)
+    3. Will return an array of 2D cordinates: [[x1,y1], [x2,y2], .......n-points] ; n=pixel width of Image
+    
 How to pass arguments-
-1. image_path ==path to a graph image
-2. x_range ==[Value of left most point on graph's x-axis, Value of right most point on graph's x-axis]
-3.y_range ==[Value of bottom most point on graph's y-axis, Value of top most point on graph's y-axis]
-4.background_value ==0 or 1 , 0: When the graph's background color is relatively darker than the curve, 1: Otherwise
-
-Caution- 
-Try to pass the Image by erasing the axes
+    1. image_path == path to a graph image
+    2. x_range == [Value of left most point on graph's x-axis, Value of right most point on graph's x-axis]
+    3. y_range == [Value of bottom most point on graph's y-axis, Value of top most point on graph's y-axis]
+    4. background_value == 0 or 1 
+        0: When the graph's background color is relatively darker than the curve 
+        1: Otherwise
 
-Return value- Will return a numpy array of structure- array = [[x1,y1], [x2,y2], .......n-points] ; n=pixel width of Image
+Caution- Try to pass the Image by erasing the axes
 """
 # Setting up
 
 setup(
     name="graph_cordinates",
     version=VERSION,
     author="Ujjawal Kumar (India)",
```

