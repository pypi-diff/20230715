# Comparing `tmp/pyclipr-0.1.0-cp39-cp39-win_amd64.whl.zip` & `tmp/pyclipr-0.1.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 152535 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat       24 b- defN 23-Jul-14 22:49 pyclipr/__init__.py
--rw-rw-rw-  2.0 fat   328192 b- defN 23-Jul-14 22:51 pyclipr/pyclipr.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     7886 b- defN 23-Jul-14 22:51 pyclipr-0.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7067 b- defN 23-Jul-14 22:51 pyclipr-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-14 22:51 pyclipr-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-14 22:51 pyclipr-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      553 b- defN 23-Jul-14 22:51 pyclipr-0.1.0.dist-info/RECORD
-7 files, 343830 bytes uncompressed, 151557 bytes compressed:  55.9%
+Zip file size: 152550 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat       24 b- defN 23-Jul-15 16:18 pyclipr/__init__.py
+-rw-rw-rw-  2.0 fat   328192 b- defN 23-Jul-15 16:20 pyclipr/pyclipr.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     7886 b- defN 23-Jul-15 16:21 pyclipr-0.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7053 b- defN 23-Jul-15 16:21 pyclipr-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-15 16:21 pyclipr-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-15 16:21 pyclipr-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      553 b- defN 23-Jul-15 16:21 pyclipr-0.1.1.dist-info/RECORD
+7 files, 343816 bytes uncompressed, 151572 bytes compressed:  55.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pyclipr/__init__.py
 Comment: 
 
 Filename: pyclipr/pyclipr.cp39-win_amd64.pyd
 Comment: 
 
-Filename: pyclipr-0.1.0.dist-info/LICENSE
+Filename: pyclipr-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: pyclipr-0.1.0.dist-info/METADATA
+Filename: pyclipr-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pyclipr-0.1.0.dist-info/WHEEL
+Filename: pyclipr-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyclipr-0.1.0.dist-info/top_level.txt
+Filename: pyclipr-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyclipr-0.1.0.dist-info/RECORD
+Filename: pyclipr-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyclipr-0.1.0.dist-info/LICENSE` & `pyclipr-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyclipr-0.1.0.dist-info/METADATA` & `pyclipr-0.1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclipr
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library for polygon clipping and offsetting based on Clipper2.
 Home-page: https://github.com/drlukeparry/pyclipr
 Author: Luke Parry
 Author-email: dev@lukeparry.uk
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/drylukeparry/pyclipr
 Project-URL: Source, https://github.com/drylukeparry/pyclipr
@@ -114,16 +114,16 @@
     # Create a clipping object
     pc = pyclipr.Clipper()
     pc.scaleFactor = int(1000)
 
     # Add the paths to the clipping object. Ensure the subject and clip arguments are set to differentiate
     # the paths during the Boolean operation. The final argument specifies if the path is
     # open.
-    pc.addPaths(offsetSquare, pyclipr.Subject, False)
-    pc.addPath(np.array(path2), pyclipr.Clip, False)
+    pc.addPaths(offsetSquare, pyclipr.Subject)
+    pc.addPath(np.array(path2), pyclipr.Clip)
 
     """ Test Polygon Clipping """
     # Below returns paths
     out  = pc.execute(pyclipr.Intersection, pyclipr.EvenOdd)
     out2 = pc.execute(pyclipr.Union, pyclipr.EvenOdd)
     out3 = pc.execute(pyclipr.Difference, pyclipr.EvenOdd)
     out4 = pc.execute(pyclipr.Xor, pyclipr.EvenOdd)
```

