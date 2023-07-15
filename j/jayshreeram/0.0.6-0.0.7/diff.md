# Comparing `tmp/jayshreeram-0.0.6-py3-none-any.whl.zip` & `tmp/jayshreeram-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1685 bytes, number of entries: 6
--rw-r--r--  2.0 unx      144 b- defN 23-Jul-14 19:08 jayshreeram/__init__.py
--rw-r--r--  2.0 unx      312 b- defN 23-Jul-14 19:08 jayshreeram-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 19:08 jayshreeram-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jul-14 19:08 jayshreeram-0.0.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-14 19:08 jayshreeram-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      491 b- defN 23-Jul-14 19:08 jayshreeram-0.0.6.dist-info/RECORD
-6 files, 1103 bytes uncompressed, 785 bytes compressed:  28.8%
+Zip file size: 1819 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      395 b- defN 23-Jul-15 05:09 jayshreeram/__init__.py
+-rw-r--r--  2.0 unx      312 b- defN 23-Jul-15 05:10 jayshreeram-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-15 05:10 jayshreeram-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-15 05:10 jayshreeram-0.0.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-15 05:10 jayshreeram-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      491 b- defN 23-Jul-15 05:10 jayshreeram-0.0.7.dist-info/RECORD
+6 files, 1354 bytes uncompressed, 919 bytes compressed:  32.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: jayshreeram/__init__.py
 Comment: 
 
-Filename: jayshreeram-0.0.6.dist-info/METADATA
+Filename: jayshreeram-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: jayshreeram-0.0.6.dist-info/WHEEL
+Filename: jayshreeram-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: jayshreeram-0.0.6.dist-info/entry_points.txt
+Filename: jayshreeram-0.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: jayshreeram-0.0.6.dist-info/top_level.txt
+Filename: jayshreeram-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: jayshreeram-0.0.6.dist-info/RECORD
+Filename: jayshreeram-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jayshreeram/__init__.py

```diff
@@ -1,7 +1,11 @@
 import sys
-
 def display():
-    print("॥ जय श्री राम ॥")
+    if sys.argv[0] != "jayshreeram" and len(sys.argv) >= 0  or sys.argv[1] != "-u" or sys.argv[2] != "-p" or sys.argv[3] != "-db":
+        print("॥ जय श्री राम ॥")
+        raise Exception("To run RESTfulApiGen run RESTfulApiGen -u <username> -p <password> -db <database_name>")
+        exit()
+    else:
+        print("HELL Yeah ")
+    
 
-    for i in range(1, len(sys.argv)):
-        print(sys.argv[i])
+display()
```

