# Comparing `tmp/yd_base-1.0.1-py3-none-any.whl.zip` & `tmp/yd_base-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 10292 bytes, number of entries: 19
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-14 23:46 yellowdot/__init__.py
--rw-r--r--  2.0 unx     8839 b- defN 23-Jul-14 23:46 yellowdot/firebase/YDFBUserUtils.py
--rw-r--r--  2.0 unx     1368 b- defN 23-Jul-14 23:46 yellowdot/firebase/YDFirebase.py
--rw-r--r--  2.0 unx     7452 b- defN 23-Jul-14 23:46 yellowdot/firebase/YDFirebaseFCM.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-14 23:46 yellowdot/firebase/__init__.py
--rw-r--r--  2.0 unx      266 b- defN 23-Jul-14 23:46 yellowdot/models/FBUserResponse.py
--rw-r--r--  2.0 unx      302 b- defN 23-Jul-14 23:46 yellowdot/models/Response.py
--rw-r--r--  2.0 unx       39 b- defN 23-Jul-14 23:46 yellowdot/models/__init__.py
--rw-r--r--  2.0 unx      359 b- defN 23-Jul-14 23:46 yellowdot/rbac/RBAC.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-14 23:46 yellowdot/rbac/__init__.py
--rw-r--r--  2.0 unx      583 b- defN 23-Jul-14 23:46 yellowdot/utils/FileLogger.py
--rw-r--r--  2.0 unx      982 b- defN 23-Jul-14 23:46 yellowdot/utils/TimeUtils.py
--rw-r--r--  2.0 unx     2023 b- defN 23-Jul-14 23:46 yellowdot/utils/YDCommon.py
--rw-r--r--  2.0 unx     1858 b- defN 23-Jul-14 23:46 yellowdot/utils/YDLogger.py
--rw-r--r--  2.0 unx       25 b- defN 23-Jul-14 23:46 yellowdot/utils/__init__.py
--rw-r--r--  2.0 unx     2164 b- defN 23-Jul-14 23:46 yd_base-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 23:46 yd_base-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-14 23:46 yd_base-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1564 b- defN 23-Jul-14 23:46 yd_base-1.0.1.dist-info/RECORD
-19 files, 27927 bytes uncompressed, 7712 bytes compressed:  72.4%
+Zip file size: 10294 bytes, number of entries: 19
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-15 00:13 yellowdot/__init__.py
+-rw-r--r--  2.0 unx     8839 b- defN 23-Jul-15 00:13 yellowdot/firebase/YDFBUserUtils.py
+-rw-r--r--  2.0 unx     1368 b- defN 23-Jul-15 00:13 yellowdot/firebase/YDFirebase.py
+-rw-r--r--  2.0 unx     7452 b- defN 23-Jul-15 00:13 yellowdot/firebase/YDFirebaseFCM.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 00:13 yellowdot/firebase/__init__.py
+-rw-r--r--  2.0 unx      266 b- defN 23-Jul-15 00:13 yellowdot/models/FBUserResponse.py
+-rw-r--r--  2.0 unx      302 b- defN 23-Jul-15 00:13 yellowdot/models/Response.py
+-rw-r--r--  2.0 unx       39 b- defN 23-Jul-15 00:13 yellowdot/models/__init__.py
+-rw-r--r--  2.0 unx      359 b- defN 23-Jul-15 00:13 yellowdot/rbac/RBAC.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 00:13 yellowdot/rbac/__init__.py
+-rw-r--r--  2.0 unx      583 b- defN 23-Jul-15 00:13 yellowdot/utils/FileLogger.py
+-rw-r--r--  2.0 unx      982 b- defN 23-Jul-15 00:13 yellowdot/utils/TimeUtils.py
+-rw-r--r--  2.0 unx     2023 b- defN 23-Jul-15 00:13 yellowdot/utils/YDCommon.py
+-rw-r--r--  2.0 unx     1858 b- defN 23-Jul-15 00:13 yellowdot/utils/YDLogger.py
+-rw-r--r--  2.0 unx       25 b- defN 23-Jul-15 00:13 yellowdot/utils/__init__.py
+-rw-r--r--  2.0 unx     2164 b- defN 23-Jul-15 00:14 yd_base-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-15 00:14 yd_base-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-15 00:14 yd_base-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1564 b- defN 23-Jul-15 00:14 yd_base-1.0.2.dist-info/RECORD
+19 files, 27927 bytes uncompressed, 7714 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: yellowdot/utils/YDLogger.py
 Comment: 
 
 Filename: yellowdot/utils/__init__.py
 Comment: 
 
-Filename: yd_base-1.0.1.dist-info/METADATA
+Filename: yd_base-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: yd_base-1.0.1.dist-info/WHEEL
+Filename: yd_base-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: yd_base-1.0.1.dist-info/top_level.txt
+Filename: yd_base-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: yd_base-1.0.1.dist-info/RECORD
+Filename: yd_base-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `yd_base-1.0.1.dist-info/METADATA` & `yd_base-1.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yd-base
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python package for yellowdot's base classes and Utilities
 Home-page: https://github.com/Yellow-Dot-Energy-Company-Ltd/yd_base_py
 Author: Bruno Kiprop and Jamie Omondi
 Author-email: brunookiprop@gmail.com,cruiseomondi90@gmail.com
 License: MIT,GNU
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `yd_base-1.0.1.dist-info/RECORD` & `yd_base-1.0.2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 yellowdot/rbac/RBAC.py,sha256=usNw7Kydc8i5w1E_s6fhNfSCAaDCcI-Dxa9rl-67El4,359
 yellowdot/rbac/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 yellowdot/utils/FileLogger.py,sha256=BvE5x1g6jRKiKl6O_ZJ-MtaUVbAL2Fo9U7w28X5Qe6g,583
 yellowdot/utils/TimeUtils.py,sha256=uAMqbuWscVaw2hc8IJlbFv_EMB3itSFwg4Nzb7BBDvU,982
 yellowdot/utils/YDCommon.py,sha256=l7A0Pag_7HdA6WYm3jfsT96pYg67ggXwOONrNEwiNvE,2023
 yellowdot/utils/YDLogger.py,sha256=aRIB6p8IBQPBlA7Zkzq2xbkosEHj9R_WYiTHOjcWD-k,1858
 yellowdot/utils/__init__.py,sha256=opvYWo2tKa1O-EhIt7V0YhaKNUomyM04EL9O6QYXxRI,25
-yd_base-1.0.1.dist-info/METADATA,sha256=xLeflkQg6l2KZNJ_ZF4Kiog_MsER3EmC2FU90399jCY,2164
-yd_base-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-yd_base-1.0.1.dist-info/top_level.txt,sha256=rviH4tlL5CkA3X2IDgg9DHH7pMU5EAJwyg5iKfOH27Q,10
-yd_base-1.0.1.dist-info/RECORD,,
+yd_base-1.0.2.dist-info/METADATA,sha256=TLn0paLBk0gFGbBNBITDV94LYzWGvbqB-CYG924sjak,2164
+yd_base-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+yd_base-1.0.2.dist-info/top_level.txt,sha256=rviH4tlL5CkA3X2IDgg9DHH7pMU5EAJwyg5iKfOH27Q,10
+yd_base-1.0.2.dist-info/RECORD,,
```

