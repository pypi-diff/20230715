# Comparing `tmp/huma_utils-0.3.0.tar.gz` & `tmp/huma_utils-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huma_utils-0.3.0.tar", max compression
+gzip compressed data, was "huma_utils-0.4.0.tar", max compression
```

## Comparing `huma_utils-0.3.0.tar` & `huma_utils-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1063 2023-06-16 22:38:13.882538 huma_utils-0.3.0/LICENSE
--rw-r--r--   0        0        0       35 2023-06-16 22:38:13.882538 huma_utils-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/__init__.py
--rw-r--r--   0        0        0      291 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/chain_utils.py
--rw-r--r--   0        0        0      330 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/datetime_utils.py
--rw-r--r--   0        0        0        0 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/py.typed
--rw-r--r--   0        0        0      428 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/pydantic_utils.py
--rw-r--r--   0        0        0      702 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/request_utils.py
--rw-r--r--   0        0        0     1113 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/string_utils.py
--rw-r--r--   0        0        0      543 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/test_helpers/address_helpers.py
--rw-r--r--   0        0        0      809 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/test_helpers/api_test_helpers.py
--rw-r--r--   0        0        0     2042 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/test_helpers/vcr_helpers.py
--rw-r--r--   0        0        0     1129 2023-06-16 22:38:13.882538 huma_utils-0.3.0/huma_utils/web3_utils.py
--rw-r--r--   0        0        0     2240 2023-06-16 22:38:13.886538 huma_utils-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 huma_utils-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-15 00:26:44.760374 huma_utils-0.4.0/LICENSE
+-rw-r--r--   0        0        0       35 2023-07-15 00:26:44.760374 huma_utils-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/__init__.py
+-rw-r--r--   0        0        0      270 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/async_utils.py
+-rw-r--r--   0        0        0      291 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/chain_utils.py
+-rw-r--r--   0        0        0      330 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/datetime_utils.py
+-rw-r--r--   0        0        0        0 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/py.typed
+-rw-r--r--   0        0        0      428 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/pydantic_utils.py
+-rw-r--r--   0        0        0      702 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/request_utils.py
+-rw-r--r--   0        0        0     1113 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/string_utils.py
+-rw-r--r--   0        0        0      543 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/test_helpers/address_helpers.py
+-rw-r--r--   0        0        0      809 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/test_helpers/api_test_helpers.py
+-rw-r--r--   0        0        0     2042 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/test_helpers/vcr_helpers.py
+-rw-r--r--   0        0        0     1129 2023-07-15 00:26:44.760374 huma_utils-0.4.0/huma_utils/web3_utils.py
+-rw-r--r--   0        0        0     2269 2023-07-15 00:26:44.764374 huma_utils-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 huma_utils-0.4.0/PKG-INFO
```

### Comparing `huma_utils-0.3.0/LICENSE` & `huma_utils-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `huma_utils-0.3.0/huma_utils/request_utils.py` & `huma_utils-0.4.0/huma_utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.3.0/huma_utils/string_utils.py` & `huma_utils-0.4.0/huma_utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.3.0/huma_utils/test_helpers/address_helpers.py` & `huma_utils-0.4.0/huma_utils/test_helpers/address_helpers.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.3.0/huma_utils/test_helpers/api_test_helpers.py` & `huma_utils-0.4.0/huma_utils/test_helpers/api_test_helpers.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.3.0/huma_utils/test_helpers/vcr_helpers.py` & `huma_utils-0.4.0/huma_utils/test_helpers/vcr_helpers.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.3.0/huma_utils/web3_utils.py` & `huma_utils-0.4.0/huma_utils/web3_utils.py`

 * *Files identical despite different names*

### Comparing `huma_utils-0.3.0/pyproject.toml` & `huma_utils-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "huma-utils"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
-authors = ["flowers-huang <flora221@stanford.edu>"]
+authors = ["Flora Huang <flora@huma.finance>", "Jiatu Liu <jiatu@huma.finance>"]
 readme = "README.md"
 packages = [{include = "huma_utils"}]
 
 [tool.poetry.dependencies]
 python = "~3.10"
 httpx = "^0.24.1"
 orjson = "^3.9.1"
```

