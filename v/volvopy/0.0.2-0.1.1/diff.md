# Comparing `tmp/volvopy-0.0.2.tar.gz` & `tmp/volvopy-0.1.1.tar.gz`

## Comparing `volvopy-0.0.2.tar` & `volvopy-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rwxr-xr-x   0        0        0     2157 2020-02-02 00:00:00.000000 volvopy-0.0.2/mkbld
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 volvopy-0.0.2/tox.ini
--rw-r--r--   0        0        0    18390 2020-02-02 00:00:00.000000 volvopy-0.0.2/docs/energy-api-specification.json
--rwxr-xr-x   0        0        0     1906 2020-02-02 00:00:00.000000 volvopy-0.0.2/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 volvopy-0.0.2/LICENSE
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 volvopy-0.0.2/README.md
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 volvopy-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 volvopy-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 volvopy-0.1.1/BUILDING.md
+-rwxr-xr-x   0        0        0     2157 2020-02-02 00:00:00.000000 volvopy-0.1.1/mkbld
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 volvopy-0.1.1/tox.ini
+-rw-r--r--   0        0        0    18390 2020-02-02 00:00:00.000000 volvopy-0.1.1/docs/energy-api-specification.json
+-rwxr-xr-x   0        0        0     1906 2020-02-02 00:00:00.000000 volvopy-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 volvopy-0.1.1/LICENSE
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 volvopy-0.1.1/README.md
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 volvopy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 volvopy-0.1.1/PKG-INFO
```

### Comparing `volvopy-0.0.2/mkbld` & `volvopy-0.1.1/mkbld`

 * *Files identical despite different names*

### Comparing `volvopy-0.0.2/tox.ini` & `volvopy-0.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `volvopy-0.0.2/docs/energy-api-specification.json` & `volvopy-0.1.1/docs/energy-api-specification.json`

 * *Files identical despite different names*

### Comparing `volvopy-0.0.2/.gitignore` & `volvopy-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `volvopy-0.0.2/LICENSE` & `volvopy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `volvopy-0.0.2/pyproject.toml` & `volvopy-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "volvopy"
 description = "Connect to the Volvo API using Python."
-version = "0.0.2"  # latest/current distribution version
-# version = "0.0.1"  # latest test version
+# version = "0.1.1"  # latest/current distribution version
+version = "0.1.1"  # latest test version
 dependencies = []
 license = "MIT"
 authors = [
   { name="Mausy5043" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `volvopy-0.0.2/PKG-INFO` & `volvopy-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volvopy
-Version: 0.0.2
+Version: 0.1.1
 Summary: Connect to the Volvo API using Python.
 Project-URL: Homepage, https://github.com/Mausy5043/volvopy
 Project-URL: Bug Tracker, https://github.com/Mausy5043/volvopy/issues
 Author: Mausy5043
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 1 - Planning
```

