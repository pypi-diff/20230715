# Comparing `tmp/pyroostermoney-0.0.1.tar.gz` & `tmp/pyroostermoney-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroostermoney-0.0.1.tar", last modified: Fri Jul 14 15:39:02 2023, max compression
+gzip compressed data, was "pyroostermoney-0.0.2.tar", last modified: Fri Jul 14 22:17:44 2023, max compression
```

## Comparing `pyroostermoney-0.0.1.tar` & `pyroostermoney-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:39:02.859916 pyroostermoney-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:39:02.855916 pyroostermoney-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:39:02.859916 pyroostermoney-0.0.1/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-14 15:38:51.000000 pyroostermoney-0.0.1/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:39:02.859916 pyroostermoney-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-14 15:38:51.000000 pyroostermoney-0.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-14 15:38:51.000000 pyroostermoney-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-14 15:38:51.000000 pyroostermoney-0.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-14 15:38:51.000000 pyroostermoney-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 15:38:51.000000 pyroostermoney-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-14 15:39:02.859916 pyroostermoney-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-14 15:38:51.000000 pyroostermoney-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:39:02.859916 pyroostermoney-0.0.1/pyroostermoney/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-14 15:38:51.000000 pyroostermoney-0.0.1/pyroostermoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-14 15:38:51.000000 pyroostermoney-0.0.1/pyroostermoney/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:39:02.859916 pyroostermoney-0.0.1/pyroostermoney/services/
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-07-14 15:38:51.000000 pyroostermoney-0.0.1/pyroostermoney/services/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-14 15:38:51.000000 pyroostermoney-0.0.1/pyroostermoney/services/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-14 15:38:51.000000 pyroostermoney-0.0.1/pyroostermoney/services/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 15:39:02.859916 pyroostermoney-0.0.1/pyroostermoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-14 15:39:02.000000 pyroostermoney-0.0.1/pyroostermoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-14 15:39:02.000000 pyroostermoney-0.0.1/pyroostermoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 15:39:02.000000 pyroostermoney-0.0.1/pyroostermoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 15:39:02.000000 pyroostermoney-0.0.1/pyroostermoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 15:39:02.000000 pyroostermoney-0.0.1/pyroostermoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-14 15:38:51.000000 pyroostermoney-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-14 15:39:02.859916 pyroostermoney-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-14 15:38:51.000000 pyroostermoney-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:17:44.219524 pyroostermoney-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:17:44.215524 pyroostermoney-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:17:44.219524 pyroostermoney-0.0.2/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:17:44.219524 pyroostermoney-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-14 22:17:44.219524 pyroostermoney-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:17:44.219524 pyroostermoney-0.0.2/pyroostermoney/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/pyroostermoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/pyroostermoney/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:17:44.219524 pyroostermoney-0.0.2/pyroostermoney/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/pyroostermoney/services/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/pyroostermoney/services/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/pyroostermoney/services/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/pyroostermoney/services/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:17:44.219524 pyroostermoney-0.0.2/pyroostermoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-14 22:17:44.000000 pyroostermoney-0.0.2/pyroostermoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-14 22:17:44.000000 pyroostermoney-0.0.2/pyroostermoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:17:44.000000 pyroostermoney-0.0.2/pyroostermoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 22:17:44.000000 pyroostermoney-0.0.2/pyroostermoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 22:17:44.000000 pyroostermoney-0.0.2/pyroostermoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-14 22:17:44.219524 pyroostermoney-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-14 22:17:35.000000 pyroostermoney-0.0.2/setup.py
```

### Comparing `pyroostermoney-0.0.1/.github/scripts/release.py` & `pyroostermoney-0.0.2/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.0.1/.github/workflows/build.yml` & `pyroostermoney-0.0.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.0.1/.gitignore` & `pyroostermoney-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.0.1/LICENSE` & `pyroostermoney-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.0.1/PKG-INFO` & `pyroostermoney-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.0.1
+Version: 0.0.2
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.0.1/pyroostermoney/__init__.py` & `pyroostermoney-0.0.2/pyroostermoney/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 
 from .services.login import ParentLoginManager
 from .services.session import SessionManager
 from .const import DEFAULT_BANK_NAME, DEFAULT_BANK_TYPE
 
 class RoosterMoney():
 
+    def __init__(self) -> None:
+        self.account = None
+        self.session = None
+
     def login(self, username, password):
+        """Starts a session to Rooster Money and logs into the API."""
         self.account = ParentLoginManager(username, password)
-        try:
-            self.session = SessionManager(self.account)
-        except:
-            raise ConnectionError("Error.")
+        self.session = SessionManager(self.account)
 
     def account_info(self):
         return self.session.requests.account_info()
     
     def request_update(self):
         self.session._update()
```

### Comparing `pyroostermoney-0.0.1/pyroostermoney/services/api.py` & `pyroostermoney-0.0.2/pyroostermoney/services/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Rooster Money API services."""
 import json
 from types import SimpleNamespace
 import requests
-from pyroostermoney.const import COUNTRY, LANGUAGE, CURRENCY, TIMEZONE, TIMEZONE_ID, BASE_URL
+from pyroostermoney.const import COUNTRY, LANGUAGE, CURRENCY, TIMEZONE, TIMEZONE_ID, BASE_URL, MOBILE_APP_VERSION
+from pyroostermoney.services.errors import InvalidAuthError
 
 HEADERS = {
     "content-type": "application/json",
     "accept": "application/json"
 }
 
 LOGIN_BODY={
@@ -28,15 +29,15 @@
     "adyenAPIVersion": "v67",
     "amount": {
         "currency": CURRENCY,
         "value": 0
     },
     "browserInfo": {
         "acceptHeader": "application/json",
-        "userAgent": "Mozilla/5.0 Rooster Money 10.3.0"
+        "userAgent": f"Mozilla/5.0 Rooster Money {MOBILE_APP_VERSION}"
     },
     "channel": "Android",
     "countryCode": COUNTRY.upper(),
     "isPreAuth": False,
     "paymentMethod": {
         "encryptedCardNumber": "",
         "encryptedExpiryMonth": "",
@@ -84,14 +85,17 @@
 
         r = s.post(
             url=f"{BASE_URL}v1/parent",
             headers=HEADERS,
             json=b
         )
 
+        if r.status_code == 401:
+            raise InvalidAuthError(username, r.status_code)
+
         RequestsHandler._ensure_success(RequestsHandler._is_success(r.status_code))
 
         return json.loads(r.content, object_hook=lambda d: SimpleNamespace(**d))
 
     def account_info(self) -> object:
         """Returns account information (/parent)"""
         r = self.s.get(
```

### Comparing `pyroostermoney-0.0.1/pyroostermoney/services/login.py` & `pyroostermoney-0.0.2/pyroostermoney/services/login.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.0.1/pyroostermoney/services/session.py` & `pyroostermoney-0.0.2/pyroostermoney/services/session.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.0.1/pyroostermoney.egg-info/PKG-INFO` & `pyroostermoney-0.0.2/pyroostermoney.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.0.1
+Version: 0.0.2
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.0.1/pyroostermoney.egg-info/SOURCES.txt` & `pyroostermoney-0.0.2/pyroostermoney.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 pyroostermoney/const.py
 pyroostermoney.egg-info/PKG-INFO
 pyroostermoney.egg-info/SOURCES.txt
 pyroostermoney.egg-info/dependency_links.txt
 pyroostermoney.egg-info/requires.txt
 pyroostermoney.egg-info/top_level.txt
 pyroostermoney/services/api.py
+pyroostermoney/services/errors.py
 pyroostermoney/services/login.py
 pyroostermoney/services/session.py
```

