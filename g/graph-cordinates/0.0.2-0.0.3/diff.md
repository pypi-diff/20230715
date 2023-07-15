# Comparing `tmp/graph_cordinates-0.0.2.tar.gz` & `tmp/graph_cordinates-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_cordinates-0.0.2.tar", last modified: Sat Jul 15 13:55:07 2023, max compression
+gzip compressed data, was "graph_cordinates-0.0.3.tar", last modified: Sat Jul 15 14:04:26 2023, max compression
```

## Comparing `graph_cordinates-0.0.2.tar` & `graph_cordinates-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 13:55:07.406964 graph_cordinates-0.0.2/
--rw-rw-rw-   0        0        0     1419 2023-07-15 13:55:07.406964 graph_cordinates-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-15 13:55:07.376026 graph_cordinates-0.0.2/graph_cordinates/
--rw-rw-rw-   0        0        0        0 2023-07-11 19:14:02.000000 graph_cordinates-0.0.2/graph_cordinates/__init__.py
--rw-rw-rw-   0        0        0     1295 2023-07-13 05:58:11.000000 graph_cordinates-0.0.2/graph_cordinates/graph_cordinates.py
-drwxrwxrwx   0        0        0        0 2023-07-15 13:55:07.405738 graph_cordinates-0.0.2/graph_cordinates.egg-info/
--rw-rw-rw-   0        0        0     1419 2023-07-15 13:55:06.000000 graph_cordinates-0.0.2/graph_cordinates.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-15 13:55:07.000000 graph_cordinates-0.0.2/graph_cordinates.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 13:55:06.000000 graph_cordinates-0.0.2/graph_cordinates.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-15 13:55:06.000000 graph_cordinates-0.0.2/graph_cordinates.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 13:55:07.406964 graph_cordinates-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1746 2023-07-15 13:53:59.000000 graph_cordinates-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 14:04:26.353105 graph_cordinates-0.0.3/
+-rw-rw-rw-   0        0        0     1348 2023-07-15 14:04:26.353105 graph_cordinates-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-15 14:04:26.346145 graph_cordinates-0.0.3/graph_cordinates/
+-rw-rw-rw-   0        0        0        0 2023-07-11 19:14:02.000000 graph_cordinates-0.0.3/graph_cordinates/__init__.py
+-rw-rw-rw-   0        0        0     1295 2023-07-13 05:58:11.000000 graph_cordinates-0.0.3/graph_cordinates/graph_cordinates.py
+drwxrwxrwx   0        0        0        0 2023-07-15 14:04:26.353105 graph_cordinates-0.0.3/graph_cordinates.egg-info/
+-rw-rw-rw-   0        0        0     1348 2023-07-15 14:04:26.000000 graph_cordinates-0.0.3/graph_cordinates.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-07-15 14:04:26.000000 graph_cordinates-0.0.3/graph_cordinates.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 14:04:26.000000 graph_cordinates-0.0.3/graph_cordinates.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-15 14:04:26.000000 graph_cordinates-0.0.3/graph_cordinates.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 14:04:26.353105 graph_cordinates-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1740 2023-07-15 14:03:59.000000 graph_cordinates-0.0.3/setup.py
```

### Comparing `graph_cordinates-0.0.2/PKG-INFO` & `graph_cordinates-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 Metadata-Version: 2.1
 Name: graph_cordinates
-Version: 0.0.2
-Summary: From Image of a curve/graph, extract and store the cordinates pairs in a 2D array, Github link (https://github.com/kumarUjjawal3621/mypython_lib)
+Version: 0.0.3
+Summary: From Image of a curve/graph, extract and store the cordinates pairs in a 2D array 
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
 
  
-How to use:
-    1. import graph_cordinates.graph_cordinates as gc
-    2. gc.get_graphcordinates(image_path,x_range,y_range,background_value)
-    3. Will return an array of 2D cordinates: [[x1,y1], [x2,y2], .......n-points] ; n=pixel width of Image
+How to use: 
+
+1. import graph_cordinates.graph_cordinates as gc 
+
+2. gc.get_graphcordinates(image_path,x_range,y_range,background_value) 
+
+3. Will return an array of 2D cordinates: [[x1,y1], [x2,y2], .......n-points] ; n=pixel width of Image 
+
     
-How to pass arguments-
-    1. image_path == path to a graph image
-    2. x_range == [Value of left most point on graph's x-axis, Value of right most point on graph's x-axis]
-    3. y_range == [Value of bottom most point on graph's y-axis, Value of top most point on graph's y-axis]
-    4. background_value == 0 or 1 
-        0: When the graph's background color is relatively darker than the curve 
-        1: Otherwise
+How to pass arguments- 
+
+1. image_path == path to a graph image 
+
+2. x_range == [Value of left most point on graph's x-axis, Value of right most point on graph's x-axis]
+
+3. y_range == [Value of bottom most point on graph's y-axis, Value of top most point on graph's y-axis]
+
+4. background_value == 0 or 1 
+
+   0: When the graph's background color is relatively darker than the curve
+
+   1: Otherwise)  
+
 
 Caution- Try to pass the Image by erasing the axes
```

### Comparing `graph_cordinates-0.0.2/graph_cordinates/graph_cordinates.py` & `graph_cordinates-0.0.3/graph_cordinates/graph_cordinates.py`

 * *Files identical despite different names*

### Comparing `graph_cordinates-0.0.2/graph_cordinates.egg-info/PKG-INFO` & `graph_cordinates-0.0.3/graph_cordinates.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,41 @@
 Metadata-Version: 2.1
 Name: graph-cordinates
-Version: 0.0.2
-Summary: From Image of a curve/graph, extract and store the cordinates pairs in a 2D array, Github link (https://github.com/kumarUjjawal3621/mypython_lib)
+Version: 0.0.3
+Summary: From Image of a curve/graph, extract and store the cordinates pairs in a 2D array 
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
 
  
-How to use:
-    1. import graph_cordinates.graph_cordinates as gc
-    2. gc.get_graphcordinates(image_path,x_range,y_range,background_value)
-    3. Will return an array of 2D cordinates: [[x1,y1], [x2,y2], .......n-points] ; n=pixel width of Image
+How to use: 
+
+1. import graph_cordinates.graph_cordinates as gc 
+
+2. gc.get_graphcordinates(image_path,x_range,y_range,background_value) 
+
+3. Will return an array of 2D cordinates: [[x1,y1], [x2,y2], .......n-points] ; n=pixel width of Image 
+
     
-How to pass arguments-
-    1. image_path == path to a graph image
-    2. x_range == [Value of left most point on graph's x-axis, Value of right most point on graph's x-axis]
-    3. y_range == [Value of bottom most point on graph's y-axis, Value of top most point on graph's y-axis]
-    4. background_value == 0 or 1 
-        0: When the graph's background color is relatively darker than the curve 
-        1: Otherwise
+How to pass arguments- 
+
+1. image_path == path to a graph image 
+
+2. x_range == [Value of left most point on graph's x-axis, Value of right most point on graph's x-axis]
+
+3. y_range == [Value of bottom most point on graph's y-axis, Value of top most point on graph's y-axis]
+
+4. background_value == 0 or 1 
+
+   0: When the graph's background color is relatively darker than the curve
+
+   1: Otherwise)  
+
 
 Caution- Try to pass the Image by erasing the axes
```

### Comparing `graph_cordinates-0.0.2/setup.py` & `graph_cordinates-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
-DESCRIPTION = 'From Image of a curve/graph, extract and store the cordinates pairs in a 2D array, Github link (https://github.com/kumarUjjawal3621/mypython_lib)'
+VERSION = '0.0.3'
+DESCRIPTION = 'From Image of a curve/graph, extract and store the cordinates pairs in a 2D array \n Github link (https://github.com/kumarUjjawal3621/mypython_lib)'
 LONG_DESCRIPTION = """ 
-How to use:
-    1. import graph_cordinates.graph_cordinates as gc
-    2. gc.get_graphcordinates(image_path,x_range,y_range,background_value)
-    3. Will return an array of 2D cordinates: [[x1,y1], [x2,y2], .......n-points] ; n=pixel width of Image
+How to use: \n
+1. import graph_cordinates.graph_cordinates as gc \n
+2. gc.get_graphcordinates(image_path,x_range,y_range,background_value) \n
+3. Will return an array of 2D cordinates: [[x1,y1], [x2,y2], .......n-points] ; n=pixel width of Image \n
     
-How to pass arguments-
-    1. image_path == path to a graph image
-    2. x_range == [Value of left most point on graph's x-axis, Value of right most point on graph's x-axis]
-    3. y_range == [Value of bottom most point on graph's y-axis, Value of top most point on graph's y-axis]
-    4. background_value == 0 or 1 
-        0: When the graph's background color is relatively darker than the curve 
-        1: Otherwise
+How to pass arguments- \n
+1. image_path == path to a graph image \n
+2. x_range == [Value of left most point on graph's x-axis, Value of right most point on graph's x-axis]\n
+3. y_range == [Value of bottom most point on graph's y-axis, Value of top most point on graph's y-axis]\n
+4. background_value == 0 or 1 \n
+   0: When the graph's background color is relatively darker than the curve\n
+   1: Otherwise)  \n
 
 Caution- Try to pass the Image by erasing the axes
 """
 # Setting up
 
 setup(
     name="graph_cordinates",
```

