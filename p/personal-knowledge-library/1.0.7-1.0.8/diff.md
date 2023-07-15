# Comparing `tmp/personal_knowledge_library-1.0.7.tar.gz` & `tmp/personal_knowledge_library-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "personal_knowledge_library-1.0.7.tar", last modified: Thu Jul 13 08:30:46 2023, max compression
+gzip compressed data, was "personal_knowledge_library-1.0.8.tar", last modified: Sat Jul 15 17:21:35 2023, max compression
```

## Comparing `personal_knowledge_library-1.0.7.tar` & `personal_knowledge_library-1.0.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:46.990393 personal_knowledge_library-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-07-13 08:30:46.990393 personal_knowledge_library-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    43169 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:46.986393 personal_knowledge_library-1.0.7/knowledge/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:46.990393 personal_knowledge_library-1.0.7/knowledge/base/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/base/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/base/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    80585 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/base/ontology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:46.990393 personal_knowledge_library-1.0.7/knowledge/nel/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/nel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/nel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/nel/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:46.990393 personal_knowledge_library-1.0.7/knowledge/ontomapping/
--rw-r--r--   0 runner    (1001) docker     (123)    17363 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/ontomapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/ontomapping/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:46.990393 personal_knowledge_library-1.0.7/knowledge/public/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/public/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/public/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/public/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)    44912 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/public/wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:46.990393 personal_knowledge_library-1.0.7/knowledge/services/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/services/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/services/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    20881 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/services/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    29652 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/services/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/services/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/services/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:46.990393 personal_knowledge_library-1.0.7/knowledge/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/utils/rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/knowledge/utils/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:30:46.990393 personal_knowledge_library-1.0.7/personal_knowledge_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-07-13 08:30:46.000000 personal_knowledge_library-1.0.7/personal_knowledge_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-13 08:30:46.000000 personal_knowledge_library-1.0.7/personal_knowledge_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:30:46.000000 personal_knowledge_library-1.0.7/personal_knowledge_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-13 08:30:46.000000 personal_knowledge_library-1.0.7/personal_knowledge_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-13 08:30:46.000000 personal_knowledge_library-1.0.7/personal_knowledge_library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-13 08:30:46.994392 personal_knowledge_library-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-13 08:30:31.000000 personal_knowledge_library-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:21:35.915992 personal_knowledge_library-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-07-15 17:21:35.915992 personal_knowledge_library-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    43169 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:21:35.911992 personal_knowledge_library-1.0.8/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:21:35.911992 personal_knowledge_library-1.0.8/knowledge/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/base/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7995 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/base/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80585 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/base/ontology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:21:35.911992 personal_knowledge_library-1.0.8/knowledge/nel/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/nel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/nel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/nel/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:21:35.911992 personal_knowledge_library-1.0.8/knowledge/ontomapping/
+-rw-r--r--   0 runner    (1001) docker     (123)    17363 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/ontomapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/ontomapping/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:21:35.911992 personal_knowledge_library-1.0.8/knowledge/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/public/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/public/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/public/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44912 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/public/wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:21:35.911992 personal_knowledge_library-1.0.8/knowledge/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/services/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20881 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/services/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29652 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/services/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/services/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/services/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:21:35.911992 personal_knowledge_library-1.0.8/knowledge/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/utils/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/knowledge/utils/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:21:35.915992 personal_knowledge_library-1.0.8/personal_knowledge_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    44039 2023-07-15 17:21:35.000000 personal_knowledge_library-1.0.8/personal_knowledge_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-15 17:21:35.000000 personal_knowledge_library-1.0.8/personal_knowledge_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 17:21:35.000000 personal_knowledge_library-1.0.8/personal_knowledge_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-15 17:21:35.000000 personal_knowledge_library-1.0.8/personal_knowledge_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-15 17:21:35.000000 personal_knowledge_library-1.0.8/personal_knowledge_library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-15 17:21:35.915992 personal_knowledge_library-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-15 17:21:20.000000 personal_knowledge_library-1.0.8/setup.py
```

### Comparing `personal_knowledge_library-1.0.7/LICENSE` & `personal_knowledge_library-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/PKG-INFO` & `personal_knowledge_library-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal_knowledge_library
-Version: 1.0.7
+Version: 1.0.8
 Summary: Library to access Wacom's Personal Knowledge graph.
 Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
 Author: Markus Weber
 Author-email: markus.weber@wacom.com
 License: Apache 2.0 License
 Keywords: semantic-knowledge;knowledge-graph
 Platform: UNKNOWN
```

### Comparing `personal_knowledge_library-1.0.7/README.md` & `personal_knowledge_library-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/__init__.py` & `personal_knowledge_library-1.0.8/knowledge/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 __author__ = "Markus Weber"
 __copyright__ = "Copyright 2021-2023 Wacom. All rights reserved."
 __credits__ = ["Markus Weber"]
 __license__ = "Wacom"
 __maintainer__ = ["Markus Weber"]
 __email__ = "markus.weber@wacom.com"
 __status__ = "beta"
-__version__ = "1.0.7"
+__version__ = "1.0.8"
 
 # Create the Logger
 logger: Union[logging.Logger, None] = None
 
 if logger is None:
     logger = logging.getLogger(__name__)
     logger.setLevel(logging.DEBUG)
```

### Comparing `personal_knowledge_library-1.0.7/knowledge/base/__init__.py` & `personal_knowledge_library-1.0.8/knowledge/base/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/base/access.py` & `personal_knowledge_library-1.0.8/knowledge/base/access.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/base/entity.py` & `personal_knowledge_library-1.0.8/knowledge/base/entity.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/base/ontology.py` & `personal_knowledge_library-1.0.8/knowledge/base/ontology.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/nel/base.py` & `personal_knowledge_library-1.0.8/knowledge/nel/base.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/nel/engine.py` & `personal_knowledge_library-1.0.8/knowledge/nel/engine.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/ontomapping/__init__.py` & `personal_knowledge_library-1.0.8/knowledge/ontomapping/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/ontomapping/manager.py` & `personal_knowledge_library-1.0.8/knowledge/ontomapping/manager.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/public/__init__.py` & `personal_knowledge_library-1.0.8/knowledge/public/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/public/cache.py` & `personal_knowledge_library-1.0.8/knowledge/public/cache.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/public/helper.py` & `personal_knowledge_library-1.0.8/knowledge/public/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -355,14 +355,17 @@
         response: Response = session.get(url)
 
         # Check the response status code
         if not response.ok:
             raise WikiDataAPIException(f"Request failed with status code : {response.status_code}. URL:= {url}")
         entity_dict_full: Dict[str, Any] = response.json()
         results: List[Dict[str, Any]] = []
+        # If no entities found
+        if "entities" not in entity_dict_full:
+            return results
         for qid, e in entity_dict_full["entities"].items():
             if qid not in entity_ids:
                 logger.warning(f"Wikidata redirect detected. "
                                f"Returned entity id={qid} is not in list of entity ids.")
             if 'missing' in e:
                 logger.warning(f"Missing entity detected. Returned entity id={qid} is not in Wikidata found.")
                 continue
```

### Comparing `personal_knowledge_library-1.0.7/knowledge/public/relations.py` & `personal_knowledge_library-1.0.8/knowledge/public/relations.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/public/wikidata.py` & `personal_knowledge_library-1.0.8/knowledge/public/wikidata.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/services/__init__.py` & `personal_knowledge_library-1.0.8/knowledge/services/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/services/base.py` & `personal_knowledge_library-1.0.8/knowledge/services/base.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/services/graph.py` & `personal_knowledge_library-1.0.8/knowledge/services/graph.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/services/group.py` & `personal_knowledge_library-1.0.8/knowledge/services/group.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/services/ontology.py` & `personal_knowledge_library-1.0.8/knowledge/services/ontology.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/services/tenant.py` & `personal_knowledge_library-1.0.8/knowledge/services/tenant.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/services/users.py` & `personal_knowledge_library-1.0.8/knowledge/services/users.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/utils/rdf.py` & `personal_knowledge_library-1.0.8/knowledge/utils/rdf.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/knowledge/utils/wikipedia.py` & `personal_knowledge_library-1.0.8/knowledge/utils/wikipedia.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/personal_knowledge_library.egg-info/PKG-INFO` & `personal_knowledge_library-1.0.8/personal_knowledge_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal-knowledge-library
-Version: 1.0.7
+Version: 1.0.8
 Summary: Library to access Wacom's Personal Knowledge graph.
 Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
 Author: Markus Weber
 Author-email: markus.weber@wacom.com
 License: Apache 2.0 License
 Keywords: semantic-knowledge;knowledge-graph
 Platform: UNKNOWN
```

### Comparing `personal_knowledge_library-1.0.7/personal_knowledge_library.egg-info/SOURCES.txt` & `personal_knowledge_library-1.0.8/personal_knowledge_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-1.0.7/setup.py` & `personal_knowledge_library-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 an older version of knowledge-service-lib :
     $ python -m pip install personal-knowledge-library
 """)
     sys.exit(1)
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
-__version__ = "1.0.7"
+__version__ = "1.0.8"
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # the setup
 setup(
     name='personal_knowledge_library',
```

