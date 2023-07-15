# Comparing `tmp/pydaraja-0.1.2.tar.gz` & `tmp/pydaraja-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydaraja-0.1.2.tar", last modified: Mon Jul 10 02:43:14 2023, max compression
+gzip compressed data, was "pydaraja-0.2.0.tar", last modified: Sat Jul 15 04:11:35 2023, max compression
```

## Comparing `pydaraja-0.1.2.tar` & `pydaraja-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:43:14.045783 pydaraja-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-10 02:43:02.000000 pydaraja-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-10 02:43:14.041782 pydaraja-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-10 02:43:02.000000 pydaraja-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:43:14.041782 pydaraja-0.1.2/pydaraja/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 02:43:02.000000 pydaraja-0.1.2/pydaraja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 02:43:02.000000 pydaraja-0.1.2/pydaraja/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-10 02:43:02.000000 pydaraja-0.1.2/pydaraja/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-10 02:43:02.000000 pydaraja-0.1.2/pydaraja/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 02:43:14.041782 pydaraja-0.1.2/pydaraja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-10 02:43:14.000000 pydaraja-0.1.2/pydaraja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-10 02:43:14.000000 pydaraja-0.1.2/pydaraja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 02:43:14.000000 pydaraja-0.1.2/pydaraja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 02:43:14.000000 pydaraja-0.1.2/pydaraja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 02:43:14.000000 pydaraja-0.1.2/pydaraja.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-10 02:43:02.000000 pydaraja-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 02:43:14.045783 pydaraja-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:11:35.342929 pydaraja-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-15 04:11:19.000000 pydaraja-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-15 04:11:35.342929 pydaraja-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-15 04:11:19.000000 pydaraja-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:11:35.342929 pydaraja-0.2.0/pydaraja/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 04:11:19.000000 pydaraja-0.2.0/pydaraja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-15 04:11:19.000000 pydaraja-0.2.0/pydaraja/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 04:11:19.000000 pydaraja-0.2.0/pydaraja/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-15 04:11:19.000000 pydaraja-0.2.0/pydaraja/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-15 04:11:19.000000 pydaraja-0.2.0/pydaraja/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:11:35.342929 pydaraja-0.2.0/pydaraja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-07-15 04:11:35.000000 pydaraja-0.2.0/pydaraja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-15 04:11:35.000000 pydaraja-0.2.0/pydaraja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 04:11:35.000000 pydaraja-0.2.0/pydaraja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-15 04:11:35.000000 pydaraja-0.2.0/pydaraja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 04:11:35.000000 pydaraja-0.2.0/pydaraja.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-15 04:11:19.000000 pydaraja-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 04:11:35.342929 pydaraja-0.2.0/setup.cfg
```

### Comparing `pydaraja-0.1.2/LICENSE` & `pydaraja-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydaraja-0.1.2/pydaraja/utils.py` & `pydaraja-0.2.0/pydaraja/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 
 import base64
 import re
 from datetime import datetime
 
 import requests
 
-from pydaraja import payment
+from pydaraja import config
 
 
 def _generate_access_token() -> str:
     """Generate an OAuth access token"""
     access_token_url = "https://sandbox.safaricom.co.ke/oauth/v1/generate?grant_type=client_credentials"
     response = requests.get(
         access_token_url,
-        auth=(payment.CONSUMER_KEY, payment.CONSUMER_SECRET),
+        auth=(config.CONSUMER_KEY, config.CONSUMER_SECRET),
         timeout=30,
     )
     access_token = response.json()["access_token"]
     return access_token
 
 
 def _generate_password() -> str:
     """Generates mpesa api password using the provided shortcode and passkey"""
 
     timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
-    password_str = payment.BUSINESS_SHORTCODE + payment.PASSKEY + timestamp
+    password_str = config.BUSINESS_SHORTCODE + config.PASSKEY + timestamp
     password_bytes = password_str.encode("ascii")
     return base64.b64encode(password_bytes).decode("utf-8")
 
 
 def _validate_phone_number(phone_number: str) -> None:
     """Validate phone number"""
```

