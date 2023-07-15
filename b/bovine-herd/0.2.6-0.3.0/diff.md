# Comparing `tmp/bovine_herd-0.2.6.tar.gz` & `tmp/bovine_herd-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine_herd-0.2.6.tar", max compression
+gzip compressed data, was "bovine_herd-0.3.0.tar", max compression
```

## Comparing `bovine_herd-0.2.6.tar` & `bovine_herd-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1243 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/README.md
--rw-r--r--   0        0        0     1513 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/bovine_herd/__init__.py
--rw-r--r--   0        0        0      275 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/bovine_herd/server/__init__.py
--rw-r--r--   0        0        0     1466 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/bovine_herd/server/activitypub.py
--rw-r--r--   0        0        0     4986 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/bovine_herd/server/endpoints.py
--rw-r--r--   0        0        0     2015 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/bovine_herd/server/wellknown.py
--rw-r--r--   0        0        0      521 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/bovine_herd/utils/__init__.py
--rw-r--r--   0        0        0     1084 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/bovine_herd/utils/test/__init__.py
--rw-r--r--   0        0        0      274 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/bovine_herd/utils/test_utils.py
--rw-r--r--   0        0        0       23 2023-06-04 18:36:16.374481 bovine_herd-0.2.6/bovine_herd/version.py
--rw-r--r--   0        0        0      875 2023-06-04 18:36:21.134507 bovine_herd-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 bovine_herd-0.2.6/setup.py
--rw-r--r--   0        0        0     2095 1970-01-01 00:00:00.000000 bovine_herd-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1243 2023-07-15 11:45:43.759733 bovine_herd-0.3.0/README.md
+-rw-r--r--   0        0        0     1788 2023-07-15 11:45:43.759733 bovine_herd-0.3.0/bovine_herd/__init__.py
+-rw-r--r--   0        0        0      275 2023-07-15 11:45:43.759733 bovine_herd-0.3.0/bovine_herd/server/__init__.py
+-rw-r--r--   0        0        0     1473 2023-07-15 11:45:43.759733 bovine_herd-0.3.0/bovine_herd/server/activitypub.py
+-rw-r--r--   0        0        0     5701 2023-07-15 11:45:43.759733 bovine_herd-0.3.0/bovine_herd/server/endpoints.py
+-rw-r--r--   0        0        0     2022 2023-07-15 11:45:43.759733 bovine_herd-0.3.0/bovine_herd/server/wellknown.py
+-rw-r--r--   0        0        0      521 2023-07-15 11:45:43.759733 bovine_herd-0.3.0/bovine_herd/utils/__init__.py
+-rw-r--r--   0        0        0     1797 2023-07-15 11:45:43.759733 bovine_herd-0.3.0/bovine_herd/utils/test/__init__.py
+-rw-r--r--   0        0        0      274 2023-07-15 11:45:43.759733 bovine_herd-0.3.0/bovine_herd/utils/test_utils.py
+-rw-r--r--   0        0        0     1117 2023-07-15 11:46:38.108131 bovine_herd-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2254 1970-01-01 00:00:00.000000 bovine_herd-0.3.0/setup.py
+-rw-r--r--   0        0        0     2175 1970-01-01 00:00:00.000000 bovine_herd-0.3.0/PKG-INFO
```

### Comparing `bovine_herd-0.2.6/README.md` & `bovine_herd-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.6/bovine_herd/server/activitypub.py` & `bovine_herd-0.3.0/bovine_herd/server/activitypub.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from importlib.metadata import version as meta_version
 
 import werkzeug
-from bovine_store.utils import path_from_request
+from bovine_store.server.utils import path_from_request
 from quart import Blueprint, current_app, request
 
 activitypub = Blueprint("activitypub", __name__, url_prefix="/activitypub")
 
 logger = logging.getLogger(__name__)
```

### Comparing `bovine_herd-0.2.6/bovine_herd/server/endpoints.py` & `bovine_herd-0.3.0/bovine_herd/server/endpoints.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,147 +1,158 @@
 import logging
 
 import bovine
 from bovine.jsonld import with_bovine_context
 from bovine.types import Visibility
-from bovine_process import handle_outbox_item, process_inbox_item, process_outbox_item
 from bovine_process.types import ProcessingItem
-from bovine_store.fedi.authorize import add_authorization
+from bovine_store.server.collection import collection_response
+from bovine_store.server.utils import path_from_request
 from bovine_store.types import EndpointType
-from bovine_store.utils import path_from_request
-from quart import Blueprint, current_app, g, make_response, request
+from quart import Blueprint, current_app, g, make_response, redirect, request
 
 logger = logging.getLogger(__name__)
 
-endpoints = Blueprint("endpoint", __name__)
-endpoints.before_request(add_authorization)
 
+def build_endpoints_blueprint(
+    handle_outbox_item, process_inbox_item, process_outbox_item
+):
+    endpoints = Blueprint("endpoint", __name__)
+
+    @endpoints.get("/<identifier>")
+    async def endpoints_get(identifier):
+        endpoint_path = path_from_request(request)
+        object_store = current_app.config["bovine_store"]
 
-@endpoints.get("/<identifier>")
-async def endpoints_get(identifier):
-    endpoint_path = path_from_request(request)
-    object_store = current_app.config["bovine_store"]
+        endpoint_type, actor = await object_store.resolve_endpoint(endpoint_path)
 
-    endpoint_type, actor = await object_store.resolve_endpoint(endpoint_path)
+        if endpoint_type is None:
+            return (
+                {
+                    "@context": "https://www.w3.org/ns/activitystreams",
+                    "type": "Object",
+                    "id": endpoint_path,
+                    "name": "Ceci n'est pas un object",
+                },
+                404,
+                {"content-type": "application/activity+json"},
+            )
 
-    if endpoint_type is None:
-        return (
-            {
-                "@context": "https://www.w3.org/ns/activitystreams",
-                "type": "Object",
-                "id": endpoint_path,
-                "name": "Ceci n'est pas un object",
-            },
-            404,
-            {"content-type": "application/activity+json"},
-        )
+        if endpoint_type == EndpointType.ACTOR:
+            logger.info("Getting %s for %s", endpoint_path, g.retriever)
 
-    if endpoint_type == EndpointType.ACTOR:
-        logger.info("Getting %s for %s", endpoint_path, g.retriever)
+            if endpoint_path == g.retriever:
+                return (
+                    actor.actor_object.build(visibility=Visibility.OWNER),
+                    200,
+                    {"content-type": "application/activity+json"},
+                )
+
+            if g.retriever is None or g.retriever == "NONE":
+                if "text" in request.headers.get("accept", ""):
+                    if actor.actor_object.url is not None:
+                        return redirect(actor.actor_object.url)
+                return {"status": "unauthorized"}, 401
 
-        if endpoint_path == g.retriever:
             return (
-                actor.actor_object.build(visibility=Visibility.OWNER),
+                actor.actor_object.build(visibility=Visibility.PUBLIC),
                 200,
                 {"content-type": "application/activity+json"},
             )
 
-        if g.retriever is None or g.retriever == "NONE":
-            return {"status": "unauthorized"}, 401
-
-        return (
-            actor.actor_object.build(visibility=Visibility.PUBLIC),
-            200,
-            {"content-type": "application/activity+json"},
-        )
-
-    if endpoint_type == EndpointType.EVENT_SOURCE:
-        actor = actor.actor_object.build(visibility=Visibility.OWNER)
-        if g.retriever != actor["id"]:
-            return {"status": "unauthorized"}, 401
-        return await handle_event_source(endpoint_path, actor)
-
-    return await object_store.collection_response(endpoint_path)
-
+        if endpoint_type == EndpointType.EVENT_SOURCE:
+            actor = actor.actor_object.build(visibility=Visibility.OWNER)
+            if g.retriever != actor["id"]:
+                return {"status": "unauthorized"}, 401
+            return await handle_event_source(endpoint_path, actor)
+
+        return await collection_response(endpoint_path)
+
+    @endpoints.post("/<identifier>")
+    async def endpoints_post(identifier):
+        endpoint_path = path_from_request(request)
+        object_store = current_app.config["bovine_store"]
+
+        endpoint_type, actor = await object_store.resolve_endpoint(endpoint_path)
+
+        if endpoint_type not in [
+            EndpointType.INBOX,
+            EndpointType.OUTBOX,
+            EndpointType.PROXY_URL,
+        ]:
+            return {"status": "method not allowed"}, 405
+
+        actor_object = actor.actor_object.build(visibility=Visibility.OWNER)
+
+        if endpoint_type == EndpointType.INBOX:
+            if not g.retriever:
+                return {"status": "unauthorized"}, 401
+            item = ProcessingItem(g.retriever, await request.get_json())
+            current_app.add_background_task(process_inbox_item, item, actor)
+            return {"status": "processing"}, 202
 
-@endpoints.post("/<identifier>")
-async def endpoints_post(identifier):
-    endpoint_path = path_from_request(request)
-    object_store = current_app.config["bovine_store"]
-
-    endpoint_type, actor = await object_store.resolve_endpoint(endpoint_path)
-
-    if endpoint_type not in [
-        EndpointType.INBOX,
-        EndpointType.OUTBOX,
-        EndpointType.PROXY_URL,
-    ]:
-        return {"status": "method not allowed"}, 405
-
-    actor_object = actor.actor_object.build(visibility=Visibility.OWNER)
-
-    if endpoint_type == EndpointType.INBOX:
-        if not g.retriever:
+        if g.retriever != actor_object["id"]:
             return {"status": "unauthorized"}, 401
-        item = ProcessingItem(g.retriever, await request.get_json())
-        current_app.add_background_task(process_inbox_item, item, actor)
-        return {"status": "processing"}, 202
 
-    if g.retriever != actor_object["id"]:
-        return {"status": "unauthorized"}, 401
+        if endpoint_type == EndpointType.OUTBOX:
+            item = ProcessingItem(g.retriever, await request.get_json())
+            item = await handle_outbox_item(item, actor)
 
-    if endpoint_type == EndpointType.OUTBOX:
-        item = ProcessingItem(g.retriever, await request.get_json())
-        item = await handle_outbox_item(item, actor)
+            current_app.add_background_task(process_outbox_item, item, actor)
 
-        current_app.add_background_task(process_outbox_item, item, actor)
-
-        return {"status": "created"}, 201, {"location": item.meta["object_location"]}
-
-    if endpoint_type == EndpointType.PROXY_URL:
-        return await proxy_url_response(actor)
+            return (
+                {"status": "created"},
+                201,
+                {"location": item.meta["object_location"]},
+            )
 
+        if endpoint_type == EndpointType.PROXY_URL:
+            return await proxy_url_response(actor)
 
-async def proxy_url_response(actor):
-    url = (await request.form)["id"]
+    async def proxy_url_response(actor):
+        url = (await request.form)["id"]
 
-    try:
-        if not url.startswith("http") and "@" in url:
-            url = await bovine.clients.lookup_account_with_webfinger(actor.session, url)
+        try:
+            if not url.startswith("http") and "@" in url:
+                url = await bovine.clients.lookup_account_with_webfinger(
+                    actor.session, url
+                )
 
-        result = await actor.retrieve(url, include=["object", "actor", "attributedTo"])
-        if result:
-            return with_bovine_context(result), 200
-        return {"status": "not found"}, 404
-    except Exception as e:
-        logger.error("Something went wrong during proxy url")
-        logger.exception(e)
-        return {"status": "something went wrong"}, 400
+            result = await actor.retrieve(
+                url, include=["object", "actor", "attributedTo"]
+            )
+            if result:
+                return with_bovine_context(result), 200
+            return {"status": "not found"}, 404
+        except Exception as e:
+            logger.error("Something went wrong during proxy url")
+            logger.exception(e)
+            return {"status": "something went wrong"}, 400
 
+    async def handle_event_source(endpoint_path, actor):
+        if endpoint_path != actor["endpoints"]["eventSource"]:
+            return {"status": "unauthorized"}, 401
 
-async def handle_event_source(endpoint_path, actor):
-    if endpoint_path != actor["endpoints"]["eventSource"]:
-        return {"status": "unauthorized"}, 401
+        logger.info("Opening event source for %s", actor["name"])
 
-    logger.info("Opening event source for %s", actor["name"])
+        if "bovine_pub_sub" not in current_app.config:
+            return {"status": "not implemented"}, 501
 
-    if "bovine_pub_sub" not in current_app.config:
-        return {"status": "not implemented"}, 501
+        pubsub = current_app.config["bovine_pub_sub"]
 
-    pubsub = current_app.config["bovine_pub_sub"]
+        response = await make_response(
+            pubsub.event_stream(endpoint_path),
+            {
+                "Content-Type": "text/event-stream",
+                "Cache-Control": "no-cache",
+                "Transfer-Encoding": "chunked",
+            },
+        )
+        response.timeout = None
 
-    response = await make_response(
-        pubsub.event_stream(endpoint_path),
-        {
-            "Content-Type": "text/event-stream",
-            "Cache-Control": "no-cache",
-            "Transfer-Encoding": "chunked",
-        },
-    )
-    response.timeout = None
+        # last_event_id = request.headers.get("last-event-id")
+        # if last_event_id:
+        #     current_app.add_background_task(
+        #         enqueue_missing_events, queue, last_event_id, actor["name"]
+        #     )
+        return response
 
-    # last_event_id = request.headers.get("last-event-id")
-    # if last_event_id:
-    #     current_app.add_background_task(
-    #         enqueue_missing_events, queue, last_event_id, actor["name"]
-    #     )
-    return response
+    return endpoints
```

### Comparing `bovine_herd-0.2.6/bovine_herd/server/wellknown.py` & `bovine_herd-0.3.0/bovine_herd/server/wellknown.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from urllib.parse import urljoin
 
 from bovine.utils import webfinger_response_json
-from bovine_store.utils import path_from_request
+from bovine_store.server.utils import path_from_request
 from quart import Blueprint, current_app, request
 
 wellknown = Blueprint("wellknown", __name__, url_prefix="/.well-known")
 
 logger = logging.getLogger(__name__)
```

### Comparing `bovine_herd-0.2.6/bovine_herd/utils/__init__.py` & `bovine_herd-0.3.0/bovine_herd/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_herd-0.2.6/setup.py` & `bovine_herd-0.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,25 +10,24 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aiodns>=3.0.0,<4.0.0',
  'aiohttp>=3.8.3,<4.0.0',
  'asyncstdlib>=3.10.5,<4.0.0',
- 'bovine-process>=0.2.0,<0.3.0',
- 'bovine-pubsub>=0.2.0,<0.3.0',
- 'bovine-store>=0.2.1,<0.3.0',
+ 'bovine-process>=0.3.0,<0.4.0',
+ 'bovine-store>=0.3.0,<0.4.0',
  'markdown>=3.4.1,<4.0.0',
  'python-markdown-math>=0.8,<0.9',
  'tortoise-orm[asyncpg]>=0.19.3,<0.20.0']
 
 setup_kwargs = {
     'name': 'bovine-herd',
-    'version': '0.2.6',
-    'description': '',
+    'version': '0.3.0',
+    'description': 'Implementation of a Fediverse server based on bovine',
     'long_description': '# bovine_herd\n\n`bovine_herd` is a `bovine` powered ActivityPub server, which interoperates with the rest of the FediVerse.\n\nRunning:\n\n```bash\npip install bovine_herd\nhypercorn bovine_herd:app\n```\n\nThis will start `bovine_herd` using an sqlite3 database.\n\n## Interacting with the fediverse\n\nAssume that you alias `$DOMAIN` so that it redirects to the above server. Then by running\n\n```bash\npip install bovine_tool\npython -mbovine_tool.register --domain $DOMAIN moocow\n```\n\nyou create a new account for __moocow__. This command returns its bovine name, which will be of the form `moocow + uuid4()`, e.g. `moocow_09c80006-483c-4826-b48c-cf5134b4e898`. By running:\n\n```bash\npython -mbovine_tool.manage --new_did_key $BOVINE_NAME\n```\n\nyou will be given a secret (an Ed25519 private key, i.e. starts with `z3u2`). Once you have this secret, you can send a message via\n\n```bash\npython -mbovine.msg --secret $SECRET --host $DOMAIN moooo\n```\n\n## Configuration\n\nThe default database connection is "sqlite://bovine.sqlite3". This can be overwridden with the environment variable "BOVINE_DB_URL".\n\n- `BOVINE_REDIS` represents how to reach redis, e.g. `redis://localhost`. If not set, redis is not used. Redis is necessary when using more than one worker.\n',
     'author': 'Helge',
     'author_email': 'helge.krueger@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://codeberg.org/bovine/bovine',
     'packages': packages,
```

### Comparing `bovine_herd-0.2.6/PKG-INFO` & `bovine_herd-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: bovine-herd
-Version: 0.2.6
-Summary: 
+Version: 0.3.0
+Summary: Implementation of a Fediverse server based on bovine
 Home-page: https://codeberg.org/bovine/bovine
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiodns (>=3.0.0,<4.0.0)
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: asyncstdlib (>=3.10.5,<4.0.0)
-Requires-Dist: bovine-process (>=0.2.0,<0.3.0)
-Requires-Dist: bovine-pubsub (>=0.2.0,<0.3.0)
-Requires-Dist: bovine-store (>=0.2.1,<0.3.0)
+Requires-Dist: bovine-process (>=0.3.0,<0.4.0)
+Requires-Dist: bovine-store (>=0.3.0,<0.4.0)
 Requires-Dist: markdown (>=3.4.1,<4.0.0)
 Requires-Dist: python-markdown-math (>=0.8,<0.9)
 Requires-Dist: tortoise-orm[asyncpg] (>=0.19.3,<0.20.0)
+Project-URL: Documentation, https://bovine-herd.readthedocs.io/en/latest/
 Project-URL: Repository, https://codeberg.org/bovine/bovine
 Description-Content-Type: text/markdown
 
 # bovine_herd
 
 `bovine_herd` is a `bovine` powered ActivityPub server, which interoperates with the rest of the FediVerse.
```

