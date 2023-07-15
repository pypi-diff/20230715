# Comparing `tmp/py_dtn7-0.3.0b0.tar.gz` & `tmp/py_dtn7-0.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_dtn7-0.3.0b0.tar", max compression
+gzip compressed data, was "py_dtn7-0.3.0b1.tar", max compression
```

## Comparing `py_dtn7-0.3.0b0.tar` & `py_dtn7-0.3.0b1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    34523 2023-03-31 12:40:40.112697 py_dtn7-0.3.0b0/LICENSE
--rw-r--r--   0        0        0     2311 2023-03-31 12:46:03.969664 py_dtn7-0.3.0b0/README.md
--rw-r--r--   0        0        0      304 2023-07-13 19:43:19.815947 py_dtn7-0.3.0b0/py_dtn7/__init__.py
--rw-r--r--   0        0        0    32831 2023-07-13 19:43:19.816479 py_dtn7-0.3.0b0/py_dtn7/bundle.py
--rw-r--r--   0        0        0     8921 2023-05-29 16:52:47.221225 py_dtn7-0.3.0b0/py_dtn7/dtn_rest_client.py
--rw-r--r--   0        0        0     6436 2023-03-31 12:40:40.113689 py_dtn7-0.3.0b0/py_dtn7/dtn_ws_client.py
--rw-r--r--   0        0        0     1045 2023-03-31 16:48:54.206682 py_dtn7-0.3.0b0/py_dtn7/utils.py
--rw-r--r--   0        0        0     1532 2023-07-13 20:25:38.992007 py_dtn7-0.3.0b0/pyproject.toml
--rw-r--r--   0        0        0     3455 1970-01-01 00:00:00.000000 py_dtn7-0.3.0b0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-03-31 12:40:40.112697 py_dtn7-0.3.0b1/LICENSE
+-rw-r--r--   0        0        0     2311 2023-03-31 12:46:03.969664 py_dtn7-0.3.0b1/README.md
+-rw-r--r--   0        0        0      304 2023-07-15 20:16:27.473163 py_dtn7-0.3.0b1/py_dtn7/__init__.py
+-rw-r--r--   0        0        0    32672 2023-07-15 20:14:08.863076 py_dtn7-0.3.0b1/py_dtn7/bundle.py
+-rw-r--r--   0        0        0     8921 2023-05-29 16:52:47.221225 py_dtn7-0.3.0b1/py_dtn7/dtn_rest_client.py
+-rw-r--r--   0        0        0     6436 2023-03-31 12:40:40.113689 py_dtn7-0.3.0b1/py_dtn7/dtn_ws_client.py
+-rw-r--r--   0        0        0     1045 2023-03-31 16:48:54.206682 py_dtn7-0.3.0b1/py_dtn7/utils.py
+-rw-r--r--   0        0        0     1532 2023-07-15 20:16:34.356838 py_dtn7-0.3.0b1/pyproject.toml
+-rw-r--r--   0        0        0     3455 1970-01-01 00:00:00.000000 py_dtn7-0.3.0b1/PKG-INFO
```

### Comparing `py_dtn7-0.3.0b0/LICENSE` & `py_dtn7-0.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `py_dtn7-0.3.0b0/README.md` & `py_dtn7-0.3.0b1/README.md`

 * *Files identical despite different names*

### Comparing `py_dtn7-0.3.0b0/py_dtn7/bundle.py` & `py_dtn7-0.3.0b1/py_dtn7/bundle.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # for postponed evaluation of annotation of Bundle.from_cbor()
 # more info: https://stackoverflow.com/a/33533514
 from __future__ import annotations
 
 from datetime import datetime
-from typing import Optional, List, Self, Tuple, Union
+from typing import Optional, List, Tuple, Union
 
 from py_dtn7.utils import from_dtn_timestamp, RUNNING_MICROPYTHON
 
 if not RUNNING_MICROPYTHON:
     from cbor2 import dumps, loads
 else:
     from cbor import dumps, loads
@@ -314,15 +314,15 @@
             "source_specific_part",
             "report_to_scheme",
             "report_to_specific_part",
             "bundle_creation_time",
             "sequence_number",
             "lifetime",
         ]
-        return all([self.__getattribute__(attr) == other.__getattribute__(attr) for attr in attrs])
+        return all(getattr(self, attr) == getattr(other, attr) for attr in attrs)
 
     @staticmethod
     def from_block_data(primary_block: list) -> PrimaryBlock:
         """
         length of array may be:
             8 if the bundle is not a fragment and has no CRC,
             9 if the bundle is not a fragment and has a CRC,
@@ -416,15 +416,15 @@
         elif 255 <= scheme <= 65535:
             raise ValueError("bundle uses reserved uri scheme {}".format(scheme))
         elif scheme > 65535:
             raise ValueError("bundle uses unknown private uri scheme {}".format(scheme))
 
     @staticmethod
     def from_full_uri(full_uri: str) -> Tuple[int, Union[str, int, List[int]]]:
-        scheme, specific_part = full_uri.split(sep=":", maxsplit=1)
+        scheme, specific_part = full_uri.split(":", 1)
 
         if scheme == URI_SCHEME_DTN_NAME:
             if specific_part == NONE_ENDPOINT_SPECIFIC_PART_NAME:
                 specific_part = NONE_ENDPOINT_SPECIFIC_PART_ENCODED
 
             return URI_SCHEME_DTN_ENCODED, specific_part
         elif scheme == URI_SCHEME_IPN_NAME:
@@ -520,15 +520,15 @@
         attrs = [
             "block_type_code",
             "block_number",
             "block_processing_control_flags",
             "crc_type",
             "data",
         ]
-        return all([self.__getattribute__(attr) == other.__getattribute__(attr) for attr in attrs])
+        return all(getattr(self, attr) == getattr(other, attr) for attr in attrs)
 
     @classmethod
     def from_block_data(cls, block: list) -> CanonicalBlock:
         # todo: move checks to init
 
         """
         length of the array may be:
@@ -787,21 +787,15 @@
             PreviousNodeBlock: "previous_node_block",
             BundleAgeBlock: "bundle_age_block",
             HopCountBlock: "hop_count_block",
             PayloadBlock: "payload_block",
             CanonicalBlock: "other_blocks",
         }
 
-        for block in [
-            previous_node_block,
-            bundle_age_block,
-            hop_count_block,
-            payload_block,
-            *other_blocks,
-        ]:
+        for block in (previous_node_block, bundle_age_block, hop_count_block, payload_block) + tuple(other_blocks):
             if block is not None:
                 self.insert_canonical_block(block)
 
         if self.primary_block.bundle_creation_time == 0 and self.bundle_age_block is None:
             raise ValueError("No bundle age block given, although creation time is zero")
 
     @staticmethod
@@ -920,17 +914,15 @@
             "payload_block",
             # other_blocks needs to be handled seperately
         ]
         # other_blocks have to be the same but not in the same order
         other_equal = all(b in other.other_blocks for b in self.other_blocks) and all(
             b in self.other_blocks for b in other.other_blocks
         )
-        return other_equal and all(
-            [self.__getattribute__(attr) == other.__getattribute__(attr) for attr in attrs]
-        )
+        return other_equal and all(getattr(self, attr) == getattr(other, attr) for attr in attrs)
 
     def _get_all_used_canonical_blocks(self):
         all_canonical_blocks = (
             self.previous_node_block,
             self.bundle_age_block,
             self.hop_count_block,
             self.payload_block,
```

### Comparing `py_dtn7-0.3.0b0/py_dtn7/dtn_rest_client.py` & `py_dtn7-0.3.0b1/py_dtn7/dtn_rest_client.py`

 * *Files identical despite different names*

### Comparing `py_dtn7-0.3.0b0/py_dtn7/dtn_ws_client.py` & `py_dtn7-0.3.0b1/py_dtn7/dtn_ws_client.py`

 * *Files identical despite different names*

### Comparing `py_dtn7-0.3.0b0/py_dtn7/utils.py` & `py_dtn7-0.3.0b1/py_dtn7/utils.py`

 * *Files identical despite different names*

### Comparing `py_dtn7-0.3.0b0/pyproject.toml` & `py_dtn7-0.3.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-dtn7"
-version = "0.3.0b0"
+version = "0.3.0b1"
 description = ""
 authors = [
     "Lukas Holst <lh700@proton.me>",
     "Thomas Schmitt <t.e.schmitt@posteo.de>",
 ]
 
 license = "AGPL-3.0-or-later"
```

### Comparing `py_dtn7-0.3.0b0/PKG-INFO` & `py_dtn7-0.3.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-dtn7
-Version: 0.3.0b0
+Version: 0.3.0b1
 Summary: 
 Home-page: https://github.com/teschmitt/py-dtn7
 License: AGPL-3.0-or-later
 Author: Lukas Holst
 Author-email: lh700@proton.me
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

