# Comparing `tmp/ccinput-1.9.0.tar.gz` & `tmp/ccinput-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccinput-1.9.0.tar", last modified: Wed Jun  7 00:55:14 2023, max compression
+gzip compressed data, was "ccinput-1.9.1.tar", last modified: Mon Jun 12 15:42:55 2023, max compression
```

## Comparing `ccinput-1.9.0.tar` & `ccinput-1.9.1.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:55:14.417142 ccinput-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-07 00:54:18.000000 ccinput-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-07 00:54:18.000000 ccinput-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-07 00:55:14.417142 ccinput-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-07 00:54:18.000000 ccinput-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:55:14.421142 ccinput-1.9.0/ccinput/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-07 00:55:14.421142 ccinput-1.9.0/ccinput/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)    90291 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/documentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:55:14.417142 ccinput-1.9.0/ccinput/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/drivers/pysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:55:14.417142 ccinput-1.9.0/ccinput/packages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/packages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/packages/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/packages/nwchem.py
--rw-r--r--   0 runner    (1001) docker     (123)    15963 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/packages/orca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/packages/psi4.py
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/packages/qchem.py
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/packages/xtb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/presets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:55:14.417142 ccinput-1.9.0/ccinput/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/test_calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)    38742 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)   111131 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)    59121 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/test_orca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/test_psi4.py
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/test_pysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    47385 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/test_qchem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/test_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    22171 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/test_xtb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/tests/testing_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    13676 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    18972 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/verify_sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-06-07 00:54:18.000000 ccinput-1.9.0/ccinput/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 00:55:14.413142 ccinput-1.9.0/ccinput.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-07 00:55:14.000000 ccinput-1.9.0/ccinput.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-07 00:55:14.000000 ccinput-1.9.0/ccinput.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 00:55:14.000000 ccinput-1.9.0/ccinput.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 00:55:14.000000 ccinput-1.9.0/ccinput.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 00:55:14.000000 ccinput-1.9.0/ccinput.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 00:55:14.000000 ccinput-1.9.0/ccinput.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 00:55:14.000000 ccinput-1.9.0/ccinput.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-07 00:54:18.000000 ccinput-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-07 00:55:14.421142 ccinput-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-07 00:54:18.000000 ccinput-1.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-07 00:54:18.000000 ccinput-1.9.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:42:55.154546 ccinput-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-12 15:42:12.000000 ccinput-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-12 15:42:12.000000 ccinput-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-12 15:42:55.154546 ccinput-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-12 15:42:12.000000 ccinput-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:42:55.154546 ccinput-1.9.1/ccinput/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-12 15:42:55.154546 ccinput-1.9.1/ccinput/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19056 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90236 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/documentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:42:55.150546 ccinput-1.9.1/ccinput/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/drivers/pysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:42:55.154546 ccinput-1.9.1/ccinput/packages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/packages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15455 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/packages/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/packages/nwchem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15963 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/packages/orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/packages/psi4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/packages/qchem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/packages/xtb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/presets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:42:55.154546 ccinput-1.9.1/ccinput/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/tests/test_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38742 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)   111131 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32113 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/tests/test_nwchem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59121 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/tests/test_orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/tests/test_psi4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/tests/test_pysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47385 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/tests/test_qchem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/tests/test_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22171 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/tests/test_xtb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/tests/testing_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18972 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/verify_sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-06-12 15:42:12.000000 ccinput-1.9.1/ccinput/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:42:55.150546 ccinput-1.9.1/ccinput.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-12 15:42:55.000000 ccinput-1.9.1/ccinput.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-12 15:42:55.000000 ccinput-1.9.1/ccinput.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:42:55.000000 ccinput-1.9.1/ccinput.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 15:42:55.000000 ccinput-1.9.1/ccinput.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:42:55.000000 ccinput-1.9.1/ccinput.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-12 15:42:55.000000 ccinput-1.9.1/ccinput.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 15:42:55.000000 ccinput-1.9.1/ccinput.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-12 15:42:12.000000 ccinput-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-12 15:42:55.154546 ccinput-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-12 15:42:12.000000 ccinput-1.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-12 15:42:12.000000 ccinput-1.9.1/versioneer.py
```

### Comparing `ccinput-1.9.0/LICENSE` & `ccinput-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/PKG-INFO` & `ccinput-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccinput
-Version: 1.9.0
+Version: 1.9.1
 Summary: Computational Chemistry Input Generator
 Home-page: http://github.com/cyllab/ccinput
 Author: Raphaël Robidas
 Author-email: Raphael.Robidas@USherbrooke.ca
 License: BSD 3-Clause
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ccinput-1.9.0/README.md` & `ccinput-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/calculation.py` & `ccinput-1.9.1/ccinput/calculation.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from itertools import zip_longest
 
 from ccinput.exceptions import (
     InvalidParameter,
     InternalError,
     ImpossibleCalculation,
     MissingParameter,
+    UnimplementedError,
 )
 from ccinput.utilities import (
     get_abs_software,
     get_method,
     get_abs_basis_set,
     get_abs_solvent,
     get_theory_level,
@@ -443,14 +444,35 @@
         elif type == 3:
             t = "angle"
         elif type == 4:
             t = "dihedral"
 
         return f"{t}: {ids_str}\n"
 
+    def to_nwchem(self):
+        ids_str = " ".join([str(i) for i in self.ids])
+        converstion_factor = 1.00
+        type = len(self.ids)
+        if type == 1:
+            t = "fix atom"
+        elif type == 2:
+            t = "spring bond"
+            converstion_factor = 1.8897259886
+        elif type == 3:
+            raise UnimplementedError(
+                "Constraints on angles are not implemented in nwchem"
+            )
+        elif type == 4:
+            t = "spring dihedral"
+
+        if self.scan:
+            pass  # TO DO
+        else:
+            return f"{t} {ids_str} 200.0 {self.start_d*converstion_factor :.8f} \n"
+
 
 def parse_freeze_constraints(arr, xyz_str, software=""):
     if len(arr) == 0:
         return []
     constr = ""
     for c in arr:
         constr += f'Freeze/{"_".join([str(i) for i in c])};'
```

### Comparing `ccinput-1.9.0/ccinput/constants.py` & `ccinput-1.9.1/ccinput/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -489,15 +489,15 @@
     "ccsd": [],
     "ccsdt": [],
     "qcisd": [],
     "qcisdt": [],
     "lpnoccsd": [],
     "lpnoccsdt": [],
     "lpnoqcisd": [],
-    "lpnoqcisdt": [],
+    "l7pnoqcisdt": [],
     "dlpnoccsd": [],
     "dlpnoccsdt": [],
     "dlpnoqcisd": [],
     "dlpnoqcisdt": [],
 }
 
 
@@ -1694,15 +1694,15 @@
         "blyp": "blyp",
         "b3lyp": "b3lyp",
         "pbe": "pbe",
         "pw91": "pw91",
         "revpbe": "revpbe",
         "rpbe": "rpbe",
     },
-    "nwchem": {  # Values are correct, keys need to be checked! - Zarko
+    "nwchem": {
         "hf": "hf",
         "rohf": "rohf",
         "uhf": "uhf",
         # exchange-correlation functionals
         "acm": "acm",
         "b3lyp": "b3lyp",
         "becke97": "becke97",
```

### Comparing `ccinput-1.9.0/ccinput/documentation.py` & `ccinput-1.9.1/ccinput/documentation.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/drivers/pysis.py` & `ccinput-1.9.1/ccinput/drivers/pysis.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/packages/gaussian.py` & `ccinput-1.9.1/ccinput/packages/gaussian.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/packages/nwchem.py` & `ccinput-1.9.1/ccinput/packages/nwchem.py`

 * *Files 23% similar despite different names*

```diff
@@ -48,77 +48,47 @@
     # Method Block
     # Calculation Block
     # Additional Block
     # Tasks
 
     KEYWORDS = {
         CalcType.OPT: ["optimize"],
-        #    CalcType.CONSTR_OPT: ["opt"],
+        CalcType.CONSTR_OPT: ["optimize"],
         CalcType.TS: ["saddle"],
         CalcType.FREQ: ["freq"],
         CalcType.NMR: ["property"],
         CalcType.SP: ["energy"],
         #    CalcType.UVVIS: ["td"],
         #    CalcType.UVVIS_TDA: ["tda"],
         CalcType.OPTFREQ: ["optimize", "freq"],
     }
-    BLOCK_KEYWORDS = {
-        "method": [
-            "sym",
-            "adapt",
-            "tol2e",
-            "vectors",
-            "tresh",
-            "maxiter",
-            "profile",
-            "diis",
-            "direct",
-            "semidirect",
-            "nr",
-            "level",
-            "convergence",
-            "grid",
-            "tolerances",
-            "decomp",
-            "odft",
-            "incore",
-            "iterations",
-            "max_ovl",
-            "cgmin",
-            "rodft",
-            "disp",
-            "xdm",
-            "noio",
-            "print",
-            "noprint",
-            "fon",
-            "nodisk",
-            "fukui",
-            "noscf",
-        ],
-        "calculation": [
-            "a",  # TO DO
-        ],
-    }
+
     BLOCK_NAMES = {
         CalcType.OPT: "driver",
         CalcType.NMR: "property",
         CalcType.FREQ: "freq",
         CalcType.OPTFREQ: "driver",
         CalcType.TS: "driver",
     }
 
     def __init__(self, calc):
         self.calc = calc
-        if self.calc.parameters.theory_level == "hf":  # Name of the block for HF is scf
-            self.calc.parameters.theory_level = "scf"
         self.calc.mem = f"{self.calc.mem} mb"
         self.has_scan = False
         self.appendix = []
         self.command_line = ""
+        if (
+            self.calc.parameters.theory_level == "hf"
+            or self.calc.parameters.method == "uhf"
+            or self.calc.parameters.method == "rhf"
+        ):  # Name of the block for HF is scf
+            self.calc.parameters.theory_level = "scf"
+        self.method_block = f"{self.calc.parameters.theory_level}"
+        self.calculation_block = ""
+        self.additional_block = ""
         self.method_block = f"{self.calc.parameters.theory_level}"
         self.calculation_block = ""
         self.additional_block = ""
         self.commands = {}
         self.solvation_radii = {}
         self.xyz_structure = ""
         self.tasks = ""
@@ -140,67 +110,94 @@
         WHITELIST = set(
             "0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ/()=-,. "
         )
         return "".join([c for c in s if c in WHITELIST])
 
     def separate_lines(self, text):
         lines = text.split(";")
+        clean = []
         for line in lines:
-            line = self.clean(line)
-        return "\n".join(lines)
+            if line != "":
+                clean.append(self.clean(line.lower()).strip())
+            else:
+                pass
+        return "\n".join(clean)
 
     def handle_tasks(self):
         for word in self.KEYWORDS[self.calc.type]:
             self.tasks += f"task {self.calc.parameters.theory_level} {word} \n"
         # handle levels of theory
-        if (
-            self.calc.parameters.method == "hf"
-            or self.calc.parameters.method in SYN_METHODS["hf"]
-        ):
-            scf_block = f"""
-            {SOFTWARE_MULTIPLICITY['nwchem'][self.calc.multiplicity]}
-            """
+        if self.calc.parameters.theory_level == "scf":
+            scf_block = "\n"
+            if self.calc.parameters.method != "hf":
+                scf_block += f"{self.calc.parameters.method} \n"
+            scf_block += f"{SOFTWARE_MULTIPLICITY['nwchem'][self.calc.multiplicity]} \n"
             self.method_block += scf_block
         if self.calc.parameters.theory_level == "dft":
             dft_block = f"""
             xc {self.calc.parameters.method}
             mult {self.calc.multiplicity}
             """
             self.method_block += dft_block
             if self.calc.parameters.d3:
                 self.method_block += "disp vdw 3 \n"
             elif self.calc.parameters.d3bj:
                 self.method_block += "disp vdw 4 \n"
+        if self.calc.type == CalcType.NMR:
+            self.calculation_block += f" \n property \n shielding \n"
 
     def handle_basis_sets(self):
         basis_set = get_basis_set(self.calc.parameters.basis_set, "nwchem")
         if basis_set != "":
             self.basis_set = f"* library {basis_set}"
 
     def handle_specifications(self):
         if self.calc.parameters.specifications != "":
+            temp = "\n"  # Here we will store frequency related specifiations in case of FREQOPT calculations
             s = self.separate_lines(self.calc.parameters.specifications)
             for spec in s.split("\n"):
+                # format of the specifications is BLOCK_NAME1(command1);BLOCK_NAME2(command2);...
                 matched = re.search(r".*\((.*)\)", spec)
                 if matched == None:
                     self.additional_block += f"{spec} \n"
                 else:
                     command = matched.group(1)
                     block_name = spec[: matched.span(1)[0] - 1]
-                    if block_name == "scf":
+                    if block_name == "scf" or block_name == "dft" or block_name == "hf":
                         self.method_block += f"{command} \n"
-                    elif block_name == "opt" or block_name == "ts":
+                    elif (block_name == "opt" or block_name == "ts") and (
+                        self.calc.type == CalcType.CONSTR_OPT
+                        or self.calc.type == CalcType.OPT
+                        or self.calc.type == CalcType.TS
+                        or self.calc.type == CalcType.OPTFREQ
+                    ):
                         if self.calculation_block == "":
                             self.calculation_block += f"\n driver \n"
                         self.calculation_block += f"{command} \n"
-                    elif block_name == "nmr":
+                    elif block_name == "nmr" and self.calc.type == CalcType.NMR:
+                        self.calculation_block += f"{command} \n"
+                    elif block_name == "freq" and self.calc.type == CalcType.FREQ:
                         if self.calculation_block == "":
-                            self.calculation_block += f" \n property \n"
+                            self.calculation_block += f"\n freq \n"
                         self.calculation_block += f"{command} \n"
-        if self.additional_block != "":
+                    elif block_name == "freq" and self.calc.type == CalcType.OPTFREQ:
+                        temp += f"{command} \n"
+            if temp != "\n":
+                self.additional_block += f"freq {temp} end \n"
+
+        # Handle contraints
+        if self.calc.type == CalcType.CONSTR_OPT:
+            if len(self.calc.constraints) == 0:
+                raise InvalidParameter("No constraint in constrained optimisation mode")
+            self.additional_block += "constraints \n"
+            for constraint in self.calc.constraints:
+                self.additional_block += constraint.to_nwchem()
+            self.additional_block += "end \n"
+
+        if self.additional_block.strip() != "":
             self.additional_block = "\n" + self.additional_block
 
     def handle_xyz(self):
         lines = [i + "\n" for i in clean_xyz(self.calc.xyz).split("\n") if i != ""]
         self.xyz_structure = "".join(lines)
 
     def handle_solvation(self):
```

### Comparing `ccinput-1.9.0/ccinput/packages/orca.py` & `ccinput-1.9.1/ccinput/packages/orca.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/packages/psi4.py` & `ccinput-1.9.1/ccinput/packages/psi4.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/packages/qchem.py` & `ccinput-1.9.1/ccinput/packages/qchem.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/packages/xtb.py` & `ccinput-1.9.1/ccinput/packages/xtb.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/presets.py` & `ccinput-1.9.1/ccinput/presets.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/tests/test_calculation.py` & `ccinput-1.9.1/ccinput/tests/test_calculation.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/tests/test_cli.py` & `ccinput-1.9.1/ccinput/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/tests/test_gaussian.py` & `ccinput-1.9.1/ccinput/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/tests/test_orca.py` & `ccinput-1.9.1/ccinput/tests/test_orca.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/tests/test_psi4.py` & `ccinput-1.9.1/ccinput/tests/test_psi4.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/tests/test_pysis.py` & `ccinput-1.9.1/ccinput/tests/test_pysis.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/tests/test_qchem.py` & `ccinput-1.9.1/ccinput/tests/test_qchem.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/tests/test_structures.py` & `ccinput-1.9.1/ccinput/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/tests/test_xtb.py` & `ccinput-1.9.1/ccinput/tests/test_xtb.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/tests/testing_utilities.py` & `ccinput-1.9.1/ccinput/tests/testing_utilities.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/utilities.py` & `ccinput-1.9.1/ccinput/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,14 +281,22 @@
                     return method[0].upper() + xc_check
 
             xc_check = is_exchange_correlation_combination(method.lower(), software)
             if isinstance(xc_check, str):
                 return xc_check
             warn(f"Unknown method '{method}'")
         if software == "nwchem":
+            if method.lower()[0] in ["u", "r"]:
+                try:
+                    abs_method = get_abs_method(method[1:])
+                except InvalidParameter:
+                    pass
+                else:
+                    if abs_method in SOFTWARE_METHODS[software]:
+                        return method[0] + SOFTWARE_METHODS[software][abs_method]
             # nwchem also supports combination of functionals
             if len(method.split()) == 2:
                 xc_check = is_exchange_correlation_combination(
                     indexify(method), "nwchem"
                 )
                 if isinstance(xc_check, str):
                     return xc_check
```

### Comparing `ccinput-1.9.0/ccinput/verify_sanity.py` & `ccinput-1.9.1/ccinput/verify_sanity.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput/wrapper.py` & `ccinput-1.9.1/ccinput/wrapper.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/ccinput.egg-info/PKG-INFO` & `ccinput-1.9.1/ccinput.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccinput
-Version: 1.9.0
+Version: 1.9.1
 Summary: Computational Chemistry Input Generator
 Home-page: http://github.com/cyllab/ccinput
 Author: Raphaël Robidas
 Author-email: Raphael.Robidas@USherbrooke.ca
 License: BSD 3-Clause
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ccinput-1.9.0/ccinput.egg-info/SOURCES.txt` & `ccinput-1.9.1/ccinput.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 ccinput/packages/psi4.py
 ccinput/packages/qchem.py
 ccinput/packages/xtb.py
 ccinput/tests/__init__.py
 ccinput/tests/test_calculation.py
 ccinput/tests/test_cli.py
 ccinput/tests/test_gaussian.py
+ccinput/tests/test_nwchem.py
 ccinput/tests/test_orca.py
 ccinput/tests/test_psi4.py
 ccinput/tests/test_pysis.py
 ccinput/tests/test_qchem.py
 ccinput/tests/test_structures.py
 ccinput/tests/test_xtb.py
 ccinput/tests/testing_utilities.py
```

### Comparing `ccinput-1.9.0/setup.py` & `ccinput-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `ccinput-1.9.0/versioneer.py` & `ccinput-1.9.1/versioneer.py`

 * *Files identical despite different names*

