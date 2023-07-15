# Comparing `tmp/eudract-py-1.2.0.tar.gz` & `tmp/eudract-py-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/sopaulin/Projets/eudract-py/dist/tmpq7r_z3hc/eudract-py-1.2.0.tar", last modified: Sun Jul 10 22:18:24 2022, max compression
+gzip compressed data, was "eudract-py-1.3.0.tar", last modified: Sat Jul 15 20:15:27 2023, max compression
```

## Comparing `eudract-py-1.2.0.tar` & `eudract-py-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 sopaulin  (1000) sopaulin  (1000)        0 2022-07-10 22:18:24.000000 eudract-py-1.2.0/
--rw-r--r--   0 sopaulin  (1000) sopaulin  (1000)     1075 2022-06-01 21:27:25.000000 eudract-py-1.2.0/LICENSE
--rw-r--r--   0 sopaulin  (1000) sopaulin  (1000)       20 2022-06-01 21:27:25.000000 eudract-py-1.2.0/MANIFEST.in
--rw-r--r--   0 sopaulin  (1000) sopaulin  (1000)     2319 2022-07-10 22:18:24.000000 eudract-py-1.2.0/PKG-INFO
--rw-r--r--   0 sopaulin  (1000) sopaulin  (1000)     1543 2022-06-01 21:27:25.000000 eudract-py-1.2.0/README.md
-drwxr-xr-x   0 sopaulin  (1000) sopaulin  (1000)        0 2022-07-10 22:18:24.000000 eudract-py-1.2.0/eudract/
--rw-r--r--   0 sopaulin  (1000) sopaulin  (1000)       26 2022-06-01 22:09:44.000000 eudract-py-1.2.0/eudract/__init__.py
--rw-r--r--   0 sopaulin  (1000) sopaulin  (1000)     6360 2022-07-10 22:02:13.000000 eudract-py-1.2.0/eudract/main.py
--rw-r--r--   0 sopaulin  (1000) sopaulin  (1000)     1154 2022-07-10 22:02:13.000000 eudract-py-1.2.0/eudract/utils.py
-drwxr-xr-x   0 sopaulin  (1000) sopaulin  (1000)        0 2022-07-10 22:18:24.000000 eudract-py-1.2.0/eudract_py.egg-info/
--rw-r--r--   0 sopaulin  (1000) sopaulin  (1000)     2319 2022-07-10 22:18:24.000000 eudract-py-1.2.0/eudract_py.egg-info/PKG-INFO
--rw-r--r--   0 sopaulin  (1000) sopaulin  (1000)      293 2022-07-10 22:18:24.000000 eudract-py-1.2.0/eudract_py.egg-info/SOURCES.txt
--rw-r--r--   0 sopaulin  (1000) sopaulin  (1000)        1 2022-07-10 22:18:24.000000 eudract-py-1.2.0/eudract_py.egg-info/dependency_links.txt
--rw-r--r--   0 sopaulin  (1000) sopaulin  (1000)        1 2022-06-01 21:29:10.000000 eudract-py-1.2.0/eudract_py.egg-info/not-zip-safe
--rw-r--r--   0 sopaulin  (1000) sopaulin  (1000)       13 2022-07-10 22:18:24.000000 eudract-py-1.2.0/eudract_py.egg-info/requires.txt
--rw-r--r--   0 sopaulin  (1000) sopaulin  (1000)        8 2022-07-10 22:18:24.000000 eudract-py-1.2.0/eudract_py.egg-info/top_level.txt
--rw-r--r--   0 sopaulin  (1000) sopaulin  (1000)       38 2022-07-10 22:18:24.000000 eudract-py-1.2.0/setup.cfg
--rw-r--r--   0 sopaulin  (1000) sopaulin  (1000)     1174 2022-07-10 22:03:59.000000 eudract-py-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:15:27.049692 eudract-py-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-15 20:15:18.000000 eudract-py-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-15 20:15:18.000000 eudract-py-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-15 20:15:27.049692 eudract-py-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-15 20:15:18.000000 eudract-py-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:15:27.045692 eudract-py-1.3.0/eudract/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-15 20:15:18.000000 eudract-py-1.3.0/eudract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-07-15 20:15:18.000000 eudract-py-1.3.0/eudract/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-15 20:15:18.000000 eudract-py-1.3.0/eudract/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:15:27.049692 eudract-py-1.3.0/eudract_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-15 20:15:27.000000 eudract-py-1.3.0/eudract_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-15 20:15:27.000000 eudract-py-1.3.0/eudract_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 20:15:27.000000 eudract-py-1.3.0/eudract_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 20:15:26.000000 eudract-py-1.3.0/eudract_py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-15 20:15:27.000000 eudract-py-1.3.0/eudract_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 20:15:27.000000 eudract-py-1.3.0/eudract_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 20:15:27.049692 eudract-py-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-15 20:15:18.000000 eudract-py-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:15:27.049692 eudract-py-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-15 20:15:18.000000 eudract-py-1.3.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-15 20:15:18.000000 eudract-py-1.3.0/tests/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `eudract-py-1.2.0/LICENSE` & `eudract-py-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eudract-py-1.2.0/PKG-INFO` & `eudract-py-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: eudract-py
-Version: 1.2.0
+Version: 1.3.0
 Summary: Eudract-py is a Python library for searching clinical trials on EUDRACT
 Home-page: http://github.com/PaulinCharliquart/eudract-py
 Author: Paulin Charliquart
 Author-email: paulincharliquart@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/PaulinCharliquart/eudract-py/issues
-Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Healthcare Industry
-Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
+Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/eudract-py.svg)](https://badge.fury.io/py/eudract-py)
 [![GitHub license](https://img.shields.io/github/license/PaulinCharliquart/eudract-py)](https://github.com/PaulinCharliquart/eudract-py/blob/main/LICENSE)
 
 # eudract-py
```

### Comparing `eudract-py-1.2.0/README.md` & `eudract-py-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `eudract-py-1.2.0/eudract/main.py` & `eudract-py-1.3.0/eudract/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,22 @@
 """
 
 import requests
 import re
 from urllib.parse import urljoin
 from bs4 import BeautifulSoup
 import json
-from eudract.utils import read_cache, write_cache, create_connection, create_table
+from warnings import warn
+from eudract.utils import (
+    read_cache,
+    write_cache,
+    create_connection,
+    create_table,
+    validate_id,
+)
 
 
 class Eudract:
     """Main class"""
 
     def __init__(self):
         self._BASE_URL = "https://www.clinicaltrialsregister.eu/"
@@ -42,15 +49,15 @@
                 "F. POPULATION OF TRIAL SUBJECTS",
                 "G. INVESTIGATOR NETWORKS TO BE INVOLVED IN THE TRIAL",
                 "N. REVIEW BY THE COMPETENT AUTHORITY OR ETHICS COMMITTEE IN THE COUNTRY CONCERNED",
                 "P. END OF TRIAL",
             ],
         }
 
-    def json_handler(self, doc, level):
+    def json_handler(self, doc, level: str):
         data = dict.fromkeys(self._SCHEMA[level], "")
         if level == "summary":
             for k in data.keys():
                 val = re.findall("(?<={}:)(.+)".format(k), doc)
                 if val:
                     data[k] = val[0].strip()
 
@@ -68,15 +75,17 @@
                     key: res[key]
                     for key in res.keys()
                     if bool(re.search("^{}[.]".format(k[0]), key))
                 }
 
         return data
 
-    def search(self, query, level="summary", to_dict=False, size=None, cache_file=None):
+    def search(
+        self, query: str, level="summary", to_dict=False, size=None, cache_file=None
+    ):
         """
         Search studies in Eudract
 
         Args:
             query (str): text to search
             level (str): type of info to extract (either summary or full)
             to_dict (Bool): Return the results as dict
@@ -84,44 +93,57 @@
             cache_file (str): Set cache filename to save results to sqlite db
 
         Returns:
             [list]: List of dictionary
         """
         next_page = ["&page=1"]
         ids = []
+        if to_dict is False:
+            warn(
+                "to_dict will be removed in the next version. Results will be returned only as dict.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
         while next_page:
             page_id = re.findall(r"\d+", next_page[0])
             r = requests.get(
                 self._SEARCH, params={"query": query, "page": page_id[0]}, verify=False
             )
             r.raise_for_status
             next_page = re.findall(
                 r"(?<=href=\").*?(?=\"\saccesskey=\"n\">\s*Next)", r.text
             )
             ids += list(set(re.findall(r"20\d{2}-\d{6}-\d{2}", r.text)))
-            if size is not None:
-                if len(ids) >= size:
-                    ids = ids[:size]
-                    break
+            if size is not None and len(ids) >= size:
+                ids = ids[:size]
+                break
         data = [self.info(el, level, to_dict, cache_file) for el in ids]
         return data
 
-    def info(self, eudract, level="summary", to_dict=False, cache_file=None):
+    def info(self, eudract: str, level="summary", to_dict=False, cache_file=None):
         """
         Get info for a study
 
         Args:
             eudract (str): Eudract ID
             level (str): type of info to extract (either summary or full)
             to_dict (Bool): Return the results as dict
             cache_file (str): Set cache filename to save results to sqlite db
 
         Returns:
             [dict]: dictionary
         """
+        if to_dict is False:
+            warn(
+                "to_dict will be removed in the next version. Results will be returned only as dict.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+        if validate_id(eudract_id=eudract) is False:
+            return None
         if cache_file:
             db = create_connection(cache_file)
             key_id = "_".join([eudract, level, str(to_dict)]).lower()
 
             if create_table(db):
                 content = read_cache(db, key_id)
                 if content:
@@ -129,26 +151,30 @@
                     return data
         if level == "summary":
             r = requests.get(
                 urljoin(self._DOWNLOAD, level),
                 params={"mode": "selected", "eudracts": eudract},
                 verify=False,
             )
+            if r.text == "":
+                return None
             if to_dict:
                 data = self.json_handler(r.text, level)
             else:
                 data = r.text
 
         if level == "full":
             if to_dict:
                 r = requests.get(self._SEARCH, params={"query": eudract}, verify=False)
                 full_url = re.findall(
                     r"ctr-search/trial/{}/[A-Z][A-Z]".format(eudract), r.text
                 )
                 r.raise_for_status
+                if len(full_url) == 0:
+                    return None
                 r_full = requests.get(
                     urljoin(self._BASE_URL, full_url[0]), verify=False
                 )
                 r.raise_for_status
                 data = self.json_handler(r_full.text, level)
             else:
                 r = requests.get(
@@ -172,10 +198,16 @@
             level (str): type of info to extract (either summary or full)
             to_dict (Bool): Return the results as dict
             cache_file (str): Set cache filename to save results to sqlite db
 
         Returns:
             [dict]: dictionary
         """
+        if to_dict is False:
+            warn(
+                "to_dict will be removed in the next version. Results will be returned only as dict.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
         return self.search(
             query="", level=level, to_dict=to_dict, cache_file=cache_file
         )
```

### Comparing `eudract-py-1.2.0/eudract/utils.py` & `eudract-py-1.3.0/eudract/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import sqlite3
+import re
+from datetime import datetime
 
 
-def create_connection(db_file):
+def create_connection(db_file: str):
     conn = None
     try:
         conn = sqlite3.connect(db_file)
         return conn
     except sqlite3.Error as e:
         print(e)
     return conn
@@ -48,7 +50,24 @@
         cur.execute(""" SELECT data from results where id = ? """, (key,))
         rows = cur.fetchone()
         res = rows[0] if rows else None
     except sqlite3.Error as e:
         print(e)
         res = None
     return res
+
+
+def validate_id(eudract_id: str):
+    """
+    Validate Eudract Id
+    """
+    test_id = re.match("^20\d{2}-\d{6}-\d{2}$", eudract_id)
+    if test_id is None:
+        return False
+    today_year = datetime.now().year
+    try:
+        eudract_year = int(eudract_id[0:4])
+    except ValueError:
+        eudract_year = 0
+    if eudract_year not in range(2000, today_year):
+        return False
+    return True
```

### Comparing `eudract-py-1.2.0/eudract_py.egg-info/PKG-INFO` & `eudract-py-1.3.0/eudract_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: eudract-py
-Version: 1.2.0
+Version: 1.3.0
 Summary: Eudract-py is a Python library for searching clinical trials on EUDRACT
 Home-page: http://github.com/PaulinCharliquart/eudract-py
 Author: Paulin Charliquart
 Author-email: paulincharliquart@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/PaulinCharliquart/eudract-py/issues
-Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Healthcare Industry
-Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
+Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 [![PyPI version](https://badge.fury.io/py/eudract-py.svg)](https://badge.fury.io/py/eudract-py)
 [![GitHub license](https://img.shields.io/github/license/PaulinCharliquart/eudract-py)](https://github.com/PaulinCharliquart/eudract-py/blob/main/LICENSE)
 
 # eudract-py
```

