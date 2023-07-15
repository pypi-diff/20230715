# Comparing `tmp/bluegenes-0.0.1.tar.gz` & `tmp/bluegenes-0.0.2.tar.gz`

## Comparing `bluegenes-0.0.1.tar` & `bluegenes-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    15553 2020-02-02 00:00:00.000000 bluegenes-0.0.1/dox.md
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bluegenes-0.0.1/bluegenes/__init__.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 bluegenes-0.0.1/bluegenes/errors.py
--rw-r--r--   0        0        0    34993 2020-02-02 00:00:00.000000 bluegenes-0.0.1/bluegenes/genes.py
--rw-r--r--   0        0        0    11188 2020-02-02 00:00:00.000000 bluegenes-0.0.1/bluegenes/optimization.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 bluegenes-0.0.1/tests/context.py
--rw-r--r--   0        0        0    42027 2020-02-02 00:00:00.000000 bluegenes-0.0.1/tests/test_genes.py
--rw-r--r--   0        0        0    17954 2020-02-02 00:00:00.000000 bluegenes-0.0.1/tests/test_optimization.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 bluegenes-0.0.1/.gitignore
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 bluegenes-0.0.1/license
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 bluegenes-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 bluegenes-0.0.1/readme.md
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 bluegenes-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    15553 2020-02-02 00:00:00.000000 bluegenes-0.0.2/dox.md
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 bluegenes-0.0.2/bluegenes/__init__.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 bluegenes-0.0.2/bluegenes/errors.py
+-rw-r--r--   0        0        0    34993 2020-02-02 00:00:00.000000 bluegenes-0.0.2/bluegenes/genes.py
+-rw-r--r--   0        0        0    11188 2020-02-02 00:00:00.000000 bluegenes-0.0.2/bluegenes/optimization.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 bluegenes-0.0.2/tests/context.py
+-rw-r--r--   0        0        0    42027 2020-02-02 00:00:00.000000 bluegenes-0.0.2/tests/test_genes.py
+-rw-r--r--   0        0        0    17954 2020-02-02 00:00:00.000000 bluegenes-0.0.2/tests/test_optimization.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 bluegenes-0.0.2/.gitignore
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 bluegenes-0.0.2/license
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 bluegenes-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 bluegenes-0.0.2/readme.md
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 bluegenes-0.0.2/PKG-INFO
```

### Comparing `bluegenes-0.0.1/dox.md` & `bluegenes-0.0.2/dox.md`

 * *Files identical despite different names*

### Comparing `bluegenes-0.0.1/bluegenes/errors.py` & `bluegenes-0.0.2/bluegenes/errors.py`

 * *Files identical despite different names*

### Comparing `bluegenes-0.0.1/bluegenes/genes.py` & `bluegenes-0.0.2/bluegenes/genes.py`

 * *Files identical despite different names*

### Comparing `bluegenes-0.0.1/bluegenes/optimization.py` & `bluegenes-0.0.2/bluegenes/optimization.py`

 * *Files identical despite different names*

### Comparing `bluegenes-0.0.1/tests/test_genes.py` & `bluegenes-0.0.2/tests/test_genes.py`

 * *Files identical despite different names*

### Comparing `bluegenes-0.0.1/tests/test_optimization.py` & `bluegenes-0.0.2/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `bluegenes-0.0.1/license` & `bluegenes-0.0.2/license`

 * *Files identical despite different names*

### Comparing `bluegenes-0.0.1/pyproject.toml` & `bluegenes-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bluegenes"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="k98kurz", email="k98kurz@gmail.com" },
 ]
 description = "Working-man's library for genetic algorithms"
 readme = "readme.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -18,9 +18,9 @@
   "Operating System :: OS Independent",
   "Intended Audience :: Science/Research",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
   "Topic :: Scientific/Engineering :: Artificial Life",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/k98kurz/bluegenes"
-"Bug Tracker" = "https://github.com/k98kurz/bluegenes/issues"
+"Homepage" = "https://github.com/k98kurz/bluegenes-python"
+"Bug Tracker" = "https://github.com/k98kurz/bluegenes-python/issues"
```

### Comparing `bluegenes-0.0.1/readme.md` & `bluegenes-0.0.2/readme.md`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 - `optimize_chromosome` - optimizes a Chromosome
 - `optimize_genome` - optimizes a Genome
 
 These optimization functions have largely similar parameters for tuning the
 optimization process. See the [Usage](#Usage) section below.
 
 For more detailed documentation, see the
-[docs file](https://github.com/k98kurz/bluegenes/blob/master/dox.md)
+[docs file](https://github.com/k98kurz/bluegenes-python/blob/master/dox.md)
 generated automagically by [autodox](https://pypi.org/project/autodox).
 
 ## Installation
 
 Installation is with pip.
 
 ```bash
```

### Comparing `bluegenes-0.0.1/PKG-INFO` & `bluegenes-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: bluegenes
-Version: 0.0.1
+Version: 0.0.2
 Summary: Working-man's library for genetic algorithms
-Project-URL: Homepage, https://github.com/k98kurz/bluegenes
-Project-URL: Bug Tracker, https://github.com/k98kurz/bluegenes/issues
+Project-URL: Homepage, https://github.com/k98kurz/bluegenes-python
+Project-URL: Bug Tracker, https://github.com/k98kurz/bluegenes-python/issues
 Author-email: k98kurz <k98kurz@gmail.com>
 License-File: license
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -51,15 +51,15 @@
 - `optimize_chromosome` - optimizes a Chromosome
 - `optimize_genome` - optimizes a Genome
 
 These optimization functions have largely similar parameters for tuning the
 optimization process. See the [Usage](#Usage) section below.
 
 For more detailed documentation, see the
-[docs file](https://github.com/k98kurz/bluegenes/blob/master/dox.md)
+[docs file](https://github.com/k98kurz/bluegenes-python/blob/master/dox.md)
 generated automagically by [autodox](https://pypi.org/project/autodox).
 
 ## Installation
 
 Installation is with pip.
 
 ```bash
```

