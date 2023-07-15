# Comparing `tmp/osmapi-3.1.0.tar.gz` & `tmp/osmapi-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osmapi-3.1.0.tar", last modified: Wed Jan 18 12:55:34 2023, max compression
+gzip compressed data, was "osmapi-4.0.0.tar", last modified: Sat Jul 15 21:40:09 2023, max compression
```

## Comparing `osmapi-3.1.0.tar` & `osmapi-4.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 12:55:34.712251 osmapi-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-01-18 12:55:25.000000 osmapi-3.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-18 12:55:25.000000 osmapi-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-01-18 12:55:34.712251 osmapi-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-01-18 12:55:25.000000 osmapi-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 12:55:34.708251 osmapi-3.1.0/osmapi/
--rw-r--r--   0 runner    (1001) docker     (123)    65917 2023-01-18 12:55:25.000000 osmapi-3.1.0/osmapi/OsmApi.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-01-18 12:55:25.000000 osmapi-3.1.0/osmapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-01-18 12:55:25.000000 osmapi-3.1.0/osmapi/dom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-01-18 12:55:25.000000 osmapi-3.1.0/osmapi/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-01-18 12:55:25.000000 osmapi-3.1.0/osmapi/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-01-18 12:55:25.000000 osmapi-3.1.0/osmapi/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-01-18 12:55:25.000000 osmapi-3.1.0/osmapi/xmlbuilder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 12:55:34.712251 osmapi-3.1.0/osmapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-01-18 12:55:33.000000 osmapi-3.1.0/osmapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-01-18 12:55:34.000000 osmapi-3.1.0/osmapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-18 12:55:33.000000 osmapi-3.1.0/osmapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-18 12:55:33.000000 osmapi-3.1.0/osmapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-18 12:55:33.000000 osmapi-3.1.0/osmapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-01-18 12:55:34.712251 osmapi-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-01-18 12:55:25.000000 osmapi-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-18 12:55:34.712251 osmapi-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-18 12:55:25.000000 osmapi-3.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-01-18 12:55:25.000000 osmapi-3.1.0/tests/capabilities_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22601 2023-01-18 12:55:25.000000 osmapi-3.1.0/tests/changeset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-01-18 12:55:25.000000 osmapi-3.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-01-18 12:55:25.000000 osmapi-3.1.0/tests/dom_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-01-18 12:55:25.000000 osmapi-3.1.0/tests/helper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-01-18 12:55:25.000000 osmapi-3.1.0/tests/node_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-01-18 12:55:25.000000 osmapi-3.1.0/tests/notes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-01-18 12:55:25.000000 osmapi-3.1.0/tests/osmapi_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10321 2023-01-18 12:55:25.000000 osmapi-3.1.0/tests/relation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-01-18 12:55:25.000000 osmapi-3.1.0/tests/way_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:40:09.484099 osmapi-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-15 21:39:57.000000 osmapi-4.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-15 21:39:57.000000 osmapi-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-15 21:40:09.484099 osmapi-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-15 21:39:57.000000 osmapi-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:40:09.484099 osmapi-4.0.0/osmapi/
+-rw-r--r--   0 runner    (1001) docker     (123)    65334 2023-07-15 21:39:57.000000 osmapi-4.0.0/osmapi/OsmApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-15 21:39:57.000000 osmapi-4.0.0/osmapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-15 21:39:57.000000 osmapi-4.0.0/osmapi/dom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-15 21:39:57.000000 osmapi-4.0.0/osmapi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-07-15 21:39:57.000000 osmapi-4.0.0/osmapi/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-15 21:39:57.000000 osmapi-4.0.0/osmapi/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-07-15 21:39:57.000000 osmapi-4.0.0/osmapi/xmlbuilder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:40:09.484099 osmapi-4.0.0/osmapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-15 21:40:09.000000 osmapi-4.0.0/osmapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-15 21:40:09.000000 osmapi-4.0.0/osmapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 21:40:09.000000 osmapi-4.0.0/osmapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 21:40:09.000000 osmapi-4.0.0/osmapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-15 21:40:09.000000 osmapi-4.0.0/osmapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-15 21:40:09.488098 osmapi-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-15 21:39:57.000000 osmapi-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 21:40:09.484099 osmapi-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 21:39:57.000000 osmapi-4.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-15 21:39:57.000000 osmapi-4.0.0/tests/capabilities_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21969 2023-07-15 21:39:57.000000 osmapi-4.0.0/tests/changeset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-15 21:39:57.000000 osmapi-4.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-15 21:39:57.000000 osmapi-4.0.0/tests/dom_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-15 21:39:57.000000 osmapi-4.0.0/tests/helper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-07-15 21:39:57.000000 osmapi-4.0.0/tests/node_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-07-15 21:39:57.000000 osmapi-4.0.0/tests/notes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-15 21:39:57.000000 osmapi-4.0.0/tests/osmapi_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-07-15 21:39:57.000000 osmapi-4.0.0/tests/relation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-07-15 21:39:57.000000 osmapi-4.0.0/tests/way_test.py
```

### Comparing `osmapi-3.1.0/LICENSE.txt` & `osmapi-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osmapi-3.1.0/PKG-INFO` & `osmapi-4.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: osmapi
-Version: 3.1.0
+Version: 4.0.0
 Summary: Python wrapper for the OSM API
 Home-page: https://github.com/metaodi/osmapi
 Author: Etienne Chové
 Author-email: chove@crans.org
 Maintainer: Stefan Oderbolz
 Maintainer-email: odi@metaodi.ch
 License: GPLv3
-Download-URL: https://github.com/metaodi/osmapi/archive/v3.1.0.zip
+Download-URL: https://github.com/metaodi/osmapi/archive/v4.0.0.zip
 Description: osmapi
         ======
         
         [![Build osmapi](https://github.com/metaodi/osmapi/actions/workflows/build.yml/badge.svg)](https://github.com/metaodi/osmapi/actions/workflows/build.yml)
         [![Coverage](https://img.shields.io/coveralls/metaodi/osmapi/develop.svg)](https://coveralls.io/r/metaodi/osmapi?branch=develop)
+        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         [![Version](https://img.shields.io/pypi/v/osmapi.svg)](https://pypi.python.org/pypi/osmapi/)
         [![License](https://img.shields.io/pypi/l/osmapi.svg)](https://github.com/metaodi/osmapi/blob/master/LICENSE.txt)
         
-        Python wrapper for the OSM API (requires Python >= 3.7)
+        Python wrapper for the OSM API (requires Python >= 3.8)
         
         ## Installation
         
         Install [`osmapi` from PyPi](https://pypi.python.org/pypi/osmapi) by using pip: 
         
             pip install osmapi
         
@@ -84,17 +85,25 @@
         ### Development
         
         If you want to help with the development of `osmapi`, you should clone this repository and install the requirements:
         
             pip install -r requirements.txt
             pip install -r test-requirements.txt
         
-        After that, it is recommended to install the `flake8` pre-commit-hook:
+        After that, it is recommended to install the pre-commit-hooks (flake8, black):
         
-            flake8 --install-hook
+            pre-commit install
+        
+        You can lint the source code using this command:
+        
+            make lint
+        
+        And if you want to reformat the files (using the black code style) simply run:
+        
+            make format
         
         ### Tests
         
         To run the tests use the following command:
         
             make test
         
@@ -120,13 +129,13 @@
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `osmapi-3.1.0/README.md` & `osmapi-4.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 osmapi
 ======
 
 [![Build osmapi](https://github.com/metaodi/osmapi/actions/workflows/build.yml/badge.svg)](https://github.com/metaodi/osmapi/actions/workflows/build.yml)
 [![Coverage](https://img.shields.io/coveralls/metaodi/osmapi/develop.svg)](https://coveralls.io/r/metaodi/osmapi?branch=develop)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Version](https://img.shields.io/pypi/v/osmapi.svg)](https://pypi.python.org/pypi/osmapi/)
 [![License](https://img.shields.io/pypi/l/osmapi.svg)](https://github.com/metaodi/osmapi/blob/master/LICENSE.txt)
 
-Python wrapper for the OSM API (requires Python >= 3.7)
+Python wrapper for the OSM API (requires Python >= 3.8)
 
 ## Installation
 
 Install [`osmapi` from PyPi](https://pypi.python.org/pypi/osmapi) by using pip: 
 
     pip install osmapi
 
@@ -73,17 +74,25 @@
 ### Development
 
 If you want to help with the development of `osmapi`, you should clone this repository and install the requirements:
 
     pip install -r requirements.txt
     pip install -r test-requirements.txt
 
-After that, it is recommended to install the `flake8` pre-commit-hook:
+After that, it is recommended to install the pre-commit-hooks (flake8, black):
 
-    flake8 --install-hook
+    pre-commit install
+
+You can lint the source code using this command:
+
+    make lint
+
+And if you want to reformat the files (using the black code style) simply run:
+
+    make format
 
 ### Tests
 
 To run the tests use the following command:
 
     make test
```

### Comparing `osmapi-3.1.0/osmapi/OsmApi.py` & `osmapi-4.0.0/osmapi/OsmApi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 """
 The OsmApi module is a wrapper for the OpenStreetMap API.
 As such it provides an easy access to the functionality of the API.
 
 You can find this module [on PyPI](https://pypi.python.org/pypi/osmapi)
 or [on GitHub](https://github.com/metaodi/osmapi).
 
@@ -45,27 +43,29 @@
 logger = logging.getLogger(__name__)
 
 
 class OsmApi:
     """
     Main class of osmapi, instanciate this class to use osmapi
     """
+
     def __init__(
-            self,
-            username=None,
-            password=None,
-            passwordfile=None,
-            appid="",
-            created_by="osmapi/%s" % __version__,
-            api="https://www.openstreetmap.org",
-            changesetauto=False,
-            changesetautotags={},
-            changesetautosize=500,
-            changesetautomulti=1,
-            session=None):
+        self,
+        username=None,
+        password=None,
+        passwordfile=None,
+        appid="",
+        created_by=f"osmapi/{__version__}",
+        api="https://www.openstreetmap.org",
+        changesetauto=False,
+        changesetautotags={},
+        changesetautosize=500,
+        changesetautomulti=1,
+        session=None,
+    ):
         """
         Initialized the OsmApi object.
 
         There are two different ways to authenticate a user.
         Either `username` and `password` are supplied directly or the path
         to a `passwordfile` is given, where on the first line username
         and password must be colon-separated (<user>:<pass>).
@@ -98,26 +98,26 @@
         # Get username
         self._username = None
         if username:
             self._username = username
         elif passwordfile:
             with open(passwordfile) as f:
                 pass_line = f.readline()
-            self._username = pass_line.split(":")[0].strip()
+            self._username = pass_line.partition(":")[0].strip()
 
         # Get password
         self._password = None
         if password:
             self._password = password
         elif passwordfile:
             with open(passwordfile) as f:
                 for line in f:
-                    line = line.strip().split(":", 1)
-                    if line[0] == self._username:
-                        self._password = line[1]
+                    key, _, value = line.strip().partition(":")
+                    if key == self._username:
+                        self._password = value
 
         # Changest informations
         # auto create and close changesets
         self._changesetauto = changesetauto
         # tags for automatic created changesets
         self._changesetautotags = changesetautotags
         # change count for auto changeset
@@ -127,42 +127,37 @@
         # close a changeset every # upload
         self._changesetautomulti = changesetautomulti
         self._changesetautocpt = 0
         # data to upload for auto group
         self._changesetautodata = []
 
         # Get API
-        self._api = api.strip('/')
+        self._api = api.strip("/")
 
         # Get created_by
         if not appid:
             self._created_by = created_by
         else:
-            self._created_by = "%s (%s)" % (appid, created_by)
+            self._created_by = f"{appid} ({created_by})"
 
         # Initialisation
         self._CurrentChangesetId = 0
 
         # Http connection
         self.http_session = session
         auth = None
         if self._username and self._password:
             auth = (self._username, self._password)
         self._session = http.OsmApiSession(
-            self._api,
-            self._created_by,
-            auth=auth,
-            session=self.http_session
+            self._api, self._created_by, auth=auth, session=self.http_session
         )
 
     def __enter__(self):
         self._session = http.OsmApiSession(
-            self._api,
-            self._created_by,
-            session=self.http_session
+            self._api, self._created_by, session=self.http_session
         )
         return self
 
     def __exit__(self, *args):
         self.close()
 
     def close(self):
@@ -257,17 +252,17 @@
 
         If the requested element has been deleted,
         `OsmApi.ElementDeletedApiError` is raised.
 
         If the requested element can not be found,
         `OsmApi.ElementNotFoundApiError` is raised.
         """
-        uri = "/api/0.6/node/%s" % (NodeId)
+        uri = f"/api/0.6/node/{NodeId}"
         if NodeVersion != -1:
-            uri += "/%s" % (NodeVersion)
+            uri += f"/{NodeVersion}"
         data = self._session._get(uri)
         data = dom.OsmResponseToDom(data, tag="node", single=True)
         return dom.DomParseNode(data)
 
     def NodeCreate(self, NodeData):
         """
         Creates a node based on the supplied `NodeData` dict:
@@ -407,15 +402,15 @@
                 '1': dict of NodeData,
                 '2': dict of NodeData,
                 ...
             }
 
         `NodeId` is the unique identifier of a node.
         """
-        uri = "/api/0.6/node/%s/history" % NodeId
+        uri = f"/api/0.6/node/{NodeId}/history"
         data = self._session._get(uri)
         nodes = dom.OsmResponseToDom(data, tag="node")
         result = {}
         for node in nodes:
             data = dom.DomParseNode(node)
             result[data["version"]] = data
         return result
@@ -439,15 +434,15 @@
                 {
                     ...
                 },
             ]
 
         The `NodeId` is a unique identifier for a node.
         """
-        uri = "/api/0.6/node/%d/ways" % NodeId
+        uri = f"/api/0.6/node/{NodeId}/ways"
         data = self._session._get(uri)
         ways = dom.OsmResponseToDom(data, tag="way", allow_empty=True)
         result = []
         for way in ways:
             data = dom.DomParseWay(way)
             result.append(data)
         return result
@@ -480,15 +475,15 @@
                 {
                     ...
                 },
             ]
 
         The `NodeId` is a unique identifier for a node.
         """
-        uri = "/api/0.6/node/%d/relations" % NodeId
+        uri = f"/api/0.6/node/{NodeId}/relations"
         data = self._session._get(uri)
         relations = dom.OsmResponseToDom(data, tag="relation", allow_empty=True)
         result = []
         for relation in relations:
             data = dom.DomParseRelation(relation)
             result.append(data)
         return result
@@ -505,15 +500,15 @@
                 ...
             }
 
         `NodeIdList` is a list containing unique identifiers
         for multiple nodes.
         """
         node_list = ",".join([str(x) for x in NodeIdList])
-        uri = "/api/0.6/nodes?nodes=%s" % node_list
+        uri = f"/api/0.6/nodes?nodes={node_list}"
         data = self._session._get(uri)
         nodes = dom.OsmResponseToDom(data, tag="node")
         result = {}
         for node in nodes:
             data = dom.DomParseNode(node)
             result[data["id"]] = data
         return result
@@ -544,17 +539,17 @@
 
         If the requested element has been deleted,
         `OsmApi.ElementDeletedApiError` is raised.
 
         If the requested element can not be found,
         `OsmApi.ElementNotFoundApiError` is raised.
         """
-        uri = "/api/0.6/way/%s" % (WayId)
+        uri = f"/api/0.6/way/{WayId}"
         if WayVersion != -1:
-            uri += "/%s" % (WayVersion)
+            uri += f"/{WayVersion}"
         data = self._session._get(uri)
         way = dom.OsmResponseToDom(data, tag="way", single=True)
         return dom.DomParseWay(way)
 
     def WayCreate(self, WayData):
         """
         Creates a way based on the supplied `WayData` dict:
@@ -691,15 +686,15 @@
                 '1': dict of WayData,
                 '2': dict of WayData,
                 ...
             }
 
         `WayId` is the unique identifier of a way.
         """
-        uri = "/api/0.6/way/%s/history" % (WayId)
+        uri = f"/api/0.6/way/{WayId}/history"
         data = self._session._get(uri)
         ways = dom.OsmResponseToDom(data, tag="way")
         result = {}
         for way in ways:
             data = dom.DomParseWay(way)
             result[data["version"]] = data
         return result
@@ -732,15 +727,15 @@
                 {
                     ...
                 },
             ]
 
         The `WayId` is a unique identifier for a way.
         """
-        uri = "/api/0.6/way/%d/relations" % WayId
+        uri = f"/api/0.6/way/{WayId}/relations"
         data = self._session._get(uri)
         relations = dom.OsmResponseToDom(data, tag="relation", allow_empty=True)
         result = []
         for relation in relations:
             data = dom.DomParseRelation(relation)
             result.append(data)
         return result
@@ -762,15 +757,15 @@
 
         If the requested element has been deleted,
         `OsmApi.ElementDeletedApiError` is raised.
 
         If the requested element can not be found,
         `OsmApi.ElementNotFoundApiError` is raised.
         """
-        uri = "/api/0.6/way/%s/full" % (WayId)
+        uri = f"/api/0.6/way/{WayId}/full"
         data = self._session._get(uri)
         return parser.ParseOsm(data)
 
     def WaysGet(self, WayIdList):
         """
         Returns dict with the id of the way as a key for
         each way in `WayIdList`:
@@ -781,15 +776,15 @@
                 '5678': dict of WayData,
                 ...
             }
 
         `WayIdList` is a list containing unique identifiers for multiple ways.
         """
         way_list = ",".join([str(x) for x in WayIdList])
-        uri = "/api/0.6/ways?ways=%s" % way_list
+        uri = f"/api/0.6/ways?ways={way_list}"
         data = self._session._get(uri)
         ways = dom.OsmResponseToDom(data, tag="way")
         result = {}
         for way in ways:
             data = dom.DomParseWay(way)
             result[data["id"]] = data
         return result
@@ -829,17 +824,17 @@
 
         If the requested element has been deleted,
         `OsmApi.ElementDeletedApiError` is raised.
 
         If the requested element can not be found,
         `OsmApi.ElementNotFoundApiError` is raised.
         """
-        uri = "/api/0.6/relation/%s" % (RelationId)
+        uri = f"/api/0.6/relation/{RelationId}"
         if RelationVersion != -1:
-            uri += "/%s" % (RelationVersion)
+            uri += f"/{RelationVersion}"
         data = self._session._get(uri)
         relation = dom.OsmResponseToDom(data, tag="relation", single=True)
         return dom.DomParseRelation(relation)
 
     def RelationCreate(self, RelationData):
         """
         Creates a relation based on the supplied `RelationData` dict:
@@ -1003,15 +998,15 @@
                 '1': dict of RelationData,
                 '2': dict of RelationData,
                 ...
             }
 
         `RelationId` is the unique identifier of a relation.
         """
-        uri = "/api/0.6/relation/%s/history" % (RelationId)
+        uri = f"/api/0.6/relation/{RelationId}/history"
         data = self._session._get(uri)
         relations = dom.OsmResponseToDom(data, tag="relation")
         result = {}
         for relation in relations:
             data = dom.DomParseRelation(relation)
             result[data["version"]] = data
         return result
@@ -1045,15 +1040,15 @@
                 {
                     ...
                 },
             ]
 
         The `RelationId` is a unique identifier for a relation.
         """
-        uri = "/api/0.6/relation/%d/relations" % RelationId
+        uri = f"/api/0.6/relation/{RelationId}/relations"
         data = self._session._get(uri)
         relations = dom.OsmResponseToDom(data, tag="relation", allow_empty=True)
         result = []
         for relation in relations:
             data = dom.DomParseRelation(relation)
             result.append(data)
         return result
@@ -1121,15 +1116,15 @@
 
         If the requested element has been deleted,
         `OsmApi.ElementDeletedApiError` is raised.
 
         If the requested element can not be found,
         `OsmApi.ElementNotFoundApiError` is raised.
         """
-        uri = "/api/0.6/relation/%s/full" % (RelationId)
+        uri = f"/api/0.6/relation/{RelationId}/full"
         data = self._session._get(uri)
         return parser.ParseOsm(data)
 
     def RelationsGet(self, RelationIdList):
         """
         Returns dict with the id of the relation as a key
         for each relation in `RelationIdList`:
@@ -1141,15 +1136,15 @@
                 ...
             }
 
         `RelationIdList` is a list containing unique identifiers
         for multiple relations.
         """
         relation_list = ",".join([str(x) for x in RelationIdList])
-        uri = "/api/0.6/relations?relations=%s" % relation_list
+        uri = f"/api/0.6/relations?relations={relation_list}"
         data = self._session._get(uri)
         relations = dom.OsmResponseToDom(data, tag="relation")
         result = {}
         for relation in relations:
             data = dom.DomParseRelation(relation)
             result[data["id"]] = data
         return result
@@ -1186,15 +1181,15 @@
         # Create a new changeset
         changeset_id = self.ChangesetCreate(ChangesetTags)
         yield changeset_id
 
         # upload data to changeset
         autosize = self._changesetautosize
         for i in range(0, len(self._changesetautodata), autosize):
-            chunk = self._changesetautodata[i:i+autosize]
+            chunk = self._changesetautodata[i : i + autosize]
             self.ChangesetUpload(chunk)
         self._changesetautodata = []
         self.ChangesetClose()
 
     def ChangesetGet(self, ChangesetId, include_discussion=False):
         """
         Returns changeset with `ChangesetId` as a dict:
@@ -1217,16 +1212,16 @@
             }
 
         `ChangesetId` is the unique identifier of a changeset.
 
         If `include_discussion` is set to `True` the changeset discussion
         will be available in the result.
         """
-        path = "/api/0.6/changeset/%s" % (ChangesetId)
-        if (include_discussion):
+        path = f"/api/0.6/changeset/{ChangesetId}"
+        if include_discussion:
             path += "?include_discussion=true"
         data = self._session._get(path)
         changeset = dom.OsmResponseToDom(data, tag="changeset", single=True)
         return dom.DomParseChangeset(changeset)
 
     def ChangesetUpdate(self, ChangesetTags={}):
         """
@@ -1243,17 +1238,17 @@
         """
         if not self._CurrentChangesetId:
             raise errors.NoChangesetOpenError("No changeset currently opened")
         if "created_by" not in ChangesetTags:
             ChangesetTags["created_by"] = self._created_by
         try:
             self._session._put(
-                "/api/0.6/changeset/%s" % (self._CurrentChangesetId),
+                f"/api/0.6/changeset/{self._CurrentChangesetId}",
                 xmlbuilder._XmlBuild("changeset", {"tag": ChangesetTags}, data=self),
-                return_value=False
+                return_value=False,
             )
         except errors.ApiError as e:
             if e.status == 409:
                 raise errors.ChangesetClosedApiError(e.status, e.reason, e.payload)
             else:
                 raise
         return self._CurrentChangesetId
@@ -1276,21 +1271,23 @@
             raise errors.ChangesetAlreadyOpenError("Changeset already opened")
         if "created_by" not in ChangesetTags:
             ChangesetTags["created_by"] = self._created_by
 
         # check if someone tries to create a test changeset to PROD
         if (
             self._api == "https://www.openstreetmap.org"
-            and ChangesetTags.get('comment') == "My first test"
+            and ChangesetTags.get("comment") == "My first test"
         ):
-            raise errors.OsmApiError("DO NOT CREATE test changesets on the production server")
+            raise errors.OsmApiError(
+                "DO NOT CREATE test changesets on the production server"
+            )
 
         result = self._session._put(
             "/api/0.6/changeset/create",
-            xmlbuilder._XmlBuild("changeset", {"tag": ChangesetTags}, data=self)
+            xmlbuilder._XmlBuild("changeset", {"tag": ChangesetTags}, data=self),
         )
         self._CurrentChangesetId = int(result)
         return self._CurrentChangesetId
 
     def ChangesetClose(self):
         """
         Closes current changeset.
@@ -1306,17 +1303,17 @@
         If the changeset is already closed,
         `OsmApi.ChangesetClosedApiError` is raised.
         """
         if not self._CurrentChangesetId:
             raise errors.NoChangesetOpenError("No changeset currently opened")
         try:
             self._session._put(
-                "/api/0.6/changeset/%s/close" % (self._CurrentChangesetId),
+                f"/api/0.6/changeset/{self._CurrentChangesetId}/close",
                 "",
-                return_value=False
+                return_value=False,
             )
             CurrentChangesetId = self._CurrentChangesetId
             self._CurrentChangesetId = 0
         except errors.ApiError as e:
             if e.status == 409:
                 raise errors.ChangesetClosedApiError(e.status, e.reason, e.payload)
             else:
@@ -1339,56 +1336,53 @@
         If no authentication information are provided,
         `OsmApi.UsernamePasswordMissingError` is raised.
 
         If the changeset is already closed,
         `OsmApi.ChangesetClosedApiError` is raised.
         """
         data = ""
-        data += "<?xml version=\"1.0\" encoding=\"UTF-8\"?>\n"
-        data += "<osmChange version=\"0.6\" generator=\""
-        data += self._created_by + "\">\n"
+        data += '<?xml version="1.0" encoding="UTF-8"?>\n'
+        data += '<osmChange version="0.6" generator="'
+        data += self._created_by + '">\n'
         for change in ChangesData:
             data += "<" + change["action"] + ">\n"
             change["data"]["changeset"] = self._CurrentChangesetId
             data += xmlbuilder._XmlBuild(
-                change["type"],
-                change["data"],
-                False,
-                data=self
+                change["type"], change["data"], False, data=self
             ).decode("utf-8")
             data += "</" + change["action"] + ">\n"
         data += "</osmChange>"
         try:
             data = self._session._post(
-                "/api/0.6/changeset/%s/upload" % (self._CurrentChangesetId),
+                f"/api/0.6/changeset/{self._CurrentChangesetId}/upload",
                 data.encode("utf-8"),
-                forceAuth=True
+                forceAuth=True,
             )
         except errors.ApiError as e:
-            if e.status == 409 and re.search(r"The changeset .* was closed at .*", e.payload):
+            if e.status == 409 and re.search(
+                r"The changeset .* was closed at .*", e.payload
+            ):
                 raise errors.ChangesetClosedApiError(e.status, e.reason, e.payload)
             else:
                 raise
         try:
             data = xml.dom.minidom.parseString(data)
             data = data.getElementsByTagName("diffResult")[0]
             data = [x for x in data.childNodes if x.nodeType == x.ELEMENT_NODE]
         except (xml.parsers.expat.ExpatError, IndexError) as e:
             raise errors.XmlResponseInvalidError(
-                "The XML response from the OSM API is invalid: %r" % e
+                f"The XML response from the OSM API is invalid: {e!r}"
             )
 
-        for i in range(len(ChangesData)):
-            if ChangesData[i]["action"] == "delete":
-                ChangesData[i]["data"].pop("version")
+        for item, change in zip(data, ChangesData):
+            if change["action"] == "delete":
+                change["data"].pop("version")
             else:
-                new_id = int(data[i].getAttribute("new_id"))
-                ChangesData[i]["data"]["id"] = new_id
-                new_version = int(data[i].getAttribute("new_version"))
-                ChangesData[i]["data"]["version"] = new_version
+                change["data"]["id"] = int(item.getAttribute("new_id"))
+                change["data"]["version"] = int(item.getAttribute("new_version"))
         return ChangesData
 
     def ChangesetDownload(self, ChangesetId):
         """
         Download data from changeset `ChangesetId`.
 
         Returns list of dict:
@@ -1396,30 +1390,31 @@
             #!python
             {
                 'type': node|way|relation,
                 'action': create|delete|modify,
                 'data': {}
             }
         """
-        uri = "/api/0.6/changeset/%s/download" % (ChangesetId)
+        uri = f"/api/0.6/changeset/{ChangesetId}/download"
         data = self._session._get(uri)
         return parser.ParseOsc(data)
 
     def ChangesetsGet(  # noqa
-            self,
-            min_lon=None,
-            min_lat=None,
-            max_lon=None,
-            max_lat=None,
-            userid=None,
-            username=None,
-            closed_after=None,
-            created_before=None,
-            only_open=False,
-            only_closed=False):
+        self,
+        min_lon=None,
+        min_lat=None,
+        max_lon=None,
+        max_lat=None,
+        userid=None,
+        username=None,
+        closed_after=None,
+        created_before=None,
+        only_open=False,
+        only_closed=False,
+    ):
         """
         Returns a dict with the id of the changeset as key
         matching all criteria:
 
             #!python
             {
                 '1234': dict of ChangesetData,
@@ -1429,32 +1424,25 @@
 
         All parameters are optional.
         """
 
         uri = "/api/0.6/changesets"
         params = {}
         if min_lon or min_lat or max_lon or max_lat:
-            params["bbox"] = ",".join(
-                [
-                    str(min_lon),
-                    str(min_lat),
-                    str(max_lon),
-                    str(max_lat)
-                ]
-            )
+            params["bbox"] = f"{min_lon},{min_lat},{max_lon},{max_lat}"
         if userid:
             params["user"] = userid
         if username:
             params["display_name"] = username
         if closed_after and not created_before:
             params["time"] = closed_after
         if created_before:
             if not closed_after:
                 closed_after = "1970-01-01T00:00:00Z"
-            params["time"] = "%s,%s" % (closed_after, created_before)
+            params["time"] = f"{closed_after},{created_before}"
         if only_open:
             params["open"] = 1
         if only_closed:
             params["closed"] = 1
 
         if params:
             uri += "?" + urllib.parse.urlencode(params)
@@ -1494,20 +1482,18 @@
 
         If no authentication information are provided,
         `OsmApi.UsernamePasswordMissingError` is raised.
 
         If the changeset is already closed,
         `OsmApi.ChangesetClosedApiError` is raised.
         """
-        params = urllib.parse.urlencode({'text': comment})
+        params = urllib.parse.urlencode({"text": comment})
         try:
             data = self._session._post(
-                "/api/0.6/changeset/%s/comment" % (ChangesetId),
-                params,
-                forceAuth=True
+                f"/api/0.6/changeset/{ChangesetId}/comment", params, forceAuth=True
             )
         except errors.ApiError as e:
             if e.status == 409:
                 raise errors.ChangesetClosedApiError(e.status, e.reason, e.payload)
             else:
                 raise
         changeset = dom.OsmResponseToDom(data, tag="changeset", single=True)
@@ -1538,17 +1524,15 @@
             }
 
         If no authentication information are provided,
         `OsmApi.UsernamePasswordMissingError` is raised.
         """
         try:
             data = self._session._post(
-                "/api/0.6/changeset/%s/subscribe" % (ChangesetId),
-                None,
-                forceAuth=True
+                f"/api/0.6/changeset/{ChangesetId}/subscribe", None, forceAuth=True
             )
         except errors.ApiError as e:
             if e.status == 409:
                 raise errors.AlreadySubscribedApiError(e.status, e.reason, e.payload)
             else:
                 raise
         changeset = dom.OsmResponseToDom(data, tag="changeset", single=True)
@@ -1579,36 +1563,27 @@
             }
 
         If no authentication information are provided,
         `OsmApi.UsernamePasswordMissingError` is raised.
         """
         try:
             data = self._session._post(
-                "/api/0.6/changeset/%s/unsubscribe" % (ChangesetId),
-                None,
-                forceAuth=True
+                f"/api/0.6/changeset/{ChangesetId}/unsubscribe", None, forceAuth=True
             )
         except errors.ElementNotFoundApiError as e:
             raise errors.NotSubscribedApiError(e.status, e.reason, e.payload)
 
         changeset = dom.OsmResponseToDom(data, tag="changeset", single=True)
         return dom.DomParseChangeset(changeset)
 
     ##################################################
     # Notes                                          #
     ##################################################
 
-    def NotesGet(
-            self,
-            min_lon,
-            min_lat,
-            max_lon,
-            max_lat,
-            limit=100,
-            closed=7):
+    def NotesGet(self, min_lon, min_lat, max_lon, max_lat, limit=100, closed=7):
         """
         Returns a list of dicts of notes in the specified bounding box:
 
             #!python
             [
                 {
                     'id': integer,
@@ -1629,16 +1604,17 @@
         to no longer be returned.
         The value 0 means only open bugs are returned,
         -1 means all bugs are returned.
 
         All parameters are optional.
         """
         uri = (
-            "/api/0.6/notes?bbox=%f,%f,%f,%f&limit=%d&closed=%d"
-            % (min_lon, min_lat, max_lon, max_lat, limit, closed)
+            f"/api/0.6/notes?bbox="
+            f"{min_lon:f},{min_lat:f},{max_lon:f},{max_lat:f}"
+            f"&limit={limit}&closed={closed}"
         )
         data = self._session._get(uri)
         return parser.ParseNotes(data)
 
     def NoteGet(self, id):
         """
         Returns a note as dict:
@@ -1653,15 +1629,15 @@
                 'uid': User ID|None
                 'user': User name|None
                 'comments': {}
             }
 
         `id` is the unique identifier of the note.
         """
-        uri = "/api/0.6/notes/%s" % (id)
+        uri = f"/api/0.6/notes/{id}"
         data = self._session._get(uri)
         noteElement = dom.OsmResponseToDom(data, tag="note", single=True)
         return dom.DomParseNote(noteElement)
 
     def NoteCreate(self, NoteData):
         """
         Creates a note based on the supplied `NoteData` dict:
@@ -1677,15 +1653,15 @@
 
             #!python
             {
                 'id': id of note,
                 'lat': latitude of note,
                 'lon': longitude of note,
                 'date_created': date when the note was created
-                'date_closed': date when the note was closed (or None if the note is open),
+                'date_closed': date when the note was closed or None if it's open,
                 'status': status of the note (open or closed),
                 'comments': [
                     {
                         'date': date of the comment,
                         'action': status of comment (opened, commented, closed),
                         'text': text of the note,
                         'html': html version of the text of the note,
@@ -1702,27 +1678,27 @@
 
     def NoteComment(self, NoteId, comment):
         """
         Adds a new comment to a note.
 
         Returns the updated note.
         """
-        path = "/api/0.6/notes/%s/comment" % NoteId
+        path = f"/api/0.6/notes/{NoteId}/comment"
         return self._NoteAction(path, comment)
 
     def NoteClose(self, NoteId, comment):
         """
         Closes a note.
 
         Returns the updated note.
 
         If no authentication information are provided,
         `OsmApi.UsernamePasswordMissingError` is raised.
         """
-        path = "/api/0.6/notes/%s/close" % NoteId
+        path = f"/api/0.6/notes/{NoteId}/close"
         return self._NoteAction(path, comment, optionalAuth=False)
 
     def NoteReopen(self, NoteId, comment):
         """
         Reopens a note.
 
         Returns the updated note.
@@ -1732,15 +1708,15 @@
 
         If the requested element has been deleted,
         `OsmApi.ElementDeletedApiError` is raised.
 
         If the requested element can not be found,
         `OsmApi.ElementNotFoundApiError` is raised.
         """
-        path = "/api/0.6/notes/%s/reopen" % NoteId
+        path = f"/api/0.6/notes/{NoteId}/reopen"
         return self._NoteAction(path, comment, optionalAuth=False)
 
     def NotesSearch(self, query, limit=100, closed=7):
         """
         Returns a list of dicts of notes that match the given search query.
 
         The limit parameter defines how many results should be returned.
@@ -1748,32 +1724,32 @@
         closed specifies the number of days a bug needs to be closed
         to no longer be returned.
         The value 0 means only open bugs are returned,
         -1 means all bugs are returned.
         """
         uri = "/api/0.6/notes/search"
         params = {}
-        params['q'] = query
-        params['limit'] = limit
-        params['closed'] = closed
+        params["q"] = query
+        params["limit"] = limit
+        params["closed"] = closed
         uri += "?" + urllib.parse.urlencode(params)
         data = self._session._get(uri)
 
         return parser.ParseNotes(data)
 
     def _NoteAction(self, path, comment=None, optionalAuth=True):
         """
         Performs an action on a Note with a comment
 
         Return the updated note
         """
         uri = path
         if comment is not None:
             params = {}
-            params['text'] = comment
+            params["text"] = comment
             uri += "?" + urllib.parse.urlencode(params)
         try:
             result = self._session._post(uri, None, optionalAuth=optionalAuth)
         except errors.ApiError as e:
             if e.status == 409:
                 raise errors.NoteAlreadyClosedApiError(e.status, e.reason, e.payload)
             else:
@@ -1795,18 +1771,15 @@
 
             #!python
             {
                 type: node|way|relation,
                 data: {}
             }
         """
-        uri = (
-            "/api/0.6/map?bbox=%f,%f,%f,%f"
-            % (min_lon, min_lat, max_lon, max_lat)
-        )
+        uri = f"/api/0.6/map?bbox={min_lon:f},{min_lat:f},{max_lon:f},{max_lat:f}"
         data = self._session._get(uri)
         return parser.ParseOsm(data)
 
     def flush(self):
         """
         Force the changes to be uploaded to OSM and the changeset to be closed
 
@@ -1823,19 +1796,17 @@
 
     ##################################################
     # Internal method                                #
     ##################################################
 
     def _do(self, action, OsmType, OsmData):
         if self._changesetauto:
-            self._changesetautodata.append({
-                "action": action,
-                "type": OsmType,
-                "data": OsmData
-            })
+            self._changesetautodata.append(
+                {"action": action, "type": OsmType, "data": OsmData}
+            )
             self._changesetautoflush()
             return None
         else:
             return self._do_manu(action, OsmType, OsmData)
 
     def _do_manu(self, action, OsmType, OsmData):  # noqa
         if not self._CurrentChangesetId:
@@ -1843,80 +1814,89 @@
                 "You need to open a changeset before uploading data"
             )
         if "timestamp" in OsmData:
             OsmData.pop("timestamp")
         OsmData["changeset"] = self._CurrentChangesetId
         if action == "create":
             if OsmData.get("id", -1) > 0:
-                raise errors.OsmTypeAlreadyExistsError(
-                    "This %s already exists" % OsmType
-                )
+                raise errors.OsmTypeAlreadyExistsError(f"This {OsmType} already exists")
             try:
                 result = self._session._put(
-                    "/api/0.6/%s/create" % OsmType,
-                    xmlbuilder._XmlBuild(OsmType, OsmData, data=self)
+                    f"/api/0.6/{OsmType}/create",
+                    xmlbuilder._XmlBuild(OsmType, OsmData, data=self),
                 )
             except errors.ApiError as e:
-                if e.status == 409 and re.search(r"The changeset .* was closed at .*", e.payload):
+                if e.status == 409 and re.search(
+                    r"The changeset .* was closed at .*", e.payload
+                ):
                     raise errors.ChangesetClosedApiError(e.status, e.reason, e.payload)
                 elif e.status == 409:
                     raise errors.VersionMismatchApiError(e.status, e.reason, e.payload)
                 elif e.status == 412:
-                    raise errors.PreconditionFailedApiError(e.status, e.reason, e.payload)
+                    raise errors.PreconditionFailedApiError(
+                        e.status, e.reason, e.payload
+                    )
                 else:
                     raise
             OsmData["id"] = int(result.strip())
             OsmData["version"] = 1
             return OsmData
         elif action == "modify":
             try:
                 result = self._session._put(
-                    "/api/0.6/%s/%s" % (OsmType, OsmData["id"]),
-                    xmlbuilder._XmlBuild(OsmType, OsmData, data=self)
+                    f"/api/0.6/{OsmType}/{OsmData['id']}",
+                    xmlbuilder._XmlBuild(OsmType, OsmData, data=self),
                 )
             except errors.ApiError as e:
                 logger.error(e.reason)
-                if e.status == 409 and re.search(r"The changeset .* was closed at .*", e.payload):
+                if e.status == 409 and re.search(
+                    r"The changeset .* was closed at .*", e.payload
+                ):
                     raise errors.ChangesetClosedApiError(e.status, e.reason, e.payload)
                 elif e.status == 409:
                     raise errors.VersionMismatchApiError(e.status, e.reason, e.payload)
                 elif e.status == 412:
-                    raise errors.PreconditionFailedApiError(e.status, e.reason, e.payload)
+                    raise errors.PreconditionFailedApiError(
+                        e.status, e.reason, e.payload
+                    )
                 else:
                     raise
             OsmData["version"] = int(result.strip())
             return OsmData
         elif action == "delete":
             try:
                 result = self._session._delete(
-                    "/api/0.6/%s/%s" % (OsmType, OsmData["id"]),
-                    xmlbuilder._XmlBuild(OsmType, OsmData, data=self)
+                    f"/api/0.6/{OsmType}/{OsmData['id']}",
+                    xmlbuilder._XmlBuild(OsmType, OsmData, data=self),
                 )
             except errors.ApiError as e:
-                if e.status == 409 and re.search(r"The changeset .* was closed at .*", e.payload):
+                if e.status == 409 and re.search(
+                    r"The changeset .* was closed at .*", e.payload
+                ):
                     raise errors.ChangesetClosedApiError(e.status, e.reason, e.payload)
                 elif e.status == 409:
                     raise errors.VersionMismatchApiError(e.status, e.reason, e.payload)
                 elif e.status == 412:
-                    raise errors.PreconditionFailedApiError(e.status, e.reason, e.payload)
+                    raise errors.PreconditionFailedApiError(
+                        e.status, e.reason, e.payload
+                    )
                 else:
                     raise
             OsmData["version"] = int(result.strip())
             OsmData["visible"] = False
             return OsmData
 
     def _changesetautoflush(self, force=False):
         autosize = self._changesetautosize
-        while ((len(self._changesetautodata) >= autosize) or
-                (force and self._changesetautodata)):
+        while (len(self._changesetautodata) >= autosize) or (
+            force and self._changesetautodata
+        ):
             if self._changesetautocpt == 0:
                 self.ChangesetCreate(self._changesetautotags)
-            self.ChangesetUpload(
-                self._changesetautodata[:autosize]
-            )
+            self.ChangesetUpload(self._changesetautodata[:autosize])
             self._changesetautodata = self._changesetautodata[autosize:]
             self._changesetautocpt += 1
             if self._changesetautocpt == self._changesetautomulti:
                 self.ChangesetClose()
                 self._changesetautocpt = 0
         if self._changesetautocpt and force:
             self.ChangesetClose()
```

### Comparing `osmapi-3.1.0/osmapi/dom.py` & `osmapi-4.0.0/osmapi/dom.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,23 +15,23 @@
     Returns the (sub-) DOM parsed from an OSM response
     """
     try:
         dom = xml.dom.minidom.parseString(response)
         osm_dom = dom.getElementsByTagName("osm")[0]
         all_data = osm_dom.getElementsByTagName(tag)
         first_element = all_data[0]
-    except (IndexError) as e:
+    except IndexError as e:
         if allow_empty:
             return []
         raise errors.XmlResponseInvalidError(
-            "The XML response from the OSM API is invalid: %r" % e
+            f"The XML response from the OSM API is invalid: {e!r}"
         )
-    except (xml.parsers.expat.ExpatError) as e:
+    except xml.parsers.expat.ExpatError as e:
         raise errors.XmlResponseInvalidError(
-            "The XML response from the OSM API is invalid: %r" % e
+            f"The XML response from the OSM API is invalid: {e!r}"
         )
 
     if single:
         return first_element
     return all_data
 
 
@@ -96,31 +96,31 @@
 
 def _DomGetAttributes(DomElement):
     """
     Returns a formated dictionnary of attributes of a DomElement.
     """
 
     def is_true(v):
-        return (v == "true")
+        return v == "true"
 
     attribute_mapping = {
-        'uid': int,
-        'changeset': int,
-        'version': int,
-        'id': int,
-        'lat': float,
-        'lon': float,
-        'open': is_true,
-        'visible': is_true,
-        'ref': int,
-        'comments_count': int,
-        'timestamp': _ParseDate,
-        'created_at': _ParseDate,
-        'closed_at': _ParseDate,
-        'date': _ParseDate,
+        "uid": int,
+        "changeset": int,
+        "version": int,
+        "id": int,
+        "lat": float,
+        "lon": float,
+        "open": is_true,
+        "visible": is_true,
+        "ref": int,
+        "comments_count": int,
+        "timestamp": _ParseDate,
+        "created_at": _ParseDate,
+        "closed_at": _ParseDate,
+        "date": _ParseDate,
     }
     result = {}
     for k, v in DomElement.attributes.items():
         try:
             result[k] = attribute_mapping[k](v)
         except KeyError:
             result[k] = v
@@ -154,34 +154,34 @@
     Returns the dictionnary of comments of a DomElement.
     """
     result = []
     try:
         discussion = DomElement.getElementsByTagName("discussion")[0]
         for t in discussion.getElementsByTagName("comment"):
             comment = _DomGetAttributes(t)
-            comment['text'] = xmlbuilder._GetXmlValue(t, "text")
+            comment["text"] = xmlbuilder._GetXmlValue(t, "text")
             result.append(comment)
     except IndexError:
         pass
     return result
 
 
 def _DomGetComments(DomElement):
     """
     Returns the list of comments of a DomElement.
     """
     result = []
     for t in DomElement.getElementsByTagName("comment"):
         comment = {}
-        comment['date'] = _ParseDate(xmlbuilder._GetXmlValue(t, "date"))
-        comment['action'] = xmlbuilder._GetXmlValue(t, "action")
-        comment['text'] = xmlbuilder._GetXmlValue(t, "text")
-        comment['html'] = xmlbuilder._GetXmlValue(t, "html")
-        comment['uid'] = xmlbuilder._GetXmlValue(t, "uid")
-        comment['user'] = xmlbuilder._GetXmlValue(t, "user")
+        comment["date"] = _ParseDate(xmlbuilder._GetXmlValue(t, "date"))
+        comment["action"] = xmlbuilder._GetXmlValue(t, "action")
+        comment["text"] = xmlbuilder._GetXmlValue(t, "text")
+        comment["html"] = xmlbuilder._GetXmlValue(t, "html")
+        comment["uid"] = xmlbuilder._GetXmlValue(t, "uid")
+        comment["user"] = xmlbuilder._GetXmlValue(t, "user")
         result.append(comment)
     return result
 
 
 def _DomGetMember(DomElement):
     """
     Returns a list of relation members.
```

### Comparing `osmapi-3.1.0/osmapi/errors.py` & `osmapi-4.0.0/osmapi/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# -*- coding: utf-8 -*-
-
 class OsmApiError(Exception):
     """
     General OsmApi error class to provide a superclass for all other errors
     """
 
 
 class MaximumRetryLimitReachedError(OsmApiError):
@@ -12,37 +10,41 @@
     """
 
 
 class UsernamePasswordMissingError(OsmApiError):
     """
     Error when username or password is missing for an authenticated request
     """
+
     pass
 
 
 class NoChangesetOpenError(OsmApiError):
     """
     Error when an operation requires an open changeset, but currently
     no changeset _is_ open
     """
+
     pass
 
 
 class ChangesetAlreadyOpenError(OsmApiError):
     """
     Error when a user tries to open a changeset when there is already
     an open changeset
     """
+
     pass
 
 
 class OsmTypeAlreadyExistsError(OsmApiError):
     """
     Error when a user tries to create an object that already exsits
     """
+
     pass
 
 
 class XmlResponseInvalidError(OsmApiError):
     """
     Error if the XML response from the OpenStreetMap API is invalid
     """
@@ -60,53 +62,54 @@
         self.reason = reason
         """Error message"""
 
         self.payload = payload
         """Payload of API when this error occured"""
 
     def __str__(self):
-        return (
-            "Request failed: %s - %s - %s"
-            % (str(self.status), self.reason, self.payload)
-        )
+        return f"Request failed: {self.status} - {self.reason} - {self.payload}"
 
 
 class AlreadySubscribedApiError(ApiError):
     """
     Error when a user tries to subscribe to a changeset
     that she is already subscribed to
     """
+
     pass
 
 
 class NotSubscribedApiError(ApiError):
     """
     Error when user tries to unsubscribe from a changeset
     that he is not subscribed to
     """
+
     pass
 
 
 class ElementDeletedApiError(ApiError):
     """
     Error when the requested element is deleted
     """
+
     pass
 
 
 class ElementNotFoundApiError(ApiError):
     """
     Error if the the requested element was not found
     """
 
 
 class ResponseEmptyApiError(ApiError):
     """
     Error when the response to the request is empty
     """
+
     pass
 
 
 class ChangesetClosedApiError(ApiError):
     """
     Error if the the changeset in question has already been closed
     """
```

### Comparing `osmapi-3.1.0/osmapi/http.py` & `osmapi-4.0.0/osmapi/http.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import time
+import datetime
+import itertools as it
 import logging
 import requests
+import time
 
 from . import errors
 
 
 logger = logging.getLogger(__name__)
 
 
 class OsmApiSession:
-
     MAX_RETRY_LIMIT = 5
     """Maximum retries if a call to the remote API fails (default: 5)"""
 
     def __init__(self, base_url, created_by, auth=None, session=None):
         self._api = base_url
         self._created_by = created_by
         self._auth = auth
@@ -49,71 +50,47 @@
 
         If the requested element can not be found,
         `OsmApi.ElementNotFoundApiError` is raised.
 
         If the response status code indicates an error,
         `OsmApi.ApiError` is raised.
         """
-        msg = (
-            "%s %s %s"
-            % (time.strftime("%Y-%m-%d %H:%M:%S"), method, path)
-        )
-        logger.debug(msg)
+        logger.debug(f"{datetime.datetime.now():%Y-%m-%d %H:%M:%S} {method} {path}")
 
         # Add API base URL to path
         path = self._api + path
 
         if auth and not self._auth:
             raise errors.UsernamePasswordMissingError("Username/Password missing")
 
-        response = self._session.request(
-            method,
-            path,
-            data=send
-        )
+        response = self._session.request(method, path, data=send)
         if response.status_code != 200:
             payload = response.content.strip()
             if response.status_code == 404:
                 raise errors.ElementNotFoundApiError(
-                    response.status_code,
-                    response.reason,
-                    payload
+                    response.status_code, response.reason, payload
                 )
             elif response.status_code == 410:
                 raise errors.ElementDeletedApiError(
-                    response.status_code,
-                    response.reason,
-                    payload
+                    response.status_code, response.reason, payload
                 )
             raise errors.ApiError(response.status_code, response.reason, payload)
         if return_value and not response.content:
             raise errors.ResponseEmptyApiError(
-                response.status_code,
-                response.reason,
-                ''
+                response.status_code, response.reason, ""
             )
 
-        msg = (
-            "%s %s %s"
-            % (time.strftime("%Y-%m-%d %H:%M:%S"), method, path)
-        )
-        logger.debug(msg)
+        logger.debug(f"{datetime.datetime.now():%Y-%m-%d %H:%M:%S} {method} {path}")
         return response.content
 
     def _http(self, cmd, path, auth, send, return_value=True):  # noqa
-        i = 0
-        while True:
-            i += 1
+        for i in it.count(1):
             try:
                 return self._http_request(
-                    cmd,
-                    path,
-                    auth,
-                    send,
-                    return_value=return_value
+                    cmd, path, auth, send, return_value=return_value
                 )
             except errors.ApiError as e:
                 if e.status >= 500:
                     if i == self.MAX_RETRY_LIMIT:
                         raise
                     if i != 1:
                         self._sleep()
@@ -122,15 +99,15 @@
                     raise
             except Exception as e:
                 logger.error(e)
                 if i == self.MAX_RETRY_LIMIT:
                     if isinstance(e, errors.OsmApiError):
                         raise
                     raise errors.MaximumRetryLimitReachedError(
-                        "Give up after %s retries" % i
+                        f"Give up after {i} retries"
                     )
                 if i != 1:
                     self._sleep()
                 self._session = self._get_http_session()
 
     def _get_http_session(self):
         """
@@ -138,30 +115,28 @@
         """
         if self._http_session:
             session = self._http_session
         else:
             session = requests.Session()
 
         session.auth = self._auth
-        session.headers.update({
-            'user-agent': self._created_by
-        })
+        session.headers.update({"user-agent": self._created_by})
         return session
 
     def _sleep(self):
         time.sleep(5)
 
     def _get(self, path):
-        return self._http('GET', path, False, None)
+        return self._http("GET", path, False, None)
 
     def _put(self, path, data, return_value=True):
-        return self._http('PUT', path, True, data, return_value=return_value)
+        return self._http("PUT", path, True, data, return_value=return_value)
 
     def _post(self, path, data, optionalAuth=False, forceAuth=False):
         # the Notes API allows certain POSTs by non-authenticated users
-        auth = (optionalAuth and self._auth)
+        auth = optionalAuth and self._auth
         if forceAuth:
             auth = True
-        return self._http('POST', path, auth, data)
+        return self._http("POST", path, auth, data)
 
     def _delete(self, path, data):
-        return self._http('DELETE', path, True, data)
+        return self._http("DELETE", path, True, data)
```

### Comparing `osmapi-3.1.0/osmapi/parser.py` & `osmapi-4.0.0/osmapi/parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,34 +18,25 @@
         }
     """
     try:
         data = xml.dom.minidom.parseString(data)
         data = data.getElementsByTagName("osm")[0]
     except (xml.parsers.expat.ExpatError, IndexError) as e:
         raise errors.XmlResponseInvalidError(
-            "The XML response from the OSM API is invalid: %r" % e
+            f"The XML response from the OSM API is invalid: {e!r}"
         )
 
     result = []
     for elem in data.childNodes:
         if elem.nodeName == "node":
-            result.append({
-                "type": elem.nodeName,
-                "data": dom.DomParseNode(elem)
-            })
+            result.append({"type": elem.nodeName, "data": dom.DomParseNode(elem)})
         elif elem.nodeName == "way":
-            result.append({
-                "type": elem.nodeName,
-                "data": dom.DomParseWay(elem)
-            })
+            result.append({"type": elem.nodeName, "data": dom.DomParseWay(elem)})
         elif elem.nodeName == "relation":
-            result.append({
-                "type": elem.nodeName,
-                "data": dom.DomParseRelation(elem)
-            })
+            result.append({"type": elem.nodeName, "data": dom.DomParseRelation(elem)})
     return result
 
 
 def ParseOsc(data):
     """
     Parse osc data.
 
@@ -59,40 +50,46 @@
         }
     """
     try:
         data = xml.dom.minidom.parseString(data)
         data = data.getElementsByTagName("osmChange")[0]
     except (xml.parsers.expat.ExpatError, IndexError) as e:
         raise errors.XmlResponseInvalidError(
-            "The XML response from the OSM API is invalid: %r" % e
+            f"The XML response from the OSM API is invalid: {e!r}"
         )
 
     result = []
     for action in data.childNodes:
         if action.nodeName == "#text":
             continue
         for elem in action.childNodes:
             if elem.nodeName == "node":
-                result.append({
-                    "action": action.nodeName,
-                    "type": elem.nodeName,
-                    "data": dom.DomParseNode(elem)
-                })
+                result.append(
+                    {
+                        "action": action.nodeName,
+                        "type": elem.nodeName,
+                        "data": dom.DomParseNode(elem),
+                    }
+                )
             elif elem.nodeName == "way":
-                result.append({
-                    "action": action.nodeName,
-                    "type": elem.nodeName,
-                    "data": dom.DomParseWay(elem)
-                })
+                result.append(
+                    {
+                        "action": action.nodeName,
+                        "type": elem.nodeName,
+                        "data": dom.DomParseWay(elem),
+                    }
+                )
             elif elem.nodeName == "relation":
-                result.append({
-                    "action": action.nodeName,
-                    "type": elem.nodeName,
-                    "data": dom.DomParseRelation(elem)
-                })
+                result.append(
+                    {
+                        "action": action.nodeName,
+                        "type": elem.nodeName,
+                        "data": dom.DomParseRelation(elem),
+                    }
+                )
     return result
 
 
 def ParseNotes(data):
     """
     Parse notes data.
```

### Comparing `osmapi-3.1.0/osmapi.egg-info/PKG-INFO` & `osmapi-4.0.0/osmapi.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: osmapi
-Version: 3.1.0
+Version: 4.0.0
 Summary: Python wrapper for the OSM API
 Home-page: https://github.com/metaodi/osmapi
 Author: Etienne Chové
 Author-email: chove@crans.org
 Maintainer: Stefan Oderbolz
 Maintainer-email: odi@metaodi.ch
 License: GPLv3
-Download-URL: https://github.com/metaodi/osmapi/archive/v3.1.0.zip
+Download-URL: https://github.com/metaodi/osmapi/archive/v4.0.0.zip
 Description: osmapi
         ======
         
         [![Build osmapi](https://github.com/metaodi/osmapi/actions/workflows/build.yml/badge.svg)](https://github.com/metaodi/osmapi/actions/workflows/build.yml)
         [![Coverage](https://img.shields.io/coveralls/metaodi/osmapi/develop.svg)](https://coveralls.io/r/metaodi/osmapi?branch=develop)
+        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         [![Version](https://img.shields.io/pypi/v/osmapi.svg)](https://pypi.python.org/pypi/osmapi/)
         [![License](https://img.shields.io/pypi/l/osmapi.svg)](https://github.com/metaodi/osmapi/blob/master/LICENSE.txt)
         
-        Python wrapper for the OSM API (requires Python >= 3.7)
+        Python wrapper for the OSM API (requires Python >= 3.8)
         
         ## Installation
         
         Install [`osmapi` from PyPi](https://pypi.python.org/pypi/osmapi) by using pip: 
         
             pip install osmapi
         
@@ -84,17 +85,25 @@
         ### Development
         
         If you want to help with the development of `osmapi`, you should clone this repository and install the requirements:
         
             pip install -r requirements.txt
             pip install -r test-requirements.txt
         
-        After that, it is recommended to install the `flake8` pre-commit-hook:
+        After that, it is recommended to install the pre-commit-hooks (flake8, black):
         
-            flake8 --install-hook
+            pre-commit install
+        
+        You can lint the source code using this command:
+        
+            make lint
+        
+        And if you want to reformat the files (using the black code style) simply run:
+        
+            make format
         
         ### Tests
         
         To run the tests use the following command:
         
             make test
         
@@ -120,13 +129,13 @@
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `osmapi-3.1.0/osmapi.egg-info/SOURCES.txt` & `osmapi-4.0.0/osmapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osmapi-3.1.0/setup.py` & `osmapi-4.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 # -*- coding: utf-8 -*-
 
 from codecs import open
 from setuptools import setup, find_packages
 import re
 
-with open('osmapi/__init__.py', 'r') as fd:
-    version = re.search(r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]',
-                        fd.read(), re.MULTILINE).group(1)
+with open("osmapi/__init__.py", "r") as fd:
+    version = re.search(
+        r'^__version__\s*=\s*[\'"]([^\'"]*)[\'"]', fd.read(), re.MULTILINE
+    ).group(1)
 
 if not version:
-    raise RuntimeError('Cannot find version information')
+    raise RuntimeError("Cannot find version information")
 
-with open('README.md', 'r', encoding="utf-8") as f:
+with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    name='osmapi',
+    name="osmapi",
     packages=find_packages(),
     version=version,
-    install_requires=['requests'],
-    python_requires='>=3.7',
-    description='Python wrapper for the OSM API',
+    install_requires=["requests"],
+    python_requires=">=3.8",
+    description="Python wrapper for the OSM API",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    author='Etienne Chové',
-    author_email='chove@crans.org',
-    maintainer='Stefan Oderbolz',
-    maintainer_email='odi@metaodi.ch',
-    url='https://github.com/metaodi/osmapi',
-    download_url='https://github.com/metaodi/osmapi/archive/v%s.zip' % version,
-    keywords=['openstreetmap', 'osm', 'api'],
-    license='GPLv3',
+    long_description_content_type="text/markdown",
+    author="Etienne Chové",
+    author_email="chove@crans.org",
+    maintainer="Stefan Oderbolz",
+    maintainer_email="odi@metaodi.ch",
+    url="https://github.com/metaodi/osmapi",
+    download_url=f"https://github.com/metaodi/osmapi/archive/v{version}.zip",
+    keywords=["openstreetmap", "osm", "api"],
+    license="GPLv3",
     classifiers=[
-        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Intended Audience :: Developers',
-        'Topic :: Scientific/Engineering :: GIS',
-        'Topic :: Software Development :: Libraries',
-        'Development Status :: 4 - Beta',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Intended Audience :: Developers",
+        "Topic :: Scientific/Engineering :: GIS",
+        "Topic :: Software Development :: Libraries",
+        "Development Status :: 4 - Beta",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `osmapi-3.1.0/tests/changeset_test.py` & `osmapi-4.0.0/tests/changeset_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,272 +8,261 @@
 def xmltosorteddict(xml):
     xml_dict = xmltodict.parse(xml, dict_constructor=dict)
     return xml_dict
 
 
 def test_Changeset_contextmanager(auth_api, add_response):
     # Setup mock
-    resp = add_response(PUT, '/changeset/create', filename='test_Changeset_create.xml')
-    resp = add_response(PUT, '/node/create', filename='test_Changeset_create_node.xml')
-    resp = add_response(PUT, '/changeset/1414/close', filename='test_Changeset_close.xml')
+    resp = add_response(PUT, "/changeset/create", filename="test_Changeset_create.xml")
+    resp = add_response(PUT, "/node/create", filename="test_Changeset_create_node.xml")
+    resp = add_response(
+        PUT, "/changeset/1414/close", filename="test_Changeset_close.xml"
+    )
 
     test_node = {
-        'lat': 47.123,
-        'lon': 8.555,
-        'tag': {
-            'amenity': 'place_of_worship',
-            'religion': 'pastafarian'
-        }
+        "lat": 47.123,
+        "lon": 8.555,
+        "tag": {"amenity": "place_of_worship", "religion": "pastafarian"},
     }
 
     # use context manager
     with auth_api.Changeset() as changeset_id:
         assert changeset_id == 1414
 
         # add test node
         node = auth_api.NodeCreate(test_node)
-        assert node['id'] == 7272
+        assert node["id"] == 7272
 
     # check requests
     assert len(resp.calls) == 3
 
 
 def test_ChangesetGet(api, add_response):
     # Setup mock
-    add_response(GET, '/changeset/123')
+    add_response(GET, "/changeset/123")
 
     # Call
     result = api.ChangesetGet(123)
 
     test_changeset = {
-        'id': 123,
-        'closed_at': datetime.datetime(2009, 9, 7, 22, 57, 37),
-        'created_at': datetime.datetime(2009, 9, 7, 21, 57, 36),
-        'discussion': [],
-        'max_lat': '52.4710193',
-        'max_lon': '-1.4831815',
-        'min_lat': '45.9667901',
-        'min_lon': '-1.4998534',
-        'open': False,
-        'user': 'randomjunk',
-        'uid': 3,
-        'tag': {
-            'comment': 'correct node bug',
-            'created_by': 'Potlatch 1.2a',
+        "id": 123,
+        "closed_at": datetime.datetime(2009, 9, 7, 22, 57, 37),
+        "created_at": datetime.datetime(2009, 9, 7, 21, 57, 36),
+        "discussion": [],
+        "max_lat": "52.4710193",
+        "max_lon": "-1.4831815",
+        "min_lat": "45.9667901",
+        "min_lon": "-1.4998534",
+        "open": False,
+        "user": "randomjunk",
+        "uid": 3,
+        "tag": {
+            "comment": "correct node bug",
+            "created_by": "Potlatch 1.2a",
         },
     }
     assert result == test_changeset
 
 
 def test_ChangesetUpdate(auth_api, add_response):
     # Setup mock
-    resp = add_response(PUT, '/changeset/create', filename='test_ChangesetCreate.xml')
-    resp = add_response(PUT, '/changeset/4321', filename='test_ChangesetUpdate.xml')
+    resp = add_response(PUT, "/changeset/create", filename="test_ChangesetCreate.xml")
+    resp = add_response(PUT, "/changeset/4321", filename="test_ChangesetUpdate.xml")
 
     # Call
     result = auth_api.ChangesetCreate()
     assert result == 4321
 
-    result = auth_api.ChangesetUpdate({'test': 'foobar'})
+    result = auth_api.ChangesetUpdate({"test": "foobar"})
     changeset_xml = xmltosorteddict(
         b'<?xml version="1.0" encoding="UTF-8"?>\n'
-        b'<osm version="0.6" generator="osmapi/3.1.0">\n'
+        b'<osm version="0.6" generator="osmapi/4.0.0">\n'
         b'  <changeset visible="true">\n'
         b'    <tag k="test" v="foobar"/>\n'
-        b'    <tag k="created_by" v="osmapi/3.1.0"/>\n'
-        b'  </changeset>\n'
-        b'</osm>\n'
+        b'    <tag k="created_by" v="osmapi/4.0.0"/>\n'
+        b"  </changeset>\n"
+        b"</osm>\n"
     )
     assert xmltosorteddict(resp.calls[1].request.body) == changeset_xml
     assert result == 4321
 
 
 def test_ChangesetUpdate_with_created_by(auth_api, add_response):
     # Setup mock
-    resp = add_response(PUT, '/changeset/create', filename='test_ChangesetCreate.xml')
-    resp = add_response(PUT, '/changeset/4321', filename='test_ChangesetUpdate.xml')
+    resp = add_response(PUT, "/changeset/create", filename="test_ChangesetCreate.xml")
+    resp = add_response(PUT, "/changeset/4321", filename="test_ChangesetUpdate.xml")
 
     # Call
     result = auth_api.ChangesetCreate()
     assert result == 4321
 
-    result = auth_api.ChangesetUpdate(
-        {
-            'test': 'foobar',
-            'created_by': 'MyTestOSMApp'
-        }
-    )
+    result = auth_api.ChangesetUpdate({"test": "foobar", "created_by": "MyTestOSMApp"})
     changeset_xml = xmltosorteddict(
         b'<?xml version="1.0" encoding="UTF-8"?>\n'
-        b'<osm version="0.6" generator="osmapi/3.1.0">\n'
+        b'<osm version="0.6" generator="osmapi/4.0.0">\n'
         b'  <changeset visible="true">\n'
         b'    <tag k="test" v="foobar"/>\n'
         b'    <tag k="created_by" v="MyTestOSMApp"/>\n'
-        b'  </changeset>\n'
-        b'</osm>\n'
+        b"  </changeset>\n"
+        b"</osm>\n"
     )
     assert xmltosorteddict(resp.calls[1].request.body) == changeset_xml
     assert result == 4321
 
 
 def test_ChangesetUpdate_wo_changeset(auth_api):
     with pytest.raises(osmapi.NoChangesetOpenError) as execinfo:
-        auth_api.ChangesetUpdate({'test': 'foobar'})
-    assert str(execinfo.value) == 'No changeset currently opened'
+        auth_api.ChangesetUpdate({"test": "foobar"})
+    assert str(execinfo.value) == "No changeset currently opened"
 
 
 def test_ChangesetCreate(auth_api, add_response):
-    resp = add_response(PUT, '/changeset/create')
-    result = auth_api.ChangesetCreate(
-        {
-            'foobar': 'A new test changeset'
-        }
-    )
+    resp = add_response(PUT, "/changeset/create")
+    result = auth_api.ChangesetCreate({"foobar": "A new test changeset"})
     assert result == 4321
 
     changeset_xml = xmltosorteddict(
         b'<?xml version="1.0" encoding="UTF-8"?>\n'
-        b'<osm version="0.6" generator="osmapi/3.1.0">\n'
+        b'<osm version="0.6" generator="osmapi/4.0.0">\n'
         b'  <changeset visible="true">\n'
         b'    <tag k="foobar" v="A new test changeset"/>\n'
-        b'    <tag k="created_by" v="osmapi/3.1.0"/>\n'
-        b'  </changeset>\n'
-        b'</osm>\n'
+        b'    <tag k="created_by" v="osmapi/4.0.0"/>\n'
+        b"  </changeset>\n"
+        b"</osm>\n"
     )
     assert xmltosorteddict(resp.calls[0].request.body) == changeset_xml
 
 
 def test_ChangesetCreate_with_created_by(auth_api, add_response):
-    resp = add_response(PUT, '/changeset/create')
+    resp = add_response(PUT, "/changeset/create")
 
     result = auth_api.ChangesetCreate(
         {
-            'foobar': 'A new test changeset',
-            'created_by': 'CoolTestApp',
+            "foobar": "A new test changeset",
+            "created_by": "CoolTestApp",
         }
     )
     assert result == 1234
 
     changeset_xml = xmltosorteddict(
         b'<?xml version="1.0" encoding="UTF-8"?>\n'
-        b'<osm version="0.6" generator="osmapi/3.1.0">\n'
+        b'<osm version="0.6" generator="osmapi/4.0.0">\n'
         b'  <changeset visible="true">\n'
         b'    <tag k="foobar" v="A new test changeset"/>\n'
         b'    <tag k="created_by" v="CoolTestApp"/>\n'
-        b'  </changeset>\n'
-        b'</osm>\n'
+        b"  </changeset>\n"
+        b"</osm>\n"
     )
     assert xmltosorteddict(resp.calls[0].request.body) == changeset_xml
 
 
 def test_ChangesetCreate_with_open_changeset(auth_api, add_response):
-    add_response(PUT, '/changeset/create')
+    add_response(PUT, "/changeset/create")
 
     auth_api.ChangesetCreate(
         {
-            'test': 'an already open changeset',
+            "test": "an already open changeset",
         }
     )
 
     with pytest.raises(osmapi.ChangesetAlreadyOpenError) as execinfo:
-        auth_api.ChangesetCreate({'test': 'foobar'})
-    assert str(execinfo.value) == 'Changeset already opened'
+        auth_api.ChangesetCreate({"test": "foobar"})
+    assert str(execinfo.value) == "Changeset already opened"
 
 
 def test_ChangesetCreate_with_prod_api_and_test_comment(prod_api):
     with pytest.raises(osmapi.OsmApiError) as execinfo:
         prod_api.ChangesetCreate(
             {
-                'comment': 'My first test',
+                "comment": "My first test",
             }
         )
-    assert str(execinfo.value) == 'DO NOT CREATE test changesets on the production server'
+    assert (
+        str(execinfo.value) == "DO NOT CREATE test changesets on the production server"
+    )
 
 
 def test_ChangesetClose(auth_api, add_response):
     # setup mock
-    resp = add_response(PUT, '/changeset/create', filename='test_Changeset_create.xml')
-    resp = add_response(PUT, '/changeset/1414/close')
+    resp = add_response(PUT, "/changeset/create", filename="test_Changeset_create.xml")
+    resp = add_response(PUT, "/changeset/1414/close")
 
     # Call
     auth_api.ChangesetCreate()
     auth_api.ChangesetClose()
 
-    assert '/api/0.6/changeset/1414/close' in resp.calls[1].request.url
+    assert "/api/0.6/changeset/1414/close" in resp.calls[1].request.url
 
 
 def test_ChangesetClose_with_no_changeset(auth_api):
     with pytest.raises(osmapi.NoChangesetOpenError) as execinfo:
         auth_api.ChangesetClose()
-    assert str(execinfo.value) == 'No changeset currently opened'
+    assert str(execinfo.value) == "No changeset currently opened"
 
 
 def test_ChangesetUpload_create_node(auth_api, add_response):
     # Setup
-    resp = add_response(PUT, '/changeset/create', body='4444')
-    resp = add_response(POST, '/changeset/4444/upload')
+    resp = add_response(PUT, "/changeset/create", body="4444")
+    resp = add_response(POST, "/changeset/4444/upload")
 
     changesdata = [
         {
-            'type': 'node',
-            'action': 'create',
-            'data': {
-                'lat': 47.123,
-                'lon': 8.555,
-                'tag': {
-                    'amenity': 'place_of_worship',
-                    'religion': 'pastafarian'
-                }
-            }
+            "type": "node",
+            "action": "create",
+            "data": {
+                "lat": 47.123,
+                "lon": 8.555,
+                "tag": {"amenity": "place_of_worship", "religion": "pastafarian"},
+            },
         }
     ]
 
     upload_xml = xmltosorteddict(
         b'<?xml version="1.0" encoding="UTF-8"?>\n'
-        b'<osmChange version="0.6" generator="osmapi/3.1.0">\n'
-        b'<create>\n'
+        b'<osmChange version="0.6" generator="osmapi/4.0.0">\n'
+        b"<create>\n"
         b'  <node lat="47.123" lon="8.555" visible="true" '
         b'changeset="4444">\n'
         b'    <tag k="amenity" v="place_of_worship"/>\n'
         b'    <tag k="religion" v="pastafarian"/>\n'
-        b'  </node>\n'
-        b'</create>\n'
-        b'</osmChange>'
+        b"  </node>\n"
+        b"</create>\n"
+        b"</osmChange>"
     )
 
     # Call
     auth_api.ChangesetCreate()
     result = auth_api.ChangesetUpload(changesdata)
 
     # Assert
     assert xmltosorteddict(resp.calls[1].request.body) == upload_xml
-    assert result[0]['type'] == changesdata[0]['type']
-    assert result[0]['action'] == changesdata[0]['action']
+    assert result[0]["type"] == changesdata[0]["type"]
+    assert result[0]["action"] == changesdata[0]["action"]
 
-    data = result[0]['data']
-    assert data['lat'] == changesdata[0]['data']['lat']
-    assert data['lon'] == changesdata[0]['data']['lon']
-    assert data['tag'] == changesdata[0]['data']['tag']
-    assert data['id'] == 4295832900
-    assert result[0]['data']['version'] == 1
+    data = result[0]["data"]
+    assert data["lat"] == changesdata[0]["data"]["lat"]
+    assert data["lon"] == changesdata[0]["data"]["lon"]
+    assert data["tag"] == changesdata[0]["data"]["tag"]
+    assert data["id"] == 4295832900
+    assert result[0]["data"]["version"] == 1
 
 
 def test_ChangesetUpload_modify_way(auth_api, add_response):
     # setup mock
-    resp = add_response(PUT, '/changeset/create', body='4444')
-    resp = add_response(POST, '/changeset/4444/upload')
+    resp = add_response(PUT, "/changeset/create", body="4444")
+    resp = add_response(POST, "/changeset/4444/upload")
 
     changesdata = [
         {
-            'type': 'way',
-            'action': 'modify',
-            'data': {
-                'id': 4294967296,
-                'version': 2,
-                'nd': [
+            "type": "way",
+            "action": "modify",
+            "data": {
+                "id": 4294967296,
+                "version": 2,
+                "nd": [
                     4295832773,
                     4295832773,
                     4294967304,
                     4294967303,
                     4294967300,
                     4608751,
                     4294967305,
@@ -281,28 +270,25 @@
                     8548430,
                     4294967296,
                     4294967301,
                     4294967298,
                     4294967306,
                     7855737,
                     4294967297,
-                    4294967299
+                    4294967299,
                 ],
-                'tag': {
-                    'highway': 'secondary',
-                    'name': 'Stansted Road'
-                }
-            }
+                "tag": {"highway": "secondary", "name": "Stansted Road"},
+            },
         }
     ]
 
     upload_xml = xmltosorteddict(
         b'<?xml version="1.0" encoding="UTF-8"?>\n'
-        b'<osmChange version="0.6" generator="osmapi/3.1.0">\n'
-        b'<modify>\n'
+        b'<osmChange version="0.6" generator="osmapi/4.0.0">\n'
+        b"<modify>\n"
         b'  <way id="4294967296" version="2" visible="true" '
         b'changeset="4444">\n'
         b'    <tag k="highway" v="secondary"/>\n'
         b'    <tag k="name" v="Stansted Road"/>\n'
         b'    <nd ref="4295832773"/>\n'
         b'    <nd ref="4295832773"/>\n'
         b'    <nd ref="4294967304"/>\n'
@@ -315,417 +301,391 @@
         b'    <nd ref="4294967296"/>\n'
         b'    <nd ref="4294967301"/>\n'
         b'    <nd ref="4294967298"/>\n'
         b'    <nd ref="4294967306"/>\n'
         b'    <nd ref="7855737"/>\n'
         b'    <nd ref="4294967297"/>\n'
         b'    <nd ref="4294967299"/>\n'
-        b'  </way>\n'
-        b'</modify>\n'
-        b'</osmChange>'
+        b"  </way>\n"
+        b"</modify>\n"
+        b"</osmChange>"
     )
 
     # Call
     auth_api.ChangesetCreate()
     result = auth_api.ChangesetUpload(changesdata)
 
     # Assert
     assert xmltosorteddict(resp.calls[1].request.body) == upload_xml
 
-    assert result[0]['type'] == changesdata[0]['type']
-    assert result[0]['action'] == changesdata[0]['action']
+    assert result[0]["type"] == changesdata[0]["type"]
+    assert result[0]["action"] == changesdata[0]["action"]
 
-    data = result[0]['data']
-    assert data['nd'] == changesdata[0]['data']['nd']
-    assert data['tag'] == changesdata[0]['data']['tag']
-    assert data['id'] == 4294967296
-    assert data['version'] == 3
+    data = result[0]["data"]
+    assert data["nd"] == changesdata[0]["data"]["nd"]
+    assert data["tag"] == changesdata[0]["data"]["tag"]
+    assert data["id"] == 4294967296
+    assert data["version"] == 3
 
 
 def test_ChangesetUpload_delete_relation(auth_api, add_response):
     # setup mock
-    resp = add_response(PUT, '/changeset/create', body='4444')
-    resp = add_response(POST, '/changeset/4444/upload')
+    resp = add_response(PUT, "/changeset/create", body="4444")
+    resp = add_response(POST, "/changeset/4444/upload")
 
     changesdata = [
         {
-            'type': 'relation',
-            'action': 'delete',
-            'data': {
-                'id': 676,
-                'version': 2,
-                'member': [
-                    {
-                        'ref': 4799,
-                        'role': 'outer',
-                        'type': 'way'
-                    },
-                    {
-                        'ref': 9391,
-                        'role': 'outer',
-                        'type': 'way'
-                    },
+            "type": "relation",
+            "action": "delete",
+            "data": {
+                "id": 676,
+                "version": 2,
+                "member": [
+                    {"ref": 4799, "role": "outer", "type": "way"},
+                    {"ref": 9391, "role": "outer", "type": "way"},
                 ],
-                'tag': {
-                    'admin_level': '9',
-                    'boundary': 'administrative',
-                    'type': 'multipolygon'
-                }
-            }
+                "tag": {
+                    "admin_level": "9",
+                    "boundary": "administrative",
+                    "type": "multipolygon",
+                },
+            },
         }
     ]
 
     upload_xml = xmltosorteddict(
         b'<?xml version="1.0" encoding="UTF-8"?>\n'
-        b'<osmChange version="0.6" generator="osmapi/3.1.0">\n'
-        b'<delete>\n'
+        b'<osmChange version="0.6" generator="osmapi/4.0.0">\n'
+        b"<delete>\n"
         b'  <relation id="676" version="2" visible="true" '
         b'changeset="4444">\n'
         b'    <tag k="admin_level" v="9"/>\n'
         b'    <tag k="boundary" v="administrative"/>\n'
         b'    <tag k="type" v="multipolygon"/>\n'
         b'    <member type="way" ref="4799" role="outer"/>\n'
         b'    <member type="way" ref="9391" role="outer"/>\n'
-        b'  </relation>\n'
-        b'</delete>\n'
-        b'</osmChange>'
+        b"  </relation>\n"
+        b"</delete>\n"
+        b"</osmChange>"
     )
 
     # Call
     auth_api.ChangesetCreate()
     result = auth_api.ChangesetUpload(changesdata)
 
     # Assert
     assert xmltosorteddict(resp.calls[1].request.body) == upload_xml
-    assert result[0]['type'] == changesdata[0]['type']
-    assert result[0]['action'] == changesdata[0]['action']
+    assert result[0]["type"] == changesdata[0]["type"]
+    assert result[0]["action"] == changesdata[0]["action"]
 
-    data = result[0]['data']
-    assert data['member'], changesdata[0]['data']['member']
-    assert data['tag'] == changesdata[0]['data']['tag']
-    assert data['id'] == 676
-    assert 'version' not in data
+    data = result[0]["data"]
+    assert data["member"], changesdata[0]["data"]["member"]
+    assert data["tag"] == changesdata[0]["data"]["tag"]
+    assert data["id"] == 676
+    assert "version" not in data
 
 
 def test_ChangesetUpload_invalid_response(auth_api, add_response):
     # setup mock
-    add_response(PUT, '/changeset/create', body='4444')
-    add_response(POST, '/changeset/4444/upload', body='4444')
+    add_response(PUT, "/changeset/create", body="4444")
+    add_response(POST, "/changeset/4444/upload", body="4444")
 
     changesdata = [
         {
-            'type': 'relation',
-            'action': 'delete',
-            'data': {
-                'id': 676,
-                'version': 2,
-                'member': [
-                    {
-                        'ref': 4799,
-                        'role': 'outer',
-                        'type': 'way'
-                    },
-                    {
-                        'ref': 9391,
-                        'role': 'outer',
-                        'type': 'way'
-                    },
+            "type": "relation",
+            "action": "delete",
+            "data": {
+                "id": 676,
+                "version": 2,
+                "member": [
+                    {"ref": 4799, "role": "outer", "type": "way"},
+                    {"ref": 9391, "role": "outer", "type": "way"},
                 ],
-                'tag': {
-                    'admin_level': '9',
-                    'boundary': 'administrative',
-                    'type': 'multipolygon'
-                }
-            }
+                "tag": {
+                    "admin_level": "9",
+                    "boundary": "administrative",
+                    "type": "multipolygon",
+                },
+            },
         }
     ]
 
     # Call + assert
     auth_api.ChangesetCreate()
     with pytest.raises(osmapi.XmlResponseInvalidError) as execinfo:
         auth_api.ChangesetUpload(changesdata)
-    assert 'The XML response from the OSM API is invalid' in str(execinfo.value)
+    assert "The XML response from the OSM API is invalid" in str(execinfo.value)
 
 
 def test_ChangesetUpload_no_auth(api):
     changesdata = [
         {
-            'type': 'node',
-            'action': 'create',
-            'data': {
-                'lat': 47.123,
-                'lon': 8.555,
-                'tag': {
-                    'amenity': 'place_of_worship',
-                    'religion': 'pastafarian'
-                }
-            }
+            "type": "node",
+            "action": "create",
+            "data": {
+                "lat": 47.123,
+                "lon": 8.555,
+                "tag": {"amenity": "place_of_worship", "religion": "pastafarian"},
+            },
         }
     ]
 
     with pytest.raises(osmapi.UsernamePasswordMissingError) as execinfo:
         api.ChangesetUpload(changesdata)
     assert str(execinfo.value) == "Username/Password missing"
 
 
 def test_ChangesetDownload(api, add_response):
     # Setup mock
-    add_response(GET, '/changeset/23123/download')
+    add_response(GET, "/changeset/23123/download")
 
     # Call
     result = api.ChangesetDownload(23123)
 
     # Assertion
     assert len(result) == 16
     assert result[1] == (
         {
-            'action': 'create',
-            'type': 'node',
-            'data': {
-                'changeset': 23123,
-                'id': 4295668171,
-                'lat': 46.4909781,
-                'lon': 11.2743295,
-                'tag': {
-                    'highway': 'traffic_signals'
-                },
-                'timestamp': datetime.datetime(2013, 5, 14, 10, 33, 4),
-                'uid': 1178,
-                'user': 'tyrTester06',
-                'version': 1,
-                'visible': True
-            }
+            "action": "create",
+            "type": "node",
+            "data": {
+                "changeset": 23123,
+                "id": 4295668171,
+                "lat": 46.4909781,
+                "lon": 11.2743295,
+                "tag": {"highway": "traffic_signals"},
+                "timestamp": datetime.datetime(2013, 5, 14, 10, 33, 4),
+                "uid": 1178,
+                "user": "tyrTester06",
+                "version": 1,
+                "visible": True,
+            },
         }
     )
 
 
 def test_ChangesetDownload_invalid_response(api, add_response):
-    add_response(GET, '/changeset/23123/download')
+    add_response(GET, "/changeset/23123/download")
     with pytest.raises(osmapi.XmlResponseInvalidError) as execinfo:
         api.ChangesetDownload(23123)
-    assert 'The XML response from the OSM API is invalid' in str(execinfo.value)
+    assert "The XML response from the OSM API is invalid" in str(execinfo.value)
 
 
 def test_ChangesetDownloadContainingUnicode(api, add_response):
-    add_response(GET, '/changeset/37393499/download')
+    add_response(GET, "/changeset/37393499/download")
 
     # This changeset contains unicode tag values
     # Note that the fixture data has been reduced from the
     # original from openstreetmap.org
     result = api.ChangesetDownload(37393499)
 
     assert len(result) == 2
     assert result[1] == (
         {
-            'action': 'create',
-            'type': 'way',
-            'data': {
-                'changeset': 37393499,
-                'id': 399491497,
-                'nd': [4022271571, 4022271567, 4022271565],
-                'tag': {'highway': 'service',
-                        # UTF-8 encoded 'LATIN SMALL LETTER O WITH STROKE'
-                        # Aka. 0xf8 in latin-1/ISO 8859-1
-                        'name': b'S\xc3\xb8nderskovvej'.decode('utf-8'),
-                        'service': 'driveway'},
-                'timestamp': datetime.datetime(2016, 2, 23, 16, 55, 35),
-                'uid': 328556,
-                'user': 'InternationalUser',
-                'version': 1,
-                'visible': True
-            }
+            "action": "create",
+            "type": "way",
+            "data": {
+                "changeset": 37393499,
+                "id": 399491497,
+                "nd": [4022271571, 4022271567, 4022271565],
+                "tag": {
+                    "highway": "service",
+                    # UTF-8 encoded 'LATIN SMALL LETTER O WITH STROKE'
+                    # Aka. 0xf8 in latin-1/ISO 8859-1
+                    "name": b"S\xc3\xb8nderskovvej".decode("utf-8"),
+                    "service": "driveway",
+                },
+                "timestamp": datetime.datetime(2016, 2, 23, 16, 55, 35),
+                "uid": 328556,
+                "user": "InternationalUser",
+                "version": 1,
+                "visible": True,
+            },
         }
     )
 
 
 def test_ChangesetsGet(api, add_response):
-    resp = add_response(GET, '/changesets')
+    resp = add_response(GET, "/changesets")
 
-    result = api.ChangesetsGet(
-        only_closed=True,
-        username='metaodi'
-    )
+    result = api.ChangesetsGet(only_closed=True, username="metaodi")
 
-    assert resp.calls[0].request.params == {'display_name': 'metaodi', 'closed': '1'}
+    assert resp.calls[0].request.params == {"display_name": "metaodi", "closed": "1"}
     assert len(result) == 10
-    assert result[41417] == ({
-        'closed_at': datetime.datetime(2014, 4, 29, 20, 25, 1),
-        'created_at': datetime.datetime(2014, 4, 29, 20, 25, 1),
-        'id': 41417,
-        'discussion': [],
-        'max_lat': '58.8997467',
-        'max_lon': '22.7364427',
-        'min_lat': '58.8501594',
-        'min_lon': '22.6984333',
-        'open': False,
-        'tag': {
-            'comment': 'Test delete of relation',
-            'created_by': 'iD 1.3.9',
-            'imagery_used': 'Bing'
-        },
-        'uid': 1841,
-        'user': 'metaodi'
-    })
+    assert result[41417] == (
+        {
+            "closed_at": datetime.datetime(2014, 4, 29, 20, 25, 1),
+            "created_at": datetime.datetime(2014, 4, 29, 20, 25, 1),
+            "id": 41417,
+            "discussion": [],
+            "max_lat": "58.8997467",
+            "max_lon": "22.7364427",
+            "min_lat": "58.8501594",
+            "min_lon": "22.6984333",
+            "open": False,
+            "tag": {
+                "comment": "Test delete of relation",
+                "created_by": "iD 1.3.9",
+                "imagery_used": "Bing",
+            },
+            "uid": 1841,
+            "user": "metaodi",
+        }
+    )
 
 
 def test_ChangesetGetWithComment(api, add_response):
-    resp = add_response(GET, '/changeset/52924')
+    resp = add_response(GET, "/changeset/52924")
 
     result = api.ChangesetGet(52924, include_discussion=True)
 
-    assert resp.calls[0].request.params == {'include_discussion': 'true'}
+    assert resp.calls[0].request.params == {"include_discussion": "true"}
     assert result == {
-        'id': 52924,
-        'closed_at': datetime.datetime(2015, 1, 1, 14, 54, 2),
-        'created_at': datetime.datetime(2015, 1, 1, 14, 54, 1),
-        'comments_count': 3,
-        'max_lat': '58.3369242',
-        'max_lon': '25.8829107',
-        'min_lat': '58.336813',
-        'min_lon': '25.8823273',
-        'discussion': [
+        "id": 52924,
+        "closed_at": datetime.datetime(2015, 1, 1, 14, 54, 2),
+        "created_at": datetime.datetime(2015, 1, 1, 14, 54, 1),
+        "comments_count": 3,
+        "max_lat": "58.3369242",
+        "max_lon": "25.8829107",
+        "min_lat": "58.336813",
+        "min_lon": "25.8823273",
+        "discussion": [
             {
-                'date':  datetime.datetime(2015, 1, 1, 18, 56, 48),
-                'text': 'test',
-                'uid': 1841,
-                'user': 'metaodi',
+                "date": datetime.datetime(2015, 1, 1, 18, 56, 48),
+                "text": "test",
+                "uid": 1841,
+                "user": "metaodi",
             },
             {
-                'date':  datetime.datetime(2015, 1, 1, 18, 58, 3),
-                'text': 'another comment',
-                'uid': 1841,
-                'user': 'metaodi',
+                "date": datetime.datetime(2015, 1, 1, 18, 58, 3),
+                "text": "another comment",
+                "uid": 1841,
+                "user": "metaodi",
             },
             {
-                'date':  datetime.datetime(2015, 1, 1, 19, 16, 5),
-                'text': 'hello',
-                'uid': 1841,
-                'user': 'metaodi',
+                "date": datetime.datetime(2015, 1, 1, 19, 16, 5),
+                "text": "hello",
+                "uid": 1841,
+                "user": "metaodi",
             },
         ],
-        'open': False,
-        'user': 'metaodi',
-        'uid': 1841,
-        'tag': {
-            'comment': 'My test',
-            'created_by': 'osmapi/0.4.1',
+        "open": False,
+        "user": "metaodi",
+        "uid": 1841,
+        "tag": {
+            "comment": "My test",
+            "created_by": "osmapi/0.4.1",
         },
     }
 
 
 def test_ChangesetComment(auth_api, add_response):
-    resp = add_response(POST, '/changeset/123/comment')
+    resp = add_response(POST, "/changeset/123/comment")
 
-    result = auth_api.ChangesetComment(
-        123,
-        comment="test comment"
-    )
+    result = auth_api.ChangesetComment(123, comment="test comment")
 
     assert resp.calls[0].request.body == "text=test+comment"
     assert result == {
-        'id': 123,
-        'closed_at': datetime.datetime(2009, 9, 7, 22, 57, 37),
-        'created_at': datetime.datetime(2009, 9, 7, 21, 57, 36),
-        'discussion': [],
-        'max_lat': '52.4710193',
-        'max_lon': '-1.4831815',
-        'min_lat': '45.9667901',
-        'min_lon': '-1.4998534',
-        'open': False,
-        'user': 'randomjunk',
-        'uid': 3,
-        'tag': {
-            'comment': 'correct node bug',
-            'created_by': 'Potlatch 1.2a',
+        "id": 123,
+        "closed_at": datetime.datetime(2009, 9, 7, 22, 57, 37),
+        "created_at": datetime.datetime(2009, 9, 7, 21, 57, 36),
+        "discussion": [],
+        "max_lat": "52.4710193",
+        "max_lon": "-1.4831815",
+        "min_lat": "45.9667901",
+        "min_lon": "-1.4998534",
+        "open": False,
+        "user": "randomjunk",
+        "uid": 3,
+        "tag": {
+            "comment": "correct node bug",
+            "created_by": "Potlatch 1.2a",
         },
     }
 
 
 def test_ChangesetComment_no_auth(api):
     with pytest.raises(osmapi.UsernamePasswordMissingError) as execinfo:
-        api.ChangesetComment(
-            123,
-            comment="test comment"
-        )
+        api.ChangesetComment(123, comment="test comment")
     assert str(execinfo.value) == "Username/Password missing"
 
 
 def test_ChangesetSubscribe(auth_api, add_response):
-    add_response(POST, '/changeset/123/subscribe')
+    add_response(POST, "/changeset/123/subscribe")
 
     result = auth_api.ChangesetSubscribe(123)
 
     assert result == {
-        'id': 123,
-        'closed_at': datetime.datetime(2009, 9, 7, 22, 57, 37),
-        'created_at': datetime.datetime(2009, 9, 7, 21, 57, 36),
-        'discussion': [],
-        'max_lat': '52.4710193',
-        'max_lon': '-1.4831815',
-        'min_lat': '45.9667901',
-        'min_lon': '-1.4998534',
-        'open': False,
-        'user': 'randomjunk',
-        'uid': 3,
-        'tag': {
-            'comment': 'correct node bug',
-            'created_by': 'Potlatch 1.2a',
+        "id": 123,
+        "closed_at": datetime.datetime(2009, 9, 7, 22, 57, 37),
+        "created_at": datetime.datetime(2009, 9, 7, 21, 57, 36),
+        "discussion": [],
+        "max_lat": "52.4710193",
+        "max_lon": "-1.4831815",
+        "min_lat": "45.9667901",
+        "min_lon": "-1.4998534",
+        "open": False,
+        "user": "randomjunk",
+        "uid": 3,
+        "tag": {
+            "comment": "correct node bug",
+            "created_by": "Potlatch 1.2a",
         },
     }
 
 
 def test_ChangesetSubscribeWhenAlreadySubscribed(auth_api, add_response):
-    add_response(POST, '/changeset/52924/subscribe', status=409)
+    add_response(POST, "/changeset/52924/subscribe", status=409)
 
     with pytest.raises(osmapi.AlreadySubscribedApiError) as execinfo:
         auth_api.ChangesetSubscribe(52924)
 
     assert execinfo.value.payload == b"You are already subscribed to changeset 52924."
-    assert execinfo.value.reason == 'Conflict'
+    assert execinfo.value.reason == "Conflict"
     assert execinfo.value.status == 409
 
 
 def test_ChangesetSubscribe_no_auth(api):
     with pytest.raises(osmapi.UsernamePasswordMissingError) as execinfo:
         api.ChangesetSubscribe(45627)
     assert str(execinfo.value) == "Username/Password missing"
 
 
 def test_ChangesetUnsubscribe(auth_api, add_response):
-    add_response(POST, '/changeset/123/unsubscribe')
+    add_response(POST, "/changeset/123/unsubscribe")
 
     result = auth_api.ChangesetUnsubscribe(123)
 
     assert result == {
-        'id': 123,
-        'closed_at': datetime.datetime(2009, 9, 7, 22, 57, 37),
-        'created_at': datetime.datetime(2009, 9, 7, 21, 57, 36),
-        'discussion': [],
-        'max_lat': '52.4710193',
-        'max_lon': '-1.4831815',
-        'min_lat': '45.9667901',
-        'min_lon': '-1.4998534',
-        'open': False,
-        'user': 'randomjunk',
-        'uid': 3,
-        'tag': {
-            'comment': 'correct node bug',
-            'created_by': 'Potlatch 1.2a',
+        "id": 123,
+        "closed_at": datetime.datetime(2009, 9, 7, 22, 57, 37),
+        "created_at": datetime.datetime(2009, 9, 7, 21, 57, 36),
+        "discussion": [],
+        "max_lat": "52.4710193",
+        "max_lon": "-1.4831815",
+        "min_lat": "45.9667901",
+        "min_lon": "-1.4998534",
+        "open": False,
+        "user": "randomjunk",
+        "uid": 3,
+        "tag": {
+            "comment": "correct node bug",
+            "created_by": "Potlatch 1.2a",
         },
     }
 
 
 def test_ChangesetUnsubscribeWhenNotSubscribed(auth_api, add_response):
-    add_response(POST, '/changeset/52924/unsubscribe', status=404)
+    add_response(POST, "/changeset/52924/unsubscribe", status=404)
 
     with pytest.raises(osmapi.NotSubscribedApiError) as execinfo:
         auth_api.ChangesetUnsubscribe(52924)
 
     assert execinfo.value.payload == b"You are not subscribed to changeset 52924."
-    assert execinfo.value.reason == 'Not Found'
+    assert execinfo.value.reason == "Not Found"
     assert execinfo.value.status == 404
 
 
 def test_ChangesetUnsubscribe_no_auth(api):
     with pytest.raises(osmapi.UsernamePasswordMissingError) as execinfo:
         api.ChangesetUnsubscribe(45627)
     assert str(execinfo.value) == "Username/Password missing"
```

### Comparing `osmapi-3.1.0/tests/dom_test.py` & `osmapi-4.0.0/tests/dom_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,54 @@
 from . import osmapi_test
 import osmapi
-import mock
+from unittest import mock
 import datetime
 
 
 class TestOsmApiDom(osmapi_test.TestOsmApi):
     def test_DomGetAttributes(self):
         mock_domelement = mock.Mock()
         mock_domelement.attributes = {
-            'uid': '12345',
-            'open': 'false',
-            'visible': 'true',
-            'lat': '47.1234',
-            'date': '2021-12-10T21:28:03Z',
-            'new_attribute': 'Test 123',
+            "uid": "12345",
+            "open": "false",
+            "visible": "true",
+            "lat": "47.1234",
+            "date": "2021-12-10T21:28:03Z",
+            "new_attribute": "Test 123",
         }
 
         result = osmapi.dom._DomGetAttributes(mock_domelement)
 
         self.assertIsInstance(result, dict)
-        self.assertEqual(result['uid'], 12345)
-        self.assertEqual(result['open'], False)
-        self.assertEqual(result['visible'], True)
-        self.assertEqual(result['lat'], 47.1234)
-        self.assertEqual(result['date'], datetime.datetime(2021, 12, 10, 21, 28, 3))
-        self.assertEqual(result['new_attribute'], 'Test 123')
+        self.assertEqual(result["uid"], 12345)
+        self.assertEqual(result["open"], False)
+        self.assertEqual(result["visible"], True)
+        self.assertEqual(result["lat"], 47.1234)
+        self.assertEqual(result["date"], datetime.datetime(2021, 12, 10, 21, 28, 3))
+        self.assertEqual(result["new_attribute"], "Test 123")
 
     def test_ParseDate(self):
         self.assertEqual(
-            osmapi.dom._ParseDate('2021-02-25T09:49:33Z'),
-            datetime.datetime(2021, 2, 25, 9, 49, 33)
+            osmapi.dom._ParseDate("2021-02-25T09:49:33Z"),
+            datetime.datetime(2021, 2, 25, 9, 49, 33),
         )
         self.assertEqual(
-            osmapi.dom._ParseDate('2021-02-25 09:49:33 UTC'),
-            datetime.datetime(2021, 2, 25, 9, 49, 33)
+            osmapi.dom._ParseDate("2021-02-25 09:49:33 UTC"),
+            datetime.datetime(2021, 2, 25, 9, 49, 33),
         )
-        with self.assertLogs('osmapi.dom', level='DEBUG') as cm:
-            self.assertEqual(
-                osmapi.dom._ParseDate('2021-02-25'),
-                '2021-02-25'
-            )
-            self.assertEqual(
-                osmapi.dom._ParseDate(''),
-                ''
-            )
+        with self.assertLogs("osmapi.dom", level="DEBUG") as cm:
+            self.assertEqual(osmapi.dom._ParseDate("2021-02-25"), "2021-02-25")
+            self.assertEqual(osmapi.dom._ParseDate(""), "")
             self.assertIsNone(osmapi.dom._ParseDate(None))
 
             # test logging output
             self.assertEqual(
                 cm.output,
                 [
-                    'DEBUG:osmapi.dom:2021-02-25 does not match %Y-%m-%d %H:%M:%S UTC',
-                    'DEBUG:osmapi.dom:2021-02-25 does not match %Y-%m-%dT%H:%M:%SZ',
-                    'DEBUG:osmapi.dom: does not match %Y-%m-%d %H:%M:%S UTC',
-                    'DEBUG:osmapi.dom: does not match %Y-%m-%dT%H:%M:%SZ',
-                    'DEBUG:osmapi.dom:None does not match %Y-%m-%d %H:%M:%S UTC',
-                    'DEBUG:osmapi.dom:None does not match %Y-%m-%dT%H:%M:%SZ',
-                ]
+                    "DEBUG:osmapi.dom:2021-02-25 does not match %Y-%m-%d %H:%M:%S UTC",
+                    "DEBUG:osmapi.dom:2021-02-25 does not match %Y-%m-%dT%H:%M:%SZ",
+                    "DEBUG:osmapi.dom: does not match %Y-%m-%d %H:%M:%S UTC",
+                    "DEBUG:osmapi.dom: does not match %Y-%m-%dT%H:%M:%SZ",
+                    "DEBUG:osmapi.dom:None does not match %Y-%m-%d %H:%M:%S UTC",
+                    "DEBUG:osmapi.dom:None does not match %Y-%m-%dT%H:%M:%SZ",
+                ],
             )
```

### Comparing `osmapi-3.1.0/tests/helper_test.py` & `osmapi-4.0.0/tests/helper_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,161 +1,113 @@
-from __future__ import (unicode_literals, absolute_import)
 from . import osmapi_test
 import osmapi
-import mock
+from unittest import mock
 import os
 
-__location__ = os.path.realpath(
-    os.path.join(
-        os.getcwd(),
-        os.path.dirname(__file__)
-    )
-)
+__location__ = os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
 
 
 class TestOsmApiHelper(osmapi_test.TestOsmApi):
     def setUp(self):
-        super(TestOsmApiHelper, self).setUp()
+        super().setUp()
         self.setupMock()
 
     def setupMock(self, status=200):
         mock_response = mock.Mock()
         mock_response.status_code = status
         mock_response.reason = "test reason"
-        mock_response.content = 'test response'
+        mock_response.content = "test response"
 
         self.mock_session = mock.Mock()
         self.mock_session.request = mock.Mock(return_value=mock_response)
         self.mock_session.close = mock.Mock()
-        self.mock_session.auth = ('testuser', 'testpassword')
+        self.mock_session.auth = ("testuser", "testpassword")
 
         self.api = osmapi.OsmApi(
             api=self.api_base,
             session=self.mock_session,
-            username='testuser',
-            password='testpassword'
+            username="testuser",
+            password="testpassword",
         )
 
     def test_passwordfile_only(self):
-        path = os.path.join(
-            __location__,
-            'fixtures',
-            'passwordfile.txt'
-        )
+        path = os.path.join(__location__, "fixtures", "passwordfile.txt")
         my_api = osmapi.OsmApi(passwordfile=path)
-        self.assertEqual('testosm', my_api._username)
-        self.assertEqual('testpass', my_api._password)
+        self.assertEqual("testosm", my_api._username)
+        self.assertEqual("testpass", my_api._password)
 
     def test_passwordfile_with_user(self):
-        path = os.path.join(
-            __location__,
-            'fixtures',
-            'passwordfile.txt'
-        )
-        my_api = osmapi.OsmApi(username='testuser', passwordfile=path)
-        self.assertEqual('testuser', my_api._username)
-        self.assertEqual('testuserpass', my_api._password)
+        path = os.path.join(__location__, "fixtures", "passwordfile.txt")
+        my_api = osmapi.OsmApi(username="testuser", passwordfile=path)
+        self.assertEqual("testuser", my_api._username)
+        self.assertEqual("testuserpass", my_api._password)
 
     def test_passwordfile_with_colon(self):
-        path = os.path.join(
-            __location__,
-            'fixtures',
-            'passwordfile_colon.txt'
-        )
-        my_api = osmapi.OsmApi(username='testuser', passwordfile=path)
-        self.assertEqual('testuser', my_api._username)
-        self.assertEqual('test:userpass', my_api._password)
+        path = os.path.join(__location__, "fixtures", "passwordfile_colon.txt")
+        my_api = osmapi.OsmApi(username="testuser", passwordfile=path)
+        self.assertEqual("testuser", my_api._username)
+        self.assertEqual("test:userpass", my_api._password)
 
     def test_close_call(self):
         self.api.close()
         self.assertEqual(self.api._session._session.close.call_count, 1)
 
     def test_close_context_manager(self):
         with osmapi.OsmApi() as my_api:
             my_api._session.close = mock.Mock()
         self.assertEqual(my_api._session.close.call_count, 1)
 
     def test_http_request_get(self):
-        response = self.api._session._http_request(
-            'GET',
-            '/api/0.6/test',
-            False,
-            None
-        )
+        response = self.api._session._http_request("GET", "/api/0.6/test", False, None)
         self.mock_session.request.assert_called_with(
-            'GET',
-            self.api_base + '/api/0.6/test',
-            data=None
+            "GET", self.api_base + "/api/0.6/test", data=None
         )
         self.assertEqual(response, "test response")
         self.assertEqual(self.mock_session.request.call_count, 1)
 
     def test_http_request_put(self):
         data = "data"
         response = self.api._session._http_request(
-            'PUT',
-            '/api/0.6/testput',
-            False,
-            data
+            "PUT", "/api/0.6/testput", False, data
         )
         self.mock_session.request.assert_called_with(
-            'PUT',
-            self.api_base + '/api/0.6/testput',
-            data="data"
+            "PUT", self.api_base + "/api/0.6/testput", data="data"
         )
         self.assertEqual(response, "test response")
 
     def test_http_request_delete(self):
         data = "delete data"
         response = self.api._session._http_request(
-            'PUT',
-            '/api/0.6/testdelete',
-            False,
-            data
+            "PUT", "/api/0.6/testdelete", False, data
         )
         self.mock_session.request.assert_called_with(
-            'PUT',
-            self.api_base + '/api/0.6/testdelete',
-            data="delete data"
+            "PUT", self.api_base + "/api/0.6/testdelete", data="delete data"
         )
         self.assertEqual(response, "test response")
 
     def test_http_request_auth(self):
         response = self.api._session._http_request(
-            'PUT',
-            '/api/0.6/testauth',
-            True,
-            None
+            "PUT", "/api/0.6/testauth", True, None
         )
         self.mock_session.request.assert_called_with(
-            'PUT',
-            self.api_base + '/api/0.6/testauth',
-            data=None
+            "PUT", self.api_base + "/api/0.6/testauth", data=None
         )
-        self.assertEqual(self.mock_session.auth, ('testuser', 'testpassword'))
+        self.assertEqual(self.mock_session.auth, ("testuser", "testpassword"))
         self.assertEqual(response, "test response")
 
     def test_http_request_410_response(self):
         self.setupMock(410)
         with self.assertRaises(osmapi.ElementDeletedApiError) as cm:
-            self.api._session._http_request(
-                'GET',
-                '/api/0.6/test410',
-                False,
-                None
-            )
+            self.api._session._http_request("GET", "/api/0.6/test410", False, None)
         self.assertEqual(cm.exception.status, 410)
         self.assertEqual(cm.exception.reason, "test reason")
         self.assertEqual(cm.exception.payload, "test response")
 
     def test_http_request_500_response(self):
         self.setupMock(500)
         with self.assertRaises(osmapi.ApiError) as cm:
             self.api._session._http_request(
-                'GET',
-                self.api_base + '/api/0.6/test500',
-                False,
-                None
+                "GET", self.api_base + "/api/0.6/test500", False, None
             )
         self.assertEqual(cm.exception.status, 500)
         self.assertEqual(cm.exception.reason, "test reason")
         self.assertEqual(cm.exception.payload, "test response")
```

### Comparing `osmapi-3.1.0/tests/node_test.py` & `osmapi-4.0.0/tests/node_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,463 +1,405 @@
-from __future__ import (unicode_literals, absolute_import)
 from . import osmapi_test
 import osmapi
-import mock
+from unittest import mock
 import datetime
 
 
 class TestOsmApiNode(osmapi_test.TestOsmApi):
     def test_NodeGet(self):
         self._session_mock()
 
         result = self.api.NodeGet(123)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
-        self.assertEqual(args[1], self.api_base + '/api/0.6/node/123')
+        self.assertEqual(args[0], "GET")
+        self.assertEqual(args[1], self.api_base + "/api/0.6/node/123")
 
-        self.assertEqual(result, {
-            'id': 123,
-            'changeset': 15293,
-            'uid': 605,
-            'timestamp': datetime.datetime(2012, 4, 18, 11, 14, 26),
-            'lat': 51.8753146,
-            'lon': -1.4857118,
-            'visible': True,
-            'version': 8,
-            'user': 'freundchen',
-            'tag': {
-                'amenity': 'school',
-                'foo': 'bar',
-                'name': 'Berolina & Schule'
+        self.assertEqual(
+            result,
+            {
+                "id": 123,
+                "changeset": 15293,
+                "uid": 605,
+                "timestamp": datetime.datetime(2012, 4, 18, 11, 14, 26),
+                "lat": 51.8753146,
+                "lon": -1.4857118,
+                "visible": True,
+                "version": 8,
+                "user": "freundchen",
+                "tag": {"amenity": "school", "foo": "bar", "name": "Berolina & Schule"},
             },
-        })
+        )
 
     def test_NodeGet_with_version(self):
         self._session_mock()
 
         result = self.api.NodeGet(123, NodeVersion=2)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
-        self.assertEqual(args[1], self.api_base + '/api/0.6/node/123/2')
+        self.assertEqual(args[0], "GET")
+        self.assertEqual(args[1], self.api_base + "/api/0.6/node/123/2")
 
-        self.assertEqual(result, {
-            'id': 123,
-            'changeset': 4152,
-            'uid': 605,
-            'timestamp': datetime.datetime(2011, 4, 18, 11, 14, 26),
-            'lat': 51.8753146,
-            'lon': -1.4857118,
-            'visible': True,
-            'version': 2,
-            'user': 'freundchen',
-            'tag': {
-                'amenity': 'school',
+        self.assertEqual(
+            result,
+            {
+                "id": 123,
+                "changeset": 4152,
+                "uid": 605,
+                "timestamp": datetime.datetime(2011, 4, 18, 11, 14, 26),
+                "lat": 51.8753146,
+                "lon": -1.4857118,
+                "visible": True,
+                "version": 2,
+                "user": "freundchen",
+                "tag": {
+                    "amenity": "school",
+                },
             },
-        })
+        )
 
     def test_NodeGet_invalid_response(self):
         self._session_mock()
 
         with self.assertRaises(osmapi.XmlResponseInvalidError):
             self.api.NodeGet(987)
 
     def test_NodeCreate_changesetauto(self):
-        for filename in ['test_NodeCreate_changesetauto.xml',
-                         'test_ChangesetUpload_create_node.xml',
-                         'test_ChangesetClose.xml']:
+        for filename in [
+            "test_NodeCreate_changesetauto.xml",
+            "test_ChangesetUpload_create_node.xml",
+            "test_ChangesetClose.xml",
+        ]:
             # setup mock
             self._session_mock(auth=True, filenames=[filename])
             self.api = osmapi.OsmApi(
                 api="api06.dev.openstreetmap.org",
                 changesetauto=True,
-                session=self.session_mock
+                session=self.session_mock,
             )
             self.api._session._sleep = mock.Mock()
 
             test_node = {
-                'lat': 47.123,
-                'lon': 8.555,
-                'tag': {
-                    'amenity': 'place_of_worship',
-                    'religion': 'pastafarian'
-                }
+                "lat": 47.123,
+                "lon": 8.555,
+                "tag": {"amenity": "place_of_worship", "religion": "pastafarian"},
             }
 
             self.assertIsNone(self.api.NodeCreate(test_node))
 
     def test_NodeCreate(self):
         self._session_mock(auth=True)
 
         # setup mock
-        self.api.ChangesetCreate = mock.Mock(
-            return_value=1111
-        )
+        self.api.ChangesetCreate = mock.Mock(return_value=1111)
         self.api._CurrentChangesetId = 1111
 
         test_node = {
-            'lat': 47.287,
-            'lon': 8.765,
-            'tag': {
-                'amenity': 'place_of_worship',
-                'religion': 'pastafarian'
-            }
+            "lat": 47.287,
+            "lon": 8.765,
+            "tag": {"amenity": "place_of_worship", "religion": "pastafarian"},
         }
 
-        cs = self.api.ChangesetCreate({
-            'comment': 'This is a test dataset'
-        })
+        cs = self.api.ChangesetCreate({"comment": "This is a test dataset"})
         self.assertEqual(cs, 1111)
         result = self.api.NodeCreate(test_node)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'PUT')
-        self.assertEqual(args[1], self.api_base + '/api/0.6/node/create')
+        self.assertEqual(args[0], "PUT")
+        self.assertEqual(args[1], self.api_base + "/api/0.6/node/create")
 
-        self.assertEqual(result['id'], 9876)
-        self.assertEqual(result['lat'], test_node['lat'])
-        self.assertEqual(result['lon'], test_node['lon'])
-        self.assertEqual(result['tag'], test_node['tag'])
+        self.assertEqual(result["id"], 9876)
+        self.assertEqual(result["lat"], test_node["lat"])
+        self.assertEqual(result["lon"], test_node["lon"])
+        self.assertEqual(result["tag"], test_node["tag"])
 
     def test_NodeCreate_wo_changeset(self):
         test_node = {
-            'lat': 47.287,
-            'lon': 8.765,
-            'tag': {
-                'amenity': 'place_of_worship',
-                'religion': 'pastafarian'
-            }
+            "lat": 47.287,
+            "lon": 8.765,
+            "tag": {"amenity": "place_of_worship", "religion": "pastafarian"},
         }
 
         with self.assertRaisesRegex(
-                osmapi.NoChangesetOpenError,
-                'need to open a changeset'):
+            osmapi.NoChangesetOpenError, "need to open a changeset"
+        ):
             self.api.NodeCreate(test_node)
 
     def test_NodeCreate_existing_node(self):
         # setup mock
-        self.api.ChangesetCreate = mock.Mock(
-            return_value=1111
-        )
+        self.api.ChangesetCreate = mock.Mock(return_value=1111)
         self.api._CurrentChangesetId = 1111
 
         test_node = {
-            'id': 123,
-            'lat': 47.287,
-            'lon': 8.765,
-            'tag': {
-                'amenity': 'place_of_worship',
-                'religion': 'pastafarian'
-            }
+            "id": 123,
+            "lat": 47.287,
+            "lon": 8.765,
+            "tag": {"amenity": "place_of_worship", "religion": "pastafarian"},
         }
 
         with self.assertRaisesRegex(
-                osmapi.OsmTypeAlreadyExistsError,
-                'This node already exists'):
+            osmapi.OsmTypeAlreadyExistsError, "This node already exists"
+        ):
             self.api.NodeCreate(test_node)
 
     def test_NodeCreate_wo_auth(self):
         self._session_mock()
 
         # setup mock
-        self.api.ChangesetCreate = mock.Mock(
-            return_value=1111
-        )
+        self.api.ChangesetCreate = mock.Mock(return_value=1111)
         self.api._CurrentChangesetId = 1111
         test_node = {
-            'lat': 47.287,
-            'lon': 8.765,
-            'tag': {
-                'amenity': 'place_of_worship',
-                'religion': 'pastafarian'
-            }
+            "lat": 47.287,
+            "lon": 8.765,
+            "tag": {"amenity": "place_of_worship", "religion": "pastafarian"},
         }
 
         with self.assertRaisesRegex(
-                osmapi.UsernamePasswordMissingError,
-                'Username/Password missing'):
+            osmapi.UsernamePasswordMissingError, "Username/Password missing"
+        ):
             self.api.NodeCreate(test_node)
 
     def test_NodeCreate_with_exception(self):
         self._session_mock(auth=True)
         self.api._session._http_request = mock.Mock(side_effect=Exception)
 
         # setup mock
-        self.api.ChangesetCreate = mock.Mock(
-            return_value=1111
-        )
+        self.api.ChangesetCreate = mock.Mock(return_value=1111)
         self.api._CurrentChangesetId = 1111
         test_node = {
-            'lat': 47.287,
-            'lon': 8.765,
-            'tag': {
-                'amenity': 'place_of_worship',
-                'religion': 'pastafarian'
-            }
+            "lat": 47.287,
+            "lon": 8.765,
+            "tag": {"amenity": "place_of_worship", "religion": "pastafarian"},
         }
 
         with self.assertRaisesRegex(
-                osmapi.MaximumRetryLimitReachedError,
-                'Give up after 5 retries'):
+            osmapi.MaximumRetryLimitReachedError, "Give up after 5 retries"
+        ):
             self.api.NodeCreate(test_node)
 
     def test_NodeUpdate(self):
         self._session_mock(auth=True)
 
         # setup mock
-        self.api.ChangesetCreate = mock.Mock(
-            return_value=1111
-        )
+        self.api.ChangesetCreate = mock.Mock(return_value=1111)
         self.api._CurrentChangesetId = 1111
 
         test_node = {
-            'id': 7676,
-            'lat': 47.287,
-            'lon': 8.765,
-            'tag': {
-                'amenity': 'place_of_worship',
-                'name': 'christian'
-            }
+            "id": 7676,
+            "lat": 47.287,
+            "lon": 8.765,
+            "tag": {"amenity": "place_of_worship", "name": "christian"},
         }
 
-        cs = self.api.ChangesetCreate({
-            'comment': 'This is a test dataset'
-        })
+        cs = self.api.ChangesetCreate({"comment": "This is a test dataset"})
         self.assertEqual(cs, 1111)
         result = self.api.NodeUpdate(test_node)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'PUT')
-        self.assertEqual(args[1], self.api_base + '/api/0.6/node/7676')
+        self.assertEqual(args[0], "PUT")
+        self.assertEqual(args[1], self.api_base + "/api/0.6/node/7676")
 
-        self.assertEqual(result['id'], 7676)
-        self.assertEqual(result['version'], 3)
-        self.assertEqual(result['lat'], test_node['lat'])
-        self.assertEqual(result['lon'], test_node['lon'])
-        self.assertEqual(result['tag'], test_node['tag'])
+        self.assertEqual(result["id"], 7676)
+        self.assertEqual(result["version"], 3)
+        self.assertEqual(result["lat"], test_node["lat"])
+        self.assertEqual(result["lon"], test_node["lon"])
+        self.assertEqual(result["tag"], test_node["tag"])
 
     def test_NodeUpdateWhenChangesetIsClosed(self):
         self._session_mock(auth=True, status=409)
 
-        self.api.ChangesetCreate = mock.Mock(
-            return_value=1111
-        )
+        self.api.ChangesetCreate = mock.Mock(return_value=1111)
         self.api._CurrentChangesetId = 1111
 
         test_node = {
-            'id': 7676,
-            'lat': 47.287,
-            'lon': 8.765,
-            'tag': {
-                'amenity': 'place_of_worship',
-                'name': 'christian'
-            }
+            "id": 7676,
+            "lat": 47.287,
+            "lon": 8.765,
+            "tag": {"amenity": "place_of_worship", "name": "christian"},
         }
 
-        self.api.ChangesetCreate({
-            'comment': 'This is a test dataset'
-        })
+        self.api.ChangesetCreate({"comment": "This is a test dataset"})
 
         with self.assertRaises(osmapi.ChangesetClosedApiError) as cm:
             self.api.NodeUpdate(test_node)
 
         self.assertEqual(cm.exception.status, 409)
         self.assertEqual(
             cm.exception.payload,
-            "The changeset 2222 was closed at 2021-11-20 09:42:47 UTC."
+            "The changeset 2222 was closed at 2021-11-20 09:42:47 UTC.",
         )
 
     def test_NodeUpdateConflict(self):
         self._session_mock(auth=True, status=409)
 
-        self.api.ChangesetCreate = mock.Mock(
-            return_value=1111
-        )
+        self.api.ChangesetCreate = mock.Mock(return_value=1111)
         self.api._CurrentChangesetId = 1111
 
         test_node = {
-            'id': 7676,
-            'lat': 47.287,
-            'lon': 8.765,
-            'tag': {
-                'amenity': 'place_of_worship',
-                'name': 'christian'
-            }
+            "id": 7676,
+            "lat": 47.287,
+            "lon": 8.765,
+            "tag": {"amenity": "place_of_worship", "name": "christian"},
         }
 
-        self.api.ChangesetCreate({
-            'comment': 'This is a test dataset'
-        })
+        self.api.ChangesetCreate({"comment": "This is a test dataset"})
 
         with self.assertRaises(osmapi.VersionMismatchApiError) as cm:
             self.api.NodeUpdate(test_node)
 
         self.assertEqual(cm.exception.status, 409)
         self.assertEqual(
             cm.exception.payload,
-            "Version does not match the current database version of the element"
+            "Version does not match the current database version of the element",
         )
 
     def test_NodeDelete(self):
         self._session_mock(auth=True)
 
         # setup mock
-        self.api.ChangesetCreate = mock.Mock(
-            return_value=1111
-        )
+        self.api.ChangesetCreate = mock.Mock(return_value=1111)
         self.api._CurrentChangesetId = 1111
 
-        test_node = {
-            'id': 7676
-        }
+        test_node = {"id": 7676}
 
-        cs = self.api.ChangesetCreate({
-            'comment': 'This is a test dataset'
-        })
+        cs = self.api.ChangesetCreate({"comment": "This is a test dataset"})
         self.assertEqual(cs, 1111)
 
         result = self.api.NodeDelete(test_node)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'DELETE')
-        self.assertEqual(args[1], self.api_base + '/api/0.6/node/7676')
-        self.assertEqual(result['id'], 7676)
-        self.assertEqual(result['version'], 4)
+        self.assertEqual(args[0], "DELETE")
+        self.assertEqual(args[1], self.api_base + "/api/0.6/node/7676")
+        self.assertEqual(result["id"], 7676)
+        self.assertEqual(result["version"], 4)
 
     def test_NodeHistory(self):
         self._session_mock()
 
         result = self.api.NodeHistory(123)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
-        self.assertEqual(args[1], self.api_base + '/api/0.6/node/123/history')
+        self.assertEqual(args[0], "GET")
+        self.assertEqual(args[1], self.api_base + "/api/0.6/node/123/history")
 
         self.assertEqual(len(result), 8)
-        self.assertEqual(result[4]['id'], 123)
-        self.assertEqual(result[4]['version'], 4)
-        self.assertEqual(result[4]['lat'], 51.8753146)
-        self.assertEqual(result[4]['lon'], -1.4857118)
+        self.assertEqual(result[4]["id"], 123)
+        self.assertEqual(result[4]["version"], 4)
+        self.assertEqual(result[4]["lat"], 51.8753146)
+        self.assertEqual(result[4]["lon"], -1.4857118)
         self.assertEqual(
-            result[4]['tag'], {
-                'empty': '',
-                'foo': 'bar',
-            }
+            result[4]["tag"],
+            {
+                "empty": "",
+                "foo": "bar",
+            },
         )
 
     def test_NodeWays(self):
         self._session_mock()
 
         result = self.api.NodeWays(234)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
-        self.assertEqual(args[1], self.api_base + '/api/0.6/node/234/ways')
+        self.assertEqual(args[0], "GET")
+        self.assertEqual(args[1], self.api_base + "/api/0.6/node/234/ways")
 
         self.assertEqual(len(result), 1)
-        self.assertEqual(result[0]['id'], 60)
-        self.assertEqual(result[0]['changeset'], 61)
+        self.assertEqual(result[0]["id"], 60)
+        self.assertEqual(result[0]["changeset"], 61)
         self.assertEqual(
-            result[0]['tag'],
+            result[0]["tag"],
             {
-                'highway': 'path',
-                'name': 'Dog walking path',
-            }
+                "highway": "path",
+                "name": "Dog walking path",
+            },
         )
 
     def test_NodeWaysNotExists(self):
         self._session_mock()
 
         result = self.api.NodeWays(404)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
-        self.assertEqual(args[1], f'{self.api_base}/api/0.6/node/404/ways')
+        self.assertEqual(args[0], "GET")
+        self.assertEqual(args[1], f"{self.api_base}/api/0.6/node/404/ways")
 
         self.assertEqual(len(result), 0)
         self.assertIsInstance(result, list)
 
     def test_NodeRelations(self):
         self._session_mock()
 
         result = self.api.NodeRelations(4295668179)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
-        self.assertEqual(
-            args[1],
-            f'{self.api_base}/api/0.6/node/4295668179/relations'
-        )
+        self.assertEqual(args[0], "GET")
+        self.assertEqual(args[1], f"{self.api_base}/api/0.6/node/4295668179/relations")
 
         self.assertEqual(len(result), 1)
-        self.assertEqual(result[0]['id'], 4294968148)
-        self.assertEqual(result[0]['changeset'], 23123)
+        self.assertEqual(result[0]["id"], 4294968148)
+        self.assertEqual(result[0]["changeset"], 23123)
         self.assertEqual(
-            result[0]['member'][1],
+            result[0]["member"][1],
             {
-                'role': 'point',
-                'ref': 4295668179,
-                'type': 'node',
-            }
+                "role": "point",
+                "ref": 4295668179,
+                "type": "node",
+            },
         )
         self.assertEqual(
-            result[0]['tag'],
+            result[0]["tag"],
             {
-                'type': 'fancy',
-            }
+                "type": "fancy",
+            },
         )
 
     def test_NodeRelationsUnusedElement(self):
         self._session_mock()
 
         result = self.api.NodeRelations(4295668179)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
-        self.assertEqual(
-            args[1],
-            self.api_base + '/api/0.6/node/4295668179/relations'
-        )
+        self.assertEqual(args[0], "GET")
+        self.assertEqual(args[1], self.api_base + "/api/0.6/node/4295668179/relations")
 
         self.assertEqual(len(result), 0)
         self.assertIsInstance(result, list)
 
     def test_NodesGet(self):
         self._session_mock()
 
         result = self.api.NodesGet([123, 345])
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
-        self.assertEqual(
-            args[1],
-            f'{self.api_base}/api/0.6/nodes?nodes=123,345'
-        )
+        self.assertEqual(args[0], "GET")
+        self.assertEqual(args[1], f"{self.api_base}/api/0.6/nodes?nodes=123,345")
 
         self.assertEqual(len(result), 2)
-        self.assertEqual(result[123], {
-            'id': 123,
-            'changeset': 15293,
-            'uid': 605,
-            'timestamp': datetime.datetime(2012, 4, 18, 11, 14, 26),
-            'lat': 51.8753146,
-            'lon': -1.4857118,
-            'visible': True,
-            'version': 8,
-            'user': 'freundchen',
-            'tag': {
-                'amenity': 'school',
-                'foo': 'bar',
-                'name': 'Berolina & Schule'
+        self.assertEqual(
+            result[123],
+            {
+                "id": 123,
+                "changeset": 15293,
+                "uid": 605,
+                "timestamp": datetime.datetime(2012, 4, 18, 11, 14, 26),
+                "lat": 51.8753146,
+                "lon": -1.4857118,
+                "visible": True,
+                "version": 8,
+                "user": "freundchen",
+                "tag": {"amenity": "school", "foo": "bar", "name": "Berolina & Schule"},
             },
-        })
-        self.assertEqual(result[345], {
-            'id': 345,
-            'changeset': 244,
-            'timestamp': datetime.datetime(2009, 9, 12, 3, 22, 59),
-            'uid': 1,
-            'visible': False,
-            'version': 2,
-            'user': 'guggis',
-            'tag': {},
-        })
+        )
+        self.assertEqual(
+            result[345],
+            {
+                "id": 345,
+                "changeset": 244,
+                "timestamp": datetime.datetime(2009, 9, 12, 3, 22, 59),
+                "uid": 1,
+                "visible": False,
+                "version": 2,
+                "user": "guggis",
+                "tag": {},
+            },
+        )
```

### Comparing `osmapi-3.1.0/tests/notes_test.py` & `osmapi-4.0.0/tests/notes_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,433 +1,430 @@
-from __future__ import (unicode_literals, absolute_import)
 from . import osmapi_test
 from datetime import datetime
 import osmapi
 
 try:
     import urlparse
 except ImportError:
     from urllib import parse as urlparse
 
 
 class TestOsmApiNotes(osmapi_test.TestOsmApi):
     def test_NotesGet(self):
         self._session_mock()
 
-        result = self.api.NotesGet(
-            -1.4998534,
-            45.9667901,
-            -1.4831815,
-            52.4710193
-        )
+        result = self.api.NotesGet(-1.4998534, 45.9667901, -1.4831815, 52.4710193)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
+        self.assertEqual(args[0], "GET")
         urlParts = urlparse.urlparse(args[1])
         params = urlparse.parse_qs(urlParts.query)
-        self.assertEqual(
-            params['bbox'][0],
-            '-1.499853,45.966790,-1.483181,52.471019'
-        )
-        self.assertEqual(params['limit'][0], '100')
-        self.assertEqual(params['closed'][0], '7')
+        self.assertEqual(params["bbox"][0], "-1.499853,45.966790,-1.483181,52.471019")
+        self.assertEqual(params["limit"][0], "100")
+        self.assertEqual(params["closed"][0], "7")
 
         self.assertEqual(len(result), 14)
-        self.assertEqual(result[2], {
-            'id': '231775',
-            'lon': -1.4929605,
-            'lat': 52.4107312,
-            'date_created': datetime(2014, 8, 28, 19, 25, 37),
-            'date_closed': datetime(2014, 9, 27, 9, 21, 41),
-            'status': 'closed',
-            'comments': [
-                {
-                    'date': datetime(2014, 8, 28, 19, 25, 37),
-                    'action': 'opened',
-                    'text': "Is it Paynes or Payne's",
-                    'html': "<p>Is it Paynes or Payne's</p>",
-                    'uid': '1486336',
-                    'user': 'Wyken Seagrave'
-                },
-                {
-                    'date': datetime(2014, 9, 26, 13, 5, 33),
-                    'action': 'commented',
-                    'text': "Royal Mail's postcode finder has PAYNES LANE",
-                    'html':
-                    (
-                        "<p>Royal Mail's postcode finder "
-                        "has PAYNES LANE</p>"
-                    ),
-                    'uid': None,
-                    'user': None
-                }
-            ]
-        })
+        self.assertEqual(
+            result[2],
+            {
+                "id": "231775",
+                "lon": -1.4929605,
+                "lat": 52.4107312,
+                "date_created": datetime(2014, 8, 28, 19, 25, 37),
+                "date_closed": datetime(2014, 9, 27, 9, 21, 41),
+                "status": "closed",
+                "comments": [
+                    {
+                        "date": datetime(2014, 8, 28, 19, 25, 37),
+                        "action": "opened",
+                        "text": "Is it Paynes or Payne's",
+                        "html": "<p>Is it Paynes or Payne's</p>",
+                        "uid": "1486336",
+                        "user": "Wyken Seagrave",
+                    },
+                    {
+                        "date": datetime(2014, 9, 26, 13, 5, 33),
+                        "action": "commented",
+                        "text": "Royal Mail's postcode finder has PAYNES LANE",
+                        "html": (
+                            "<p>Royal Mail's postcode finder " "has PAYNES LANE</p>"
+                        ),
+                        "uid": None,
+                        "user": None,
+                    },
+                ],
+            },
+        )
 
     def test_NotesGet_empty(self):
         self._session_mock()
 
         result = self.api.NotesGet(
-            -93.8472901,
-            35.9763601,
-            -80,
-            36.176360100000004,
-            limit=1,
-            closed=0
+            -93.8472901, 35.9763601, -80, 36.176360100000004, limit=1, closed=0
         )
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
+        self.assertEqual(args[0], "GET")
         urlParts = urlparse.urlparse(args[1])
         params = urlparse.parse_qs(urlParts.query)
 
-        self.assertEqual(params['limit'][0], '1')
-        self.assertEqual(params['closed'][0], '0')
+        self.assertEqual(params["limit"][0], "1")
+        self.assertEqual(params["closed"][0], "0")
 
         self.assertEqual(len(result), 0)
         self.assertEqual(result, [])
 
     def test_NoteGet(self):
         self._session_mock()
 
         result = self.api.NoteGet(1111)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
-        self.assertEqual(args[1], self.api_base + '/api/0.6/notes/1111')
+        self.assertEqual(args[0], "GET")
+        self.assertEqual(args[1], self.api_base + "/api/0.6/notes/1111")
 
-        self.assertEqual(result, {
-            'id': '1111',
-            'lon': 12.3133135,
-            'lat': 37.9305489,
-            'date_created': datetime(2013, 5, 1, 20, 58, 21),
-            'date_closed': datetime(2013, 8, 21, 16, 43, 26),
-            'status': 'closed',
-            'comments': [
-                {
-                    'date': datetime(2013, 5, 1, 20, 58, 21),
-                    'action': 'opened',
-                    'text': "It does not exist this path",
-                    'html': "<p>It does not exist this path</p>",
-                    'uid': '1363438',
-                    'user': 'giuseppemari'
-                },
-                {
-                    'date': datetime(2013, 8, 21, 16, 43, 26),
-                    'action': 'closed',
-                    'text': "there is no path signed",
-                    'html': "<p>there is no path signed</p>",
-                    'uid': '1714220',
-                    'user': 'luschi'
-                }
-            ]
-        })
+        self.assertEqual(
+            result,
+            {
+                "id": "1111",
+                "lon": 12.3133135,
+                "lat": 37.9305489,
+                "date_created": datetime(2013, 5, 1, 20, 58, 21),
+                "date_closed": datetime(2013, 8, 21, 16, 43, 26),
+                "status": "closed",
+                "comments": [
+                    {
+                        "date": datetime(2013, 5, 1, 20, 58, 21),
+                        "action": "opened",
+                        "text": "It does not exist this path",
+                        "html": "<p>It does not exist this path</p>",
+                        "uid": "1363438",
+                        "user": "giuseppemari",
+                    },
+                    {
+                        "date": datetime(2013, 8, 21, 16, 43, 26),
+                        "action": "closed",
+                        "text": "there is no path signed",
+                        "html": "<p>there is no path signed</p>",
+                        "uid": "1714220",
+                        "user": "luschi",
+                    },
+                ],
+            },
+        )
 
     def test_NoteGet_invalid_xml(self):
         self._session_mock()
 
         with self.assertRaises(osmapi.XmlResponseInvalidError):
             self.api.NoteGet(1111)
 
     def test_NoteCreate(self):
         self._session_mock(auth=True)
 
-        note = {
-            'lat': 47.123,
-            'lon': 8.432,
-            'text': 'This is a test'
-        }
+        note = {"lat": 47.123, "lon": 8.432, "text": "This is a test"}
         result = self.api.NoteCreate(note)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'POST')
+        self.assertEqual(args[0], "POST")
         urlParts = urlparse.urlparse(args[1])
         params = urlparse.parse_qs(urlParts.query)
-        self.assertEqual(params['lat'][0], '47.123')
-        self.assertEqual(params['lon'][0], '8.432')
-        self.assertEqual(params['text'][0], 'This is a test')
-
-        self.assertEqual(result, {
-            'id': '816',
-            'lat': 47.123,
-            'lon': 8.432,
-            'date_created': datetime(2014, 10, 3, 15, 21, 21),
-            'date_closed': None,
-            'status': 'open',
-            'comments': [
-                {
-                    'date': datetime(2014, 10, 3, 15, 21, 22),
-                    'action': 'opened',
-                    'text': "This is a test",
-                    'html': "<p>This is a test</p>",
-                    'uid': '1841',
-                    'user': 'metaodi'
-                }
-            ]
-        })
+        self.assertEqual(params["lat"][0], "47.123")
+        self.assertEqual(params["lon"][0], "8.432")
+        self.assertEqual(params["text"][0], "This is a test")
+
+        self.assertEqual(
+            result,
+            {
+                "id": "816",
+                "lat": 47.123,
+                "lon": 8.432,
+                "date_created": datetime(2014, 10, 3, 15, 21, 21),
+                "date_closed": None,
+                "status": "open",
+                "comments": [
+                    {
+                        "date": datetime(2014, 10, 3, 15, 21, 22),
+                        "action": "opened",
+                        "text": "This is a test",
+                        "html": "<p>This is a test</p>",
+                        "uid": "1841",
+                        "user": "metaodi",
+                    }
+                ],
+            },
+        )
 
     def test_NoteCreateAnonymous(self):
         self._session_mock()
 
-        note = {
-            'lat': 47.123,
-            'lon': 8.432,
-            'text': 'test 123'
-        }
+        note = {"lat": 47.123, "lon": 8.432, "text": "test 123"}
         result = self.api.NoteCreate(note)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'POST')
+        self.assertEqual(args[0], "POST")
         urlParts = urlparse.urlparse(args[1])
         params = urlparse.parse_qs(urlParts.query)
-        self.assertEqual(params['lat'][0], '47.123')
-        self.assertEqual(params['lon'][0], '8.432')
-        self.assertEqual(params['text'][0], 'test 123')
-
-        self.assertEqual(result, {
-            'id': '842',
-            'lat': 58.3368222,
-            'lon': 25.8826183,
-            'date_created': datetime(2015, 1, 3, 10, 49, 39),
-            'date_closed': None,
-            'status': 'open',
-            'comments': [
-                {
-                    'date': datetime(2015, 1, 3, 10, 49, 39),
-                    'action': 'opened',
-                    'text': "test 123",
-                    'html': "<p>test 123</p>",
-                    'uid': None,
-                    'user': None,
-                }
-            ]
-        })
+        self.assertEqual(params["lat"][0], "47.123")
+        self.assertEqual(params["lon"][0], "8.432")
+        self.assertEqual(params["text"][0], "test 123")
+
+        self.assertEqual(
+            result,
+            {
+                "id": "842",
+                "lat": 58.3368222,
+                "lon": 25.8826183,
+                "date_created": datetime(2015, 1, 3, 10, 49, 39),
+                "date_closed": None,
+                "status": "open",
+                "comments": [
+                    {
+                        "date": datetime(2015, 1, 3, 10, 49, 39),
+                        "action": "opened",
+                        "text": "test 123",
+                        "html": "<p>test 123</p>",
+                        "uid": None,
+                        "user": None,
+                    }
+                ],
+            },
+        )
 
     def test_NoteComment(self):
         self._session_mock(auth=True)
 
-        result = self.api.NoteComment(812, 'This is a comment')
+        result = self.api.NoteComment(812, "This is a comment")
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'POST')
+        self.assertEqual(args[0], "POST")
         self.assertEqual(
-            args[1],
-            self.api_base + '/api/0.6/notes/812/comment?text=This+is+a+comment'
+            args[1], self.api_base + "/api/0.6/notes/812/comment?text=This+is+a+comment"
         )
 
-        self.assertEqual(result, {
-            'id': '812',
-            'lat': 47.123,
-            'lon': 8.432,
-            'date_created': datetime(2014, 10, 3, 15, 11, 5),
-            'date_closed': None,
-            'status': 'open',
-            'comments': [
-                {
-                    'date': datetime(2014, 10, 3, 15, 11, 5),
-                    'action': 'opened',
-                    'text': "This is a test",
-                    'html': "<p>This is a test</p>",
-                    'uid': '1841',
-                    'user': 'metaodi'
-                },
-                {
-                    'date': datetime(2014, 10, 4, 22, 36, 35),
-                    'action': 'commented',
-                    'text': "This is a comment",
-                    'html': "<p>This is a comment</p>",
-                    'uid': '1841',
-                    'user': 'metaodi'
-                }
-            ]
-        })
+        self.assertEqual(
+            result,
+            {
+                "id": "812",
+                "lat": 47.123,
+                "lon": 8.432,
+                "date_created": datetime(2014, 10, 3, 15, 11, 5),
+                "date_closed": None,
+                "status": "open",
+                "comments": [
+                    {
+                        "date": datetime(2014, 10, 3, 15, 11, 5),
+                        "action": "opened",
+                        "text": "This is a test",
+                        "html": "<p>This is a test</p>",
+                        "uid": "1841",
+                        "user": "metaodi",
+                    },
+                    {
+                        "date": datetime(2014, 10, 4, 22, 36, 35),
+                        "action": "commented",
+                        "text": "This is a comment",
+                        "html": "<p>This is a comment</p>",
+                        "uid": "1841",
+                        "user": "metaodi",
+                    },
+                ],
+            },
+        )
 
     def test_NoteCommentAnonymous(self):
         self._session_mock()
 
-        result = self.api.NoteComment(842, 'blubb')
+        result = self.api.NoteComment(842, "blubb")
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'POST')
+        self.assertEqual(args[0], "POST")
         self.assertEqual(
-            args[1],
-            self.api_base + '/api/0.6/notes/842/comment?text=blubb'
+            args[1], self.api_base + "/api/0.6/notes/842/comment?text=blubb"
         )
 
-        self.assertEqual(result, {
-            'id': '842',
-            'lat': 58.3368222,
-            'lon': 25.8826183,
-            'date_created': datetime(2015, 1, 3, 10, 49, 39),
-            'date_closed': None,
-            'status': 'open',
-            'comments': [
-                {
-                    'date': datetime(2015, 1, 3, 10, 49, 39),
-                    'action': 'opened',
-                    'text': "test 123",
-                    'html': "<p>test 123</p>",
-                    'uid': None,
-                    'user': None,
-                },
-                {
-                    'date': datetime(2015, 1, 3, 11, 6, 0),
-                    'action': 'commented',
-                    'text': "blubb",
-                    'html': "<p>blubb</p>",
-                    'uid': None,
-                    'user': None,
-                }
-            ]
-        })
+        self.assertEqual(
+            result,
+            {
+                "id": "842",
+                "lat": 58.3368222,
+                "lon": 25.8826183,
+                "date_created": datetime(2015, 1, 3, 10, 49, 39),
+                "date_closed": None,
+                "status": "open",
+                "comments": [
+                    {
+                        "date": datetime(2015, 1, 3, 10, 49, 39),
+                        "action": "opened",
+                        "text": "test 123",
+                        "html": "<p>test 123</p>",
+                        "uid": None,
+                        "user": None,
+                    },
+                    {
+                        "date": datetime(2015, 1, 3, 11, 6, 0),
+                        "action": "commented",
+                        "text": "blubb",
+                        "html": "<p>blubb</p>",
+                        "uid": None,
+                        "user": None,
+                    },
+                ],
+            },
+        )
 
     def test_NoteCommentOnClosedNote(self):
         self._session_mock(status=409)
 
         with self.assertRaises(osmapi.NoteAlreadyClosedApiError) as cm:
-            self.api.NoteComment(817, 'Comment on closed note')
+            self.api.NoteComment(817, "Comment on closed note")
 
         self.assertEqual(cm.exception.status, 409)
         self.assertEqual(
-            cm.exception.payload,
-            "The note 817 was closed at 2022-04-29 20:57:20 UTC"
+            cm.exception.payload, "The note 817 was closed at 2022-04-29 20:57:20 UTC"
         )
 
     def test_NoteComment_non_existing_note(self):
         self._session_mock(status=404)
 
         with self.assertRaises(osmapi.ElementNotFoundApiError) as cm:
-            self.api.NoteComment(817, 'Comment on closed note')
+            self.api.NoteComment(817, "Comment on closed note")
 
         self.assertEqual(cm.exception.status, 404)
 
     def test_NoteClose(self):
         self._session_mock(auth=True)
 
-        result = self.api.NoteClose(819, 'Close this note!')
+        result = self.api.NoteClose(819, "Close this note!")
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'POST')
+        self.assertEqual(args[0], "POST")
         self.assertEqual(
-            args[1],
-            self.api_base + '/api/0.6/notes/819/close?text=Close+this+note%21'
+            args[1], self.api_base + "/api/0.6/notes/819/close?text=Close+this+note%21"
         )
 
-        self.assertEqual(result, {
-            'id': '815',
-            'lat': 47.123,
-            'lon': 8.432,
-            'date_created': datetime(2014, 10, 3, 15, 20, 57),
-            'date_closed': datetime(2014, 10, 5, 16, 35, 13),
-            'status': 'closed',
-            'comments': [
-                {
-                    'date': datetime(2014, 10, 3, 15, 20, 57),
-                    'action': 'opened',
-                    'text': "This is a test",
-                    'html': "<p>This is a test</p>",
-                    'uid': '1841',
-                    'user': 'metaodi'
-                },
-                {
-                    'date': datetime(2014, 10, 5, 16, 35, 13),
-                    'action': 'closed',
-                    'text': "Close this note!",
-                    'html': "<p>Close this note!</p>",
-                    'uid': '1841',
-                    'user': 'metaodi'
-                }
-            ]
-        })
+        self.assertEqual(
+            result,
+            {
+                "id": "815",
+                "lat": 47.123,
+                "lon": 8.432,
+                "date_created": datetime(2014, 10, 3, 15, 20, 57),
+                "date_closed": datetime(2014, 10, 5, 16, 35, 13),
+                "status": "closed",
+                "comments": [
+                    {
+                        "date": datetime(2014, 10, 3, 15, 20, 57),
+                        "action": "opened",
+                        "text": "This is a test",
+                        "html": "<p>This is a test</p>",
+                        "uid": "1841",
+                        "user": "metaodi",
+                    },
+                    {
+                        "date": datetime(2014, 10, 5, 16, 35, 13),
+                        "action": "closed",
+                        "text": "Close this note!",
+                        "html": "<p>Close this note!</p>",
+                        "uid": "1841",
+                        "user": "metaodi",
+                    },
+                ],
+            },
+        )
 
     def test_NoteAlreadyClosed(self):
         self._session_mock(auth=True, status=409)
 
         with self.assertRaises(osmapi.NoteAlreadyClosedApiError) as cm:
-            self.api.NoteClose(819, 'Close this note!')
+            self.api.NoteClose(819, "Close this note!")
 
         self.assertEqual(cm.exception.status, 409)
         self.assertEqual(
-            cm.exception.payload,
-            "The note 819 was closed at 2022-04-29 20:57:20 UTC"
+            cm.exception.payload, "The note 819 was closed at 2022-04-29 20:57:20 UTC"
         )
 
     def test_NoteReopen(self):
         self._session_mock(auth=True)
 
-        result = self.api.NoteReopen(815, 'Reopen this note!')
+        result = self.api.NoteReopen(815, "Reopen this note!")
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'POST')
+        self.assertEqual(args[0], "POST")
         self.assertEqual(
             args[1],
-            (self.api_base +
-             '/api/0.6/notes/815/reopen?text=Reopen+this+note%21')
+            (self.api_base + "/api/0.6/notes/815/reopen?text=Reopen+this+note%21"),
         )
 
-        self.assertEqual(result, {
-            'id': '815',
-            'lat': 47.123,
-            'lon': 8.432,
-            'date_created': datetime(2014, 10, 3, 15, 20, 57),
-            'date_closed': None,
-            'status': 'open',
-            'comments': [
-                {
-                    'date': datetime(2014, 10, 3, 15, 20, 57),
-                    'action': 'opened',
-                    'text': "This is a test",
-                    'html': "<p>This is a test</p>",
-                    'uid': '1841',
-                    'user': 'metaodi'
-                },
-                {
-                    'date': datetime(2014, 10, 5, 16, 35, 13),
-                    'action': 'closed',
-                    'text': "Close this note!",
-                    'html': "<p>Close this note!</p>",
-                    'uid': '1841',
-                    'user': 'metaodi'
-                },
-                {
-                    'date': datetime(2014, 10, 5, 16, 44, 56),
-                    'action': 'reopened',
-                    'text': "Reopen this note!",
-                    'html': "<p>Reopen this note!</p>",
-                    'uid': '1841',
-                    'user': 'metaodi'
-                }
-            ]
-        })
+        self.assertEqual(
+            result,
+            {
+                "id": "815",
+                "lat": 47.123,
+                "lon": 8.432,
+                "date_created": datetime(2014, 10, 3, 15, 20, 57),
+                "date_closed": None,
+                "status": "open",
+                "comments": [
+                    {
+                        "date": datetime(2014, 10, 3, 15, 20, 57),
+                        "action": "opened",
+                        "text": "This is a test",
+                        "html": "<p>This is a test</p>",
+                        "uid": "1841",
+                        "user": "metaodi",
+                    },
+                    {
+                        "date": datetime(2014, 10, 5, 16, 35, 13),
+                        "action": "closed",
+                        "text": "Close this note!",
+                        "html": "<p>Close this note!</p>",
+                        "uid": "1841",
+                        "user": "metaodi",
+                    },
+                    {
+                        "date": datetime(2014, 10, 5, 16, 44, 56),
+                        "action": "reopened",
+                        "text": "Reopen this note!",
+                        "html": "<p>Reopen this note!</p>",
+                        "uid": "1841",
+                        "user": "metaodi",
+                    },
+                ],
+            },
+        )
 
     def test_NotesSearch(self):
         self._session_mock()
 
-        result = self.api.NotesSearch('street')
+        result = self.api.NotesSearch("street")
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
+        self.assertEqual(args[0], "GET")
         urlParts = urlparse.urlparse(args[1])
         params = urlparse.parse_qs(urlParts.query)
-        self.assertEqual(params['q'][0], 'street')
-        self.assertEqual(params['limit'][0], '100')
-        self.assertEqual(params['closed'][0], '7')
+        self.assertEqual(params["q"][0], "street")
+        self.assertEqual(params["limit"][0], "100")
+        self.assertEqual(params["closed"][0], "7")
 
         self.assertEqual(len(result), 3)
-        self.assertEqual(result[1], {
-            'id': '788',
-            'lon': 11.96395,
-            'lat': 57.70301,
-            'date_created': datetime(2014, 7, 16, 16, 12, 41),
-            'date_closed': None,
-            'status': 'open',
-            'comments': [
-                {
-                    'date': datetime(2014, 7, 16, 16, 12, 41),
-                    'action': 'opened',
-                    'text': "One way street:\ncomment",
-                    'html': "<p>One way street:\n<br />comment</p>",
-                    'uid': None,
-                    'user': None
-                }
-            ]
-        })
+        self.assertEqual(
+            result[1],
+            {
+                "id": "788",
+                "lon": 11.96395,
+                "lat": 57.70301,
+                "date_created": datetime(2014, 7, 16, 16, 12, 41),
+                "date_closed": None,
+                "status": "open",
+                "comments": [
+                    {
+                        "date": datetime(2014, 7, 16, 16, 12, 41),
+                        "action": "opened",
+                        "text": "One way street:\ncomment",
+                        "html": "<p>One way street:\n<br />comment</p>",
+                        "uid": None,
+                        "user": None,
+                    }
+                ],
+            },
+        )
```

### Comparing `osmapi-3.1.0/tests/osmapi_test.py` & `osmapi-4.0.0/tests/osmapi_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,19 @@
-from __future__ import unicode_literals
 from osmapi import OsmApi
-import mock
+from unittest import mock
 import os
 import unittest
 
-__location__ = os.path.realpath(
-    os.path.join(
-        os.getcwd(),
-        os.path.dirname(__file__)
-    )
-)
+__location__ = os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
 
 
 class TestOsmApi(unittest.TestCase):
     def setUp(self):
         self.api_base = "http://api06.dev.openstreetmap.org"
-        self.api = OsmApi(
-            api=self.api_base
-        )
+        self.api = OsmApi(api=self.api_base)
         self.maxDiff = None
         print(self._testMethodName)
         print(self.api)
 
     def _session_mock(self, auth=False, filenames=None, status=200):
         response_mock = mock.Mock()
         response_mock.status_code = status
@@ -34,38 +26,31 @@
 
         self.session_mock = mock.Mock()
         self.session_mock.request = mock.Mock(return_value=response_mock)
 
         if auth:
             self.api = OsmApi(
                 api=self.api_base,
-                username='testuser',
-                password='testpassword',
-                session=self.session_mock
+                username="testuser",
+                password="testpassword",
+                session=self.session_mock,
             )
         else:
-            self.api = OsmApi(
-                api=self.api_base,
-                session=self.session_mock
-            )
+            self.api = OsmApi(api=self.api_base, session=self.session_mock)
 
         self.api._get_http_session = mock.Mock(return_value=self.session_mock)
         self.api._session._sleep = mock.Mock()
 
     def _return_values(self, filenames):
         if filenames is None:
             filenames = [self._testMethodName + ".xml"]
 
         return_values = []
         for filename in filenames:
-            path = os.path.join(
-                __location__,
-                'fixtures',
-                filename
-            )
+            path = os.path.join(__location__, "fixtures", filename)
             try:
                 with open(path) as file:
                     return_values.append(file.read())
             except Exception:
                 pass
         return return_values
```

### Comparing `osmapi-3.1.0/tests/relation_test.py` & `osmapi-4.0.0/tests/relation_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,339 +1,252 @@
-from __future__ import (unicode_literals, absolute_import)
 from . import osmapi_test
 import osmapi
-import mock
+from unittest import mock
 import datetime
 
 
 class TestOsmApiRelation(osmapi_test.TestOsmApi):
     def test_RelationGet(self):
         self._session_mock()
 
         result = self.api.RelationGet(321)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
-        self.assertEqual(args[1], self.api_base + '/api/0.6/relation/321')
+        self.assertEqual(args[0], "GET")
+        self.assertEqual(args[1], self.api_base + "/api/0.6/relation/321")
 
-        self.assertEqual(result, {
-            'id': 321,
-            'changeset': 434,
-            'uid': 12,
-            'timestamp': datetime.datetime(2009, 9, 15, 22, 24, 25),
-            'visible': True,
-            'version': 1,
-            'user': 'green525',
-            'tag': {
-                'admin_level': '9',
-                'boundary': 'administrative',
-                'type': 'multipolygon',
+        self.assertEqual(
+            result,
+            {
+                "id": 321,
+                "changeset": 434,
+                "uid": 12,
+                "timestamp": datetime.datetime(2009, 9, 15, 22, 24, 25),
+                "visible": True,
+                "version": 1,
+                "user": "green525",
+                "tag": {
+                    "admin_level": "9",
+                    "boundary": "administrative",
+                    "type": "multipolygon",
+                },
+                "member": [
+                    {"ref": 6908, "role": "outer", "type": "way"},
+                    {"ref": 6352, "role": "outer", "type": "way"},
+                    {"ref": 5669, "role": "outer", "type": "way"},
+                    {"ref": 5682, "role": "outer", "type": "way"},
+                    {"ref": 6909, "role": "outer", "type": "way"},
+                    {"ref": 6355, "role": "outer", "type": "way"},
+                    {"ref": 6910, "role": "outer", "type": "way"},
+                    {"ref": 6911, "role": "outer", "type": "way"},
+                    {"ref": 6912, "role": "outer", "type": "way"},
+                ],
             },
-            'member': [
-                {
-                    'ref': 6908,
-                    'role': 'outer',
-                    'type': 'way'
-                },
-                {
-                    'ref': 6352,
-                    'role': 'outer',
-                    'type': 'way'
-                },
-                {
-                    'ref': 5669,
-                    'role': 'outer',
-                    'type': 'way'
-                },
-                {
-                    'ref': 5682,
-                    'role': 'outer',
-                    'type': 'way'
-                },
-                {
-                    'ref': 6909,
-                    'role': 'outer',
-                    'type': 'way'
-                },
-                {
-                    'ref': 6355,
-                    'role': 'outer',
-                    'type': 'way'
-                },
-                {
-                    'ref': 6910,
-                    'role': 'outer',
-                    'type': 'way'
-                },
-                {
-                    'ref': 6911,
-                    'role': 'outer',
-                    'type': 'way'
-                },
-                {
-                    'ref': 6912,
-                    'role': 'outer',
-                    'type': 'way'
-                }
-            ]
-        })
+        )
 
     def test_RelationGet_with_version(self):
         self._session_mock()
 
         result = self.api.RelationGet(765, 2)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
-        self.assertEqual(args[1], self.api_base + '/api/0.6/relation/765/2')
+        self.assertEqual(args[0], "GET")
+        self.assertEqual(args[1], self.api_base + "/api/0.6/relation/765/2")
 
-        self.assertEqual(result['id'], 765)
-        self.assertEqual(result['changeset'], 41378)
-        self.assertEqual(result['user'], 'metaodi')
-        self.assertEqual(result['tag']['source'], 'test')
+        self.assertEqual(result["id"], 765)
+        self.assertEqual(result["changeset"], 41378)
+        self.assertEqual(result["user"], "metaodi")
+        self.assertEqual(result["tag"]["source"], "test")
 
     def test_RelationCreate(self):
         self._session_mock(auth=True)
 
         # setup mock
-        self.api.ChangesetCreate = mock.Mock(
-            return_value=3333
-        )
+        self.api.ChangesetCreate = mock.Mock(return_value=3333)
         self.api._CurrentChangesetId = 3333
 
         test_relation = {
-            'tag': {
-                'type': 'test',
+            "tag": {
+                "type": "test",
             },
-            'member': [
-                {
-                    'ref': 6908,
-                    'role': 'outer',
-                    'type': 'way'
-                },
-                {
-                    'ref': 6352,
-                    'role': 'point',
-                    'type': 'node'
-                },
-            ]
+            "member": [
+                {"ref": 6908, "role": "outer", "type": "way"},
+                {"ref": 6352, "role": "point", "type": "node"},
+            ],
         }
 
-        cs = self.api.ChangesetCreate({
-            'comment': 'This is a test relation'
-        })
+        cs = self.api.ChangesetCreate({"comment": "This is a test relation"})
         self.assertEqual(cs, 3333)
 
         result = self.api.RelationCreate(test_relation)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'PUT')
-        self.assertEqual(args[1], self.api_base + '/api/0.6/relation/create')
+        self.assertEqual(args[0], "PUT")
+        self.assertEqual(args[1], self.api_base + "/api/0.6/relation/create")
 
-        self.assertEqual(result['id'], 8989)
-        self.assertEqual(result['version'], 1)
-        self.assertEqual(result['member'], test_relation['member'])
-        self.assertEqual(result['tag'], test_relation['tag'])
+        self.assertEqual(result["id"], 8989)
+        self.assertEqual(result["version"], 1)
+        self.assertEqual(result["member"], test_relation["member"])
+        self.assertEqual(result["tag"], test_relation["tag"])
 
     def test_RelationCreate_existing_node(self):
         # setup mock
-        self.api.ChangesetCreate = mock.Mock(
-            return_value=1111
-        )
+        self.api.ChangesetCreate = mock.Mock(return_value=1111)
         self.api._CurrentChangesetId = 1111
 
         test_relation = {
-            'id': 456,
-            'tag': {
-                'type': 'test',
+            "id": 456,
+            "tag": {
+                "type": "test",
             },
-            'member': [
-                {
-                    'ref': 6908,
-                    'role': 'outer',
-                    'type': 'way'
-                },
-                {
-                    'ref': 6352,
-                    'role': 'point',
-                    'type': 'node'
-                },
-            ]
+            "member": [
+                {"ref": 6908, "role": "outer", "type": "way"},
+                {"ref": 6352, "role": "point", "type": "node"},
+            ],
         }
 
         with self.assertRaisesRegex(
-                osmapi.OsmTypeAlreadyExistsError,
-                'This relation already exists'):
+            osmapi.OsmTypeAlreadyExistsError, "This relation already exists"
+        ):
             self.api.RelationCreate(test_relation)
 
     def test_RelationUpdate(self):
         self._session_mock(auth=True)
 
         # setup mock
-        self.api.ChangesetCreate = mock.Mock(
-            return_value=3333
-        )
+        self.api.ChangesetCreate = mock.Mock(return_value=3333)
         self.api._CurrentChangesetId = 3333
 
         test_relation = {
-            'id': 8989,
-            'tag': {
-                'type': 'test update',
+            "id": 8989,
+            "tag": {
+                "type": "test update",
             },
-            'member': [
-                {
-                    'ref': 6908,
-                    'role': 'outer',
-                    'type': 'way'
-                }
-            ]
+            "member": [{"ref": 6908, "role": "outer", "type": "way"}],
         }
 
-        cs = self.api.ChangesetCreate({
-            'comment': 'This is a test relation'
-        })
+        cs = self.api.ChangesetCreate({"comment": "This is a test relation"})
         self.assertEqual(cs, 3333)
 
         result = self.api.RelationUpdate(test_relation)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'PUT')
-        self.assertEqual(args[1], self.api_base + '/api/0.6/relation/8989')
+        self.assertEqual(args[0], "PUT")
+        self.assertEqual(args[1], self.api_base + "/api/0.6/relation/8989")
 
-        self.assertEqual(result['id'], 8989)
-        self.assertEqual(result['version'], 42)
-        self.assertEqual(result['member'], test_relation['member'])
-        self.assertEqual(result['tag'], test_relation['tag'])
+        self.assertEqual(result["id"], 8989)
+        self.assertEqual(result["version"], 42)
+        self.assertEqual(result["member"], test_relation["member"])
+        self.assertEqual(result["tag"], test_relation["tag"])
 
     def test_RelationDelete(self):
         self._session_mock(auth=True)
 
         # setup mock
-        self.api.ChangesetCreate = mock.Mock(
-            return_value=3333
-        )
+        self.api.ChangesetCreate = mock.Mock(return_value=3333)
         self.api._CurrentChangesetId = 3333
 
-        test_relation = {
-            'id': 8989
-        }
+        test_relation = {"id": 8989}
 
-        cs = self.api.ChangesetCreate({
-            'comment': 'This is a test relation'
-        })
+        cs = self.api.ChangesetCreate({"comment": "This is a test relation"})
         self.assertEqual(cs, 3333)
 
         result = self.api.RelationDelete(test_relation)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'DELETE')
-        self.assertEqual(args[1], self.api_base + '/api/0.6/relation/8989')
+        self.assertEqual(args[0], "DELETE")
+        self.assertEqual(args[1], self.api_base + "/api/0.6/relation/8989")
 
-        self.assertEqual(result['id'], 8989)
-        self.assertEqual(result['version'], 43)
+        self.assertEqual(result["id"], 8989)
+        self.assertEqual(result["version"], 43)
 
     def test_RelationHistory(self):
         self._session_mock()
 
         result = self.api.RelationHistory(2470397)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
-        self.assertEqual(
-            args[1],
-            f'{self.api_base}/api/0.6/relation/2470397/history'
-        )
+        self.assertEqual(args[0], "GET")
+        self.assertEqual(args[1], f"{self.api_base}/api/0.6/relation/2470397/history")
 
         self.assertEqual(len(result), 2)
-        self.assertEqual(result[1]['id'], 2470397)
-        self.assertEqual(result[1]['version'], 1)
+        self.assertEqual(result[1]["id"], 2470397)
+        self.assertEqual(result[1]["version"], 1)
         self.assertEqual(
-            result[1]['tag'], {
-                'restriction': 'only_straight_on',
-                'type': 'restriction',
-            }
+            result[1]["tag"],
+            {
+                "restriction": "only_straight_on",
+                "type": "restriction",
+            },
         )
-        self.assertEqual(result[2]['version'], 2)
+        self.assertEqual(result[2]["version"], 2)
 
     def test_RelationRelations(self):
         self._session_mock()
 
         result = self.api.RelationRelations(1532552)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
-        self.assertEqual(
-            args[1],
-            f'{self.api_base}/api/0.6/relation/1532552/relations'
-        )
+        self.assertEqual(args[0], "GET")
+        self.assertEqual(args[1], f"{self.api_base}/api/0.6/relation/1532552/relations")
 
         self.assertEqual(len(result), 1)
-        self.assertEqual(result[0]['id'], 1532553)
-        self.assertEqual(result[0]['version'], 85)
-        self.assertEqual(len(result[0]['member']), 120)
-        self.assertEqual(result[0]['tag']['type'], 'network')
-        self.assertEqual(
-            result[0]['tag']['name'],
-            'Aargauischer Radroutennetz'
-        )
+        self.assertEqual(result[0]["id"], 1532553)
+        self.assertEqual(result[0]["version"], 85)
+        self.assertEqual(len(result[0]["member"]), 120)
+        self.assertEqual(result[0]["tag"]["type"], "network")
+        self.assertEqual(result[0]["tag"]["name"], "Aargauischer Radroutennetz")
 
     def test_RelationRelationsUnusedElement(self):
         self._session_mock()
 
         result = self.api.RelationRelations(1532552)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
-        self.assertEqual(
-            args[1],
-            f'{self.api_base}/api/0.6/relation/1532552/relations'
-        )
+        self.assertEqual(args[0], "GET")
+        self.assertEqual(args[1], f"{self.api_base}/api/0.6/relation/1532552/relations")
 
         self.assertEqual(len(result), 0)
         self.assertIsInstance(result, list)
 
     def test_RelationFull(self):
         self._session_mock()
 
         result = self.api.RelationFull(2470397)
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
-        self.assertEqual(
-            args[1],
-            f'{self.api_base}/api/0.6/relation/2470397/full'
-        )
+        self.assertEqual(args[0], "GET")
+        self.assertEqual(args[1], f"{self.api_base}/api/0.6/relation/2470397/full")
 
         self.assertEqual(len(result), 11)
-        self.assertEqual(result[1]['data']['id'], 101142277)
-        self.assertEqual(result[1]['data']['version'], 8)
-        self.assertEqual(result[1]['type'], 'node')
-        self.assertEqual(result[10]['data']['id'], 2470397)
-        self.assertEqual(result[10]['data']['version'], 2)
-        self.assertEqual(result[10]['type'], 'relation')
+        self.assertEqual(result[1]["data"]["id"], 101142277)
+        self.assertEqual(result[1]["data"]["version"], 8)
+        self.assertEqual(result[1]["type"], "node")
+        self.assertEqual(result[10]["data"]["id"], 2470397)
+        self.assertEqual(result[10]["data"]["version"], 2)
+        self.assertEqual(result[10]["type"], "relation")
 
     def test_RelationsGet(self):
         self._session_mock()
 
         result = self.api.RelationsGet([1532552, 1532553])
 
         args, kwargs = self.session_mock.request.call_args
-        self.assertEqual(args[0], 'GET')
+        self.assertEqual(args[0], "GET")
         self.assertEqual(
-            args[1],
-            f'{self.api_base}/api/0.6/relations?relations=1532552,1532553'
+            args[1], f"{self.api_base}/api/0.6/relations?relations=1532552,1532553"
         )
 
         self.assertEqual(len(result), 2)
-        self.assertEqual(result[1532553]['id'], 1532553)
-        self.assertEqual(result[1532553]['version'], 85)
-        self.assertEqual(result[1532553]['user'], 'SimonPoole')
-        self.assertEqual(result[1532552]['id'], 1532552)
-        self.assertEqual(result[1532552]['visible'], True)
-        self.assertEqual(result[1532552]['tag']['route'], 'bicycle')
+        self.assertEqual(result[1532553]["id"], 1532553)
+        self.assertEqual(result[1532553]["version"], 85)
+        self.assertEqual(result[1532553]["user"], "SimonPoole")
+        self.assertEqual(result[1532552]["id"], 1532552)
+        self.assertEqual(result[1532552]["visible"], True)
+        self.assertEqual(result[1532552]["tag"]["route"], "bicycle")
 
     def test_RelationFull_with_deleted_relation(self):
         self._session_mock(filenames=[], status=410)
 
         with self.assertRaises(osmapi.ElementDeletedApiError) as context:
             self.api.RelationFull(2911456)
         self.assertEqual(410, context.exception.status)
```

