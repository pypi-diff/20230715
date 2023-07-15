# Comparing `tmp/betfair_parser-0.4.4.tar.gz` & `tmp/betfair_parser-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betfair_parser-0.4.4.tar", max compression
+gzip compressed data, was "betfair_parser-0.4.5.tar", max compression
```

## Comparing `betfair_parser-0.4.4.tar` & `betfair_parser-0.4.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1286 2023-06-26 20:38:03.031096 betfair_parser-0.4.4/LICENSE.txt
--rw-r--r--   0        0        0     3277 2023-06-26 20:38:03.031096 betfair_parser-0.4.4/README.md
--rw-r--r--   0        0        0        0 2023-06-26 20:38:03.031096 betfair_parser-0.4.4/betfair_parser/__init__.py
--rw-r--r--   0        0        0     2090 2023-06-26 20:38:03.031096 betfair_parser-0.4.4/betfair_parser/client.py
--rw-r--r--   0        0        0     2417 2023-06-26 20:38:03.031096 betfair_parser-0.4.4/betfair_parser/endpoints.py
--rw-r--r--   0        0        0      741 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/__init__.py
--rw-r--r--   0        0        0       85 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/accounts/__init__.py
--rw-r--r--   0        0        0     2929 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/accounts/enums.py
--rw-r--r--   0        0        0     3278 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/accounts/operations.py
--rw-r--r--   0        0        0    11161 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/accounts/type_definitions.py
--rw-r--r--   0        0        0       84 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/betting/__init__.py
--rw-r--r--   0        0        0    21951 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/betting/enums.py
--rw-r--r--   0        0        0     9634 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/betting/listings.py
--rw-r--r--   0        0        0      134 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/betting/operations.py
--rw-r--r--   0        0        0     8860 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/betting/orders.py
--rw-r--r--   0        0        0    32923 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/betting/type_definitions.py
--rw-r--r--   0        0        0      238 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/common/__init__.py
--rw-r--r--   0        0        0     9771 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/common/enums.py
--rw-r--r--   0        0        0     4829 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/common/messages.py
--rw-r--r--   0        0        0     1493 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/common/type_definitions.py
--rw-r--r--   0        0        0     2773 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/heartbeat.py
--rw-r--r--   0        0        0     8653 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/identity.py
--rw-r--r--   0        0        0     3645 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/navigation.py
--rw-r--r--   0        0        0     3172 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/race_status.py
--rw-r--r--   0        0        0      399 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/streaming/__init__.py
--rw-r--r--   0        0        0     5989 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/streaming/mcm.py
--rw-r--r--   0        0        0     2247 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/streaming/ocm.py
--rw-r--r--   0        0        0     2507 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/spec/streaming/status.py
--rw-r--r--   0        0        0     2319 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/strenums.py
--rw-r--r--   0        0        0      902 2023-06-26 20:38:03.035096 betfair_parser-0.4.4/betfair_parser/util.py
--rw-r--r--   0        0        0     1731 2023-06-26 20:38:23.011106 betfair_parser-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 betfair_parser-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1286 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/LICENSE.txt
+-rw-r--r--   0        0        0     3277 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/README.md
+-rw-r--r--   0        0        0        0 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/__init__.py
+-rw-r--r--   0        0        0     2090 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/client.py
+-rw-r--r--   0        0        0     2417 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/endpoints.py
+-rw-r--r--   0        0        0      741 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/__init__.py
+-rw-r--r--   0        0        0       85 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/accounts/__init__.py
+-rw-r--r--   0        0        0     2929 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/accounts/enums.py
+-rw-r--r--   0        0        0     3278 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/accounts/operations.py
+-rw-r--r--   0        0        0    11161 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/accounts/type_definitions.py
+-rw-r--r--   0        0        0       84 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/betting/__init__.py
+-rw-r--r--   0        0        0    21951 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/betting/enums.py
+-rw-r--r--   0        0        0     9634 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/betting/listings.py
+-rw-r--r--   0        0        0      134 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/betting/operations.py
+-rw-r--r--   0        0        0     8860 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/betting/orders.py
+-rw-r--r--   0        0        0    32923 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/betting/type_definitions.py
+-rw-r--r--   0        0        0      238 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/common/__init__.py
+-rw-r--r--   0        0        0     9771 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/common/enums.py
+-rw-r--r--   0        0        0     4829 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/common/messages.py
+-rw-r--r--   0        0        0     1493 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/common/type_definitions.py
+-rw-r--r--   0        0        0     2773 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/heartbeat.py
+-rw-r--r--   0        0        0     8653 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/identity.py
+-rw-r--r--   0        0        0     3645 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/navigation.py
+-rw-r--r--   0        0        0     3172 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/race_status.py
+-rw-r--r--   0        0        0      399 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/streaming/__init__.py
+-rw-r--r--   0        0        0     5989 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/streaming/mcm.py
+-rw-r--r--   0        0        0     2247 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/streaming/ocm.py
+-rw-r--r--   0        0        0     2507 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/spec/streaming/status.py
+-rw-r--r--   0        0        0     2319 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/strenums.py
+-rw-r--r--   0        0        0      760 2023-07-15 06:48:19.576725 betfair_parser-0.4.5/betfair_parser/util.py
+-rw-r--r--   0        0        0     1712 2023-07-15 06:48:38.713019 betfair_parser-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     3726 1970-01-01 00:00:00.000000 betfair_parser-0.4.5/PKG-INFO
```

### Comparing `betfair_parser-0.4.4/LICENSE.txt` & `betfair_parser-0.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/README.md` & `betfair_parser-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/client.py` & `betfair_parser-0.4.5/betfair_parser/client.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/endpoints.py` & `betfair_parser-0.4.5/betfair_parser/endpoints.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/exceptions.py` & `betfair_parser-0.4.5/betfair_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/spec/accounts/enums.py` & `betfair_parser-0.4.5/betfair_parser/spec/accounts/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/spec/accounts/operations.py` & `betfair_parser-0.4.5/betfair_parser/spec/accounts/operations.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/spec/accounts/type_definitions.py` & `betfair_parser-0.4.5/betfair_parser/spec/accounts/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/spec/betting/enums.py` & `betfair_parser-0.4.5/betfair_parser/spec/betting/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         "to process the bet but please allow up to 15 seconds for a timed out order to appear. After this "
         "time any unprocessed bets will automatically be Lapsed and no longer be available on the Exchange."
     )
 
 
 class ExecutionReportErrorCode(DocumentedEnum):
     ERROR_IN_MATCHER = doc(
-        "The matcher is not healthy. Please note: The error will also be returned is you attempt concurrent "
+        "The matcher is not healthy. Please note: The error will also be returned if you attempt concurrent "
         "'cancel all' bets requests using cancelOrders which isn't permitted."
     )
     PROCESSED_WITH_ERRORS = doc(
         "The order itself has been accepted, but at least one (possibly all) actions have generated errors."
     )
     BET_ACTION_ERROR = doc(
         "There is an error with an action that has caused the entire order to be rejected. Check the "
```

### Comparing `betfair_parser-0.4.4/betfair_parser/spec/betting/listings.py` & `betfair_parser-0.4.5/betfair_parser/spec/betting/listings.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/spec/betting/orders.py` & `betfair_parser-0.4.5/betfair_parser/spec/betting/orders.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/spec/betting/type_definitions.py` & `betfair_parser-0.4.5/betfair_parser/spec/betting/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/spec/common/enums.py` & `betfair_parser-0.4.5/betfair_parser/spec/common/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/spec/common/messages.py` & `betfair_parser-0.4.5/betfair_parser/spec/common/messages.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/spec/common/type_definitions.py` & `betfair_parser-0.4.5/betfair_parser/spec/common/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/spec/heartbeat.py` & `betfair_parser-0.4.5/betfair_parser/spec/heartbeat.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/spec/identity.py` & `betfair_parser-0.4.5/betfair_parser/spec/identity.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/spec/navigation.py` & `betfair_parser-0.4.5/betfair_parser/spec/navigation.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/spec/race_status.py` & `betfair_parser-0.4.5/betfair_parser/spec/race_status.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/spec/streaming/mcm.py` & `betfair_parser-0.4.5/betfair_parser/spec/streaming/mcm.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/spec/streaming/ocm.py` & `betfair_parser-0.4.5/betfair_parser/spec/streaming/ocm.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/spec/streaming/status.py` & `betfair_parser-0.4.5/betfair_parser/spec/streaming/status.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/strenums.py` & `betfair_parser-0.4.5/betfair_parser/strenums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.4.4/betfair_parser/util.py` & `betfair_parser-0.4.5/betfair_parser/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 import bz2
 import tarfile
 import typing
 
-import fsspec
 import msgspec
 
 from betfair_parser.spec.streaming import stream_decode
 
 
-def iter_file(fsspec_url: str):
-    with fsspec.open(fsspec_url, compression="infer") as f:
-        yield from iter_stream(f)
-
-
 def iter_tar_file(tar_file: str, file_path: str):
     tf = tarfile.open(tar_file)
     assert file_path in tf.getnames(), f"Can't find `{file_path}` in {tf.getnames()[:5]}... "
     f = tf.extractfile(file_path)
     assert f is not None
     if file_path.endswith("bz2"):
         f = bz2.open(f)
```

### Comparing `betfair_parser-0.4.4/pyproject.toml` & `betfair_parser-0.4.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -37,23 +37,22 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "betfair_parser"
-version = "0.4.4"
+version = "0.4.5"
 description = "A betfair parser"
 readme = "README.md"
 authors = ["Bradley McElroy <bradley.mcelroy@live.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-msgspec = "^0.16.0"
-fsspec = ">=2022"
+msgspec = ">=0.16"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1"
 pytest-benchmark = "^4.0"
 requests = "^2.20"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `betfair_parser-0.4.4/PKG-INFO` & `betfair_parser-0.4.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: betfair-parser
-Version: 0.4.4
+Version: 0.4.5
 Summary: A betfair parser
 Author: Bradley McElroy
 Author-email: bradley.mcelroy@live.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fsspec (>=2022)
-Requires-Dist: msgspec (>=0.16.0,<0.17.0)
+Requires-Dist: msgspec (>=0.16)
 Description-Content-Type: text/markdown
 
 [![GitHub Build Status](https://img.shields.io/github/actions/workflow/status/limx0/betfair_parser/build.yml?branch=main&logo=github)](https://github.com/limx0/betfair_parser/actions)
 [![PyPI](https://img.shields.io/pypi/v/betfair_parser.svg?style=flat)](https://pypi.org/project/betfair_parser/)
 ![Python Version](https://img.shields.io/pypi/pyversions/betfair_parser)
 ![License](https://img.shields.io/github/license/limx0/betfair_parser)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

