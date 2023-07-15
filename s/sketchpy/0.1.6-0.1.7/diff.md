# Comparing `tmp/sketchpy-0.1.6.tar.gz` & `tmp/sketchpy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sketchpy-0.1.6.tar", last modified: Wed Jul 12 11:49:20 2023, max compression
+gzip compressed data, was "sketchpy-0.1.7.tar", last modified: Sat Jul 15 11:05:23 2023, max compression
```

## Comparing `sketchpy-0.1.6.tar` & `sketchpy-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 11:49:20.325994 sketchpy-0.1.6/
--rw-rw-rw-   0        0        0     1084 2022-09-22 04:18:14.000000 sketchpy-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     7351 2023-07-12 11:49:20.322995 sketchpy-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-12 11:49:20.326993 sketchpy-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     6246 2023-07-12 11:49:04.000000 sketchpy-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 11:49:20.251037 sketchpy-0.1.6/sketchpy/
--rw-rw-rw-   0        0        0        0 2023-07-06 16:25:29.000000 sketchpy-0.1.6/sketchpy/__init__.py
--rw-rw-rw-   0        0        0    28242 2023-07-12 11:32:29.000000 sketchpy-0.1.6/sketchpy/canvas.py
--rw-rw-rw-   0        0        0   102115 2023-07-12 11:46:20.000000 sketchpy-0.1.6/sketchpy/library.py
-drwxrwxrwx   0        0        0        0 2023-07-12 11:49:20.319997 sketchpy-0.1.6/sketchpy.egg-info/
--rw-rw-rw-   0        0        0     7351 2023-07-12 11:49:19.000000 sketchpy-0.1.6/sketchpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-07-12 11:49:20.000000 sketchpy-0.1.6/sketchpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 11:49:19.000000 sketchpy-0.1.6/sketchpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-07-12 11:49:19.000000 sketchpy-0.1.6/sketchpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-12 11:49:19.000000 sketchpy-0.1.6/sketchpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 11:05:23.071568 sketchpy-0.1.7/
+-rw-rw-rw-   0        0        0     1084 2022-09-22 04:18:14.000000 sketchpy-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     7351 2023-07-15 11:05:23.067569 sketchpy-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-15 11:05:23.072565 sketchpy-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     6246 2023-07-15 10:37:08.000000 sketchpy-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 11:05:22.998611 sketchpy-0.1.7/sketchpy/
+-rw-rw-rw-   0        0        0        0 2023-07-06 16:25:29.000000 sketchpy-0.1.7/sketchpy/__init__.py
+-rw-rw-rw-   0        0        0    28372 2023-07-15 10:37:05.000000 sketchpy-0.1.7/sketchpy/canvas.py
+-rw-rw-rw-   0        0        0   102115 2023-07-12 11:46:20.000000 sketchpy-0.1.7/sketchpy/library.py
+drwxrwxrwx   0        0        0        0 2023-07-15 11:05:23.065569 sketchpy-0.1.7/sketchpy.egg-info/
+-rw-rw-rw-   0        0        0     7351 2023-07-15 11:05:22.000000 sketchpy-0.1.7/sketchpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-07-15 11:05:22.000000 sketchpy-0.1.7/sketchpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 11:05:22.000000 sketchpy-0.1.7/sketchpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-07-15 11:05:22.000000 sketchpy-0.1.7/sketchpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-15 11:05:22.000000 sketchpy-0.1.7/sketchpy.egg-info/top_level.txt
```

### Comparing `sketchpy-0.1.6/LICENSE` & `sketchpy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sketchpy-0.1.6/PKG-INFO` & `sketchpy-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sketchpy
-Version: 0.1.6
+Version: 0.1.7
 Summary: sketchpy
 Home-page: UNKNOWN
 Author: Mr Mystery
 Author-email: sriramanand23@gmail.com
 License: UNKNOWN
 Description: 
         # Welcome to sketchpy
```

### Comparing `sketchpy-0.1.6/setup.py` & `sketchpy-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 DESCRIPTION = 'sketchpy'
 LONG_DESCRIPTION = """
 # Welcome to sketchpy
 
 <h2>Intro to the project and some quick information,followed by an image of the project.<h2>
 
 <div align="center">
```

### Comparing `sketchpy-0.1.6/sketchpy/canvas.py` & `sketchpy-0.1.7/sketchpy/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -672,15 +672,15 @@
             tu.done()
             help()
 
 
 
 
 class trace_from_image:
-    def __init__(self, path, scale = 0.5, intensity = 230, save = False):
+    def __init__(self, path, scale = 0.5, intensity = 230, save = False, details = 10, blur = 31):
         '''path -> path of the image to be sketched
 
         scale - > scaling factor for the sketched image,
 
         less than 1 => smaller than original image,
         equal to 1 => original size
 
@@ -695,14 +695,16 @@
         self.pen = tu.Turtle()
         self.img = cv2.imread(path, 0)
         self.x_off = int(-1*(self.img.shape[1]//2) *self.scale)
         self.y_off = int((self.img.shape[0]//2)*self.scale)
         self.intensity = intensity
         self.save = save
         self.window = tu.Screen()
+        self.details = details
+        self.blur = blur
 
 
     def move_to(self, x, y):
         self.pen.up()
         self.pen.goto(x, y)
         self.pen.down()
 
@@ -714,50 +716,50 @@
             kernel = np.ones((1, 1), np.uint8)
             binary_image = cv2.morphologyEx(
                 binary_image, cv2.MORPH_OPEN, kernel, iterations=3)
             binary_image = cv2.morphologyEx(
                 binary_image, cv2.MORPH_CLOSE, kernel, iterations=3)
             num_labels, labels, stats, _ = cv2.connectedComponentsWithStats(binary_image)
             output_image = np.zeros((self.img.shape[0], self.img.shape[1], 3), dtype=np.uint8)
-            min_region_size = 40
+            min_region_size = self.details
 
             for label in range(1, num_labels):
                 region_size = stats[label, cv2.CC_STAT_AREA]
                 if region_size > min_region_size:
                     region = np.where(labels == label, 255, 0).astype(np.uint8)
                     output_image[np.where(labels == label)] = (
                         255, 255, 255)
 
             invert = cv2.bitwise_not(output_image)  
-            blur = cv2.GaussianBlur(invert, (31, 31), 0)
+            blur = cv2.GaussianBlur(invert, (self.blur, self.blur), 0)
             invertedblur = cv2.bitwise_not(blur)
             sketch = cv2.divide(output_image, invertedblur, scale=256.0)
 
             cv2.imwrite("ttmp.jpg", sketch)
             self.img = cv2.imread("ttmp.jpg")
 
 
             grey_img = cv2.cvtColor(self.img, cv2.COLOR_BGR2GRAY)
             invert = cv2.bitwise_not(grey_img) 
-            blur = cv2.GaussianBlur(invert, (21, 21), 0)
+            blur = cv2.GaussianBlur(invert, (self.blur, self.blur), 0)
             invertedblur = cv2.bitwise_not(blur)
             sketch = cv2.divide(grey_img, invertedblur, scale=256.0)
             ret, thresh = cv2.threshold(sketch, self.intensity, 255, 0)
             ctu, hire = cv2.findContours(thresh, cv2.RETR_TREE, cv2.CHAIN_APPROX_NONE)        
     
             return ctu 
         except Exception as e:
             print("error found!!!")
             print(f"ERROR: {e}")
             print('''you can contact me on my youtube channel: https://www.youtube.com/c/codehub03 \\n discord : https://discord.gg/r2KFa73PM2 \\n instagram : https://www.instagram.com/mr.m_y_s_t_e_r_y/''')
 
     def draw(self):
         ctu = self.processimage()
         for n, pos in enumerate(ctu):
-            if len(pos) <= 100:
+            if len(pos) <= self.details:
                 continue
             mask = np.zeros(self.img.shape[:2], dtype=np.uint8)
             cv2.drawContours(mask, ctu, n, (255), thickness=cv2.FILLED)
             average_color = cv2.mean(self.img, mask=mask)
             rgb = 1 - average_color[0]/255, 1 - \
                 average_color[1]/255, 1-average_color[2]/255
             te = pos.flatten()
```

### Comparing `sketchpy-0.1.6/sketchpy/library.py` & `sketchpy-0.1.7/sketchpy/library.py`

 * *Files identical despite different names*

### Comparing `sketchpy-0.1.6/sketchpy.egg-info/PKG-INFO` & `sketchpy-0.1.7/sketchpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sketchpy
-Version: 0.1.6
+Version: 0.1.7
 Summary: sketchpy
 Home-page: UNKNOWN
 Author: Mr Mystery
 Author-email: sriramanand23@gmail.com
 License: UNKNOWN
 Description: 
         # Welcome to sketchpy
```

