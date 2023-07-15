# Comparing `tmp/pyroostermoney-0.1.0.tar.gz` & `tmp/pyroostermoney-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroostermoney-0.1.0.tar", last modified: Sat Jul 15 21:27:21 2023, max compression
+gzip compressed data, was "pyroostermoney-0.1.1.tar", last modified: Sat Jul 15 21:49:56 2023, max compression
```

## Comparing `pyroostermoney-0.1.0.tar` & `pyroostermoney-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:27:21.334201 pyroostermoney-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:27:21.330201 pyroostermoney-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:27:21.334201 pyroostermoney-0.1.0/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:27:21.334201 pyroostermoney-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-15 21:27:21.334201 pyroostermoney-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:27:21.334201 pyroostermoney-0.1.0/pyroostermoney/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/pyroostermoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/pyroostermoney/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:27:21.334201 pyroostermoney-0.1.0/pyroostermoney/child/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/pyroostermoney/child/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/pyroostermoney/child/child.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/pyroostermoney/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/pyroostermoney/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/pyroostermoney/roostermoney.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:27:21.334201 pyroostermoney-0.1.0/pyroostermoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-15 21:27:21.000000 pyroostermoney-0.1.0/pyroostermoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-15 21:27:21.000000 pyroostermoney-0.1.0/pyroostermoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 21:27:21.000000 pyroostermoney-0.1.0/pyroostermoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 21:27:21.000000 pyroostermoney-0.1.0/pyroostermoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-15 21:27:21.000000 pyroostermoney-0.1.0/pyroostermoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-15 21:27:21.334201 pyroostermoney-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-15 21:27:07.000000 pyroostermoney-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:49:56.385661 pyroostermoney-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:49:56.385661 pyroostermoney-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:49:56.385661 pyroostermoney-0.1.1/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:49:56.385661 pyroostermoney-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-15 21:49:56.389661 pyroostermoney-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:49:56.385661 pyroostermoney-0.1.1/pyroostermoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/pyroostermoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/pyroostermoney/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:49:56.385661 pyroostermoney-0.1.1/pyroostermoney/child/
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/pyroostermoney/child/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/pyroostermoney/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/pyroostermoney/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/pyroostermoney/roostermoney.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:49:56.385661 pyroostermoney-0.1.1/pyroostermoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-15 21:49:56.000000 pyroostermoney-0.1.1/pyroostermoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-15 21:49:56.000000 pyroostermoney-0.1.1/pyroostermoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 21:49:56.000000 pyroostermoney-0.1.1/pyroostermoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 21:49:56.000000 pyroostermoney-0.1.1/pyroostermoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-15 21:49:56.000000 pyroostermoney-0.1.1/pyroostermoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-15 21:49:56.389661 pyroostermoney-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-15 21:49:45.000000 pyroostermoney-0.1.1/setup.py
```

### Comparing `pyroostermoney-0.1.0/.github/scripts/release.py` & `pyroostermoney-0.1.1/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.0/.github/workflows/build.yml` & `pyroostermoney-0.1.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.0/.gitignore` & `pyroostermoney-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.0/LICENSE` & `pyroostermoney-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.0/PKG-INFO` & `pyroostermoney-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.1.0
+Version: 0.1.1
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.1.0/pyroostermoney/api.py` & `pyroostermoney-0.1.1/pyroostermoney/api.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.0/pyroostermoney/child/child.py` & `pyroostermoney-0.1.1/pyroostermoney/child/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-"""The main child account class and further actions."""
+"""Defines some standard values for a Natwest Rooster Money child."""
 
 import datetime
 
 from pyroostermoney.const import URLS
 from pyroostermoney.api import RoosterSession
 
 class ChildAccount:
     """The child account."""
 
     def __init__(self, raw_response: dict, session: RoosterSession) -> None:
-        raw_response = raw_response["response"]
+        if "response" in raw_response:
+            raw_response = raw_response["response"]
         self.interest_rate = raw_response["interestRate"]
         self.available_pocket_money = raw_response["availablePocketMoney"]
         self.currency = raw_response["currency"]
         self.first_name = raw_response["firstName"]
         self.surname = raw_response["surname"]
         self.gender = "male" if raw_response["gender"] == 1 else "female"
         self.uses_real_money = True if raw_response["realMoneyStatus"] == 1 else False
```

### Comparing `pyroostermoney-0.1.0/pyroostermoney/const.py` & `pyroostermoney-0.1.1/pyroostermoney/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Static Rooster Money variables"""
 
-VERSION="0.1.0"
+VERSION="0.1.1"
 BASE_URL="https://api.rooster.money"
 LANGUAGE="en-GB"
 COUNTRY="gb"
 CURRENCY="GBP"
 TIMEZONE_ID=60
 TIMEZONE="GMT+01:00"
 DEFAULT_PRECISION=2
```

### Comparing `pyroostermoney-0.1.0/pyroostermoney/exceptions.py` & `pyroostermoney-0.1.1/pyroostermoney/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.1.0/pyroostermoney/roostermoney.py` & `pyroostermoney-0.1.1/pyroostermoney/roostermoney.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,23 @@
 
     def __init__(self, username: str, password: str) -> None:
         super().__init__(
             username=username,
             password=password
         )
 
+    async def get_children(self) -> list[ChildAccount]:
+        """Returns a list of available children."""
+        account_info = await self.get_account_info()
+        children = account_info["response"]["children"]
+        output = []
+        for child in children:
+            output.append(ChildAccount(child, self))
+        return output
+
     async def get_account_info(self) -> dict:
         """Returns the account info for the current user."""
         return await self.internal_request_handler(url=URLS.get("get_account_info"))
 
     async def get_child_account(self, user_id) -> ChildAccount:
         """Fetches and returns a given child account details."""
         response = await self.internal_request_handler(
```

### Comparing `pyroostermoney-0.1.0/pyroostermoney.egg-info/PKG-INFO` & `pyroostermoney-0.1.1/pyroostermoney.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.1.0
+Version: 0.1.1
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.1.0/pyroostermoney.egg-info/SOURCES.txt` & `pyroostermoney-0.1.1/pyroostermoney.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,9 +14,8 @@
 pyroostermoney/exceptions.py
 pyroostermoney/roostermoney.py
 pyroostermoney.egg-info/PKG-INFO
 pyroostermoney.egg-info/SOURCES.txt
 pyroostermoney.egg-info/dependency_links.txt
 pyroostermoney.egg-info/requires.txt
 pyroostermoney.egg-info/top_level.txt
-pyroostermoney/child/__init__.py
-pyroostermoney/child/child.py
+pyroostermoney/child/__init__.py
```

