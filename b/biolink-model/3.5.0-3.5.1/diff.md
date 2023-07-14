# Comparing `tmp/biolink-model-3.5.0.tar.gz` & `tmp/biolink-model-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biolink-model-3.5.0.tar", last modified: Fri Jul  7 19:06:29 2023, max compression
+gzip compressed data, was "biolink-model-3.5.1.tar", last modified: Fri Jul 14 23:53:33 2023, max compression
```

## Comparing `biolink-model-3.5.0.tar` & `biolink-model-3.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 SMoxon     (502) staff       (20)        0 2023-07-07 19:06:29.731304 biolink-model-3.5.0/
--rw-r--r--   0 SMoxon     (502) staff       (20)      762 2022-11-30 01:03:34.000000 biolink-model-3.5.0/AUTHORS
--rw-r--r--   0 SMoxon     (502) staff       (20)      523 2022-11-03 00:23:30.000000 biolink-model-3.5.0/LICENSE
--rw-r--r--   0 SMoxon     (502) staff       (20)     7187 2023-07-07 19:06:29.731443 biolink-model-3.5.0/PKG-INFO
--rw-r--r--   0 SMoxon     (502) staff       (20)     6330 2023-05-16 23:18:34.000000 biolink-model-3.5.0/README.md
-drwxr-xr-x   0 SMoxon     (502) staff       (20)        0 2023-07-07 19:06:29.726397 biolink-model-3.5.0/biolink/
--rw-r--r--   0 SMoxon     (502) staff       (20)      721 2022-11-03 00:23:30.000000 biolink-model-3.5.0/biolink/__init__.py
--rw-r--r--   0 SMoxon     (502) staff       (20)   654646 2023-07-07 19:04:58.000000 biolink-model-3.5.0/biolink/model.py
--rw-r--r--   0 SMoxon     (502) staff       (20)  1252606 2023-07-07 19:04:58.000000 biolink-model-3.5.0/biolink/pydanticmodel.py
-drwxr-xr-x   0 SMoxon     (502) staff       (20)        0 2023-07-07 19:06:29.729832 biolink-model-3.5.0/biolink_model.egg-info/
--rw-r--r--   0 SMoxon     (502) staff       (20)     7187 2023-07-07 19:06:29.000000 biolink-model-3.5.0/biolink_model.egg-info/PKG-INFO
--rw-r--r--   0 SMoxon     (502) staff       (20)      357 2023-07-07 19:06:29.000000 biolink-model-3.5.0/biolink_model.egg-info/SOURCES.txt
--rw-r--r--   0 SMoxon     (502) staff       (20)        1 2023-07-07 19:06:29.000000 biolink-model-3.5.0/biolink_model.egg-info/dependency_links.txt
--rw-r--r--   0 SMoxon     (502) staff       (20)       25 2023-07-07 19:06:29.000000 biolink-model-3.5.0/biolink_model.egg-info/requires.txt
--rw-r--r--   0 SMoxon     (502) staff       (20)        8 2023-07-07 19:06:29.000000 biolink-model-3.5.0/biolink_model.egg-info/top_level.txt
--rw-r--r--   0 SMoxon     (502) staff       (20)     1016 2023-06-30 21:13:29.000000 biolink-model-3.5.0/pyproject.toml
--rw-r--r--   0 SMoxon     (502) staff       (20)      841 2023-07-07 19:06:29.732041 biolink-model-3.5.0/setup.cfg
--rw-r--r--   0 SMoxon     (502) staff       (20)     1366 2023-06-30 21:23:16.000000 biolink-model-3.5.0/setup.py
-drwxr-xr-x   0 SMoxon     (502) staff       (20)        0 2023-07-07 19:06:29.730868 biolink-model-3.5.0/tests/
--rw-r--r--   0 SMoxon     (502) staff       (20)      617 2022-11-03 00:23:30.000000 biolink-model-3.5.0/tests/test_biolink_model.py
--rw-r--r--   0 SMoxon     (502) staff       (20)      720 2022-11-03 00:23:30.000000 biolink-model-3.5.0/tests/test_pythongen.py
+drwxr-xr-x   0 SMoxon     (502) staff       (20)        0 2023-07-14 23:53:33.574882 biolink-model-3.5.1/
+-rw-r--r--   0 SMoxon     (502) staff       (20)      762 2022-11-30 01:03:34.000000 biolink-model-3.5.1/AUTHORS
+-rw-r--r--   0 SMoxon     (502) staff       (20)      523 2022-11-03 00:23:30.000000 biolink-model-3.5.1/LICENSE
+-rw-r--r--   0 SMoxon     (502) staff       (20)     7187 2023-07-14 23:53:33.575073 biolink-model-3.5.1/PKG-INFO
+-rw-r--r--   0 SMoxon     (502) staff       (20)     6330 2023-05-16 23:18:34.000000 biolink-model-3.5.1/README.md
+drwxr-xr-x   0 SMoxon     (502) staff       (20)        0 2023-07-14 23:53:33.570363 biolink-model-3.5.1/biolink/
+-rw-r--r--   0 SMoxon     (502) staff       (20)      721 2022-11-03 00:23:30.000000 biolink-model-3.5.1/biolink/__init__.py
+-rw-r--r--   0 SMoxon     (502) staff       (20)   654646 2023-07-14 23:49:45.000000 biolink-model-3.5.1/biolink/model.py
+-rw-r--r--   0 SMoxon     (502) staff       (20)  1252606 2023-07-14 23:52:16.000000 biolink-model-3.5.1/biolink/pydanticmodel.py
+drwxr-xr-x   0 SMoxon     (502) staff       (20)        0 2023-07-14 23:53:33.573622 biolink-model-3.5.1/biolink_model.egg-info/
+-rw-r--r--   0 SMoxon     (502) staff       (20)     7187 2023-07-14 23:53:33.000000 biolink-model-3.5.1/biolink_model.egg-info/PKG-INFO
+-rw-r--r--   0 SMoxon     (502) staff       (20)      357 2023-07-14 23:53:33.000000 biolink-model-3.5.1/biolink_model.egg-info/SOURCES.txt
+-rw-r--r--   0 SMoxon     (502) staff       (20)        1 2023-07-14 23:53:33.000000 biolink-model-3.5.1/biolink_model.egg-info/dependency_links.txt
+-rw-r--r--   0 SMoxon     (502) staff       (20)       25 2023-07-14 23:53:33.000000 biolink-model-3.5.1/biolink_model.egg-info/requires.txt
+-rw-r--r--   0 SMoxon     (502) staff       (20)        8 2023-07-14 23:53:33.000000 biolink-model-3.5.1/biolink_model.egg-info/top_level.txt
+-rw-r--r--   0 SMoxon     (502) staff       (20)     1034 2023-07-14 23:49:45.000000 biolink-model-3.5.1/pyproject.toml
+-rw-r--r--   0 SMoxon     (502) staff       (20)      841 2023-07-14 23:53:33.576112 biolink-model-3.5.1/setup.cfg
+-rw-r--r--   0 SMoxon     (502) staff       (20)     1366 2023-07-14 23:51:04.000000 biolink-model-3.5.1/setup.py
+drwxr-xr-x   0 SMoxon     (502) staff       (20)        0 2023-07-14 23:53:33.574491 biolink-model-3.5.1/tests/
+-rw-r--r--   0 SMoxon     (502) staff       (20)      617 2022-11-03 00:23:30.000000 biolink-model-3.5.1/tests/test_biolink_model.py
+-rw-r--r--   0 SMoxon     (502) staff       (20)      720 2022-11-03 00:23:30.000000 biolink-model-3.5.1/tests/test_pythongen.py
```

### Comparing `biolink-model-3.5.0/AUTHORS` & `biolink-model-3.5.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `biolink-model-3.5.0/LICENSE` & `biolink-model-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biolink-model-3.5.0/PKG-INFO` & `biolink-model-3.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biolink-model
-Version: 3.5.0
+Version: 3.5.1
 Summary: 'A high level datamodel of biological entities and associations'
 Home-page: https://github.com/biolink/biolink-model
 Author: ('Deepak Unni', 'Sierra Moxon')
 Author-email: smoxon@lbl.gov
 License: BSD
 Keywords: NCATS NCATS-Translator Biolink-Model Biolink LinkML Datamodel
 Platform: UNKNOWN
```

### Comparing `biolink-model-3.5.0/README.md` & `biolink-model-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `biolink-model-3.5.0/biolink/__init__.py` & `biolink-model-3.5.1/biolink/__init__.py`

 * *Files identical despite different names*

### Comparing `biolink-model-3.5.0/biolink/model.py` & `biolink-model-3.5.1/biolink/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 2320 4175 746f 2067 656e 6572 6174 6564  # Auto generated
 00000010: 2066 726f 6d20 6269 6f6c 696e 6b2d 6d6f   from biolink-mo
 00000020: 6465 6c2e 7961 6d6c 2062 7920 7079 7468  del.yaml by pyth
 00000030: 6f6e 6765 6e2e 7079 2076 6572 7369 6f6e  ongen.py version
 00000040: 3a20 302e 392e 300a 2320 4765 6e65 7261  : 0.9.0.# Genera
 00000050: 7469 6f6e 2064 6174 653a 2032 3032 332d  tion date: 2023-
-00000060: 3036 2d33 3054 3231 3a31 333a 3531 0a23  06-30T21:13:51.#
+00000060: 3037 2d31 3454 3233 3a30 313a 3533 0a23  07-14T23:01:53.#
 00000070: 2053 6368 656d 613a 2042 696f 6c69 6e6b   Schema: Biolink
 00000080: 2d4d 6f64 656c 0a23 0a23 2069 643a 2068  -Model.#.# id: h
 00000090: 7474 7073 3a2f 2f77 3369 642e 6f72 672f  ttps://w3id.org/
 000000a0: 6269 6f6c 696e 6b2f 6269 6f6c 696e 6b2d  biolink/biolink-
 000000b0: 6d6f 6465 6c0a 2320 6465 7363 7269 7074  model.# descript
 000000c0: 696f 6e3a 2045 6e74 6974 7920 616e 6420  ion: Entity and 
 000000d0: 6173 736f 6369 6174 696f 6e20 7461 786f  association taxo
@@ -79,15 +79,15 @@
 000004e0: 206c 696e 6b6d 6c5f 7275 6e74 696d 652e   linkml_runtime.
 000004f0: 7574 696c 732e 6d65 7461 6d6f 6465 6c63  utils.metamodelc
 00000500: 6f72 6520 696d 706f 7274 2042 6f6f 6c2c  ore import Bool,
 00000510: 2055 5249 6f72 4355 5249 452c 2058 5344   URIorCURIE, XSD
 00000520: 4461 7465 2c20 5853 4454 696d 650a 0a6d  Date, XSDTime..m
 00000530: 6574 616d 6f64 656c 5f76 6572 7369 6f6e  etamodel_version
 00000540: 203d 2022 312e 372e 3022 0a76 6572 7369   = "1.7.0".versi
-00000550: 6f6e 203d 2022 332e 342e 3322 0a0a 2320  on = "3.4.3"..# 
+00000550: 6f6e 203d 2022 332e 352e 3022 0a0a 2320  on = "3.5.0"..# 
 00000560: 4f76 6572 7772 6974 6520 6461 7461 636c  Overwrite datacl
 00000570: 6173 7365 7320 5f69 6e69 745f 666e 2074  asses _init_fn t
 00000580: 6f20 6164 6420 2a2a 6b77 6172 6773 2069  o add **kwargs i
 00000590: 6e20 5f5f 696e 6974 5f5f 0a64 6174 6163  n __init__.datac
 000005a0: 6c61 7373 6573 2e5f 696e 6974 5f66 6e20  lasses._init_fn 
 000005b0: 3d20 6461 7461 636c 6173 7365 735f 696e  = dataclasses_in
 000005c0: 6974 5f66 6e5f 7769 7468 5f6b 7761 7267  it_fn_with_kwarg
```

### Comparing `biolink-model-3.5.0/biolink/pydanticmodel.py` & `biolink-model-3.5.1/biolink/pydanticmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 metamodel_version = "None"
-version = "3.4.3"
+version = "3.5.1"
 
 class WeakRefShimBaseModel(BaseModel):
    __slots__ = '__weakref__'
 
 class ConfiguredBaseModel(WeakRefShimBaseModel,
                 validate_assignment = True,
                 validate_all = True,
```

### Comparing `biolink-model-3.5.0/biolink_model.egg-info/PKG-INFO` & `biolink-model-3.5.1/biolink_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biolink-model
-Version: 3.5.0
+Version: 3.5.1
 Summary: 'A high level datamodel of biological entities and associations'
 Home-page: https://github.com/biolink/biolink-model
 Author: ('Deepak Unni', 'Sierra Moxon')
 Author-email: smoxon@lbl.gov
 License: BSD
 Keywords: NCATS NCATS-Translator Biolink-Model Biolink LinkML Datamodel
 Platform: UNKNOWN
```

### Comparing `biolink-model-3.5.0/pyproject.toml` & `biolink-model-3.5.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -27,9 +27,9 @@
 yamllint = "^1.30.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.codespell]
-skip = '.idea,.venv,.git,*.pdf,*.svg,context.*,prefix-map,biolink,docs,json-schema,graphql,biolink-model.g*,biolink-model.t*,biolink-model.s*,biolink-model.o*,biolink-model.p*,'
+skip = 'SEMMEDDB*,semmed*,.idea,.venv,.git,*.pdf,*.svg,context.*,prefix-map,biolink,docs,json-schema,graphql,biolink-model.g*,biolink-model.t*,biolink-model.s*,biolink-model.o*,biolink-model.p*,'
 ignore-words-list = 'amination,ehr,mor,brite,nin,mirgate'
```

### Comparing `biolink-model-3.5.0/setup.cfg` & `biolink-model-3.5.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = biolink_model
 description = 'A high level datamodel of biological entities and associations'
-version = 3.5.0
+version = 3.5.1
 url = https://github.com/biolink/biolink-model
 author = Harold Solbrig
 author-email = smoxon@lbl.gov
 summary = Biolink Model
 home-page = https://biolink.github.io/biolink-model/docs/
 license = CC0 1.0 Universal
 python-requires = >=3.9
```

### Comparing `biolink-model-3.5.0/setup.py` & `biolink-model-3.5.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 with open("requirements.txt", "r") as FH:
     REQUIREMENTS = FH.readlines()
 
 NAME = 'biolink-model'
-VERSION = '3.5.0'
+VERSION = '3.5.1'
 
 DESCRIPTION = 'Biolink Model: A high level datamodel of biological entities and associations'
 URL = 'https://github.com/biolink/biolink-model'
 AUTHOR = 'Deepak Unni', 'Sierra Moxon'
 EMAIL = 'smoxon@lbl.gov'
 REQUIRES_PYTHON = '>=3.9'
 LICENSE = 'BSD'
```

### Comparing `biolink-model-3.5.0/tests/test_biolink_model.py` & `biolink-model-3.5.1/tests/test_biolink_model.py`

 * *Files identical despite different names*

### Comparing `biolink-model-3.5.0/tests/test_pythongen.py` & `biolink-model-3.5.1/tests/test_pythongen.py`

 * *Files identical despite different names*

