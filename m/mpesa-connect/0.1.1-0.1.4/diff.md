# Comparing `tmp/mpesa_connect-0.1.1.tar.gz` & `tmp/mpesa_connect-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpesa_connect-0.1.1.tar", max compression
+gzip compressed data, was "mpesa_connect-0.1.4.tar", max compression
```

## Comparing `mpesa_connect-0.1.1.tar` & `mpesa_connect-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1213 2023-01-27 14:14:16.039133 mpesa_connect-0.1.1/.env.example
--rw-r--r--   0        0        0      162 2023-01-31 11:09:00.682687 mpesa_connect-0.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1068 2023-01-27 21:27:52.883082 mpesa_connect-0.1.1/LICENSE
--rw-r--r--   0        0        0     4476 2023-02-04 15:14:49.760053 mpesa_connect-0.1.1/README.md
--rw-r--r--   0        0        0     1099 2023-02-08 19:35:05.342150 mpesa_connect-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      396 2023-02-03 11:30:17.755253 mpesa_connect-0.1.1/src/mpesa_connect/__init__.py
--rw-r--r--   0        0        0     1448 2023-02-01 10:32:49.312697 mpesa_connect-0.1.1/src/mpesa_connect/account_balance.py
--rw-r--r--   0        0        0      796 2023-01-25 16:02:31.229824 mpesa_connect-0.1.1/src/mpesa_connect/app.py
--rw-r--r--   0        0        0      561 2023-01-25 20:56:44.992227 mpesa_connect-0.1.1/src/mpesa_connect/authorization.py
--rw-r--r--   0        0        0     1396 2023-01-27 13:30:13.595890 mpesa_connect-0.1.1/src/mpesa_connect/b2c.py
--rw-r--r--   0        0        0     1911 2023-01-26 15:09:53.428732 mpesa_connect-0.1.1/src/mpesa_connect/base.py
--rw-r--r--   0        0        0     2096 2023-01-25 21:33:39.437252 mpesa_connect-0.1.1/src/mpesa_connect/c2b.py
--rw-r--r--   0        0        0      560 2023-01-23 21:30:25.255138 mpesa_connect-0.1.1/src/mpesa_connect/enums.py
--rw-r--r--   0        0        0        0 2023-02-08 19:29:41.617927 mpesa_connect-0.1.1/src/mpesa_connect/py.typed
--rw-r--r--   0        0        0     3360 2023-01-25 21:32:58.831940 mpesa_connect-0.1.1/src/mpesa_connect/stk_push.py
--rw-r--r--   0        0        0     1639 2023-01-27 14:07:04.201797 mpesa_connect-0.1.1/src/mpesa_connect/transaction_status.py
--rw-r--r--   0        0        0      723 2023-01-26 15:06:40.753044 mpesa_connect-0.1.1/src/mpesa_connect/urls.py
--rw-r--r--   0        0        0      571 2023-01-25 20:04:34.631613 mpesa_connect-0.1.1/src/mpesa_connect/utils.py
--rw-r--r--   0        0        0        0 2023-01-18 14:04:06.592406 mpesa_connect-0.1.1/test/__init__.py
--rw-r--r--   0        0        0     5132 2023-02-04 15:24:20.344902 mpesa_connect-0.1.1/test/test_services.py
--rw-r--r--   0        0        0      541 2023-02-04 15:22:46.243668 mpesa_connect-0.1.1/test/test_utils.py
--rw-r--r--   0        0        0     5423 1970-01-01 00:00:00.000000 mpesa_connect-0.1.1/setup.py
--rw-r--r--   0        0        0     5349 1970-01-01 00:00:00.000000 mpesa_connect-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1213 2023-01-27 14:14:16.039133 mpesa_connect-0.1.4/.env.example
+-rw-r--r--   0        0        0      162 2023-01-31 11:09:00.682687 mpesa_connect-0.1.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1068 2023-01-27 21:27:52.883082 mpesa_connect-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4476 2023-02-04 15:14:49.760053 mpesa_connect-0.1.4/README.md
+-rw-r--r--   0        0        0     1099 2023-07-15 06:05:09.920585 mpesa_connect-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      396 2023-02-03 11:30:17.755253 mpesa_connect-0.1.4/src/mpesa_connect/__init__.py
+-rw-r--r--   0        0        0     1448 2023-02-01 10:32:49.312697 mpesa_connect-0.1.4/src/mpesa_connect/account_balance.py
+-rw-r--r--   0        0        0      873 2023-03-17 06:05:45.124186 mpesa_connect-0.1.4/src/mpesa_connect/app.py
+-rw-r--r--   0        0        0      643 2023-07-15 06:04:49.881319 mpesa_connect-0.1.4/src/mpesa_connect/authorization.py
+-rw-r--r--   0        0        0     1396 2023-01-27 13:30:13.595890 mpesa_connect-0.1.4/src/mpesa_connect/b2c.py
+-rw-r--r--   0        0        0     1911 2023-01-26 15:09:53.428732 mpesa_connect-0.1.4/src/mpesa_connect/base.py
+-rw-r--r--   0        0        0     2096 2023-01-25 21:33:39.437252 mpesa_connect-0.1.4/src/mpesa_connect/c2b.py
+-rw-r--r--   0        0        0      560 2023-01-23 21:30:25.255138 mpesa_connect-0.1.4/src/mpesa_connect/enums.py
+-rw-r--r--   0        0        0        0 2023-02-08 19:29:41.617927 mpesa_connect-0.1.4/src/mpesa_connect/py.typed
+-rw-r--r--   0        0        0     3447 2023-03-05 19:09:52.933094 mpesa_connect-0.1.4/src/mpesa_connect/stk_push.py
+-rw-r--r--   0        0        0     1639 2023-01-27 14:07:04.201797 mpesa_connect-0.1.4/src/mpesa_connect/transaction_status.py
+-rw-r--r--   0        0        0      723 2023-01-26 15:06:40.753044 mpesa_connect-0.1.4/src/mpesa_connect/urls.py
+-rw-r--r--   0        0        0      571 2023-01-25 20:04:34.631613 mpesa_connect-0.1.4/src/mpesa_connect/utils.py
+-rw-r--r--   0        0        0        0 2023-01-18 14:04:06.592406 mpesa_connect-0.1.4/test/__init__.py
+-rw-r--r--   0        0        0     5132 2023-02-04 15:24:20.344902 mpesa_connect-0.1.4/test/test_services.py
+-rw-r--r--   0        0        0      541 2023-02-04 15:22:46.243668 mpesa_connect-0.1.4/test/test_utils.py
+-rw-r--r--   0        0        0     5349 1970-01-01 00:00:00.000000 mpesa_connect-0.1.4/PKG-INFO
```

### Comparing `mpesa_connect-0.1.1/.env.example` & `mpesa_connect-0.1.4/.env.example`

 * *Files identical despite different names*

### Comparing `mpesa_connect-0.1.1/LICENSE` & `mpesa_connect-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mpesa_connect-0.1.1/README.md` & `mpesa_connect-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mpesa_connect-0.1.1/pyproject.toml` & `mpesa_connect-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpesa-connect"
-version = "0.1.1"
+version = "0.1.4"
 description = "A wrapper library for the Daraja Mpesa API"
 authors = ["Emz D <seaworndrift@gmail.com>"]
 homepage = "https://github.com/enwawerueli/mpesa-connect"
 repository = "https://github.com/enwawerueli/mpesa-connect"
 license = "MIT"
 readme = "README.md"
 packages = [
```

### Comparing `mpesa_connect-0.1.1/src/mpesa_connect/account_balance.py` & `mpesa_connect-0.1.4/src/mpesa_connect/account_balance.py`

 * *Files identical despite different names*

### Comparing `mpesa_connect-0.1.1/src/mpesa_connect/app.py` & `mpesa_connect-0.1.4/src/mpesa_connect/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from typing import Any
+from typing import Any, Union
 from enum import Enum
 
 from .urls import DOMAIN_PRODUCTION, DOMAIN_SANDBOX
 
 
 class AppDomain(Enum):
     SANDBOX = DOMAIN_SANDBOX
     PRODUCTION = DOMAIN_PRODUCTION
 
 
 class App:
     def __init__(
         self,
         *,
-        domain: AppDomain,
+        domain: Union[AppDomain, str],
         consumer_key: str,
         consumer_secret: str,
     ) -> None:
-        self.domain = domain
+        self.domain = AppDomain[domain.upper()] if isinstance(domain, str) else domain
         self.consumer_key = consumer_key
         self.consumer_secret = consumer_secret
 
     @property
     def base_url(self) -> str:
         return self.domain.value
```

### Comparing `mpesa_connect-0.1.1/src/mpesa_connect/authorization.py` & `mpesa_connect-0.1.4/src/mpesa_connect/authorization.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from typing import Any
 from urllib.parse import urljoin
 
 import requests
 
+from .app import App
 from .base import Service
 from .urls import PATH_OAUTH_GENERATE
 from .utils import base64encode
 
 
 class Authorization(Service):
+    def __init__(self, app: App, /):
+        self.app = app
+
     def generate_token(self) -> Any:
         credentials = base64encode(
             f"{self.app.consumer_key}:{self.app.consumer_secret}"
         )
         response = requests.get(
             urljoin(self.app.base_url, PATH_OAUTH_GENERATE),
             headers={"Authorization": f"Basic {credentials}"},
```

### Comparing `mpesa_connect-0.1.1/src/mpesa_connect/b2c.py` & `mpesa_connect-0.1.4/src/mpesa_connect/b2c.py`

 * *Files identical despite different names*

### Comparing `mpesa_connect-0.1.1/src/mpesa_connect/base.py` & `mpesa_connect-0.1.4/src/mpesa_connect/base.py`

 * *Files identical despite different names*

### Comparing `mpesa_connect-0.1.1/src/mpesa_connect/c2b.py` & `mpesa_connect-0.1.4/src/mpesa_connect/c2b.py`

 * *Files identical despite different names*

### Comparing `mpesa_connect-0.1.1/src/mpesa_connect/enums.py` & `mpesa_connect-0.1.4/src/mpesa_connect/enums.py`

 * *Files identical despite different names*

### Comparing `mpesa_connect-0.1.1/src/mpesa_connect/stk_push.py` & `mpesa_connect-0.1.4/src/mpesa_connect/stk_push.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,17 @@
         *,
         business_short_code: int,
         amount: int,
         phone_number: int,
         call_back_url: str,
         account_reference: str,
         transaction_desc: str,
-        transaction_type: Optional[Union[TransactionType, str]] = None,
+        transaction_type: Union[
+            TransactionType, str
+        ] = TransactionType.CUSTOMER_PAY_BILL_ONLINE,
         party_a: Optional[str] = None,
         party_b: Optional[str] = None,
         password: Optional[str] = None,
         timestamp: Optional[str] = None,
         pass_key: Optional[str] = None,
         access_token: Optional[str] = None,
     ) -> Any:
@@ -33,16 +35,17 @@
                 pass_key,
                 timestamp,
             )
         payload = {
             "BusinessShortCode": business_short_code,
             "Password": password,
             "Timestamp": timestamp,
-            "TransactionType": transaction_type
-            or TransactionType.CUSTOMER_PAY_BILL_ONLINE.value,
+            "TransactionType": transaction_type.value
+            if isinstance(transaction_type, TransactionType)
+            else transaction_type,
             "Amount": amount,
             "PartyA": party_a or phone_number,
             "PartyB": party_b or business_short_code,
             "PhoneNumber": phone_number,
             "CallBackURL": call_back_url,
             "AccountReference": account_reference,
             "TransactionDesc": transaction_desc,
```

### Comparing `mpesa_connect-0.1.1/src/mpesa_connect/transaction_status.py` & `mpesa_connect-0.1.4/src/mpesa_connect/transaction_status.py`

 * *Files identical despite different names*

### Comparing `mpesa_connect-0.1.1/src/mpesa_connect/urls.py` & `mpesa_connect-0.1.4/src/mpesa_connect/urls.py`

 * *Files identical despite different names*

### Comparing `mpesa_connect-0.1.1/src/mpesa_connect/utils.py` & `mpesa_connect-0.1.4/src/mpesa_connect/utils.py`

 * *Files identical despite different names*

### Comparing `mpesa_connect-0.1.1/test/test_services.py` & `mpesa_connect-0.1.4/test/test_services.py`

 * *Files identical despite different names*

### Comparing `mpesa_connect-0.1.1/test/test_utils.py` & `mpesa_connect-0.1.4/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `mpesa_connect-0.1.1/PKG-INFO` & `mpesa_connect-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpesa-connect
-Version: 0.1.1
+Version: 0.1.4
 Summary: A wrapper library for the Daraja Mpesa API
 Home-page: https://github.com/enwawerueli/mpesa-connect
 License: MIT
 Keywords: daraja,mpesa,payment
 Author: Emz D
 Author-email: seaworndrift@gmail.com
 Requires-Python: >=3.8,<4.0
```

