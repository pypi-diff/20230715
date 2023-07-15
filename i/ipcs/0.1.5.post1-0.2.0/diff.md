# Comparing `tmp/ipcs-0.1.5.post1.tar.gz` & `tmp/ipcs-0.2.0.tar.gz`

## Comparing `ipcs-0.1.5.post1.tar` & `ipcs-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/CONTRIBUTING.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/mypy.ini
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/test.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/.github/dependabot.yml
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/.venv/.gitignore
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/docs/conf.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/docs/event_reference.rst
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/docs/index.rst
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/docs/ipcs.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/docs/modules.rst
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/docs/requirements.txt
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/examples/chat.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/examples/readme.md
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/src/ipcs/__init__.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/src/ipcs/__main__.py
--rw-r--r--   0        0        0    19183 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/src/ipcs/client.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/src/ipcs/connection.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/src/ipcs/errors.py
--rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/src/ipcs/server.py
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/src/ipcs/types_.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/src/ipcs/utils.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/LICENSE
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/README.md
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/pyproject.toml
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 ipcs-0.1.5.post1/PKG-INFO
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 ipcs-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ipcs-0.2.0/mypy.ini
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipcs-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ipcs-0.2.0/.venv/.gitignore
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 ipcs-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 ipcs-0.2.0/docs/event_reference.rst
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 ipcs-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 ipcs-0.2.0/docs/ipcs.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 ipcs-0.2.0/docs/modules.rst
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 ipcs-0.2.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ipcs-0.2.0/examples/chat_room/chat.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 ipcs-0.2.0/examples/chat_room/readme.md
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 ipcs-0.2.0/src/ipcs/__init__.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 ipcs-0.2.0/src/ipcs/__main__.py
+-rw-r--r--   0        0        0    19115 2020-02-02 00:00:00.000000 ipcs-0.2.0/src/ipcs/client.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 ipcs-0.2.0/src/ipcs/connection.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 ipcs-0.2.0/src/ipcs/errors.py
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 ipcs-0.2.0/src/ipcs/server.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 ipcs-0.2.0/src/ipcs/types_.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 ipcs-0.2.0/src/ipcs/utils.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 ipcs-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ipcs-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 ipcs-0.2.0/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 ipcs-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 ipcs-0.2.0/PKG-INFO
```

### Comparing `ipcs-0.1.5.post1/docs/conf.py` & `ipcs-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5.post1/docs/event_reference.rst` & `ipcs-0.2.0/docs/event_reference.rst`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5.post1/docs/index.rst` & `ipcs-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5.post1/docs/ipcs.rst` & `ipcs-0.2.0/docs/ipcs.rst`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5.post1/examples/chat.py` & `ipcs-0.2.0/examples/chat_room/chat.py`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5.post1/src/ipcs/__main__.py` & `ipcs-0.2.0/src/ipcs/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from argparse import ArgumentParser
 import logging
 
 try:
-    from ipcs import __version__, Server, Request
-    from ipcs.client import logger
+    from ipcs import __version__, Server, Request, logger
 except ImportError:
     from sys import path as spath
     spath.insert(0, __file__[:-17])
-    from ipcs import __version__, Server, Request
-    from ipcs.client import logger
+    from ipcs import __version__, Server, Request, logger
 
 
 logger.setLevel(logging.INFO)
 handler = logging.StreamHandler()
 handler.setFormatter(logging.Formatter("[%(name)s] [%(levelname)s] %(message)s"))
 logger.addHandler(handler)
```

### Comparing `ipcs-0.1.5.post1/src/ipcs/client.py` & `ipcs-0.2.0/src/ipcs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 
 from .types_ import RequestPayload, ResponsePayload, WebSocketProtocol
 from .errors import IdIsNotFound, RequestError
 from .utils import SimpleAttrDict, error_to_str, payload_to_str
 from .connection import Connection
 
 
-logger = getLogger("ipcs")
-"Log output destination. ipcs use logging from the standard library."
+logger = getLogger(__name__)
 
 
 def _debug():
     import logging
     handler = logging.StreamHandler()
     handler.setFormatter(logging.Formatter("[%(name)s] [%(levelname)s] %(message)s"))
     logging.basicConfig(level=logging.DEBUG, handlers=(handler,))
```

### Comparing `ipcs-0.1.5.post1/src/ipcs/connection.py` & `ipcs-0.2.0/src/ipcs/connection.py`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5.post1/src/ipcs/errors.py` & `ipcs-0.2.0/src/ipcs/errors.py`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5.post1/src/ipcs/server.py` & `ipcs-0.2.0/src/ipcs/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-__all__ = ("ConnectionForServer", "Server")
+__all__ = ("ConnectionForServer", "Server", "logger")
 
 from typing import Any
 
 from asyncio import Future
+from logging import getLogger
 
 from websockets.exceptions import ConnectionClosed
 from websockets.server import serve
 
 from orjson import loads, dumps
 
 from .types_ import WebSocketProtocol, RequestPayload, ResponsePayload
 from .utils import payload_to_str
 from .connection import Connection
-from .client import AbcClient, logger
+from .client import AbcClient
+
+
+logger = getLogger(__name__)
 
 
 class ConnectionForServer(Connection):
     """Class that extends :class:`Connection` for :class:`Server`.
 
     Args:
         ws: This is the websocket to the client connected by this connection."""
```

### Comparing `ipcs-0.1.5.post1/src/ipcs/types_.py` & `ipcs-0.2.0/src/ipcs/types_.py`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5.post1/src/ipcs/utils.py` & `ipcs-0.2.0/src/ipcs/utils.py`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5.post1/LICENSE` & `ipcs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5.post1/README.md` & `ipcs-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ipcs-0.1.5.post1/pyproject.toml` & `ipcs-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ipcs"
-version = "0.1.5.post1"
+version = "0.2.0"
 description = "Simple IPC server/client"
 keywords = ["ipc", "networking"]
 license = "MIT"
 readme = "README.md"
 license-files = { paths = ["LICENSE"] }
 classifiers = [
     "Programming Language :: Python :: 3.11",
@@ -13,15 +13,15 @@
 ]
 authors = [
     { name = "Takagi Tasuku", email = "tasuren@outlook.jp" }
 ]
 requires-python = ">= 3.10"
 dependencies = [
     "websockets~=11.0.3",
-    "orjson~=3.9.1",
+    "orjson~=3.9.2",
 ]
 
 [project.urls]
 Source = "https://github.com/tasuren/ipcs"
 Documentation = "https://ipcs.readthedocs.io/"
 Donate = "https://www.buymeacoffee.com/tasuren"
 Chat = "https://discord.gg/kfMwZUyGFG"
```

### Comparing `ipcs-0.1.5.post1/PKG-INFO` & `ipcs-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ipcs
-Version: 0.1.5.post1
+Version: 0.2.0
 Summary: Simple IPC server/client
 Project-URL: Source, https://github.com/tasuren/ipcs
 Project-URL: Documentation, https://ipcs.readthedocs.io/
 Project-URL: Donate, https://www.buymeacoffee.com/tasuren
 Project-URL: Chat, https://discord.gg/kfMwZUyGFG
 Author-email: Takagi Tasuku <tasuren@outlook.jp>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ipc,networking
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
-Requires-Dist: orjson~=3.9.1
+Requires-Dist: orjson~=3.9.2
 Requires-Dist: websockets~=11.0.3
 Description-Content-Type: text/markdown
 
 [![PyPI](https://img.shields.io/pypi/v/ipcs)](https://pypi.org/project/ipcs/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ipcs) ![PyPI - Downloads](https://img.shields.io/pypi/dm/ipcs) ![PyPI - License](https://img.shields.io/pypi/l/ipcs) [![Documentation Status](https://readthedocs.org/projects/ipcs/badge/?version=latest)](https://ipcs.readthedocs.io/en/latest/?badge=latest) [![Buy Me a Coffee](https://img.shields.io/badge/-tasuren-E9EEF3?label=Buy%20Me%20a%20Coffee&logo=buymeacoffee)](https://www.buymeacoffee.com/tasuren)
 # ipcs
 A library for Python for IPC.  
 (Although it is written as IPC, it can also be used for communication with an external server.)
```

