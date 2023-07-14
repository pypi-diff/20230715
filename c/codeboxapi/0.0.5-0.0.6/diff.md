# Comparing `tmp/codeboxapi-0.0.5.tar.gz` & `tmp/codeboxapi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeboxapi-0.0.5.tar", max compression
+gzip compressed data, was "codeboxapi-0.0.6.tar", max compression
```

## Comparing `codeboxapi-0.0.5.tar` & `codeboxapi-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-07-09 12:26:51.625346 codeboxapi-0.0.5/LICENSE
--rw-r--r--   0        0        0     1124 2023-07-09 15:46:48.719311 codeboxapi-0.0.5/README.md
--rw-r--r--   0        0        0      447 2023-07-11 16:58:07.407377 codeboxapi-0.0.5/codeboxapi/__init__.py
--rw-r--r--   0        0        0       89 2023-07-11 17:29:00.964544 codeboxapi-0.0.5/codeboxapi/box/__init__.py
--rw-r--r--   0        0        0     2351 2023-07-13 21:08:10.583088 codeboxapi-0.0.5/codeboxapi/box/basebox.py
--rw-r--r--   0        0        0     5406 2023-07-13 21:07:44.997003 codeboxapi-0.0.5/codeboxapi/box/codebox.py
--rw-r--r--   0        0        0    15864 2023-07-13 21:03:53.020903 codeboxapi-0.0.5/codeboxapi/box/localbox.py
--rw-r--r--   0        0        0      386 2023-07-11 16:38:34.010791 codeboxapi-0.0.5/codeboxapi/config.py
--rw-r--r--   0        0        0     1822 2023-07-09 12:26:51.659184 codeboxapi-0.0.5/codeboxapi/errors.py
--rw-r--r--   0        0        0      590 2023-07-12 14:35:14.261440 codeboxapi-0.0.5/codeboxapi/schema.py
--rw-r--r--   0        0        0     2457 2023-07-13 21:12:43.142966 codeboxapi-0.0.5/codeboxapi/utils.py
--rw-r--r--   0        0        0      595 2023-07-13 17:41:29.816671 codeboxapi-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1863 1970-01-01 00:00:00.000000 codeboxapi-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-09 12:26:51.625346 codeboxapi-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1124 2023-07-14 23:30:25.010671 codeboxapi-0.0.6/README.md
+-rw-r--r--   0        0        0      447 2023-07-11 16:58:07.407377 codeboxapi-0.0.6/codeboxapi/__init__.py
+-rw-r--r--   0        0        0       89 2023-07-11 17:29:00.964544 codeboxapi-0.0.6/codeboxapi/box/__init__.py
+-rw-r--r--   0        0        0     2351 2023-07-13 21:08:10.583088 codeboxapi-0.0.6/codeboxapi/box/basebox.py
+-rw-r--r--   0        0        0     5632 2023-07-14 12:27:21.432883 codeboxapi-0.0.6/codeboxapi/box/codebox.py
+-rw-r--r--   0        0        0    15864 2023-07-13 21:03:53.020903 codeboxapi-0.0.6/codeboxapi/box/localbox.py
+-rw-r--r--   0        0        0      386 2023-07-14 23:28:15.423391 codeboxapi-0.0.6/codeboxapi/config.py
+-rw-r--r--   0        0        0     1822 2023-07-09 12:26:51.659184 codeboxapi-0.0.6/codeboxapi/errors.py
+-rw-r--r--   0        0        0      590 2023-07-12 14:35:14.261440 codeboxapi-0.0.6/codeboxapi/schema.py
+-rw-r--r--   0        0        0     2883 2023-07-14 23:29:29.893039 codeboxapi-0.0.6/codeboxapi/utils.py
+-rw-r--r--   0        0        0      595 2023-07-14 23:30:34.861998 codeboxapi-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 codeboxapi-0.0.6/PKG-INFO
```

### Comparing `codeboxapi-0.0.5/LICENSE` & `codeboxapi-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.5/README.md` & `codeboxapi-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.5/codeboxapi/box/basebox.py` & `codeboxapi-0.0.6/codeboxapi/box/basebox.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.5/codeboxapi/box/codebox.py` & `codeboxapi-0.0.6/codeboxapi/box/codebox.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,18 @@
     async def acodebox_request(
         self,
         method,
         endpoint,
         *args, **kwargs
     ) -> dict[str, Any]:
         self._update()
+        if self.session is None:
+            raise RuntimeError("CodeBox session not started")
         return await abase_request(
+            self.session,
             method,
             f"/codebox/{self.id}" + endpoint,
             *args, **kwargs
         )
     
     def status(self):
         return CodeBoxStatus(
@@ -188,14 +191,18 @@
             ** self.codebox_request(
                 method="POST",
                 endpoint="/stop",
             )
         )
 
     async def astop(self) -> CodeBoxStatus:
+        if self.session:
+            await self.session.close()
+            self.session = None
+        
         return CodeBoxStatus(
             ** await self.acodebox_request(
                 method="POST",
                 endpoint="/stop",
             )
         )
```

### Comparing `codeboxapi-0.0.5/codeboxapi/box/localbox.py` & `codeboxapi-0.0.6/codeboxapi/box/localbox.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.5/codeboxapi/errors.py` & `codeboxapi-0.0.6/codeboxapi/errors.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.5/codeboxapi/schema.py` & `codeboxapi-0.0.6/codeboxapi/schema.py`

 * *Files identical despite different names*

### Comparing `codeboxapi-0.0.5/codeboxapi/utils.py` & `codeboxapi-0.0.6/codeboxapi/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import requests  # type: ignore
-from aiohttp import ClientSession, ClientResponse
+from aiohttp import ClientSession, ClientResponse, FormData
 from codeboxapi.config import settings
 
 
 def build_request_data(
     method: str, 
     endpoint: str, 
     body: dict | None = None, 
@@ -30,20 +30,20 @@
     }
     handler = handlers.get(response.headers['Content-Type'].split(';')[0], lambda r: r.content.decode())
     if response.status_code != 200:
         raise Exception(f"Error: {response.status_code} {response.content.decode()}")
     return handler(response)
 
 
-async def handle_response_async(response: ClientResponse):
-    async def json_handler(r: ClientResponse):
+async def handle_response_async(response: ClientResponse) -> dict:
+    async def json_handler(r: ClientResponse) -> dict:
         return json.loads(await r.text())
         
-    async def default_handler(r: ClientResponse):
-        return await r.text()
+    async def default_handler(r: ClientResponse) -> dict:
+        return {"text": await r.text()}  # TODO: fix schema
     
     handlers = {
         "application/json": json_handler,
         # Add other content type handlers here
     }
     handler = handlers.get(response.headers['Content-Type'].split(';')[0], default_handler)
     if response.status != 200:
@@ -68,13 +68,23 @@
     method: str, 
     endpoint: str, 
     body: dict | None = None, 
     files: dict | None = None, 
     content_type: str = "application/json"
 ) -> dict:
     request_data = build_request_data(method, endpoint, body, files, content_type)
-    response = await session.request(**request_data)
+    if files is not None:
+        data = FormData()
+        for key, file in files.items():
+            data.add_field(key, file)
+        request_data.pop("files")
+        request_data.pop("json")
+        request_data["data"] = data
+        response = await session.request(method, request_data["url"], data=data)
+    else:
+        request_data.pop("files")
+        response = await session.request(**request_data)
     return await handle_response_async(response)
 
 
 def set_api_key(api_key: str) -> None:
     settings.CODEBOX_API_KEY = api_key
```

### Comparing `codeboxapi-0.0.5/pyproject.toml` & `codeboxapi-0.0.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "codeboxapi"
-version = "0.0.5"
+version = "0.0.6"
 description = "CodeBox is the simplest cloud infrastructure for your LLM Apps and Services."
 authors = ["Shroominic <pleurae-berets.0u@icloud.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 python-dotenv = "^1.0.0"
 websockets = "^11.0.3"
 aiohttp = "^3.8.4"
 requests = "^2.31.0"
+jupyter-kernel-gateway = "^2.5.2"
 
 [tool.poetry.extras]
 image_support = ["Pillow"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.0"
-jupyter-kernel-gateway = "^2.5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `codeboxapi-0.0.5/PKG-INFO` & `codeboxapi-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: codeboxapi
-Version: 0.0.5
+Version: 0.0.6
 Summary: CodeBox is the simplest cloud infrastructure for your LLM Apps and Services.
 License: MIT
 Author: Shroominic
 Author-email: pleurae-berets.0u@icloud.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: image-support
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: jupyter-kernel-gateway (>=2.5.2,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: websockets (>=11.0.3,<12.0.0)
 Description-Content-Type: text/markdown
 
 # CodeBox
```

