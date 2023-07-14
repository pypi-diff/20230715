# Comparing `tmp/yd_base-1.0.0rc0-py3-none-any.whl.zip` & `tmp/yd_base-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,21 @@
-Zip file size: 8634 bytes, number of entries: 15
--rw-r--r--  2.0 unx       31 b- defN 23-Jul-14 19:36 yellowdot/__init__.py
--rw-r--r--  2.0 unx     8839 b- defN 23-Jul-14 19:36 yellowdot/firebase/YDFBUserUtils.py
--rw-r--r--  2.0 unx     1368 b- defN 23-Jul-14 19:36 yellowdot/firebase/YDFirebase.py
--rw-r--r--  2.0 unx     7452 b- defN 23-Jul-14 19:36 yellowdot/firebase/YDFirebaseFCM.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-14 19:36 yellowdot/firebase/__init__.py
--rw-r--r--  2.0 unx      266 b- defN 23-Jul-14 19:36 yellowdot/models/FBUserResponse.py
--rw-r--r--  2.0 unx      302 b- defN 23-Jul-14 19:36 yellowdot/models/Response.py
--rw-r--r--  2.0 unx       39 b- defN 23-Jul-14 19:36 yellowdot/models/__init__.py
--rw-r--r--  2.0 unx      904 b- defN 23-Jul-14 19:36 yellowdot/utils/YDCommon.py
--rw-r--r--  2.0 unx     1858 b- defN 23-Jul-14 19:36 yellowdot/utils/YDLogger.py
--rw-r--r--  2.0 unx       25 b- defN 23-Jul-14 19:36 yellowdot/utils/__init__.py
--rw-r--r--  2.0 unx     2167 b- defN 23-Jul-14 19:37 yd_base-1.0.0rc0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 19:37 yd_base-1.0.0rc0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-14 19:37 yd_base-1.0.0rc0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1249 b- defN 23-Jul-14 19:37 yd_base-1.0.0rc0.dist-info/RECORD
-15 files, 24602 bytes uncompressed, 6544 bytes compressed:  73.4%
+Zip file size: 10292 bytes, number of entries: 19
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-14 23:46 yellowdot/__init__.py
+-rw-r--r--  2.0 unx     8839 b- defN 23-Jul-14 23:46 yellowdot/firebase/YDFBUserUtils.py
+-rw-r--r--  2.0 unx     1368 b- defN 23-Jul-14 23:46 yellowdot/firebase/YDFirebase.py
+-rw-r--r--  2.0 unx     7452 b- defN 23-Jul-14 23:46 yellowdot/firebase/YDFirebaseFCM.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-14 23:46 yellowdot/firebase/__init__.py
+-rw-r--r--  2.0 unx      266 b- defN 23-Jul-14 23:46 yellowdot/models/FBUserResponse.py
+-rw-r--r--  2.0 unx      302 b- defN 23-Jul-14 23:46 yellowdot/models/Response.py
+-rw-r--r--  2.0 unx       39 b- defN 23-Jul-14 23:46 yellowdot/models/__init__.py
+-rw-r--r--  2.0 unx      359 b- defN 23-Jul-14 23:46 yellowdot/rbac/RBAC.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-14 23:46 yellowdot/rbac/__init__.py
+-rw-r--r--  2.0 unx      583 b- defN 23-Jul-14 23:46 yellowdot/utils/FileLogger.py
+-rw-r--r--  2.0 unx      982 b- defN 23-Jul-14 23:46 yellowdot/utils/TimeUtils.py
+-rw-r--r--  2.0 unx     2023 b- defN 23-Jul-14 23:46 yellowdot/utils/YDCommon.py
+-rw-r--r--  2.0 unx     1858 b- defN 23-Jul-14 23:46 yellowdot/utils/YDLogger.py
+-rw-r--r--  2.0 unx       25 b- defN 23-Jul-14 23:46 yellowdot/utils/__init__.py
+-rw-r--r--  2.0 unx     2164 b- defN 23-Jul-14 23:46 yd_base-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-14 23:46 yd_base-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-14 23:46 yd_base-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1564 b- defN 23-Jul-14 23:46 yd_base-1.0.1.dist-info/RECORD
+19 files, 27927 bytes uncompressed, 7712 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -18,29 +18,41 @@
 
 Filename: yellowdot/models/Response.py
 Comment: 
 
 Filename: yellowdot/models/__init__.py
 Comment: 
 
+Filename: yellowdot/rbac/RBAC.py
+Comment: 
+
+Filename: yellowdot/rbac/__init__.py
+Comment: 
+
+Filename: yellowdot/utils/FileLogger.py
+Comment: 
+
+Filename: yellowdot/utils/TimeUtils.py
+Comment: 
+
 Filename: yellowdot/utils/YDCommon.py
 Comment: 
 
 Filename: yellowdot/utils/YDLogger.py
 Comment: 
 
 Filename: yellowdot/utils/__init__.py
 Comment: 
 
-Filename: yd_base-1.0.0rc0.dist-info/METADATA
+Filename: yd_base-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: yd_base-1.0.0rc0.dist-info/WHEEL
+Filename: yd_base-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: yd_base-1.0.0rc0.dist-info/top_level.txt
+Filename: yd_base-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: yd_base-1.0.0rc0.dist-info/RECORD
+Filename: yd_base-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yellowdot/__init__.py

```diff
@@ -1,2 +1 @@
-00000000: 6672 6f6d 2079 656c 6c6f 7764 6f74 2e6d  from yellowdot.m
-00000010: 6f64 656c 7320 696d 706f 7274 202a 0a    odels import *.
+00000000: 0a                                       .
```

## yellowdot/utils/YDCommon.py

```diff
@@ -1,7 +1,8 @@
+import re
 import uuid
 
 """This is a singleton class that contains all the common variables and functions used in the project"""
 
 # Codes for the different types of objects in the database
 yd_uid_code = "YDUID"
 yd_order_code = "YDORDER"
@@ -29,7 +30,44 @@
             YDCommon._instance = YDCommon()
         return YDCommon._instance
 
     # Generates a random uid for the user
     @staticmethod
     def generate_uid():
         return uuid.uuid4().hex[:30]
+
+    # Body handler for the request
+    @staticmethod
+    def get_body(request):
+        return request.body.decode('utf-8')
+
+    # Checks if the given string is a valid email
+    @staticmethod
+    def is_valid_email(email):
+        # Check if the email matches email address format
+        if re.match(r"[^@]+@[^@]+\.[^@]+", email):
+            return True
+        return False
+
+    # Checks if the given string is a valid phone number
+    @staticmethod
+    def is_valid_phone(phone):
+        # Check if the phone matches phone number format
+        if re.match(r"^\d{10}$", phone):
+            return True
+        return False
+
+    # Check if request body is greater than 5MB
+    @staticmethod
+    def is_body_too_large(request):
+        if len(request.body) > 5242880:
+            return True
+        return False
+
+    # Check if the given string is a valid password
+    @staticmethod
+    def is_valid_password(password):
+        # Check if the password matches password format
+        if re.match(r"^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)[a-zA-Z\d]{8,}$", password):
+            return True
+        return False
+
```

## Comparing `yd_base-1.0.0rc0.dist-info/METADATA` & `yd_base-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yd-base
-Version: 1.0.0rc0
+Version: 1.0.1
 Summary: A python package for yellowdot's base classes and Utilities
 Home-page: https://github.com/Yellow-Dot-Energy-Company-Ltd/yd_base_py
 Author: Bruno Kiprop and Jamie Omondi
 Author-email: brunookiprop@gmail.com,cruiseomondi90@gmail.com
 License: MIT,GNU
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

## Comparing `yd_base-1.0.0rc0.dist-info/RECORD` & `yd_base-1.0.1.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-yellowdot/__init__.py,sha256=JYALVfGefM1gPa6vV881EuKDVNLp8Z_8PsT6TkKis-I,31
+yellowdot/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 yellowdot/firebase/YDFBUserUtils.py,sha256=V-rzDvXPPC5mhH3lBlU2QLzs4EsdboqOfqsLC3CAgio,8839
 yellowdot/firebase/YDFirebase.py,sha256=m-rbhGYpsXz41S_GLUcEOoMmtACG6c9L9zSeYN6lq-0,1368
 yellowdot/firebase/YDFirebaseFCM.py,sha256=I9o5XOI07hcaOEidVL373GJRT_BS_uNVC_b94oIyqhY,7452
 yellowdot/firebase/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 yellowdot/models/FBUserResponse.py,sha256=I_MYNihUZD2e3KjSi1rM2nTt74_lAFAu4qUV8q2dXsk,266
 yellowdot/models/Response.py,sha256=OmcwbFl0qDEHKE82Pg_juDK2xVTrsKs_2CBNqC5P-Qc,302
 yellowdot/models/__init__.py,sha256=lUT7osAnLGXY9Z8XN1YdjkrBoPA0XDbO-Di9idglK58,39
-yellowdot/utils/YDCommon.py,sha256=NJKJsRAEVdNrW6_Vfg4rXD9uxYrhXmlPw8HBBV9yg_Q,904
+yellowdot/rbac/RBAC.py,sha256=usNw7Kydc8i5w1E_s6fhNfSCAaDCcI-Dxa9rl-67El4,359
+yellowdot/rbac/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+yellowdot/utils/FileLogger.py,sha256=BvE5x1g6jRKiKl6O_ZJ-MtaUVbAL2Fo9U7w28X5Qe6g,583
+yellowdot/utils/TimeUtils.py,sha256=uAMqbuWscVaw2hc8IJlbFv_EMB3itSFwg4Nzb7BBDvU,982
+yellowdot/utils/YDCommon.py,sha256=l7A0Pag_7HdA6WYm3jfsT96pYg67ggXwOONrNEwiNvE,2023
 yellowdot/utils/YDLogger.py,sha256=aRIB6p8IBQPBlA7Zkzq2xbkosEHj9R_WYiTHOjcWD-k,1858
 yellowdot/utils/__init__.py,sha256=opvYWo2tKa1O-EhIt7V0YhaKNUomyM04EL9O6QYXxRI,25
-yd_base-1.0.0rc0.dist-info/METADATA,sha256=7plVDT24UoCOfrUbavpz5I2DIrJAhBeD1D2RRUYDjsg,2167
-yd_base-1.0.0rc0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-yd_base-1.0.0rc0.dist-info/top_level.txt,sha256=rviH4tlL5CkA3X2IDgg9DHH7pMU5EAJwyg5iKfOH27Q,10
-yd_base-1.0.0rc0.dist-info/RECORD,,
+yd_base-1.0.1.dist-info/METADATA,sha256=xLeflkQg6l2KZNJ_ZF4Kiog_MsER3EmC2FU90399jCY,2164
+yd_base-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+yd_base-1.0.1.dist-info/top_level.txt,sha256=rviH4tlL5CkA3X2IDgg9DHH7pMU5EAJwyg5iKfOH27Q,10
+yd_base-1.0.1.dist-info/RECORD,,
```

