# Comparing `tmp/vtype-1.1.2.tar.gz` & `tmp/vtype-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtype-1.1.2.tar", last modified: Fri Jul 14 17:49:46 2023, max compression
+gzip compressed data, was "vtype-1.1.3.tar", last modified: Sat Jul 15 15:51:18 2023, max compression
```

## Comparing `vtype-1.1.2.tar` & `vtype-1.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11036 2023-07-14 17:01:09.601742 vtype-1.1.2/LICENSE
--rw-r--r--   0        0        0      426 2023-07-14 16:35:39.816109 vtype-1.1.2/README.md
--rw-r--r--   0        0        0      521 2023-07-14 17:49:46.433367 vtype-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      145 2023-07-13 08:30:36.887445 vtype-1.1.2/vtype/__init__.py
--rw-r--r--   0        0        0    10283 2023-07-14 17:14:22.785588 vtype-1.1.2/vtype/_core.py
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 vtype-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11036 2023-07-14 17:01:09.601742 vtype-1.1.3/LICENSE
+-rw-r--r--   0        0        0      426 2023-07-14 16:35:39.816109 vtype-1.1.3/README.md
+-rw-r--r--   0        0        0      521 2023-07-15 15:51:17.796729 vtype-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-07-15 10:01:07.545479 vtype-1.1.3/vtype/__init__.py
+-rw-r--r--   0        0        0    11852 2023-07-15 10:00:57.374543 vtype-1.1.3/vtype/_core.py
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 vtype-1.1.3/PKG-INFO
```

### Comparing `vtype-1.1.2/LICENSE` & `vtype-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vtype-1.1.2/pyproject.toml` & `vtype-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "vtype"
-version = "1.1.2"
+version = "1.1.3"
 description = "一些自定义的数据类型"
 dependencies = []
 keywords = ["vtype"]
 
 readme = "README.md"
 authors = [{name = "lcctoor.com", email = "lcctoor@outlook.com"}]
 license = {file = "LICENSE"}
```

### Comparing `vtype-1.1.2/vtype/_core.py` & `vtype-1.1.3/vtype/_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import re
 from math import ceil
 from collections import deque
 import hashlib
 from hashlib import shake_256
 from fractions import Fraction
-from typing import Any
+from typing import Any, List, Union
 
 
 class missing_arguments_error(Exception): ...
 
 
 ########################################## vbool ##########################################
 
@@ -306,8 +306,62 @@
     def beforeGet(self, obj): return obj
     def beforePut(self, obj): return obj
 
 
 class OrmIndexError(IndexError):
     # 供 coolmysql、coolmongo、asymysql、asymongo 调用
     def __repr__(self):
-        return 'OrmIndexError'
+        return 'OrmIndexError'
+
+
+class _CoolQueue:
+    ''' 一个先进先出, 可设置最大容量, 可固定元素的队列 '''
+
+    def __init__(self, maxlen: int=None):
+        self._core: List[dict] = []
+        self.maxlen = maxlen or float('inf')
+
+    def _trim(self):
+        _core = self._core
+        if len(_core) > self.maxlen:
+            dc = len(_core) - self.maxlen
+            indexes = []
+            for i,x in enumerate(_core):
+                if not x['pin']:
+                    indexes.append(i)
+                if len(indexes) == dc:
+                    break
+            for i in indexes[::-1]:
+                _core.pop(i)
+
+    def add_many(self, *objs):
+        for x in objs:
+            self._core.append({'obj':x, 'pin':False})
+        self._trim()
+
+    def __iter__(self):
+        for x in self._core:
+            yield x['obj']
+
+    def pin(self, *indexes):
+        for i in indexes:
+            self._core[i]['pin'] = True
+
+    def unpin(self, *indexes):
+        for i in indexes:
+            self._core[i]['pin'] = False
+
+    def copy(self):
+        que = self.__class__(maxlen=self.maxlen)
+        que._core = self._core.copy()
+        return que
+    
+    def deepcopy(self): ...  # 创建这个方法是为了提醒用户: copy 方法是浅拷贝
+
+    def __add__(self, obj: Union[list, '_CoolQueue']):
+        que = self.copy()
+        if isinstance(obj, self.__class__):
+            que._core += obj._core
+            que._trim()
+        else:
+            que.add_many(*obj)
+        return que
```

### Comparing `vtype-1.1.2/PKG-INFO` & `vtype-1.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtype
-Version: 1.1.2
+Version: 1.1.3
 Summary: 一些自定义的数据类型
 Keywords: vtype
 Author-email: "lcctoor.com" <lcctoor@outlook.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: HomePage, https://lcctoor.github.io/lccpy/?package=vtype
```

