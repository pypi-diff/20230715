# Comparing `tmp/volttron_lib_tagging-0.1.1a0.tar.gz` & `tmp/volttron_lib_tagging-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_lib_tagging-0.1.1a0.tar", max compression
+gzip compressed data, was "volttron_lib_tagging-0.1.1a1.tar", max compression
```

## Comparing `volttron_lib_tagging-0.1.1a0.tar` & `volttron_lib_tagging-0.1.1a1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     4436 2023-07-11 20:56:05.347373 volttron_lib_tagging-0.1.1a0/README.md
--rw-r--r--   0        0        0     1793 2023-07-11 20:56:05.347373 volttron_lib_tagging-0.1.1a0/data_model/categories.csv
--rw-r--r--   0        0        0    15336 2023-07-11 20:56:05.347373 volttron_lib_tagging-0.1.1a0/data_model/category_tags.txt
--rw-r--r--   0        0        0      349 2023-07-11 20:56:05.347373 volttron_lib_tagging-0.1.1a0/data_model/tag_refs.csv
--rw-r--r--   0        0        0    20679 2023-07-11 20:56:05.347373 volttron_lib_tagging-0.1.1a0/data_model/tags.csv
--rw-r--r--   0        0        0     7674 2023-07-11 20:56:05.347373 volttron_lib_tagging-0.1.1a0/data_model/units.txt
--rw-r--r--   0        0        0     1329 2023-07-11 20:58:39.297537 volttron_lib_tagging-0.1.1a0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-11 20:56:05.347373 volttron_lib_tagging-0.1.1a0/src/tagging/base/__init__.py
--rw-r--r--   0        0        0    37172 2023-07-11 20:56:05.347373 volttron_lib_tagging-0.1.1a0/src/tagging/base/base_tagging.py
--rw-r--r--   0        0        0     6005 2023-07-11 20:56:05.347373 volttron_lib_tagging-0.1.1a0/src/tagging/base/parsetab.py
--rw-r--r--   0        0        0        0 2023-07-11 20:56:05.347373 volttron_lib_tagging-0.1.1a0/tests/tagging/testing/__init__.py
--rw-r--r--   0        0        0    21843 2023-07-11 20:56:05.347373 volttron_lib_tagging-0.1.1a0/tests/tagging/testing/integration_test_interface.py
--rw-r--r--   0        0        0     1111 2023-07-11 20:56:05.347373 volttron_lib_tagging-0.1.1a0/tests/tagging/testing/test_base_tagging_unit.py
--rw-r--r--   0        0        0     5474 1970-01-01 00:00:00.000000 volttron_lib_tagging-0.1.1a0/setup.py
--rw-r--r--   0        0        0     5223 1970-01-01 00:00:00.000000 volttron_lib_tagging-0.1.1a0/PKG-INFO
+-rw-r--r--   0        0        0     4436 2023-07-14 23:33:39.338296 volttron_lib_tagging-0.1.1a1/README.md
+-rw-r--r--   0        0        0     1365 2023-07-14 23:35:48.591126 volttron_lib_tagging-0.1.1a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 23:33:39.338296 volttron_lib_tagging-0.1.1a1/src/tagging/base/__init__.py
+-rw-r--r--   0        0        0    37162 2023-07-14 23:33:39.338296 volttron_lib_tagging-0.1.1a1/src/tagging/base/base_tagging.py
+-rw-r--r--   0        0        0     6005 2023-07-14 23:33:39.338296 volttron_lib_tagging-0.1.1a1/src/tagging/base/parsetab.py
+-rw-r--r--   0        0        0     1793 2023-07-14 23:33:39.338296 volttron_lib_tagging-0.1.1a1/src/tagging/data_model/categories.csv
+-rw-r--r--   0        0        0    15336 2023-07-14 23:33:39.338296 volttron_lib_tagging-0.1.1a1/src/tagging/data_model/category_tags.txt
+-rw-r--r--   0        0        0      349 2023-07-14 23:33:39.338296 volttron_lib_tagging-0.1.1a1/src/tagging/data_model/tag_refs.csv
+-rw-r--r--   0        0        0    20679 2023-07-14 23:33:39.338296 volttron_lib_tagging-0.1.1a1/src/tagging/data_model/tags.csv
+-rw-r--r--   0        0        0     7674 2023-07-14 23:33:39.338296 volttron_lib_tagging-0.1.1a1/src/tagging/data_model/units.txt
+-rw-r--r--   0        0        0        0 2023-07-14 23:33:39.338296 volttron_lib_tagging-0.1.1a1/tests/tagging/testing/__init__.py
+-rw-r--r--   0        0        0    21843 2023-07-14 23:33:39.338296 volttron_lib_tagging-0.1.1a1/tests/tagging/testing/integration_test_interface.py
+-rw-r--r--   0        0        0     1111 2023-07-14 23:33:39.338296 volttron_lib_tagging-0.1.1a1/tests/tagging/testing/test_base_tagging_unit.py
+-rw-r--r--   0        0        0     5503 1970-01-01 00:00:00.000000 volttron_lib_tagging-0.1.1a1/setup.py
+-rw-r--r--   0        0        0     5223 1970-01-01 00:00:00.000000 volttron_lib_tagging-0.1.1a1/PKG-INFO
```

### Comparing `volttron_lib_tagging-0.1.1a0/README.md` & `volttron_lib_tagging-0.1.1a1/README.md`

 * *Files identical despite different names*

### Comparing `volttron_lib_tagging-0.1.1a0/data_model/categories.csv` & `volttron_lib_tagging-0.1.1a1/src/tagging/data_model/categories.csv`

 * *Files identical despite different names*

### Comparing `volttron_lib_tagging-0.1.1a0/data_model/category_tags.txt` & `volttron_lib_tagging-0.1.1a1/src/tagging/data_model/category_tags.txt`

 * *Files identical despite different names*

### Comparing `volttron_lib_tagging-0.1.1a0/data_model/tags.csv` & `volttron_lib_tagging-0.1.1a1/src/tagging/data_model/tags.csv`

 * *Files identical despite different names*

### Comparing `volttron_lib_tagging-0.1.1a0/data_model/units.txt` & `volttron_lib_tagging-0.1.1a1/src/tagging/data_model/units.txt`

 * *Files identical despite different names*

### Comparing `volttron_lib_tagging-0.1.1a0/pyproject.toml` & `volttron_lib_tagging-0.1.1a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 [tool.poetry]
 name = "volttron-lib-tagging"
-version = "0.1.1a0"
+version = "0.1.1a1"
 description = "A base tagging agent api with extension points for using with the VOLTTRON platform. This base agent works with Haystack 3 tags"
 authors = ["VOLTTRON Team <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/eclipse-volttron/volttron-lib-tagging"
 homepage = "https://github.com/eclipse-volttron/volttron-lib-tagging"
 keywords = []
 packages = [ { include = "tagging", from = "src" }, { include = "tagging", from = "tests" } ]
-include = ["data_model"]
+
+[tool.setuptools.package-data]
+"tagging.data_model" = ["*"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 volttron = ">=10.0.3a9,<11.0"
 ply = "^3.11"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `volttron_lib_tagging-0.1.1a0/src/tagging/base/base_tagging.py` & `volttron_lib_tagging-0.1.1a1/src/tagging/base/base_tagging.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 :py:meth:`BaseTaggingAgent.get_topics_by_tags` for syntax definition of query
 
 """
 
 import logging
 import os
 import re
+from importlib.resources import path as get_path
 
 from abc import abstractmethod
 
 from volttron.client.known_identities import PLATFORM_HISTORIAN
 from volttron.client.vip.agent import Agent, Core, RPC
 from volttron.client.vip.agent.errors import Unreachable
 
@@ -75,16 +76,15 @@
         super(BaseTaggingAgent, self).__init__(**kwargs)
         self.valid_tags = dict()
         self.tag_refs = dict()
         self.historian_vip_identity = historian_vip_identity
         if historian_vip_identity is None:
             self.historian_vip_identity = PLATFORM_HISTORIAN
         current_dir = os.path.dirname(os.path.abspath(__file__))
-        self.resource_sub_dir = os.path.join(current_dir, "../../..",
-                                             "data_model")
+        self.resource_sub_dir = str(get_path('tagging','data_model'))
         if not os.path.isdir(self.resource_sub_dir):
             raise ValueError("Unable to access resources directory: " +
                              self.resource_sub_dir)
 
         _log.debug("Done init of base tagging service")
 
     @Core.receiver("onstart")
```

### Comparing `volttron_lib_tagging-0.1.1a0/src/tagging/base/parsetab.py` & `volttron_lib_tagging-0.1.1a1/src/tagging/base/parsetab.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_tagging-0.1.1a0/tests/tagging/testing/integration_test_interface.py` & `volttron_lib_tagging-0.1.1a1/tests/tagging/testing/integration_test_interface.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_tagging-0.1.1a0/tests/tagging/testing/test_base_tagging_unit.py` & `volttron_lib_tagging-0.1.1a1/tests/tagging/testing/test_base_tagging_unit.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_tagging-0.1.1a0/setup.py` & `volttron_lib_tagging-0.1.1a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
  'tagging': 'tests/tagging',
  'tagging.testing': 'tests/tagging/testing'}
 
 packages = \
 ['tagging', 'tagging.base', 'tagging.testing']
 
 package_data = \
-{'': ['*']}
+{'': ['*'], 'tagging': ['data_model/*']}
 
 install_requires = \
 ['ply>=3.11,<4.0', 'volttron>=10.0.3a9,<11.0']
 
 setup_kwargs = {
     'name': 'volttron-lib-tagging',
-    'version': '0.1.1a0',
+    'version': '0.1.1a1',
     'description': 'A base tagging agent api with extension points for using with the VOLTTRON platform. This base agent works with Haystack 3 tags',
     'long_description': "[![Eclipse VOLTTRON™](https://img.shields.io/badge/Eclips%20VOLTTRON--red.svg)](https://eclipse-volttron.readthedocs.io/en/latest/)\n![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)\n![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)\n[![Run Pytests](https://github.com/eclipse-volttron/volttron-lib-tagging/actions/workflows/run-tests.yml/badge.svg)](https://github.com/eclipse-volttron/volttron-lib-tagging/actions/workflows/run-tests.yml)\n[![pypi version](https://img.shields.io/pypi/v/volttron-lib-tagging.svg)](https://pypi.org/project/volttron-lib-tagging/)\n\nVOLTTRON base tagging library that provide common tagging api for users to associate haystack based tags and values to \ntopic names and topic name prefixes. Implementing agents can persist tags in specific data store. \n\nTags used by this library have to be pre-defined in a resource file at volttron_data/tagging_resources. The\nlibrary validates against this predefined list of tags every time user add tags to topics. Tags can be added to one \ntopic at a time or multiple topics by using a topic name pattern(regular expression). This library uses tags from \n[project haystack](https://project-haystack.org/) and adds a few custom tags for campus and VOLTTRON point name.\n\nEach tag has an associated value and users can query for topic names based tags and its values using a simplified \nsql-like query string. Queries can specify tag names with values or tags without values for boolean tags(markers). \nQueries can combine multiple conditions with keyword AND, and OR, and use the keyword NOT to negate a conditions.\n\n## Requirements\n\n - Python >= 3.10\n\n## Installation\n\nThis library can be installed using ```pip install volttron-lib-tagging```. However, this is not necessary. Any \nimplementing tagging agent that uses this library will automatically install it as part of its installation. \nFor example,  installing [SQLiteTaggingAgent](https://github.com/eclipse-volttron/volttron-sqlite-tagging) will \nautomatically install volttron-lib-tagging into the same python environment\n\n## Dependencies and Limitations\n\n1. When adding tags to topics this library calls the platform.historian's (or a configured historian's) \n   get_topic_list and hence requires a platform.historian or configured historian to be running, but it doesn't require \n   the historian to use sqlite3 or any specific database. It requires historian to be running only for using this \n   api (add_tags) and does not require historian to be running for any other api. \n2. Resource files that provides the list of valid tags is mandatory and should be in \n   data_model/tags.csv\n3. Tagging library only provides APIs to query for topic names based on tags. Once the list of topic names is retrieved, \n   users should use the historian APIs to get the data corresponding to those topics. \n4. Current version of tagging library does not support versioning of tag/values. When tags values are set it will \n   overwrite any existing tag entries in the database\n\n## Development\n\nPlease see the following for contributing guidelines [contributing](https://github.com/eclipse-volttron/volttron-core/blob/develop/CONTRIBUTING.md).\n\nPlease see the following helpful guide about [developing modular VOLTTRON agents](https://github.com/eclipse-volttron/volttron-core/blob/develop/DEVELOPING_ON_MODULAR.md)\n\n# Disclaimer Notice\n\nThis material was prepared as an account of work sponsored by an agency of the\nUnited States Government.  Neither the United States Government nor the United\nStates Department of Energy, nor Battelle, nor any of their employees, nor any\njurisdiction or organization that has cooperated in the development of these\nmaterials, makes any warranty, express or implied, or assumes any legal\nliability or responsibility for the accuracy, completeness, or usefulness or any\ninformation, apparatus, product, software, or process disclosed, or represents\nthat its use would not infringe privately owned rights.\n\nReference herein to any specific commercial product, process, or service by\ntrade name, trademark, manufacturer, or otherwise does not necessarily\nconstitute or imply its endorsement, recommendation, or favoring by the United\nStates Government or any agency thereof, or Battelle Memorial Institute. The\nviews and opinions of authors expressed herein do not necessarily state or\nreflect those of the United States Government or any agency thereof.\n",
     'author': 'VOLTTRON Team',
     'author_email': 'volttron@pnnl.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/eclipse-volttron/volttron-lib-tagging',
```

### Comparing `volttron_lib_tagging-0.1.1a0/PKG-INFO` & `volttron_lib_tagging-0.1.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-lib-tagging
-Version: 0.1.1a0
+Version: 0.1.1a1
 Summary: A base tagging agent api with extension points for using with the VOLTTRON platform. This base agent works with Haystack 3 tags
 Home-page: https://github.com/eclipse-volttron/volttron-lib-tagging
 License: Apache-2.0
 Author: VOLTTRON Team
 Author-email: volttron@pnnl.gov
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

