# Comparing `tmp/adafri-0.0.19.1.tar.gz` & `tmp/adafri-0.0.19.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.19.1.tar", last modified: Sat Jul 15 05:41:00 2023, max compression
+gzip compressed data, was "adafri-0.0.19.2.tar", last modified: Sat Jul 15 07:56:59 2023, max compression
```

## Comparing `adafri-0.0.19.1.tar` & `adafri-0.0.19.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 05:41:00.097190 adafri-0.0.19.1/
--rw-r--r--   0 ibrahima   (502) staff       (20)      495 2023-07-15 05:41:00.096752 adafri-0.0.19.1/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 05:41:00.072665 adafri-0.0.19.1/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       56 2023-07-12 01:19:08.000000 adafri-0.0.19.1/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 05:41:00.077229 adafri-0.0.19.1/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.1/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.1/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19.1/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 05:41:00.077901 adafri-0.0.19.1/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       86 2023-07-12 12:02:53.000000 adafri-0.0.19.1/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 05:41:00.078642 adafri-0.0.19.1/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.1/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 05:41:00.081160 adafri-0.0.19.1/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.1/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.1/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.1/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 05:41:00.082223 adafri-0.0.19.1/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-12 12:28:46.000000 adafri-0.0.19.1/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 05:41:00.084338 adafri-0.0.19.1/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.1/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.1/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 05:41:00.085519 adafri-0.0.19.1/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.1/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 05:41:00.086063 adafri-0.0.19.1/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      594 2023-07-13 01:00:40.000000 adafri-0.0.19.1/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 05:41:00.091760 adafri-0.0.19.1/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.1/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6467 2023-07-15 05:40:29.000000 adafri-0.0.19.1/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.1/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9437 2023-07-13 22:02:43.000000 adafri-0.0.19.1/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2985 2023-07-12 11:23:27.000000 adafri-0.0.19.1/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9045 2023-07-13 22:38:46.000000 adafri-0.0.19.1/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.1/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 05:41:00.093149 adafri-0.0.19.1/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.1/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.1/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 05:41:00.093644 adafri-0.0.19.1/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.1/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 05:41:00.095845 adafri-0.0.19.1/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.1/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.1/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.1/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 05:41:00.074993 adafri-0.0.19.1/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      495 2023-07-15 05:41:00.000000 adafri-0.0.19.1/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1046 2023-07-15 05:41:00.000000 adafri-0.0.19.1/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-15 05:41:00.000000 adafri-0.0.19.1/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-15 05:41:00.000000 adafri-0.0.19.1/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-15 05:41:00.097370 adafri-0.0.19.1/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)     1009 2023-07-15 05:40:55.000000 adafri-0.0.19.1/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 07:56:59.282664 adafri-0.0.19.2/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      495 2023-07-15 07:56:59.282163 adafri-0.0.19.2/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 07:56:59.256543 adafri-0.0.19.2/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       56 2023-07-12 01:19:08.000000 adafri-0.0.19.2/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 07:56:59.260836 adafri-0.0.19.2/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       44 2023-07-12 11:52:19.000000 adafri-0.0.19.2/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.19.2/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    15213 2023-07-13 01:22:12.000000 adafri-0.0.19.2/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 07:56:59.261597 adafri-0.0.19.2/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       86 2023-07-12 12:02:53.000000 adafri-0.0.19.2/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 07:56:59.262327 adafri-0.0.19.2/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.19.2/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 07:56:59.264391 adafri-0.0.19.2/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.19.2/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4532 2023-07-13 02:05:51.000000 adafri-0.0.19.2/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.19.2/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 07:56:59.265267 adafri-0.0.19.2/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-12 12:28:46.000000 adafri-0.0.19.2/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 07:56:59.266560 adafri-0.0.19.2/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       39 2023-07-12 12:02:09.000000 adafri-0.0.19.2/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1226 2023-07-13 01:57:34.000000 adafri-0.0.19.2/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 07:56:59.267422 adafri-0.0.19.2/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.19.2/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 07:56:59.267899 adafri-0.0.19.2/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      594 2023-07-13 01:00:40.000000 adafri-0.0.19.2/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 07:56:59.274877 adafri-0.0.19.2/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.19.2/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6514 2023-07-15 07:56:20.000000 adafri-0.0.19.2/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.19.2/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9623 2023-07-15 07:54:11.000000 adafri-0.0.19.2/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2985 2023-07-12 11:23:27.000000 adafri-0.0.19.2/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9045 2023-07-13 22:38:46.000000 adafri-0.0.19.2/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3212 2023-07-12 22:48:16.000000 adafri-0.0.19.2/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 07:56:59.276860 adafri-0.0.19.2/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.19.2/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-13 16:13:01.000000 adafri-0.0.19.2/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 07:56:59.277547 adafri-0.0.19.2/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.19.2/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 07:56:59.280763 adafri-0.0.19.2/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.19.2/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9327 2023-07-13 16:13:19.000000 adafri-0.0.19.2/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5205 2023-07-12 04:59:49.000000 adafri-0.0.19.2/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-15 07:56:59.258656 adafri-0.0.19.2/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      495 2023-07-15 07:56:59.000000 adafri-0.0.19.2/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1046 2023-07-15 07:56:59.000000 adafri-0.0.19.2/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-15 07:56:59.000000 adafri-0.0.19.2/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-15 07:56:59.000000 adafri-0.0.19.2/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-15 07:56:59.282916 adafri-0.0.19.2/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1009 2023-07-15 07:56:54.000000 adafri-0.0.19.2/setup.py
```

### Comparing `adafri-0.0.19.1/adafri/utils/response.py` & `adafri-0.0.19.2/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.1/adafri/utils/utils.py` & `adafri-0.0.19.2/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.1/adafri/v1/account/models/account.py` & `adafri-0.0.19.2/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.1/adafri/v1/account/models/account_fields.py` & `adafri-0.0.19.2/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.1/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.19.2/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.1/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.19.2/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.1/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.19.2/adafri/v1/auth/oauth/models/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .....utils.response import ApiResponse, Error, ResponseStatus, StatusCode
 from werkzeug.security import gen_salt
 import time
 from typing import Any
 from dataclasses import dataclass
 import json
 from authlib.oauth2.rfc6749 import ClientMixin
+from authlib.oauth2.rfc6749.util import list_to_scope, scope_to_list
 import secrets
 import pydash
 
 @dataclass(init=False)
 class OAuthClient(ClientMixin, FirebaseCollectionBase):
     id: str
     name: str
@@ -140,13 +141,12 @@
     
     def check_grant_type(self, grant_type):
         return grant_type in self.grant_types
     
     def get_allowed_scope(self, scope):
         if not scope:
             return ''
-        allowed = self.scopes
-        scopes = ArrayUtils.array_to_string([s for s in json.loads(scope) if s in allowed])
-        return scopes
+        allowed = set(scope_to_list(self.scope))
+        return list_to_scope([s for s in scope.split() if s in allowed])
     
     def check_redirect_uri(self, redirect_uri):
         return redirect_uri in self.allowed_redirect_uris
```

### Comparing `adafri-0.0.19.1/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.19.2/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.1/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.19.2/adafri/v1/auth/oauth/models/grant.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from ....base.firebase_collection import (FirebaseCollectionBase, getTimestamp)
 from .grant_fields import GrantFields, GrantFieldsProps, STANDARD_FIELDS, GRANT_COLLECTION
 from .....utils.response import ApiResponse, Error, ResponseStatus, StatusCode
 from typing import Any
 from dataclasses import dataclass
 from authlib.oauth2.rfc6749 import AuthorizationCodeMixin
 from authlib.oauth2.rfc6749 import grants
-from authlib.common.urls import add_params_to_uri 
+from authlib.common.urls import add_params_to_uri
+from authlib.oauth2.rfc6749.util import list_to_scope, scope_to_list
 from authlib.oauth2.rfc6749.errors import AccessDeniedError
 from ....user import User
 import pydash
 
 import os
 @dataclass(init=False)
 class OAuthGrant(AuthorizationCodeMixin, FirebaseCollectionBase):
@@ -91,16 +92,19 @@
 
         authorization_code_model.id = Crypto().generate_id(authorization_code_model.code+"~"+authorization_code_model.client_id);
         return ApiResponse(ResponseStatus.OK, StatusCode.status_200, authorization_code_model, None);
 
     def get_redirect_uri(self):
         return self.redirect_uri
     
-    def get_scope(self):
-        return ArrayUtils.array_to_string(self.scopes)
+    def get_scope(self, scope):
+        if not scope:
+            return ''
+        allowed = set(scope_to_list(self.scope))
+        return list_to_scope([s for s in scope.split() if s in allowed])
     
     @staticmethod
     def create(**kwargs):
         authorization_code = OAuthGrant().generate(**kwargs);
         if authorization_code.status == ResponseStatus.ERROR:
             return authorization_code
```

### Comparing `adafri-0.0.19.1/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.19.2/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.1/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.19.2/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.1/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.19.2/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.1/adafri/v1/base/firebase_collection.py` & `adafri-0.0.19.2/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.1/adafri/v1/user/models/user.py` & `adafri-0.0.19.2/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.1/adafri/v1/user/models/user_fields.py` & `adafri-0.0.19.2/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.1/adafri.egg-info/SOURCES.txt` & `adafri-0.0.19.2/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.19.1/setup.py` & `adafri-0.0.19.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.19.1' 
+VERSION = '0.0.19.2' 
 DESCRIPTION = 'Adafri python module'
 LONG_DESCRIPTION = 'Adafri python module helper'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="adafri",
```

