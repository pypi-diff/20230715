# Comparing `tmp/jayshreeram-0.0.8-py3-none-any.whl.zip` & `tmp/jayshreeram-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1877 bytes, number of entries: 6
--rw-r--r--  2.0 unx      643 b- defN 23-Jul-15 10:48 jayshreeram/__init__.py
--rw-r--r--  2.0 unx      312 b- defN 23-Jul-15 10:54 jayshreeram-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-15 10:54 jayshreeram-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jul-15 10:54 jayshreeram-0.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Jul-15 10:54 jayshreeram-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      491 b- defN 23-Jul-15 10:54 jayshreeram-0.0.8.dist-info/RECORD
-6 files, 1602 bytes uncompressed, 977 bytes compressed:  39.0%
+Zip file size: 1876 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      647 b- defN 23-Jul-15 11:15 jayshreeram/__init__.py
+-rw-r--r--  2.0 unx      312 b- defN 23-Jul-15 11:17 jayshreeram-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-15 11:17 jayshreeram-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-15 11:17 jayshreeram-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-Jul-15 11:17 jayshreeram-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      491 b- defN 23-Jul-15 11:17 jayshreeram-0.0.9.dist-info/RECORD
+6 files, 1606 bytes uncompressed, 976 bytes compressed:  39.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: jayshreeram/__init__.py
 Comment: 
 
-Filename: jayshreeram-0.0.8.dist-info/METADATA
+Filename: jayshreeram-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: jayshreeram-0.0.8.dist-info/WHEEL
+Filename: jayshreeram-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: jayshreeram-0.0.8.dist-info/entry_points.txt
+Filename: jayshreeram-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: jayshreeram-0.0.8.dist-info/top_level.txt
+Filename: jayshreeram-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: jayshreeram-0.0.8.dist-info/RECORD
+Filename: jayshreeram-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jayshreeram/__init__.py

```diff
@@ -1,18 +1,18 @@
 import sys
 import os
 def display():
     if len(sys.argv) == 1 or sys.argv[1] != "-u" or sys.argv[3] != "-p" or sys.argv[5] != "-db":
         print("॥ जय श्री राम ॥")
         raise Exception("To run RESTfulApiGen run RESTfulApiGen -u <username> -p <password> -db <database_name>")
-        exit()
     else:
         print("HELL Yeah ")
         if not os.environ.get(sys.argv[4]):
             print(sys.argv[4])
         else:
             print(os.environ.get(sys.argv[4]))
+            exit()
         
     
 
 display()
 #  or sys.argv[5] != "--demo" or sys.argv[5] != "--demo-gunincorn" or sys.argv[5] != "--demo-react" or sys.argv[5] != "-react"
```

