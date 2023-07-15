# Comparing `tmp/betfair_parser-0.4.5.tar.gz` & `tmp/betfair_parser-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betfair_parser-0.4.5.tar", max compression
+gzip compressed data, was "betfair_parser-0.4.6.tar", max compression
```

## Comparing `betfair_parser-0.4.5.tar` & `betfair_parser-0.4.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1286 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/LICENSE.txt
--rw-r--r--   0        0        0     3277 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/README.md
--rw-r--r--   0        0        0        0 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/__init__.py
--rw-r--r--   0        0        0     2090 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/client.py
--rw-r--r--   0        0        0     2417 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/endpoints.py
--rw-r--r--   0        0        0      741 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/__init__.py
--rw-r--r--   0        0        0       85 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/accounts/__init__.py
--rw-r--r--   0        0        0     2929 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/accounts/enums.py
--rw-r--r--   0        0        0     3278 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/accounts/operations.py
--rw-r--r--   0        0        0    11161 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/accounts/type_definitions.py
--rw-r--r--   0        0        0       84 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/betting/__init__.py
--rw-r--r--   0        0        0    21951 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/betting/enums.py
--rw-r--r--   0        0        0     9634 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/betting/listings.py
--rw-r--r--   0        0        0      134 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/betting/operations.py
--rw-r--r--   0        0        0     8860 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/betting/orders.py
--rw-r--r--   0        0        0    32923 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/betting/type_definitions.py
--rw-r--r--   0        0        0      238 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/common/__init__.py
--rw-r--r--   0        0        0     9771 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/common/enums.py
--rw-r--r--   0        0        0     4829 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/common/messages.py
--rw-r--r--   0        0        0     1493 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/common/type_definitions.py
--rw-r--r--   0        0        0     2773 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/heartbeat.py
--rw-r--r--   0        0        0     8653 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/identity.py
--rw-r--r--   0        0        0     3645 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/navigation.py
--rw-r--r--   0        0        0     3172 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/race_status.py
--rw-r--r--   0        0        0      399 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/streaming/__init__.py
--rw-r--r--   0        0        0     5989 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/streaming/mcm.py
--rw-r--r--   0        0        0     2247 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/streaming/ocm.py
--rw-r--r--   0        0        0     2507 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/streaming/status.py
--rw-r--r--   0        0        0     2319 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/strenums.py
--rw-r--r--   0        0        0      760 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/util.py
--rw-r--r--   0        0        0     1712 2023-07-15 06:48:38.713019 betfair_parser-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     3726 1970-01-01 00:00:00.000000 betfair_parser-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1286 2023-07-15 06:52:24.248659 betfair_parser-0.4.6/LICENSE.txt
+-rw-r--r--   0        0        0     3277 2023-07-15 06:52:24.248659 betfair_parser-0.4.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-15 06:52:24.248659 betfair_parser-0.4.6/betfair_parser/__init__.py
+-rw-r--r--   0        0        0     2090 2023-07-15 06:52:24.248659 betfair_parser-0.4.6/betfair_parser/client.py
+-rw-r--r--   0        0        0     2417 2023-07-15 06:52:24.248659 betfair_parser-0.4.6/betfair_parser/endpoints.py
+-rw-r--r--   0        0        0      741 2023-07-15 06:52:24.248659 betfair_parser-0.4.6/betfair_parser/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-15 06:52:24.248659 betfair_parser-0.4.6/betfair_parser/spec/__init__.py
+-rw-r--r--   0        0        0       85 2023-07-15 06:52:24.248659 betfair_parser-0.4.6/betfair_parser/spec/accounts/__init__.py
+-rw-r--r--   0        0        0     2929 2023-07-15 06:52:24.248659 betfair_parser-0.4.6/betfair_parser/spec/accounts/enums.py
+-rw-r--r--   0        0        0     3278 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/accounts/operations.py
+-rw-r--r--   0        0        0    11161 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/accounts/type_definitions.py
+-rw-r--r--   0        0        0       84 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/betting/__init__.py
+-rw-r--r--   0        0        0    21951 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/betting/enums.py
+-rw-r--r--   0        0        0     9634 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/betting/listings.py
+-rw-r--r--   0        0        0      134 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/betting/operations.py
+-rw-r--r--   0        0        0     8860 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/betting/orders.py
+-rw-r--r--   0        0        0    32923 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/betting/type_definitions.py
+-rw-r--r--   0        0        0      238 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/common/__init__.py
+-rw-r--r--   0        0        0     9771 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/common/enums.py
+-rw-r--r--   0        0        0     4829 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/common/messages.py
+-rw-r--r--   0        0        0     1493 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/common/type_definitions.py
+-rw-r--r--   0        0        0     2773 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/heartbeat.py
+-rw-r--r--   0        0        0     8653 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/identity.py
+-rw-r--r--   0        0        0     3645 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/navigation.py
+-rw-r--r--   0        0        0     3172 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/race_status.py
+-rw-r--r--   0        0        0      399 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/streaming/__init__.py
+-rw-r--r--   0        0        0     5989 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/streaming/mcm.py
+-rw-r--r--   0        0        0     2247 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/streaming/ocm.py
+-rw-r--r--   0        0        0     2507 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/spec/streaming/status.py
+-rw-r--r--   0        0        0     2319 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/strenums.py
+-rw-r--r--   0        0        0      760 2023-07-15 06:52:24.252659 betfair_parser-0.4.6/betfair_parser/util.py
+-rw-r--r--   0        0        0     1712 2023-07-15 06:52:38.880624 betfair_parser-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     3726 1970-01-01 00:00:00.000000 betfair_parser-0.4.6/PKG-INFO
```

### Comparing `betfair_parser-0.4.5/LICENSE.txt` & `betfair_parser-0.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/README.md` & `betfair_parser-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/client.py` & `betfair_parser-0.4.6/betfair_parser/client.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/endpoints.py` & `betfair_parser-0.4.6/betfair_parser/endpoints.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/exceptions.py` & `betfair_parser-0.4.6/betfair_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/spec/accounts/enums.py` & `betfair_parser-0.4.6/betfair_parser/spec/accounts/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/spec/accounts/operations.py` & `betfair_parser-0.4.6/betfair_parser/spec/accounts/operations.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/spec/accounts/type_definitions.py` & `betfair_parser-0.4.6/betfair_parser/spec/accounts/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/spec/betting/enums.py` & `betfair_parser-0.4.6/betfair_parser/spec/betting/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/spec/betting/listings.py` & `betfair_parser-0.4.6/betfair_parser/spec/betting/listings.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/spec/betting/orders.py` & `betfair_parser-0.4.6/betfair_parser/spec/betting/orders.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/spec/betting/type_definitions.py` & `betfair_parser-0.4.6/betfair_parser/spec/betting/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/spec/common/enums.py` & `betfair_parser-0.4.6/betfair_parser/spec/common/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/spec/common/messages.py` & `betfair_parser-0.4.6/betfair_parser/spec/common/messages.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/spec/common/type_definitions.py` & `betfair_parser-0.4.6/betfair_parser/spec/common/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/spec/heartbeat.py` & `betfair_parser-0.4.6/betfair_parser/spec/heartbeat.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/spec/identity.py` & `betfair_parser-0.4.6/betfair_parser/spec/identity.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/spec/navigation.py` & `betfair_parser-0.4.6/betfair_parser/spec/navigation.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/spec/race_status.py` & `betfair_parser-0.4.6/betfair_parser/spec/race_status.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/spec/streaming/mcm.py` & `betfair_parser-0.4.6/betfair_parser/spec/streaming/mcm.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/spec/streaming/ocm.py` & `betfair_parser-0.4.6/betfair_parser/spec/streaming/ocm.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/spec/streaming/status.py` & `betfair_parser-0.4.6/betfair_parser/spec/streaming/status.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/strenums.py` & `betfair_parser-0.4.6/betfair_parser/strenums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/betfair_parser/util.py` & `betfair_parser-0.4.6/betfair_parser/util.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.5/pyproject.toml` & `betfair_parser-0.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "betfair_parser"
-version = "0.4.5"
+version = "0.4.6"
 description = "A betfair parser"
 readme = "README.md"
 authors = ["Bradley McElroy <bradley.mcelroy@live.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 msgspec = ">=0.16"
```

### Comparing `betfair_parser-0.4.5/PKG-INFO` & `betfair_parser-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betfair-parser
-Version: 0.4.5
+Version: 0.4.6
 Summary: A betfair parser
 Author: Bradley McElroy
 Author-email: bradley.mcelroy@live.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

