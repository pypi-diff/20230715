# Comparing `tmp/mostats-1.0.7-py3-none-any.whl.zip` & `tmp/mostats-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 18774 bytes, number of entries: 8
+Zip file size: 18791 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-02 08:19 mostats/__init__.py
--rw-r--r--  2.0 unx    13141 b- defN 23-Jul-15 18:02 mostats/getCluster.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Jul-15 18:12 mostats-1.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     5555 b- defN 23-Jul-15 18:12 mostats-1.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-15 18:12 mostats-1.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jul-15 18:12 mostats-1.0.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-15 18:12 mostats-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      633 b- defN 23-Jul-15 18:12 mostats-1.0.7.dist-info/RECORD
-8 files, 54630 bytes uncompressed, 17666 bytes compressed:  67.7%
+-rw-r--r--  2.0 unx    13354 b- defN 23-Jul-15 18:15 mostats/getCluster.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Jul-15 18:16 mostats-1.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5555 b- defN 23-Jul-15 18:16 mostats-1.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-15 18:16 mostats-1.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-15 18:16 mostats-1.0.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-15 18:16 mostats-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      633 b- defN 23-Jul-15 18:16 mostats-1.0.8.dist-info/RECORD
+8 files, 54843 bytes uncompressed, 17683 bytes compressed:  67.8%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: mostats/__init__.py
 Comment: 
 
 Filename: mostats/getCluster.py
 Comment: 
 
-Filename: mostats-1.0.7.dist-info/LICENSE
+Filename: mostats-1.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: mostats-1.0.7.dist-info/METADATA
+Filename: mostats-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: mostats-1.0.7.dist-info/WHEEL
+Filename: mostats-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: mostats-1.0.7.dist-info/entry_points.txt
+Filename: mostats-1.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: mostats-1.0.7.dist-info/top_level.txt
+Filename: mostats-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: mostats-1.0.7.dist-info/RECORD
+Filename: mostats-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mostats/getCluster.py

```diff
@@ -33,16 +33,20 @@
                             help='Expected IOPS\n')
     args = argparser.parse_args()
     
     print('\nMostats - Get the MongoDB database statistic to an excel file\nPlease follow the instruction by run mostats -h\n')
 
     if args.namefile != "":
         cname = read_file(args.namefile)
+        if(len(conn_pool) != len(cname)) and (len(cname) >0 ):
+            raise Exception(f'The number of MongoDB URL "{len(conn_pool)}" doesnt match with the number of cluster name "{len(cname)}"')
     elif args.name != "": 
         cname = args.name
+        if(len(conn_pool) != len(cname)) and (len(cname) >0 ):
+            raise Exception(f'The number of MongoDB URL "{len(conn_pool)}" doesnt match with the number of cluster name "{len(cname)}"')
 
     if args.urlfile != "":
         conn_pool = read_file(args.urlfile)          
     else: 
         conn_pool = args.url       
 
     if args.name == "":
@@ -51,16 +55,15 @@
         print(f'Get the database information from : "{conn_pool}" with cluster name "{args.name}" and save to "{args.excelfile}"')
     #print('\n')
     print('\nPlease wait as it might take a while...')
 
     more_info = args.moreinfo
     counter = 0
 
-    if(len(conn_pool) != len(cname)) and (len(cname) >0 ):
-        raise Exception(f'The number of MongoDB URL "{len(conn_pool)}" doesnt match with the number of cluster name "{len(cname)}"')
+    
     
     try:
         for conn in conn_pool:
             print(f'Getting database information from {conn}. Progress: {counter+1}/{len(conn_pool)}')
             totalindex = 0
             totalindexsize =0
             totaluniqueindex =0
```

## Comparing `mostats-1.0.7.dist-info/LICENSE` & `mostats-1.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mostats-1.0.7.dist-info/METADATA` & `mostats-1.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mostats
-Version: 1.0.7
+Version: 1.0.8
 Summary: Get the MongoDB database statistic to a local CSV file
 Home-page: https://github.com/pix3lize/mostats
 Author: Hendri Tjipto
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
```

