# Comparing `tmp/adafri-0.0.19.31.tar.gz` & `tmp/adafri-0.0.19.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.19.31.tar", last modified: Sat Jul 15 08:08:28 2023, max compression
+gzip compressed data, was "adafri-0.0.19.32.tar", last modified: Sat Jul 15 08:15:26 2023, max compression
```

## Comparing `adafri-0.0.19.31.tar` & `adafri-0.0.19.32.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:08:28.582288 adafri-0.0.19.31/
--rw-r--r--   0 ibrahima   (502) staff       (20)      496 2023-07-15 08:08:28.581889 adafri-0.0.19.31/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:08:28.556402 adafri-0.0.19.31/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       56 2023-07-12 01:19:08.000000 adafri-0.0.19.31/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:08:28.561477 adafri-0.0.19.31/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.31/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.31/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19.31/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:08:28.562213 adafri-0.0.19.31/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       86 2023-07-12 12:02:53.000000 adafri-0.0.19.31/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:08:28.563081 adafri-0.0.19.31/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.31/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:08:28.565502 adafri-0.0.19.31/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.31/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.31/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.31/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:08:28.566462 adafri-0.0.19.31/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-12 12:28:46.000000 adafri-0.0.19.31/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:08:28.567897 adafri-0.0.19.31/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.31/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.31/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:08:28.568827 adafri-0.0.19.31/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.31/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:08:28.569150 adafri-0.0.19.31/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      594 2023-07-13 01:00:40.000000 adafri-0.0.19.31/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:08:28.575822 adafri-0.0.19.31/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.31/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-15 07:56:20.000000 adafri-0.0.19.31/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.31/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9475 2023-07-15 08:08:12.000000 adafri-0.0.19.31/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2985 2023-07-12 11:23:27.000000 adafri-0.0.19.31/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9045 2023-07-13 22:38:46.000000 adafri-0.0.19.31/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.31/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:08:28.577564 adafri-0.0.19.31/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.31/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.31/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:08:28.578298 adafri-0.0.19.31/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.31/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:08:28.580817 adafri-0.0.19.31/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.31/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.31/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.31/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:08:28.559227 adafri-0.0.19.31/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      496 2023-07-15 08:08:28.000000 adafri-0.0.19.31/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1046 2023-07-15 08:08:28.000000 adafri-0.0.19.31/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-15 08:08:28.000000 adafri-0.0.19.31/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-15 08:08:28.000000 adafri-0.0.19.31/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-15 08:08:28.582428 adafri-0.0.19.31/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)     1010 2023-07-15 08:08:20.000000 adafri-0.0.19.31/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.683614 adafri-0.0.19.32/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      496 2023-07-15 08:15:26.683107 adafri-0.0.19.32/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.653950 adafri-0.0.19.32/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       56 2023-07-12 01:19:08.000000 adafri-0.0.19.32/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.659134 adafri-0.0.19.32/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.32/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.32/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19.32/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.659885 adafri-0.0.19.32/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       86 2023-07-12 12:02:53.000000 adafri-0.0.19.32/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.660713 adafri-0.0.19.32/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.32/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.663115 adafri-0.0.19.32/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.32/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.32/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.32/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.663982 adafri-0.0.19.32/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-12 12:28:46.000000 adafri-0.0.19.32/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.665668 adafri-0.0.19.32/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.32/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.32/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.666569 adafri-0.0.19.32/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.32/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.666874 adafri-0.0.19.32/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      594 2023-07-13 01:00:40.000000 adafri-0.0.19.32/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.673697 adafri-0.0.19.32/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.32/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-15 07:56:20.000000 adafri-0.0.19.32/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.32/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9475 2023-07-15 08:08:12.000000 adafri-0.0.19.32/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2985 2023-07-12 11:23:27.000000 adafri-0.0.19.32/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9139 2023-07-15 08:15:04.000000 adafri-0.0.19.32/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.32/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.675707 adafri-0.0.19.32/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.32/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.32/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.676403 adafri-0.0.19.32/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.32/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.681695 adafri-0.0.19.32/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.32/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.32/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.32/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 08:15:26.656699 adafri-0.0.19.32/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      496 2023-07-15 08:15:26.000000 adafri-0.0.19.32/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1046 2023-07-15 08:15:26.000000 adafri-0.0.19.32/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-15 08:15:26.000000 adafri-0.0.19.32/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-15 08:15:26.000000 adafri-0.0.19.32/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-15 08:15:26.683843 adafri-0.0.19.32/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1010 2023-07-15 08:15:20.000000 adafri-0.0.19.32/setup.py
```

### Comparing `adafri-0.0.19.31/adafri/utils/response.py` & `adafri-0.0.19.32/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.31/adafri/utils/utils.py` & `adafri-0.0.19.32/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.31/adafri/v1/account/models/account.py` & `adafri-0.0.19.32/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.31/adafri/v1/account/models/account_fields.py` & `adafri-0.0.19.32/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.31/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.19.32/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.31/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.19.32/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.31/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.19.32/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.31/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.19.32/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.31/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.19.32/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.31/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.19.32/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.31/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.19.32/adafri/v1/auth/oauth/models/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .....utils.response import ApiResponse, Error, ResponseStatus, StatusCode
 from typing import Any
 from dataclasses import dataclass
 from ....user import User
 from authlib.oauth2.rfc7009 import RevocationEndpoint
 from authlib.oauth2.rfc6750 import BearerTokenValidator
 from authlib.oauth2.rfc6749 import grants
-from authlib.oauth2.rfc6749 import TokenMixin
+from authlib.oauth2.rfc6749 import TokenMixin, scope_to_list
 from authlib.oauth2.rfc6750 import BearerTokenGenerator
 from datetime import datetime, timedelta
 import json
 from flask import abort, Response
 
 @dataclass(init=False)
 class OAuthToken(TokenMixin, FirebaseCollectionBase):
@@ -135,15 +135,17 @@
 
 class TokenValidator(BearerTokenValidator):
     def authenticate_token(self, token_string):
         token_request = OAuthToken().query([{"key":"access_token", "comp": "==", "value": token_string}], True)
         return token_request
     
     def validate_token(self, token, scopes, request):
-        token_scopes = json.loads(token.scope);
+        token_scopes = scope_to_list(token.scope);
+        print('token_scopes', token_scopes)
+        print('scopes', scopes)
         insufficient = self.scope_insufficient(token_scopes, scopes);
         if insufficient:
             response = ApiResponse(ResponseStatus.ERROR, StatusCode.status_400, None, Error("Insufficient privilegies","INVALID_REQUEST", 1)).to_json()
             return abort(Response(response=json.dumps(response), status=401, mimetype='application/json'))        
         return None
 
 class TokenRevocationEndpoint(RevocationEndpoint):
```

### Comparing `adafri-0.0.19.31/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.19.32/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.31/adafri/v1/base/firebase_collection.py` & `adafri-0.0.19.32/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.31/adafri/v1/user/models/user.py` & `adafri-0.0.19.32/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.31/adafri/v1/user/models/user_fields.py` & `adafri-0.0.19.32/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.31/adafri.egg-info/SOURCES.txt` & `adafri-0.0.19.32/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.31/setup.py` & `adafri-0.0.19.32/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.19.31' 
+VERSION = '0.0.19.32' 
 DESCRIPTION = 'Adafri python module'
 LONG_DESCRIPTION = 'Adafri python module helper'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="adafri",
```

