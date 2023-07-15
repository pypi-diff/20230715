# Comparing `tmp/bovine_store-0.2.6.tar.gz` & `tmp/bovine_store-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine_store-0.2.6.tar", max compression
+gzip compressed data, was "bovine_store-0.3.0.tar", max compression
```

## Comparing `bovine_store-0.2.6.tar` & `bovine_store-0.3.0.tar`

### file list

```diff
@@ -1,75 +1,45 @@
--rw-r--r--   0        0        0     2857 2023-06-04 18:31:36.370115 bovine_store-0.2.6/README.md
--rw-r--r--   0        0        0     6755 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/__init__.py
--rw-r--r--   0        0        0     1115 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/actor/__init__.py
--rw-r--r--   0        0        0     1587 2023-06-04 18:33:42.427369 bovine_store-0.2.6/bovine_store/actor/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     8275 2023-06-04 18:33:43.307378 bovine_store-0.2.6/bovine_store/actor/__pycache__/bovine_store_actor.cpython-310.pyc
--rw-r--r--   0        0        0     1831 2023-06-04 18:33:43.311378 bovine_store-0.2.6/bovine_store/actor/__pycache__/register.cpython-310.pyc
--rw-r--r--   0        0        0     1525 2023-06-04 18:33:44.071386 bovine_store-0.2.6/bovine_store/actor/__pycache__/test_bovine_application_actor.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     5966 2023-06-04 18:33:44.075386 bovine_store-0.2.6/bovine_store/actor/__pycache__/test_bovine_store_actor.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     4341 2023-06-04 18:33:44.087386 bovine_store-0.2.6/bovine_store/actor/__pycache__/test_register.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     8175 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/actor/bovine_store_actor.py
--rw-r--r--   0        0        0     1844 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/actor/register.py
--rw-r--r--   0        0        0      731 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/actor/test_bovine_application_actor.py
--rw-r--r--   0        0        0     5217 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/actor/test_bovine_store_actor.py
--rw-r--r--   0        0        0     1684 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/actor/test_register.py
--rw-r--r--   0        0        0     2694 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/blueprint.py
--rw-r--r--   0        0        0      892 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/config.py
--rw-r--r--   0        0        0        0 2023-06-04 18:31:36.514116 bovine_store-0.2.6/bovine_store/fedi/__init__.py
--rw-r--r--   0        0        0      178 2023-06-04 18:33:44.063386 bovine_store-0.2.6/bovine_store/fedi/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1149 2023-06-04 18:33:44.063386 bovine_store-0.2.6/bovine_store/fedi/__pycache__/authorize.cpython-310.pyc
--rw-r--r--   0        0        0     1533 2023-06-04 18:33:44.095386 bovine_store-0.2.6/bovine_store/fedi/__pycache__/retrieve_public_key.cpython-310.pyc
--rw-r--r--   0        0        0     2854 2023-06-04 18:33:44.091386 bovine_store-0.2.6/bovine_store/fedi/__pycache__/test_authorize.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3976 2023-06-04 18:33:44.095386 bovine_store-0.2.6/bovine_store/fedi/__pycache__/test_retrieve_public_key.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1021 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/fedi/authorize.py
--rw-r--r--   0        0        0     1597 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/fedi/retrieve_public_key.py
--rw-r--r--   0        0        0     2469 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/fedi/test_authorize.py
--rw-r--r--   0        0        0     3986 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/fedi/test_retrieve_public_key.py
--rw-r--r--   0        0        0     2285 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/models.py
--rw-r--r--   0        0        0     1356 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/store/__init__.py
--rw-r--r--   0        0        0     1126 2023-06-04 18:33:42.703372 bovine_store-0.2.6/bovine_store/store/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2995 2023-06-04 18:33:43.311378 bovine_store-0.2.6/bovine_store/store/__pycache__/collection.cpython-310.pyc
--rw-r--r--   0        0        0     1394 2023-06-04 18:33:43.311378 bovine_store-0.2.6/bovine_store/store/__pycache__/remote.cpython-310.pyc
--rw-r--r--   0        0        0     1636 2023-06-04 18:33:43.307378 bovine_store-0.2.6/bovine_store/store/__pycache__/retrieve_object.cpython-310.pyc
--rw-r--r--   0        0        0     2619 2023-06-04 18:33:42.931374 bovine_store-0.2.6/bovine_store/store/__pycache__/store.cpython-310.pyc
--rw-r--r--   0        0        0     1471 2023-06-04 18:33:44.103386 bovine_store-0.2.6/bovine_store/store/__pycache__/test_application_actor_data.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     7060 2023-06-04 18:33:44.115386 bovine_store-0.2.6/bovine_store/store/__pycache__/test_collection.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2714 2023-06-04 18:33:44.119386 bovine_store-0.2.6/bovine_store/store/__pycache__/test_retrieve_object.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     4796 2023-06-04 18:33:44.127386 bovine_store-0.2.6/bovine_store/store/__pycache__/test_store.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2943 2023-06-04 18:33:44.135386 bovine_store-0.2.6/bovine_store/store/__pycache__/test_store_remote.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1111 2023-06-04 18:33:44.139387 bovine_store-0.2.6/bovine_store/store/__pycache__/test_utils.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      809 2023-06-04 18:33:43.303378 bovine_store-0.2.6/bovine_store/store/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0     4394 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/store/collection.py
--rw-r--r--   0        0        0     1101 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/store/remote.py
--rw-r--r--   0        0        0     1343 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/store/retrieve_object.py
--rw-r--r--   0        0        0     2544 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/store/store.py
--rw-r--r--   0        0        0      533 2023-06-04 18:31:36.370115 bovine_store-0.2.6/bovine_store/store/test_application_actor_data.py
--rw-r--r--   0        0        0     4100 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/store/test_collection.py
--rw-r--r--   0        0        0     1657 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/store/test_retrieve_object.py
--rw-r--r--   0        0        0     3591 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/store/test_store.py
--rw-r--r--   0        0        0     1904 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/store/test_store_remote.py
--rw-r--r--   0        0        0      184 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/store/test_utils.py
--rw-r--r--   0        0        0      582 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/store/utils.py
--rw-r--r--   0        0        0     3541 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/templates/fallback.html
--rw-r--r--   0        0        0      314 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/test_bovine_admin_store.py
--rw-r--r--   0        0        0      475 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/test_store.py
--rw-r--r--   0        0        0      479 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/types.py
--rw-r--r--   0        0        0      951 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/utils/__init__.py
--rw-r--r--   0        0        0     1359 2023-06-04 18:33:43.307378 bovine_store-0.2.6/bovine_store/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1611 2023-06-04 18:33:43.311378 bovine_store-0.2.6/bovine_store/utils/__pycache__/collection.cpython-310.pyc
--rw-r--r--   0        0        0     1397 2023-06-04 18:33:44.039385 bovine_store-0.2.6/bovine_store/utils/__pycache__/ordered_collection.cpython-310.pyc
--rw-r--r--   0        0        0     1009 2023-06-04 18:33:43.307378 bovine_store-0.2.6/bovine_store/utils/__pycache__/permissions.cpython-310.pyc
--rw-r--r--   0        0        0     2660 2023-06-04 18:33:44.043386 bovine_store-0.2.6/bovine_store/utils/__pycache__/test.cpython-310.pyc
--rw-r--r--   0        0        0     1682 2023-06-04 18:33:44.143386 bovine_store-0.2.6/bovine_store/utils/__pycache__/test_path.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1381 2023-06-04 18:33:44.143386 bovine_store-0.2.6/bovine_store/utils/__pycache__/test_permissions.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1481 2023-06-04 18:33:44.147387 bovine_store-0.2.6/bovine_store/utils/__pycache__/test_summary.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1245 2023-06-04 18:33:44.151387 bovine_store-0.2.6/bovine_store/utils/__pycache__/test_test.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1124 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/utils/collection.py
--rw-r--r--   0        0        0     1288 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/utils/ordered_collection.py
--rw-r--r--   0        0        0      680 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/utils/permissions.py
--rw-r--r--   0        0        0     2231 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/utils/test.py
--rw-r--r--   0        0        0      619 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/utils/test_path.py
--rw-r--r--   0        0        0      726 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/utils/test_permissions.py
--rw-r--r--   0        0        0      294 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/utils/test_summary.py
--rw-r--r--   0        0        0      375 2023-06-04 18:31:36.374115 bovine_store-0.2.6/bovine_store/utils/test_test.py
--rw-r--r--   0        0        0      917 2023-06-04 18:31:36.374115 bovine_store-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     3553 1970-01-01 00:00:00.000000 bovine_store-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1252 2023-07-15 11:45:43.763733 bovine_store-0.3.0/README.md
+-rw-r--r--   0        0        0     6698 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/__init__.py
+-rw-r--r--   0        0        0     1465 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/actor/__init__.py
+-rw-r--r--   0        0        0    10417 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/actor/bovine_store_actor.py
+-rw-r--r--   0        0        0     1844 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/actor/register.py
+-rw-r--r--   0        0        0      731 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/actor/test_bovine_application_actor.py
+-rw-r--r--   0        0        0     5217 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/actor/test_bovine_store_actor.py
+-rw-r--r--   0        0        0     1684 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/actor/test_register.py
+-rw-r--r--   0        0        0     3798 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/models.py
+-rw-r--r--   0        0        0     1716 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/server/__init__.py
+-rw-r--r--   0        0        0     1194 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/server/authorize.py
+-rw-r--r--   0        0        0     2631 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/server/blueprint.py
+-rw-r--r--   0        0        0     1108 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/server/collection.py
+-rw-r--r--   0        0        0      843 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/server/config.py
+-rw-r--r--   0        0        0     1288 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/server/ordered_collection.py
+-rw-r--r--   0        0        0     1585 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/server/retrieve_public_key.py
+-rw-r--r--   0        0        0     3541 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/server/templates/fallback.html
+-rw-r--r--   0        0        0     2501 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/server/test_authorize.py
+-rw-r--r--   0        0        0      624 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/server/test_path.py
+-rw-r--r--   0        0        0     3986 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/server/test_retrieve_public_key.py
+-rw-r--r--   0        0        0      387 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/server/utils.py
+-rw-r--r--   0        0        0     1356 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/store/__init__.py
+-rw-r--r--   0        0        0     4375 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/store/collection.py
+-rw-r--r--   0        0        0     1101 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/store/remote.py
+-rw-r--r--   0        0        0     1343 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/store/retrieve_object.py
+-rw-r--r--   0        0        0     2544 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/store/store.py
+-rw-r--r--   0        0        0      533 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/store/test_application_actor_data.py
+-rw-r--r--   0        0        0     4100 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/store/test_collection.py
+-rw-r--r--   0        0        0     1657 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/store/test_retrieve_object.py
+-rw-r--r--   0        0        0     3591 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/store/test_store.py
+-rw-r--r--   0        0        0     1904 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/store/test_store_remote.py
+-rw-r--r--   0        0        0      184 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/store/test_utils.py
+-rw-r--r--   0        0        0      582 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/store/utils.py
+-rw-r--r--   0        0        0      314 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/test_bovine_admin_store.py
+-rw-r--r--   0        0        0      475 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/test_store.py
+-rw-r--r--   0        0        0      479 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/types.py
+-rw-r--r--   0        0        0     1073 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/utils/__init__.py
+-rw-r--r--   0        0        0      680 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/utils/permissions.py
+-rw-r--r--   0        0        0     2626 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/utils/test.py
+-rw-r--r--   0        0        0      726 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/utils/test_permissions.py
+-rw-r--r--   0        0        0      294 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/utils/test_summary.py
+-rw-r--r--   0        0        0      375 2023-07-15 11:45:43.763733 bovine_store-0.3.0/bovine_store/utils/test_test.py
+-rw-r--r--   0        0        0     1047 2023-07-15 11:46:38.108131 bovine_store-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2162 1970-01-01 00:00:00.000000 bovine_store-0.3.0/setup.py
+-rw-r--r--   0        0        0     2023 1970-01-01 00:00:00.000000 bovine_store-0.3.0/PKG-INFO
```

### Comparing `bovine_store-0.2.6/README.md` & `bovine_store-0.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: bovine-store
+Version: 0.3.0
+Summary: Store for ActivityPub activities, actors and objects
+Home-page: https://codeberg.org/bovine/bovine
+License: MIT
+Author: Helge
+Author-email: helge.krueger@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: bovine (>=0.3.0,<0.4.0)
+Requires-Dist: quart (>=0.18.3,<0.19.0)
+Requires-Dist: tortoise-orm[asyncpg] (>=0.19.3,<0.20.0)
+Project-URL: Documentation, https://bovine-store.readthedocs.io/en/latest/
+Project-URL: Repository, https://codeberg.org/bovine/bovine
+Description-Content-Type: text/markdown
+
 # bovine_store
 
 `bovine_store` is meant to be the module handling storing of
 local ActivityPub objects and caching of remote ActivityPub
 objects.
 
 ## Usage
@@ -12,38 +32,22 @@
 
 - [ ] When properties of actor are updated, send an update Activity
   - Doesn't fit into the current bovine framework ... bovine_store doesn't know how to send activities
 - [ ] Generally rework the actor properties mechanism. It is currently not possible to emulate say Mastodon featured collection with it.
 - [ ] bovine_store.models.BovineActorKeyPair needs renamings; and work, e.g. a future identity column should have a uniqueness constraint.
 - [ ] Generally the code quality is not as high as it should be.
 
-## Design discussion
-
-Some goals and design decisions:
-
-- Objects with an id are stored separately and can be looked up via this id. This is done by json-ld magic.
-- Collections are not stored. Instead for local items, the information that the item belongs to a collection is stored. `bovine_store.store.collection` contains the coroutines necessary to build the collection from this information. All collections are assumed to ActivityStreams 2 `OrderedCollection` and ordered by the database id.
-- Every object is currently assigned an `owner`. The idea was that an activity is owner by its actor. This can then be propagated to the subobjects, e.g. the object, attachments, and so on. Unfortunately, this is too naive:
-  - Some implementations include remote objects, e.g. the object being liked in a Like Activity.
-  - Mastodon includes its custom emojis. These have an id and should probably belong to the server.
-- There are three kinds of visibility.
-  - An object is always visible to its owner
-  - Public Objects are assigned `VisibilityType.PUBLIC`. These can viewed by all users providing valid authentication.
-  - Furthemore, by adding actors to the `VisibileTo` list of an object. This can be made visible to the corresponding actors.
-- An item is visible to be inside a collection if and only if said item is visible. This should probably be augmented by visible to the owner of the collection.
-- `bovine_store.blueprint` contains a quart blueprint with the basic retrievel mechanism for the stored objects.
-- `bovine_store.collection` contains the helper routine for collection responses.
-
 ## Examples
 
 A demonstration webserver can be seen using
 
 ```bash
 poetry run python examples/basic_app.py
 ```
 
 Note this is a very basic example. Instructions what the example does are
 printed to the command line after start.
 
 Note: This example creates two files `db.sqlite3`, which contains the
 database and `context_cache.sqlite`, which contains the cache of json-ld
 contexts.
+
```

### Comparing `bovine_store-0.2.6/bovine_store/__init__.py` & `bovine_store-0.3.0/bovine_store/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import aiohttp
 from urllib.parse import urljoin
 from typing import Optional, Tuple, Callable
 
+
 import bovine_store
 
 from .types import EndpointType
 from .actor.bovine_store_actor import BovineStoreActor
 from .actor.register import register
 from .models import BovineActor, BovineActorEndpoint, BovineActorKeyPair
 
 from .utils import user_to_account_and_actor_url
-from bovine_store.utils.collection import collection_response
 
 from .store import load_application_actor_data
 from .store.retrieve_object import retrieve_remote_object
 from .store.utils import domain_from_host
 
 
 class BovineStore:
@@ -90,16 +90,16 @@
         app_actor = bovine_store.actor.BovineApplicationActor(
             {**application_data, "account_url": account_url}
         )
         await app_actor.init(session=self.session)
 
         return app_actor
 
-    async def collection_response(self, collection_id):
-        return await collection_response(collection_id)
+    # async def collection_response(self, collection_id):
+    #     return await collection_response(collection_id)
 
 
 class BovineAdminStore:
     """Store for managing actors. This store should be used to create
     actor management interfaces.
 
     These can be kept separate from the actual fediverse server implementation.
```

### Comparing `bovine_store-0.2.6/bovine_store/actor/__init__.py` & `bovine_store-0.3.0/bovine_store/actor/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,32 +3,41 @@
 
 from bovine_store.types import ObjectType
 from bovine_store.store.store import store_remote_object
 from bovine_store.store.retrieve_object import retrieve_remote_object
 
 
 class BovineApplicationActor(bovine.BovineActor):
-    """Actor that represents the bovine application"""
+    """Actor that represents the bovine application,
+    used when acting on behalf of a remote actor when the affected local
+    actor is unknown.
+
+    * Retrieving public keys for authorization checks
+    """
 
     def __init__(self, config):
         config["public_key_url"] = config["account_url"] + "#main-key"
         super().__init__(config)
 
         self.actor_object = Actor(
             id=config["account_url"],
             preferred_username="bovine",
             public_key=config["public_key"],
             public_key_name="main-key",
             type="Application",
         ).build()
 
     async def store_remote_actor(self, item):
+        """Stores a remote actor. Actors are assumed to be publicly
+        readable and to own themselves"""
+
         return await store_remote_object(
             item.get("id", "NO_OWNER"),
             item,
             as_public=True,
             visible_to=[self.actor_object["id"]],
             object_type=ObjectType.REMOTE,
         )
 
     async def retrieve(self, key_url):
+        """retrieves a remote object form the database as the application actor"""
         return await retrieve_remote_object(self.actor_object["id"], key_url)
```

### Comparing `bovine_store-0.2.6/bovine_store/actor/bovine_store_actor.py` & `bovine_store-0.3.0/bovine_store/actor/bovine_store_actor.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,14 +19,19 @@
 from bovine_store.store.utils import domain_from_host
 from bovine_store.store.collection import collection_all
 
 logger = logging.getLogger(__name__)
 
 
 class BovineStoreActor(BovineActor):
+    """Represents an actor controlled by bovine and stored in the database.
+    This class should be used to perform actions as this actor. In particular,
+    instances of this class are passed to bovine_process when performing
+    side effects."""
+
     def __init__(self, config: dict, actor_object: Actor, endpoints: List[str] = []):
         self.actor_object: Actor = actor_object
 
         self.domain = domain_from_host(actor_object.id)
         self.endpoints = endpoints
 
         super().__init__(config)
@@ -36,15 +41,27 @@
         result = await StoredJsonObject.get_or_none(id=object_id)
         if not result:
             return None
         if result.owner != self.actor_object.id:
             return None
         return result.content
 
-    async def retrieve(self, object_id: str, include=[], skip_fetch: bool = False):
+    async def retrieve(
+        self, object_id: str, include=[], skip_fetch: bool = False
+    ) -> dict | None:
+        """Retrieves the object with identified by object_id. The logic is
+        as follows:
+
+        * If object is in database and either local or remote and last updated
+            in the last day, the object is returned from the database
+        * Otherwise the object is fetched (as the actor) unless skip_fetch is set
+        * Finally if include lists properties to be resolved, these objects
+            are obtained using the above logic, and then added to the Object
+
+        """
         data = await self._retrieve_object_from_database(
             object_id, skip_fetch=skip_fetch
         )
 
         if data is None:
             return data
 
@@ -96,30 +113,37 @@
         except Exception as ex:
             logger.info("Failed to retrieve %s with %s", object_id, ex)
             for log_line in traceback.format_exc().splitlines():
                 logger.info(log_line)
 
             return None
 
-    async def store(self, item, as_public: bool = False, visible_to=[]):
+    async def store(self, item: dict, as_public: bool = False, visible_to=[]):
+        """Stores object in database"""
         return await store_remote_object(
             self.actor_id,
             item,
             as_public=as_public,
             visible_to=visible_to,
             object_type=ObjectType.LOCAL,
         )
 
-    async def update(self, item):
+    async def update(self, item: dict):
+        """Updates object in database"""
         await update_remote_object(self.actor_object.id, item)
 
     async def retrieve_for(self, retriever, object_id, include=[]):
         return await retrieve_remote_object(retriever, object_id, include=include)
 
-    async def store_for(self, owner, item, as_public=False, visible_to=[]):
+    async def store_for(self, owner: str, item: dict, as_public=False, visible_to=[]):
+        """Stores a remote object
+
+        :param owner: The actor who has submitted the object
+        :param item: The object to store"""
+
         return await store_remote_object(
             owner, item, as_public=as_public, visible_to=visible_to, domain=self.domain
         )
 
     async def update_for(self, owner, item):
         return await update_remote_object(owner, item)
 
@@ -142,21 +166,39 @@
         return await CollectionItem.create(
             part_of=self.actor_object.following, object_id=object_id
         )
 
     async def add_to_interaction(
         self, interaction: str, object_id: str, remote_id: str
     ):
+        """Adds to an interaction collection
+
+        :param interaction:
+            The interaction either replies, shares, or likes
+        :param object_id:
+            id of the object being interacted with
+        :param remote_id:
+            id of the interaction, e.g. of the Like or Dislike
+        """
         return await CollectionItem.create(
             part_of=f"{object_id}/{interaction}", object_id=remote_id
         )
 
     async def remove_from_interaction(
         self, interaction: str, object_id: str, remote_id: str
     ):
+        """Removes an interaction from the corresponding collection
+
+        :param interaction:
+            The interaction either replies, shares, or likes
+        :param object_id:
+            id of the object being interacted with
+        :param remote_id:
+            id of the interaction, e.g. of the Like or Dislike
+        """
         obj = await CollectionItem.get_or_none(
             part_of=f"{object_id}/{interaction}", object_id=remote_id
         )
         if obj:
             await obj.delete()
 
     async def remove_references(self, remote_id: str):
@@ -171,14 +213,18 @@
         result = await asyncio.gather(*tasks)
         result = set(sum(result, []))
 
         logger.info("Resolved %s to %s", ", ".join(endpoints), ", ".join(result))
         return result
 
     def generate_new_object_id(self) -> str:
+        """Creates a new object id
+
+        This contains a hard coded path; probably should replace with something better.
+        """
         return urljoin(self.actor_object.id, "/objects/" + str(uuid.uuid4()))
 
     @staticmethod
     def _is_stale(result):
         if result is None:
             return True
         if result.object_type == ObjectType.LOCAL:
@@ -186,58 +232,66 @@
 
         updated = result.updated
         updated = updated.replace(tzinfo=timezone.utc)
 
         return updated < (datetime.now(tz=timezone.utc) - timedelta(days=1))
 
     @staticmethod
-    async def from_database(user, session):
-        mapped_endpoints = {x.endpoint_type: x for x in user.endpoints}
+    async def from_database(stored_actor, session):
+        """Creates BovineStoreAction from database object
+
+        :param stored_actor:
+            The BovineActor object from the database
+        :param session:
+            An aiohttp.ClientSession"""
+        mapped_endpoints = {x.endpoint_type: x for x in stored_actor.endpoints}
         account_url = mapped_endpoints[EndpointType.ACTOR].name
 
-        def get_server_key(user):
-            for iter_keypair in user.keypairs:
+        def get_server_key(stored_actor):
+            for iter_keypair in stored_actor.keypairs:
                 if iter_keypair.name == "serverKey":
                     return iter_keypair
-            return user.keypairs[0]
+            return stored_actor.keypairs[0]
 
-        keypair = get_server_key(user)
+        keypair = get_server_key(stored_actor)
         public_key_url = f"{account_url}#{keypair.name}"
 
         config = {
             "account_url": account_url,
             "public_key_url": public_key_url,
             "private_key": keypair.private_key,
         }
 
         endpoints = [
             x.name
-            for x in user.endpoints
+            for x in stored_actor.endpoints
             if x.endpoint_type in [EndpointType.FOLLOWERS, EndpointType.COLLECTION]
         ]
 
         actor_object = Actor(
             id=account_url,
-            preferred_username=user.handle_name,
+            preferred_username=stored_actor.handle_name,
             inbox=mapped_endpoints[EndpointType.INBOX].name,
             outbox=mapped_endpoints[EndpointType.OUTBOX].name,
             event_source=mapped_endpoints[EndpointType.EVENT_SOURCE].name,
             followers=mapped_endpoints[EndpointType.FOLLOWERS].name,
             following=mapped_endpoints[EndpointType.FOLLOWING].name,
             proxy_url=mapped_endpoints[EndpointType.PROXY_URL].name,
             public_key=keypair.public_key,
             public_key_name=keypair.name,
         )
 
-        if "type" in user.properties:
-            actor_object.type = user.properties["type"]
-        if "name" in user.properties:
-            actor_object.name = user.properties["name"]
-        if "summary" in user.properties:
-            actor_object.summary = user.properties["summary"]
-        if "icon" in user.properties:
-            actor_object.icon = user.properties["icon"]
+        if "type" in stored_actor.properties:
+            actor_object.type = stored_actor.properties["type"]
+        if "name" in stored_actor.properties:
+            actor_object.name = stored_actor.properties["name"]
+        if "summary" in stored_actor.properties:
+            actor_object.summary = stored_actor.properties["summary"]
+        if "icon" in stored_actor.properties:
+            actor_object.icon = stored_actor.properties["icon"]
+        if "url" in stored_actor.properties:
+            actor_object.url = stored_actor.properties["url"]
 
         actor = BovineStoreActor(config, actor_object, endpoints=endpoints)
         await actor.init(session=session)
 
         return actor
```

### Comparing `bovine_store-0.2.6/bovine_store/actor/register.py` & `bovine_store-0.3.0/bovine_store/actor/register.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/bovine_store/actor/test_bovine_application_actor.py` & `bovine_store-0.3.0/bovine_store/actor/test_bovine_application_actor.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/bovine_store/actor/test_bovine_store_actor.py` & `bovine_store-0.3.0/bovine_store/actor/test_bovine_store_actor.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/bovine_store/actor/test_register.py` & `bovine_store-0.3.0/bovine_store/actor/test_register.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/bovine_store/blueprint.py` & `bovine_store-0.3.0/bovine_store/server/blueprint.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
 
 from quart import Blueprint, g, request, current_app, render_template, redirect
 
-from .utils import determine_summary, path_from_request
-from .utils.collection import add_sub_collections
-from .fedi.authorize import add_authorization
+from bovine_store.utils import determine_summary, add_sub_collections
+
+from .collection import collection_response
+from .utils import path_from_request
 
 logger = logging.getLogger(__name__)
 
 bovine_store_blueprint = Blueprint(
     "bovine_store", __name__, template_folder="templates"
 )
-bovine_store_blueprint.before_request(add_authorization)
 
 
 @bovine_store_blueprint.get("/<uuid>")
 async def retrieve_from_store(uuid):
     logger.info("Request for uuid %s at %s", uuid, request.url)
 
     object_path = path_from_request(request)
@@ -85,8 +85,8 @@
 
     store = current_app.config["bovine_store"]
     obj = await store.retrieve_for_get(g.retriever, object_path)
 
     if not obj:
         return {"status": "unauthorized"}, 401
 
-    return await store.collection_response(endpoint_path)
+    return await collection_response(endpoint_path)
```

### Comparing `bovine_store-0.2.6/bovine_store/config.py` & `bovine_store-0.3.0/bovine_store/server/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import aiohttp
 from quart import Quart
 
 from bovine.crypto import build_validate_http_signature
 
-from . import BovineStore
-from .fedi.retrieve_public_key import retrieve_public_key
+from bovine_store import BovineStore
+from .retrieve_public_key import retrieve_public_key
 
 
 async def configure_bovine_store(app: Quart):
-    """configures the quart app with a bovine_store"""
     if "session" not in app.config:
         app.config["session"] = aiohttp.ClientSession()
 
     app.config["bovine_store"] = BovineStore(
         session=app.config["session"],
     )
```

### Comparing `bovine_store-0.2.6/bovine_store/fedi/authorize.py` & `bovine_store-0.3.0/bovine_store/server/authorize.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,17 +23,19 @@
         didkey
     )
 
     return actor_id
 
 
 async def add_authorization():
-    if g.get("retriever"):
+    """Adds the retriever to g.retriever based on the HTTP Signature"""
+    if request.path.startswith("/activitypub"):
+        g.retriever = None
         return
 
-    if "authorization" in request.headers and request.headers[
-        "authorization"
-    ].startswith("Moo-Auth-1"):
-        g.retriever = await compute_moo_auth_result()
-        return
-
-    g.retriever = await current_app.config["validate_http_signature"](request)
+    if not g.get("retriever"):
+        if "authorization" in request.headers and request.headers[
+            "authorization"
+        ].startswith("Moo-Auth-1"):
+            g.retriever = await compute_moo_auth_result()
+        else:
+            g.retriever = await current_app.config["validate_http_signature"](request)
```

### Comparing `bovine_store-0.2.6/bovine_store/fedi/retrieve_public_key.py` & `bovine_store-0.3.0/bovine_store/server/retrieve_public_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from typing import Tuple
 from quart import current_app, request
 
 from bovine.jsonld import value_from_object
-from bovine_store.utils import path_from_request
+from .utils import path_from_request
 
 logger = logging.getLogger(__name__)
 
 
 async def refetch_public_key(app_actor, store, key_url: str) -> dict | None:
     data = await app_actor.get(key_url, fail_silently=True)
     if data is None:
```

### Comparing `bovine_store-0.2.6/bovine_store/fedi/test_authorize.py` & `bovine_store-0.3.0/bovine_store/server/test_authorize.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,16 +25,16 @@
         "acct:name",
         "mock",
     )
 
     headers = {
         "Date": "Wed, 15 Mar 2023 17:28:15 GMT",
         "Host": "myhost.tld",
-        "Authorization": "Moo-Auth-1 did:key:z6MkekwC6R9bj9ErToB7AiZJfyCSDhaZe1UxhDbCqJrhqpS5",
-        "X-Moo-Signature": "z5ahdHCbP9aJEsDtvG1MEZpxPzuvGKYcdXdKvMq5YL21Z2umxjs1SopCY2Ap8vZxVjTEf6dYbGuB7mtgcgUyNdBLe",
+        "Authorization": "Moo-Auth-1 did:key:z6MkekwC6R9bj9ErToB7AiZJfyCSDhaZe1UxhDbCqJrhqpS5",  # noqa
+        "X-Moo-Signature": "z5ahdHCbP9aJEsDtvG1MEZpxPzuvGKYcdXdKvMq5YL21Z2umxjs1SopCY2Ap8vZxVjTEf6dYbGuB7mtgcgUyNdBLe",  # noqa
     }
     async with test_app.test_request_context(
         "/path/to/resource", method="GET", headers=headers
     ):
         await add_authorization()
 
         assert g.retriever == "mock"
@@ -51,16 +51,16 @@
         "mock",
     )
 
     headers = {
         "Date": "Wed, 15 Mar 2023 17:28:15 GMT",
         "Host": "myhost.tld",
         "Digest": "sha-256=MILb5lUDD6Z0pDSxhgxj+hMBEw0uTzP3g2qUJGHMp9k=",
-        "Authorization": "Moo-Auth-1 did:key:z6MkekwC6R9bj9ErToB7AiZJfyCSDhaZe1UxhDbCqJrhqpS5",
-        "X-Moo-Signature": "z4vPkJaoaSVQp5DrMb8EvCajJcerW36rsyWDELTWQ3cYmaonnGfb8WHiwH54BShidCcmpoyHjanVRYNrXXXka4jAn",
+        "Authorization": "Moo-Auth-1 did:key:z6MkekwC6R9bj9ErToB7AiZJfyCSDhaZe1UxhDbCqJrhqpS5",  # noqa
+        "X-Moo-Signature": "z4vPkJaoaSVQp5DrMb8EvCajJcerW36rsyWDELTWQ3cYmaonnGfb8WHiwH54BShidCcmpoyHjanVRYNrXXXka4jAn",  # noqa
     }
     async with test_app.test_request_context(
         "/path/to/resource", method="POST", headers=headers, json={"cows": "good"}
     ):
         await add_authorization()
 
         assert g.retriever == "mock"
```

### Comparing `bovine_store-0.2.6/bovine_store/fedi/test_retrieve_public_key.py` & `bovine_store-0.3.0/bovine_store/server/test_retrieve_public_key.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/bovine_store/store/__init__.py` & `bovine_store-0.3.0/bovine_store/store/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/bovine_store/store/collection.py` & `bovine_store-0.3.0/bovine_store/store/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,16 +72,14 @@
         query = query.filter(id__lt=min_id).order_by("-id")
     elif kwargs.get("max_id"):
         max_id = int(kwargs.get("max_id"))
         query = query.filter(id__gt=max_id).order_by("id")
 
     result = await query.limit(limit).all()
 
-    print(result)
-
     next_prev = {}
     if len(result) > 0:
         min_id = max(x.id for x in result)
         max_id = min(x.id for x in result)
         next_prev = {
             "prev": f"max_id={min_id}",
             "next": f"min_id={max_id}",
```

### Comparing `bovine_store-0.2.6/bovine_store/store/remote.py` & `bovine_store-0.3.0/bovine_store/store/remote.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/bovine_store/store/retrieve_object.py` & `bovine_store-0.3.0/bovine_store/store/retrieve_object.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/bovine_store/store/store.py` & `bovine_store-0.3.0/bovine_store/store/store.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/bovine_store/store/test_application_actor_data.py` & `bovine_store-0.3.0/bovine_store/store/test_application_actor_data.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/bovine_store/store/test_collection.py` & `bovine_store-0.3.0/bovine_store/store/test_collection.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/bovine_store/store/test_retrieve_object.py` & `bovine_store-0.3.0/bovine_store/store/test_retrieve_object.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/bovine_store/store/test_store.py` & `bovine_store-0.3.0/bovine_store/store/test_store.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/bovine_store/store/test_store_remote.py` & `bovine_store-0.3.0/bovine_store/store/test_store_remote.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/bovine_store/store/utils.py` & `bovine_store-0.3.0/bovine_store/store/utils.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/bovine_store/templates/fallback.html` & `bovine_store-0.3.0/bovine_store/server/templates/fallback.html`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/bovine_store/utils/collection.py` & `bovine_store-0.3.0/bovine_store/server/collection.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 
 from .ordered_collection import ordered_collection_responder
 from bovine_store.store.collection import collection_count, collection_items
 
 logger = logging.getLogger(__name__)
 
 
-async def collection_response(endpoint_path):
+async def collection_response(endpoint_path: str):
+    """Returns the response for a GET request to the endpoint path.
+
+    The endpoint_path is assumed to represent an ordered collection.
+    The GET request can have the query parameters `first`, `last`,
+    `mind_id`, `max_id` that are treated according to FIXME."""
     arguments = {
         name: request.args.get(name)
         for name in ["first", "last", "min_id", "max_id"]
         if request.args.get(name) is not None
     }
 
     logger.info("Retrieving %s for %s", endpoint_path, g.retriever)
@@ -25,19 +30,7 @@
 
     return await ordered_collection_responder(
         endpoint_path,
         ccount,
         citems,
         **arguments,
     )
-
-
-def add_sub_collections(obj: dict) -> dict:
-    obj_type = obj.get("type")
-    obj_id = obj.get("id")
-    if obj_type not in ["Note", "Article", "Page"] or not obj_id:
-        return obj
-
-    for key in ["replies", "shares", "likes"]:
-        obj[key] = f"{obj_id}/{key}"
-
-    return obj
```

### Comparing `bovine_store-0.2.6/bovine_store/utils/ordered_collection.py` & `bovine_store-0.3.0/bovine_store/server/ordered_collection.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/bovine_store/utils/permissions.py` & `bovine_store-0.3.0/bovine_store/utils/permissions.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/bovine_store/utils/test.py` & `bovine_store-0.3.0/bovine_store/utils/test.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from dataclasses import dataclass
 from unittest.mock import AsyncMock
 import pytest
 from tortoise import Tortoise, connections
 from quart import Quart
 
 from bovine_store import BovineStore, BovineAdminStore
-from bovine_store.blueprint import bovine_store_blueprint
+from bovine_store.server.authorize import add_authorization
+from bovine_store.server.blueprint import bovine_store_blueprint
 
 
 async def init_connection(db_url):
     await Tortoise.init(db_url=db_url, modules={"models": ["bovine_store.models"]})
     await Tortoise.generate_schemas()
 
 
@@ -29,17 +30,22 @@
 
 @pytest.fixture
 async def store():
     if not os.environ.get("POSTGRES"):
         db_file = "test_db.db"
         db_url = f"sqlite://{db_file}"
 
+        response_mock = AsyncMock()
+        response_mock.raise_for_status = lambda: 1
+        session_mock = AsyncMock()
+        session_mock.get.return_value = response_mock
+
         store = BovineStore(
             db_url,
-            session=AsyncMock(),
+            session=session_mock,
         )
 
         await init_connection(db_url)
 
         yield store
         await close_connection()
         os.unlink(db_file)
@@ -86,10 +92,16 @@
     app = Quart(__name__)
 
     app.config["bovine_store"] = store
     app.config["session"] = store.session
 
     app.config["validate_http_signature"] = AsyncMock(return_value="owner")
 
+    try:  # FIXME
+        bovine_store_blueprint.before_request(add_authorization)
+    except Exception:
+        ...
     app.register_blueprint(bovine_store_blueprint)
 
     yield app
+
+    await store.session.close()
```

### Comparing `bovine_store-0.2.6/bovine_store/utils/test_path.py` & `bovine_store-0.3.0/bovine_store/server/test_path.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest.mock import MagicMock
 
-from . import path_from_request
+from .utils import path_from_request
 
 
 def test_path_from_request():
     request = MagicMock(url="http://localhost/some/path", headers={})
 
     assert path_from_request(request) == "http://localhost/some/path"
```

### Comparing `bovine_store-0.2.6/bovine_store/utils/test_permissions.py` & `bovine_store-0.3.0/bovine_store/utils/test_permissions.py`

 * *Files identical despite different names*

### Comparing `bovine_store-0.2.6/pyproject.toml` & `bovine_store-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "bovine-store"
-version = "0.2.6"
+version = "0.3.0"
 description = "Store for ActivityPub activities, actors and objects"
 authors = ["Helge <helge.krueger@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bovine_store"}]
 repository = "https://codeberg.org/bovine/bovine"
+documentation = "https://bovine-store.readthedocs.io/en/latest/"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 tortoise-orm = {extras = ["asyncpg"], version = "^0.19.3"}
 quart = "^0.18.3"
-bovine = "^0.2.1"
+bovine = "^0.3.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 black = "^23.1.0"
 isort = "^5.12.0"
 pytest-asyncio = "^0.20.3"
 mypy = "^1.1.1"
@@ -31,10 +32,13 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode="auto"
 log_cli= 1
 log_cli_level="info"
+filterwarnings = [
+    'ignore:.*Werkzeug:DeprecationWarning',
+]
 
 [tool.ruff.per-file-ignores]
 "bovine_store/fedi/test_authorize.py" = ["E501"]
```

