# Comparing `tmp/pypura-0.1.6.tar.gz` & `tmp/pypura-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypura-0.1.6.tar", max compression
+gzip compressed data, was "pypura-0.1.7.tar", max compression
```

## Comparing `pypura-0.1.6.tar` & `pypura-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-07-03 16:25:32.832779 pypura-0.1.6/LICENSE
--rw-r--r--   0        0        0       76 2023-07-03 16:25:32.832779 pypura-0.1.6/README.md
--rw-r--r--   0        0        0      754 2023-07-03 16:25:56.572957 pypura-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      251 2023-07-03 16:25:56.576957 pypura-0.1.6/pypura/__init__.py
--rw-r--r--   0        0        0      414 2023-07-03 16:25:32.836779 pypura-0.1.6/pypura/const.py
--rw-r--r--   0        0        0      200 2023-07-03 16:25:32.836779 pypura-0.1.6/pypura/exceptions.py
--rw-r--r--   0        0        0    32132 2023-07-03 16:25:32.836779 pypura-0.1.6/pypura/fragrances.json
--rw-r--r--   0        0        0     6705 2023-07-03 16:25:32.836779 pypura-0.1.6/pypura/pura.py
--rw-r--r--   0        0        0        0 2023-07-03 16:25:32.836779 pypura-0.1.6/pypura/py.typed
--rw-r--r--   0        0        0      803 2023-07-03 16:25:32.836779 pypura-0.1.6/pypura/utils.py
--rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 pypura-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-15 18:44:35.092850 pypura-0.1.7/LICENSE
+-rw-r--r--   0        0        0       76 2023-07-15 18:44:35.092850 pypura-0.1.7/README.md
+-rw-r--r--   0        0        0      761 2023-07-15 18:44:55.021085 pypura-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      251 2023-07-15 18:44:55.025085 pypura-0.1.7/pypura/__init__.py
+-rw-r--r--   0        0        0      414 2023-07-15 18:44:35.096850 pypura-0.1.7/pypura/const.py
+-rw-r--r--   0        0        0      200 2023-07-15 18:44:35.096850 pypura-0.1.7/pypura/exceptions.py
+-rw-r--r--   0        0        0    32768 2023-07-15 18:44:35.096850 pypura-0.1.7/pypura/fragrances.json
+-rw-r--r--   0        0        0     6705 2023-07-15 18:44:35.096850 pypura-0.1.7/pypura/pura.py
+-rw-r--r--   0        0        0        0 2023-07-15 18:44:35.096850 pypura-0.1.7/pypura/py.typed
+-rw-r--r--   0        0        0      803 2023-07-15 18:44:35.096850 pypura-0.1.7/pypura/utils.py
+-rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 pypura-0.1.7/PKG-INFO
```

### Comparing `pypura-0.1.6/LICENSE` & `pypura-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pypura-0.1.6/pyproject.toml` & `pypura-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypura"
-version = "0.1.6"
+version = "0.1.7"
 description = "Python package for interacting with Pura smart fragrance diffuser"
 authors = ["Nathan Spencer <natekspencer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 include = ["pypura/py.typed"]
 
 [tool.poetry.dependencies]
@@ -25,9 +25,9 @@
 
 [tool.poetry-dynamic-versioning]
 enable = true
 vcs = "git"
 style = "semver"
 
 [build-system]
-requires = ["poetry-core", "poetry-dynamic-versioning"]
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `pypura-0.1.6/pypura/fragrances.json` & `pypura-0.1.7/pypura/fragrances.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9804560260586319%*

 * *Differences: {'insert': "[(0, OrderedDict([('name', 'Chamomile Lavender'), ('type', 'Car Fragrance'), ('sku', "*

 * *           "'AJWC'), ('brand', 'LAFCO')])), (3, OrderedDict([('name', 'Del Mar'), ('type', 'Car "*

 * *           "Fragrance'), ('sku', 'DEMC'), ('brand', 'GUY FOX')])), (11, OrderedDict([('name', 'Sea "*

 * *           "& Dune'), ('type', 'Car Fragrance'), ('sku', 'SDNC'), ('brand', 'LAFCO')])), (12, "*

 * *           "OrderedDict([('name', 'SoHo'), ('type', 'Car Fragrance'), ('sku', 'SOHC'), ('brand', "*

 * *           "'GUY FO […]*

```diff
@@ -1,21 +1,33 @@
 [
     {
+        "brand": "LAFCO",
+        "name": "Chamomile Lavender",
+        "sku": "AJWC",
+        "type": "Car Fragrance"
+    },
+    {
         "brand": "Pura",
         "name": "Coastal Palm",
         "sku": "CJIC",
         "type": "Car Fragrance"
     },
     {
         "brand": "Pura",
         "name": "Cucumber & Mint",
         "sku": "CBMC",
         "type": "Car Fragrance"
     },
     {
+        "brand": "GUY FOX",
+        "name": "Del Mar",
+        "sku": "DEMC",
+        "type": "Car Fragrance"
+    },
+    {
         "brand": "Unify Co.",
         "name": "Dew",
         "sku": "DEWC",
         "type": "Car Fragrance"
     },
     {
         "brand": "Pura",
@@ -50,14 +62,26 @@
     {
         "brand": "Unify Co.",
         "name": "Salt",
         "sku": "SLTC",
         "type": "Car Fragrance"
     },
     {
+        "brand": "LAFCO",
+        "name": "Sea & Dune",
+        "sku": "SDNC",
+        "type": "Car Fragrance"
+    },
+    {
+        "brand": "GUY FOX",
+        "name": "SoHo",
+        "sku": "SOHC",
+        "type": "Car Fragrance"
+    },
+    {
         "brand": "Bridgewater Candle Company",
         "name": "Sweet Grace",
         "sku": "LWZC",
         "type": "Car Fragrance"
     },
     {
         "brand": "Pura",
@@ -1082,14 +1106,20 @@
     {
         "brand": "Caswell-Massey",
         "name": "Old Faithful",
         "sku": "OLF",
         "type": "Fragrance"
     },
     {
+        "brand": "Apotheke",
+        "name": "Orange Blossom Neroli",
+        "sku": "OBN",
+        "type": "Fragrance"
+    },
+    {
         "brand": "Antica Farmacista",
         "name": "Orange Blossom, Lilac & Jasmine",
         "sku": "DZI",
         "type": "Fragrance"
     },
     {
         "brand": "Caswell-Massey",
@@ -1232,14 +1262,20 @@
     {
         "brand": "Capri Blue",
         "name": "Pumpkin Dulce",
         "sku": "VCW",
         "type": "Fragrance"
     },
     {
+        "brand": "Thymes",
+        "name": "Pumpkin Laurel",
+        "sku": "PKL",
+        "type": "Fragrance"
+    },
+    {
         "brand": "Votivo",
         "name": "RED CURRANT",
         "sku": "FZE",
         "type": "Fragrance"
     },
     {
         "brand": "Ellis Brooklyn",
```

### Comparing `pypura-0.1.6/pypura/pura.py` & `pypura-0.1.7/pypura/pura.py`

 * *Files identical despite different names*

### Comparing `pypura-0.1.6/pypura/utils.py` & `pypura-0.1.7/pypura/utils.py`

 * *Files identical despite different names*

### Comparing `pypura-0.1.6/PKG-INFO` & `pypura-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypura
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package for interacting with Pura smart fragrance diffuser
 License: MIT
 Author: Nathan Spencer
 Author-email: natekspencer@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

