# Comparing `tmp/dynamic-sh-0.0.4.tar.gz` & `tmp/dynamic-sh-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamic-sh-0.0.4.tar", last modified: Wed Jul 12 22:00:24 2023, max compression
+gzip compressed data, was "dynamic-sh-0.0.5.tar", last modified: Sat Jul 15 14:39:38 2023, max compression
```

## Comparing `dynamic-sh-0.0.4.tar` & `dynamic-sh-0.0.5.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 22:00:24.375376 dynamic-sh-0.0.4/
--rw-r--r--   0 omarwaseem   (501) staff       (20)      654 2023-07-12 22:00:24.375256 dynamic-sh-0.0.4/PKG-INFO
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/README.md
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 22:00:24.371747 dynamic-sh-0.0.4/dynamic/
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1400 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/dynamic/__init__.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 22:00:24.372555 dynamic-sh-0.0.4/dynamic/classes/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/dynamic/classes/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1280 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/dynamic/classes/agent.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      133 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/dynamic/classes/chain.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      245 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/dynamic/classes/logger.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1289 2023-07-11 18:24:11.000000 dynamic-sh-0.0.4/dynamic/classes/message.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 22:00:24.373041 dynamic-sh-0.0.4/dynamic/protocols/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/dynamic/protocols/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)    10102 2023-07-11 18:24:11.000000 dynamic-sh-0.0.4/dynamic/protocols/server.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1419 2023-07-11 18:24:11.000000 dynamic-sh-0.0.4/dynamic/protocols/ws.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 22:00:24.373197 dynamic-sh-0.0.4/dynamic/request/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/dynamic/request/__init__.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 22:00:24.373272 dynamic-sh-0.0.4/dynamic/response/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/dynamic/response/__init__.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 22:00:24.373597 dynamic-sh-0.0.4/dynamic/router/
--rw-r--r--   0 omarwaseem   (501) staff       (20)       47 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/dynamic/router/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     2607 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/dynamic/router/get_file_routes.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     2113 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/dynamic/router/router.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 22:00:24.374093 dynamic-sh-0.0.4/dynamic/runners/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-12 21:59:30.000000 dynamic-sh-0.0.4/dynamic/runners/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      603 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/dynamic/runners/callable.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 22:00:24.374627 dynamic-sh-0.0.4/dynamic/runners/langchain/
--rw-r--r--   0 omarwaseem   (501) staff       (20)      174 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/dynamic/runners/langchain/__init__.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1472 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/dynamic/runners/langchain/agent.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      687 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/dynamic/runners/langchain/chain.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      202 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/dynamic/runners/langchain/config.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      316 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/dynamic/runners/runner.py
--rw-r--r--   0 omarwaseem   (501) staff       (20)      847 2023-07-08 22:39:44.000000 dynamic-sh-0.0.4/dynamic/runners/utils.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 22:00:24.374750 dynamic-sh-0.0.4/dynamic/static/
--rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-12 21:59:30.000000 dynamic-sh-0.0.4/dynamic/static/__init__.py
-drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-12 22:00:24.375112 dynamic-sh-0.0.4/dynamic_sh.egg-info/
--rw-r--r--   0 omarwaseem   (501) staff       (20)      654 2023-07-12 22:00:24.000000 dynamic-sh-0.0.4/dynamic_sh.egg-info/PKG-INFO
--rw-r--r--   0 omarwaseem   (501) staff       (20)      823 2023-07-12 22:00:24.000000 dynamic-sh-0.0.4/dynamic_sh.egg-info/SOURCES.txt
--rw-r--r--   0 omarwaseem   (501) staff       (20)        1 2023-07-12 22:00:24.000000 dynamic-sh-0.0.4/dynamic_sh.egg-info/dependency_links.txt
--rw-r--r--   0 omarwaseem   (501) staff       (20)        8 2023-07-12 22:00:24.000000 dynamic-sh-0.0.4/dynamic_sh.egg-info/top_level.txt
--rw-r--r--   0 omarwaseem   (501) staff       (20)      596 2023-07-12 21:59:40.000000 dynamic-sh-0.0.4/pyproject.toml
--rw-r--r--   0 omarwaseem   (501) staff       (20)       38 2023-07-12 22:00:24.375409 dynamic-sh-0.0.4/setup.cfg
--rw-r--r--   0 omarwaseem   (501) staff       (20)     1046 2023-07-12 21:59:36.000000 dynamic-sh-0.0.4/setup.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.151260 dynamic-sh-0.0.5/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      654 2023-07-15 14:39:38.151141 dynamic-sh-0.0.5/PKG-INFO
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     7836 2023-07-15 14:38:48.000000 dynamic-sh-0.0.5/README.md
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.147453 dynamic-sh-0.0.5/dynamic/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)       83 2023-07-15 14:38:48.000000 dynamic-sh-0.0.5/dynamic/__init__.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.148248 dynamic-sh-0.0.5/dynamic/classes/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.5/dynamic/classes/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1331 2023-07-15 14:38:48.000000 dynamic-sh-0.0.5/dynamic/classes/agent.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      133 2023-07-08 22:39:44.000000 dynamic-sh-0.0.5/dynamic/classes/chain.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      245 2023-07-08 22:39:44.000000 dynamic-sh-0.0.5/dynamic/classes/logger.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1289 2023-07-11 18:24:11.000000 dynamic-sh-0.0.5/dynamic/classes/message.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1474 2023-07-15 14:38:48.000000 dynamic-sh-0.0.5/dynamic/decorator.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.148677 dynamic-sh-0.0.5/dynamic/protocols/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.5/dynamic/protocols/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)    10232 2023-07-15 14:38:48.000000 dynamic-sh-0.0.5/dynamic/protocols/server.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1419 2023-07-11 18:24:11.000000 dynamic-sh-0.0.5/dynamic/protocols/ws.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.148947 dynamic-sh-0.0.5/dynamic/request/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.5/dynamic/request/__init__.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.149037 dynamic-sh-0.0.5/dynamic/response/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-08 22:39:44.000000 dynamic-sh-0.0.5/dynamic/response/__init__.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.149486 dynamic-sh-0.0.5/dynamic/router/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)       47 2023-07-08 22:39:44.000000 dynamic-sh-0.0.5/dynamic/router/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     3851 2023-07-15 14:38:48.000000 dynamic-sh-0.0.5/dynamic/router/file_routes_builder.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     2607 2023-07-08 22:39:44.000000 dynamic-sh-0.0.5/dynamic/router/get_file_routes.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     2552 2023-07-15 14:38:48.000000 dynamic-sh-0.0.5/dynamic/router/router.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.149959 dynamic-sh-0.0.5/dynamic/runners/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-12 21:59:30.000000 dynamic-sh-0.0.5/dynamic/runners/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      603 2023-07-08 22:39:44.000000 dynamic-sh-0.0.5/dynamic/runners/callable.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.150485 dynamic-sh-0.0.5/dynamic/runners/langchain/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      174 2023-07-08 22:39:44.000000 dynamic-sh-0.0.5/dynamic/runners/langchain/__init__.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1472 2023-07-08 22:39:44.000000 dynamic-sh-0.0.5/dynamic/runners/langchain/agent.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      687 2023-07-08 22:39:44.000000 dynamic-sh-0.0.5/dynamic/runners/langchain/chain.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      202 2023-07-08 22:39:44.000000 dynamic-sh-0.0.5/dynamic/runners/langchain/config.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      316 2023-07-08 22:39:44.000000 dynamic-sh-0.0.5/dynamic/runners/runner.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      847 2023-07-08 22:39:44.000000 dynamic-sh-0.0.5/dynamic/runners/utils.py
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1378 2023-07-15 14:38:48.000000 dynamic-sh-0.0.5/dynamic/start_server.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.150610 dynamic-sh-0.0.5/dynamic/static/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        0 2023-07-12 21:59:30.000000 dynamic-sh-0.0.5/dynamic/static/__init__.py
+drwxr-xr-x   0 omarwaseem   (501) staff       (20)        0 2023-07-15 14:39:38.150980 dynamic-sh-0.0.5/dynamic_sh.egg-info/
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      654 2023-07-15 14:39:38.000000 dynamic-sh-0.0.5/dynamic_sh.egg-info/PKG-INFO
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      906 2023-07-15 14:39:38.000000 dynamic-sh-0.0.5/dynamic_sh.egg-info/SOURCES.txt
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        1 2023-07-15 14:39:38.000000 dynamic-sh-0.0.5/dynamic_sh.egg-info/dependency_links.txt
+-rw-r--r--   0 omarwaseem   (501) staff       (20)        8 2023-07-15 14:39:38.000000 dynamic-sh-0.0.5/dynamic_sh.egg-info/top_level.txt
+-rw-r--r--   0 omarwaseem   (501) staff       (20)      596 2023-07-15 14:39:20.000000 dynamic-sh-0.0.5/pyproject.toml
+-rw-r--r--   0 omarwaseem   (501) staff       (20)       38 2023-07-15 14:39:38.151296 dynamic-sh-0.0.5/setup.cfg
+-rw-r--r--   0 omarwaseem   (501) staff       (20)     1046 2023-07-15 14:39:16.000000 dynamic-sh-0.0.5/setup.py
```

### Comparing `dynamic-sh-0.0.4/PKG-INFO` & `dynamic-sh-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-sh
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dynamic ⚡ is a new open-source framework that streamlines the process of building production-ready applications with LLMs. Now in beta.
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dynamic-sh-0.0.4/dynamic/__init__.py` & `dynamic-sh-0.0.5/dynamic/start_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import logging
 from typing import Any, List, Optional
 
 from dynamic.classes.logger import setup_logging
 from dynamic.protocols.server import Server
 from dynamic.router import Router, Route
-from dynamic.router.get_file_routes import get_file_routes, has_file_based_routing
+from dynamic.router.file_routes_builder import FileRoutesBuilder
 
 host = os.environ.get("HOST", "0.0.0.0")
 port = int(os.environ.get("PORT", 8000))
 
 
 setup_logging()
 
@@ -20,15 +20,14 @@
         routes: Optional[List[Any]] = None,
         static_dir=None,
         test_ws=False
     ):
     
     router = _handle_router(router, routes)
 
-    logging.info(f"Starting server on {host}:{port}")
     server = Server(router, host=host, port=port, static_dir=static_dir)
     if test_ws:
         server._add_test_ws_html()
     server.start()
 
     return server
 
@@ -40,17 +39,18 @@
                 path=path,
                 handle=handle,
             ) for path, handle in routes.items()
         ]
     else:
         routes = []
 
-    if has_file_based_routing():
+    builder = FileRoutesBuilder()
+    if builder.has_file_based_routing():
         logging.info("Building file based routes...")
-        routes += get_file_routes()
+        routes += builder.get_file_routes()
 
     if router:
         router.routes += routes
     else:
         router = Router(routes=routes)
 
     return router
```

### Comparing `dynamic-sh-0.0.4/dynamic/classes/agent.py` & `dynamic-sh-0.0.5/dynamic/classes/agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 class DynamicAgent:
     def __init__(self, llm, **kwargs):
         self.llm = llm
         self.kwargs = kwargs
 
     def _initialize_agent_with_websocket(self, websocket: WebSocket):
+        # TODO: Minimize the number of agent inits
         logging.info("Setting up streaming settings for agent...")
         llm = self.llm
 
         llm.streaming = True
         llm.verbose = True
         llm.callbacks = [WebsocketCallbackHandler(websocket)]
```

### Comparing `dynamic-sh-0.0.4/dynamic/classes/message.py` & `dynamic-sh-0.0.5/dynamic/classes/message.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.4/dynamic/protocols/server.py` & `dynamic-sh-0.0.5/dynamic/protocols/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,17 @@
     def add_route(self, route: Route) -> None:
         """Dynamically add routes"""
         handle = route.handle
         path = route.path
         runner = route.runner
         runner_config_type = route.runner_config_type
 
+        if route.streaming and route.inline:
+            raise Exception(f"Routes cannot have both streaming=True and inline=True. Offending route: {route.path}, {route.methods}")
+
         async def run_inline_route(req: Request):
             """Non-streaming simple route"""
             # collect data
             data = await req.json()
 
             # setup runner config
             config_dict = data.get("config")
@@ -99,19 +102,19 @@
                 message="Ran inline route successfully!",
                 output=output
             )
         if route.streaming and isinstance(route.handle, DynamicAgent):
             logging.info(f"Adding websocket route {route.path}")
             self.app.websocket(route.path)(self.websocket_handler)
         elif route.inline:
-            logging.info(f"Adding inline route {route.path}")
-            self.app.add_api_route(path, run_inline_route, methods=["GET", "POST"])
+            logging.info(f"Adding inline route {route.path}, methods={route.methods}")
+            self.app.add_api_route(path, run_inline_route, methods=route.methods)
         else:
-            logging.info(f"Adding route {route.path}")
-            self.app.add_api_route(path, handle, methods=["GET", "PUT", "POST", "DELETE"])
+            logging.info(f"Adding route path={route.path}, methods={route.methods}")
+            self.app.add_api_route(path, handle, methods=route.methods)
 
     def start(self):
         logging.info(f"Starting server on host:port {self.host}:{self.port}")
         uvicorn.run(
             self.app,
             host=self.host,
             port=self.port,
@@ -169,15 +172,14 @@
             try:
                 received_json = await websocket.receive_json()
                 incoming_message = ClientMessage(**received_json)
                 logging.info(f"Received message: {incoming_message.to_json_dump()}")
 
                 outgoing_message = await handle_msg(incoming_message)
 
-                logging.info(f"Outgoing message: {outgoing_message.to_json_dump()}")
                 await send_msg(outgoing_message)
 
             except WebSocketDisconnect as e:
                 logging.info("WebSocketDisconnect")
                 self.connection_manager.disconnect(websocket_id)
                 break
             # TODO: Update error messaging
```

### Comparing `dynamic-sh-0.0.4/dynamic/protocols/ws.py` & `dynamic-sh-0.0.5/dynamic/protocols/ws.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.4/dynamic/router/get_file_routes.py` & `dynamic-sh-0.0.5/dynamic/router/get_file_routes.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.4/dynamic/router/router.py` & `dynamic-sh-0.0.5/dynamic/router/router.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,20 +24,22 @@
 }
 
 class Route:
     def __init__(
             self,
             path: str,
             handle: Callable,
+            methods: List[str] = ["GET"],
             inline: bool = False,
             streaming: bool = False,
             route_type: Optional[RouteType] = None,
     ):
         self.path = path
         self.handle = handle
+        self.methods = methods
         self.inline = inline
         self.streaming = streaming
         self.route_type = route_type
 
         self.runner, self.runner_config_type = get_runner(self.handle)
         if route_type:
             assert _ROUTE_TYPE_TO_RUNNER[route_type] == self.runner, f"The route_type set {route_type.value} does not match the runner retrieved via handler, {self.runner}."
@@ -46,27 +48,29 @@
         else:
             self.route_type = _RUNNER_TO_ROUTE_TYPE[self.runner]
 
 
 
 class Router:
     def __init__(self, routes: List[Route] = []):
-        self.routes = []
+        self.routes: List[Route] = []
 
         # error checks routes, duplicate paths are problematic atm
         for route in routes:
             self.add_route(route)
     
-    def get_route(self, path: str) -> Union[Route, None]:
+    def get_route(self, path: str, method: str = "GET") -> Union[Route, None]:
         for route in self.routes:
-            if route.path == path:
+            if route.path == path and (method in route.methods or route.streaming):
                 return route
         
         return None
     
     def add_route(self, route: Route):
-        paths = [r.path for r in self.routes]
-        if route.path in paths:
-            raise Exception(f"Duplicate path found, \"{route.path}\". All routes must have unique path (both http and websocket).")
+        for r in self.routes:
+            overlapping_methods = set(r.methods).intersection(set(route.methods))
+            # the route path is the same and if one the methods already has an existing handler, then raise exception
+            if r.path == route.path and len(overlapping_methods) > 0:
+                raise Exception(f"Duplicate path (\"{route.path}\") + method(s) found, {overlapping_methods}. All incoming routes must have unique path (both http and websocket) and methods.")
 
         self.routes.append(route)
```

### Comparing `dynamic-sh-0.0.4/dynamic/runners/callable.py` & `dynamic-sh-0.0.5/dynamic/runners/callable.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.4/dynamic/runners/langchain/agent.py` & `dynamic-sh-0.0.5/dynamic/runners/langchain/agent.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.4/dynamic/runners/langchain/chain.py` & `dynamic-sh-0.0.5/dynamic/runners/langchain/chain.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.4/dynamic/runners/utils.py` & `dynamic-sh-0.0.5/dynamic/runners/utils.py`

 * *Files identical despite different names*

### Comparing `dynamic-sh-0.0.4/dynamic_sh.egg-info/PKG-INFO` & `dynamic-sh-0.0.5/dynamic_sh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamic-sh
-Version: 0.0.4
+Version: 0.0.5
 Summary: Dynamic ⚡ is a new open-source framework that streamlines the process of building production-ready applications with LLMs. Now in beta.
 Author-email: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `dynamic-sh-0.0.4/dynamic_sh.egg-info/SOURCES.txt` & `dynamic-sh-0.0.5/dynamic_sh.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 README.md
 pyproject.toml
 setup.py
 dynamic/__init__.py
+dynamic/decorator.py
+dynamic/start_server.py
 dynamic/classes/__init__.py
 dynamic/classes/agent.py
 dynamic/classes/chain.py
 dynamic/classes/logger.py
 dynamic/classes/message.py
 dynamic/protocols/__init__.py
 dynamic/protocols/server.py
 dynamic/protocols/ws.py
 dynamic/request/__init__.py
 dynamic/response/__init__.py
 dynamic/router/__init__.py
+dynamic/router/file_routes_builder.py
 dynamic/router/get_file_routes.py
 dynamic/router/router.py
 dynamic/runners/__init__.py
 dynamic/runners/callable.py
 dynamic/runners/runner.py
 dynamic/runners/utils.py
 dynamic/runners/langchain/__init__.py
```

### Comparing `dynamic-sh-0.0.4/pyproject.toml` & `dynamic-sh-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dynamic-sh"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = [
     "Furqan Rydhan <furqan.rydhan@gmail.com>",
     "Aman Ibrahim <amanmibra@gmail.com>"
 ]
 readme = "README.md"
 keywords = ["llm", "langchain"]
```

### Comparing `dynamic-sh-0.0.4/setup.py` & `dynamic-sh-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 for name in ['dynamic-sh', 'dynamic-llm', 'dynamic-api']:
     setup(
         name=name,
-        version='0.0.4',
+        version='0.0.5',
         description='Dynamic ⚡ is a new open-source framework that streamlines the process of building production-ready applications with LLMs. Now in beta.',
         authors=['Furqan Rydhan <furqan@f.inc>', 'Aman Ibrahim <amanmibra@gmail.com>'],
         author_email='',
         packages=find_packages(),
         install_requires=[
             # List of package dependencies
         ],
```

