# Comparing `tmp/bovine_process-0.2.6.tar.gz` & `tmp/bovine_process-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine_process-0.2.6.tar", max compression
+gzip compressed data, was "bovine_process-0.3.0.tar", max compression
```

## Comparing `bovine_process-0.2.6.tar` & `bovine_process-0.3.0.tar`

### file list

```diff
@@ -1,52 +1,30 @@
--rw-r--r--   0        0        0     1619 2023-06-04 18:31:36.366115 bovine_process-0.2.6/README.md
--rw-r--r--   0        0        0     1664 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/__init__.py
--rw-r--r--   0        0        0      770 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/add_to_queue.py
--rw-r--r--   0        0        0     1176 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/incoming/__init__.py
--rw-r--r--   0        0        0     1152 2023-06-04 18:34:44.991995 bovine_process-0.2.6/bovine_process/incoming/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      978 2023-06-04 18:34:44.995995 bovine_process-0.2.6/bovine_process/incoming/__pycache__/follow_accept.cpython-310.pyc
--rw-r--r--   0        0        0      813 2023-06-04 18:34:44.995995 bovine_process-0.2.6/bovine_process/incoming/__pycache__/handle_update.cpython-310.pyc
--rw-r--r--   0        0        0      948 2023-06-04 18:34:44.999995 bovine_process-0.2.6/bovine_process/incoming/__pycache__/incoming_delete.cpython-310.pyc
--rw-r--r--   0        0        0     2131 2023-06-04 18:34:44.999995 bovine_process-0.2.6/bovine_process/incoming/__pycache__/interactions.cpython-310.pyc
--rw-r--r--   0        0        0     1066 2023-06-04 18:34:44.999995 bovine_process-0.2.6/bovine_process/incoming/__pycache__/store_incoming.cpython-310.pyc
--rw-r--r--   0        0        0     1637 2023-06-04 18:34:45.067995 bovine_process-0.2.6/bovine_process/incoming/__pycache__/test_handle_update.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1880 2023-06-04 18:34:45.103996 bovine_process-0.2.6/bovine_process/incoming/__pycache__/test_store_incoming.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      863 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/incoming/follow_accept.py
--rw-r--r--   0        0        0      709 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/incoming/handle_update.py
--rw-r--r--   0        0        0      847 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/incoming/incoming_delete.py
--rw-r--r--   0        0        0     2501 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/incoming/interactions.py
--rw-r--r--   0        0        0      877 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/incoming/store_incoming.py
--rw-r--r--   0        0        0     1414 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/incoming/test_handle_update.py
--rw-r--r--   0        0        0      983 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/incoming/test_store_incoming.py
--rw-r--r--   0        0        0      693 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/outgoing/__init__.py
--rw-r--r--   0        0        0      733 2023-06-04 18:34:44.999995 bovine_process-0.2.6/bovine_process/outgoing/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      820 2023-06-04 18:34:44.999995 bovine_process-0.2.6/bovine_process/outgoing/__pycache__/accept_follow.cpython-310.pyc
--rw-r--r--   0        0        0      960 2023-06-04 18:34:44.999995 bovine_process-0.2.6/bovine_process/outgoing/__pycache__/outgoing_delete.cpython-310.pyc
--rw-r--r--   0        0        0      887 2023-06-04 18:34:45.003995 bovine_process-0.2.6/bovine_process/outgoing/__pycache__/outgoing_update.cpython-310.pyc
--rw-r--r--   0        0        0     1132 2023-06-04 18:34:45.003995 bovine_process-0.2.6/bovine_process/outgoing/__pycache__/store_outgoing.cpython-310.pyc
--rw-r--r--   0        0        0     1613 2023-06-04 18:34:45.107996 bovine_process-0.2.6/bovine_process/outgoing/__pycache__/test_outgoing_update.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      604 2023-06-04 18:34:45.003995 bovine_process-0.2.6/bovine_process/outgoing/__pycache__/update_id.cpython-310.pyc
--rw-r--r--   0        0        0      642 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/outgoing/accept_follow.py
--rw-r--r--   0        0        0      878 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/outgoing/outgoing_delete.py
--rw-r--r--   0        0        0      943 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/outgoing/outgoing_update.py
--rw-r--r--   0        0        0      972 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/outgoing/store_outgoing.py
--rw-r--r--   0        0        0     1626 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/outgoing/test_outgoing_update.py
--rw-r--r--   0        0        0      386 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/outgoing/update_id.py
--rw-r--r--   0        0        0     1598 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/send_item.py
--rw-r--r--   0        0        0      364 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/test_types.py
--rw-r--r--   0        0        0      723 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/types.py
--rw-r--r--   0        0        0        0 2023-06-04 18:31:36.498116 bovine_process-0.2.6/bovine_process/utils/__init__.py
--rw-r--r--   0        0        0      183 2023-06-04 18:34:44.995995 bovine_process-0.2.6/bovine_process/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1156 2023-06-04 18:34:44.995995 bovine_process-0.2.6/bovine_process/utils/__pycache__/by_activity_type.cpython-310.pyc
--rw-r--r--   0        0        0     1324 2023-06-04 18:34:44.995995 bovine_process-0.2.6/bovine_process/utils/__pycache__/processor_list.cpython-310.pyc
--rw-r--r--   0        0        0     2420 2023-06-04 18:34:45.111996 bovine_process-0.2.6/bovine_process/utils/__pycache__/test_by_activity_type.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1077 2023-06-04 18:34:45.115996 bovine_process-0.2.6/bovine_process/utils/__pycache__/test_processor_list.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1591 2023-06-04 18:34:45.119996 bovine_process-0.2.6/bovine_process/utils/__pycache__/test_update_id.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      515 2023-06-04 18:34:45.003995 bovine_process-0.2.6/bovine_process/utils/__pycache__/update_id.cpython-310.pyc
--rw-r--r--   0        0        0      741 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/utils/by_activity_type.py
--rw-r--r--   0        0        0      844 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/utils/processor_list.py
--rw-r--r--   0        0        0     1084 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/utils/test_by_activity_type.py
--rw-r--r--   0        0        0      429 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/utils/test_processor_list.py
--rw-r--r--   0        0        0      759 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/utils/test_update_id.py
--rw-r--r--   0        0        0      481 2023-06-04 18:31:36.366115 bovine_process-0.2.6/bovine_process/utils/update_id.py
--rw-r--r--   0        0        0      939 2023-06-04 18:31:36.370115 bovine_process-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2309 1970-01-01 00:00:00.000000 bovine_process-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1619 2023-07-15 11:45:43.759733 bovine_process-0.3.0/README.md
+-rw-r--r--   0        0        0     1664 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/__init__.py
+-rw-r--r--   0        0        0      936 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/add_to_queue.py
+-rw-r--r--   0        0        0     1859 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/incoming/__init__.py
+-rw-r--r--   0        0        0      863 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/incoming/follow_accept.py
+-rw-r--r--   0        0        0      709 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/incoming/handle_update.py
+-rw-r--r--   0        0        0      847 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/incoming/incoming_delete.py
+-rw-r--r--   0        0        0     3124 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/incoming/interactions.py
+-rw-r--r--   0        0        0      877 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/incoming/store_incoming.py
+-rw-r--r--   0        0        0     1414 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/incoming/test_handle_update.py
+-rw-r--r--   0        0        0      983 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/incoming/test_store_incoming.py
+-rw-r--r--   0        0        0      757 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/outgoing/__init__.py
+-rw-r--r--   0        0        0      642 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/outgoing/accept_follow.py
+-rw-r--r--   0        0        0      878 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/outgoing/outgoing_delete.py
+-rw-r--r--   0        0        0      943 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/outgoing/outgoing_update.py
+-rw-r--r--   0        0        0      972 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/outgoing/store_outgoing.py
+-rw-r--r--   0        0        0     1626 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/outgoing/test_outgoing_update.py
+-rw-r--r--   0        0        0      804 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/outgoing/test_update_id.py
+-rw-r--r--   0        0        0      989 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/outgoing/update_id.py
+-rw-r--r--   0        0        0     1842 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/send_item.py
+-rw-r--r--   0        0        0      364 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/test_types.py
+-rw-r--r--   0        0        0      723 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/types.py
+-rw-r--r--   0        0        0        0 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/utils/__init__.py
+-rw-r--r--   0        0        0      741 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/utils/by_activity_type.py
+-rw-r--r--   0        0        0      844 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/utils/processor_list.py
+-rw-r--r--   0        0        0     1084 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/utils/test_by_activity_type.py
+-rw-r--r--   0        0        0      429 2023-07-15 11:45:43.759733 bovine_process-0.3.0/bovine_process/utils/test_processor_list.py
+-rw-r--r--   0        0        0     1093 2023-07-15 11:46:38.108131 bovine_process-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 bovine_process-0.3.0/setup.py
+-rw-r--r--   0        0        0     2386 1970-01-01 00:00:00.000000 bovine_process-0.3.0/PKG-INFO
```

### Comparing `bovine_process-0.2.6/README.md` & `bovine_process-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.6/bovine_process/__init__.py` & `bovine_process-0.3.0/bovine_process/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.6/bovine_process/incoming/__init__.py` & `bovine_process-0.3.0/bovine_process/incoming/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import logging
+
 from bovine.jsonld import with_external_context
 
 from bovine_process.add_to_queue import add_to_queue
 from bovine_process.utils.processor_list import ProcessorList
 
 from .follow_accept import follow_accept
 from .handle_update import handle_update
@@ -11,36 +13,56 @@
     delete_reply_handler,
     like_handler,
     reply_handler,
     undo_handler,
 )
 from .store_incoming import add_incoming_to_inbox, store_incoming
 
+logger = logging.getLogger(__name__)
+
 
 async def sanitize(item, actor):
     item.data = with_external_context(item.data)
+
+    if item.submitter != item.data["actor"]:
+        logger.error("Got wrong submitter for an activity %s", item.submitter)
+        logger.error(item.data)
+        # return
+
     return item
 
 
-default_inbox_process = (
-    ProcessorList()
-    .add(sanitize)
-    .add_for_types(
-        Create=store_incoming,
-        Update=handle_update,
-        Delete=incoming_delete,
-        Accept=follow_accept,
-    )
-    .add(store_incoming)
-    .add(add_incoming_to_inbox)
-    .add_for_types(
+interaction_handlers = {
+    **dict(
         Announce=announce_handler,
         Create=reply_handler,
         Delete=delete_reply_handler,
         Dislike=like_handler,
         Like=like_handler,
         Undo=undo_handler,
-        **{"http://litepub.social/ns#EmojiReact": like_handler}
-    )
+    ),
+    "http://litepub.social/ns#EmojiReact": like_handler,
+}
+"""The handlers being called for interactions"""
+
+crud_handlers = dict(Update=handle_update, Delete=incoming_delete)
+"""The handlers being called for CRUD operations"""
+
+social_handlers = dict(Accept=follow_accept)
+"""The handlers being called for social interactions, i.e. updating the social graph
+
+FIXME: Missing undo_follow ... and the other nonsense, I need somebody to draw me
+a state machine for"""
+
+
+default_inbox_process = (
+    ProcessorList()
+    .add(sanitize)
+    .add(store_incoming)
+    .add(add_incoming_to_inbox)
+    .add_for_types(**crud_handlers)
+    .add_for_types(**social_handlers)
+    .add_for_types(**interaction_handlers)
     .add(add_to_queue)
     .apply
 )
+"""Represents the default process undertaken by an inbox item"""
```

### Comparing `bovine_process-0.2.6/bovine_process/incoming/follow_accept.py` & `bovine_process-0.3.0/bovine_process/incoming/follow_accept.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.6/bovine_process/incoming/handle_update.py` & `bovine_process-0.3.0/bovine_process/incoming/handle_update.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.6/bovine_process/incoming/incoming_delete.py` & `bovine_process-0.3.0/bovine_process/incoming/incoming_delete.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.6/bovine_process/incoming/interactions.py` & `bovine_process-0.3.0/bovine_process/incoming/interactions.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,36 +4,48 @@
 
 from bovine_process.types import ProcessingItem
 
 logger = logging.getLogger(__name__)
 
 
 async def like_handler(item: ProcessingItem, actor) -> ProcessingItem:
+    """Adds object to the likes collection of the liked object, if
+
+    * object being liked is owner by the receiving actor"""
+
     object_to_like = item.data.get("object")
     obj = await actor.retrieve_own_object(id_for_object(object_to_like))
     if obj:
         obj_id = id_for_object(obj)
         logger.info("Like Handler %s", obj_id)
         await actor.add_to_interaction("likes", obj_id, item.data.get("id"))
 
     return item
 
 
 async def announce_handler(item: ProcessingItem, actor) -> ProcessingItem:
+    """Adds object to the shares collection of the announced object, if
+
+    * object being announced is owner by the receiving actor"""
+
     object_to_share = item.data.get("object")
     obj = await actor.retrieve_own_object(id_for_object(object_to_share))
     if obj:
         obj_id = id_for_object(obj)
         logger.info("Announce Handler %s", obj_id)
         await actor.add_to_interaction("shares", obj_id, item.data.get("id"))
 
     return item
 
 
 async def reply_handler(item: ProcessingItem, actor) -> ProcessingItem:
+    """Adds object to the replies collection. Object being replied to
+    is determined from `inReplyTo`. Reply is added if the object
+    belongs to the receiving actor."""
+
     remote = item.data.get("object")
     if not remote:
         return item
     in_reply_to = remote.get("inReplyTo")
     if not in_reply_to:
         return item
 
@@ -44,24 +56,29 @@
         logger.info("Reply Handler %s", obj_id)
         await actor.add_to_interaction("replies", obj_id, remote.get("id"))
 
     return item
 
 
 async def delete_reply_handler(item: ProcessingItem, actor) -> ProcessingItem:
+    """If a reply is deleted, removes it from the replies collection"""
+
     remote = item.data.get("object")
     if not remote:
         return item
 
     await actor.remove_references(remote)
 
     return item
 
 
 async def undo_handler(item: ProcessingItem, actor) -> ProcessingItem:
+    """For an Undo of a Like, Dislike, Announce , they are removed from
+    the appropriate collection."""
+
     object_to_undo = id_for_object(item.data.get("object"))
     obj = await actor.retrieve(object_to_undo)
     if obj is None:
         return item
     remote_actor = id_for_object(item.data.get("actor"))
     if obj.get("actor") != remote_actor:
         logger.error("Mismatching actor in undo from %s", remote_actor)
```

### Comparing `bovine_process-0.2.6/bovine_process/incoming/store_incoming.py` & `bovine_process-0.3.0/bovine_process/incoming/store_incoming.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.6/bovine_process/incoming/test_handle_update.py` & `bovine_process-0.3.0/bovine_process/incoming/test_handle_update.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.6/bovine_process/incoming/test_store_incoming.py` & `bovine_process-0.3.0/bovine_process/incoming/test_store_incoming.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.6/bovine_process/outgoing/__init__.py` & `bovine_process-0.3.0/bovine_process/outgoing/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,12 +14,13 @@
     .add(add_outgoing_to_outbox)
     .add_for_types(
         Update=outgoing_update,
         Delete=outgoing_delete,
     )
     .apply
 )
+"""Defines the synchrnous part of sending an outgoing object"""
 
 
 default_async_outbox_process = (
     ProcessorList().add_for_types(Accept=accept_follow).add(add_to_queue).apply
 )
```

### Comparing `bovine_process-0.2.6/bovine_process/outgoing/accept_follow.py` & `bovine_process-0.3.0/bovine_process/outgoing/accept_follow.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.6/bovine_process/outgoing/outgoing_delete.py` & `bovine_process-0.3.0/bovine_process/outgoing/outgoing_delete.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.6/bovine_process/outgoing/outgoing_update.py` & `bovine_process-0.3.0/bovine_process/outgoing/outgoing_update.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.6/bovine_process/outgoing/store_outgoing.py` & `bovine_process-0.3.0/bovine_process/outgoing/store_outgoing.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.6/bovine_process/outgoing/test_outgoing_update.py` & `bovine_process-0.3.0/bovine_process/outgoing/test_outgoing_update.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.6/bovine_process/send_item.py` & `bovine_process-0.3.0/bovine_process/send_item.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,21 @@
     except Exception as ex:
         logger.warning("Sending to %s failed with %s", inbox, ex)
         for log_line in traceback.format_exc().splitlines():
             logger.warning(log_line)
 
 
 async def send_outbox_item(item, actor):
+    """Sends the item to all the specfied outboxes
+
+    Collections are resolved if they are part of actor.endpoints and then
+    resolved via actor.resolve_endpoints.
+
+    inboxes from actors are fetched from the database or refetched
+    """
     logger.info("Sending outbox item")
 
     recipients = recipients_for_object(item.data)
     recipients = remove_public(recipients)
 
     endpoints = [x for x in recipients if x in actor.endpoints]
```

### Comparing `bovine_process-0.2.6/bovine_process/types.py` & `bovine_process-0.3.0/bovine_process/types.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.6/bovine_process/utils/by_activity_type.py` & `bovine_process-0.3.0/bovine_process/utils/by_activity_type.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.6/bovine_process/utils/processor_list.py` & `bovine_process-0.3.0/bovine_process/utils/processor_list.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.6/bovine_process/utils/test_by_activity_type.py` & `bovine_process-0.3.0/bovine_process/utils/test_by_activity_type.py`

 * *Files identical despite different names*

### Comparing `bovine_process-0.2.6/bovine_process/utils/test_update_id.py` & `bovine_process-0.3.0/bovine_process/outgoing/test_update_id.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import uuid
 from unittest.mock import AsyncMock
 
 from quart import Quart
 
-from .update_id import update_id
+from .update_id import update_id_function
 
 app = Quart(__name__)
 
 
 async def test_update_id():
     actor = AsyncMock()
     actor.generate_new_object_id = lambda: str(uuid.uuid4())
 
     data = {"id": "id"}
-    result = await update_id(data, actor)
+    result = await update_id_function(data, actor)
     assert result["id"] != "id"
 
     data = {"object": "test"}
-    result = await update_id(data, actor)
+    result = await update_id_function(data, actor)
     assert result["id"]
 
     # if in store; id is not updated
     data = {"object": {"id": "id"}}
-    result = await update_id(data, actor)
+    result = await update_id_function(data, actor)
     assert result["object"]["id"] == "id"
 
     actor.retrieve.return_value = None
     data = {"object": {"id": "id"}}
-    result = await update_id(data, actor)
+    result = await update_id_function(data, actor)
     assert result["object"]["id"] != "id"
```

### Comparing `bovine_process-0.2.6/pyproject.toml` & `bovine_process-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 [tool.poetry]
 name = "bovine-process"
-version = "0.2.6"
+version = "0.3.0"
 description = "Processing of Side Effects of ActivityPub Activities for an ActivityPub Server"
 authors = ["Helge <helge.krueger@gmail.com>"]
 readme = "README.md"
 packages = [{include = "bovine_process"}]
 license = "MIT"
 repository = "https://codeberg.org/bovine/bovine"
+documentation = "https://bovine-process.readthedocs.io/en/latest/"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-bovine-store = "^0.2.1"
+bovine-store = "^0.3.0"
 tortoise-orm = {extras = ["asyncpg"], version = "^0.19.3"}
 
 [tool.poetry.group.test.dependencies]
 black = "^23.1.0"
 pytest = "^7.2.2"
 pytest-asyncio = "^0.20.3"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 black = "^23.3.0"
 mypy = "^1.2.0"
 ruff = "^0.0.261"
 
+
+[tool.poetry.group.doc.dependencies]
+sphinx = "^6.1.3"
+sphinx-rtd-theme = "^1.2.0"
+
+
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 line-length = 88
```

### Comparing `bovine_process-0.2.6/PKG-INFO` & `bovine_process-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: bovine-process
-Version: 0.2.6
+Version: 0.3.0
 Summary: Processing of Side Effects of ActivityPub Activities for an ActivityPub Server
 Home-page: https://codeberg.org/bovine/bovine
 License: MIT
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bovine-store (>=0.2.1,<0.3.0)
+Requires-Dist: bovine-store (>=0.3.0,<0.4.0)
 Requires-Dist: tortoise-orm[asyncpg] (>=0.19.3,<0.20.0)
+Project-URL: Documentation, https://bovine-process.readthedocs.io/en/latest/
 Project-URL: Repository, https://codeberg.org/bovine/bovine
 Description-Content-Type: text/markdown
 
 # bovine_process
 
 `bovine_process` consists of the side effect logic of Activity objects. This means it contains the code, the logic that for an incoming object, one executes:
```

