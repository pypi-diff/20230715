# Comparing `tmp/volttron_lib_boptest_integration-0.1.1rc1.tar.gz` & `tmp/volttron_lib_boptest_integration-0.1.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_lib_boptest_integration-0.1.1rc1.tar", max compression
+gzip compressed data, was "volttron_lib_boptest_integration-0.1.1rc2.tar", max compression
```

## Comparing `volttron_lib_boptest_integration-0.1.1rc1.tar` & `volttron_lib_boptest_integration-0.1.1rc2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11927 2023-07-15 05:17:31.853172 volttron_lib_boptest_integration-0.1.1rc1/LICENSE
--rw-r--r--   0        0        0     9418 2023-07-15 05:17:31.853172 volttron_lib_boptest_integration-0.1.1rc1/README.md
--rw-r--r--   0        0        0     1856 2023-07-15 05:19:39.890171 volttron_lib_boptest_integration-0.1.1rc1/pyproject.toml
--rw-r--r--   0        0        0        1 2023-07-15 05:17:31.857172 volttron_lib_boptest_integration-0.1.1rc1/src/boptest_integration/__init__.py
--rw-r--r--   0        0        0    13693 2023-07-15 05:17:31.857172 volttron_lib_boptest_integration-0.1.1rc1/src/boptest_integration/boptest_integration.py
--rw-r--r--   0        0        0      108 2023-07-15 05:17:31.857172 volttron_lib_boptest_integration-0.1.1rc1/src/boptest_integration/controllers/__init__.py
--rw-r--r--   0        0        0     3252 2023-07-15 05:17:31.857172 volttron_lib_boptest_integration-0.1.1rc1/src/boptest_integration/controllers/controller.py
--rw-r--r--   0        0        0     1537 2023-07-15 05:17:31.857172 volttron_lib_boptest_integration-0.1.1rc1/src/boptest_integration/controllers/pid.py
--rw-r--r--   0        0        0     4610 2023-07-15 05:17:31.857172 volttron_lib_boptest_integration-0.1.1rc1/src/boptest_integration/controllers/pidTwoZones.py
--rw-r--r--   0        0        0     1179 2023-07-15 05:17:31.857172 volttron_lib_boptest_integration-0.1.1rc1/src/boptest_integration/controllers/sup.py
--rw-r--r--   0        0        0     9666 2023-07-15 05:17:31.857172 volttron_lib_boptest_integration-0.1.1rc1/src/boptest_integration/interface.py
--rw-r--r--   0        0        0    10690 1970-01-01 00:00:00.000000 volttron_lib_boptest_integration-0.1.1rc1/PKG-INFO
+-rw-r--r--   0        0        0    11927 2023-07-15 05:26:00.995697 volttron_lib_boptest_integration-0.1.1rc2/LICENSE
+-rw-r--r--   0        0        0     9418 2023-07-15 05:26:00.995697 volttron_lib_boptest_integration-0.1.1rc2/README.md
+-rw-r--r--   0        0        0     1856 2023-07-15 05:27:47.983273 volttron_lib_boptest_integration-0.1.1rc2/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-07-15 05:26:00.999697 volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/__init__.py
+-rw-r--r--   0        0        0    13693 2023-07-15 05:26:00.999697 volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/boptest_integration.py
+-rw-r--r--   0        0        0      108 2023-07-15 05:26:00.999697 volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/controllers/__init__.py
+-rw-r--r--   0        0        0     3252 2023-07-15 05:26:00.999697 volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/controllers/controller.py
+-rw-r--r--   0        0        0     1537 2023-07-15 05:26:00.999697 volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/controllers/pid.py
+-rw-r--r--   0        0        0     4610 2023-07-15 05:26:00.999697 volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/controllers/pidTwoZones.py
+-rw-r--r--   0        0        0     1179 2023-07-15 05:26:00.999697 volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/controllers/sup.py
+-rw-r--r--   0        0        0     9666 2023-07-15 05:26:00.999697 volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/interface.py
+-rw-r--r--   0        0        0    10690 1970-01-01 00:00:00.000000 volttron_lib_boptest_integration-0.1.1rc2/PKG-INFO
```

### Comparing `volttron_lib_boptest_integration-0.1.1rc1/LICENSE` & `volttron_lib_boptest_integration-0.1.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1rc1/README.md` & `volttron_lib_boptest_integration-0.1.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1rc1/pyproject.toml` & `volttron_lib_boptest_integration-0.1.1rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ignore_missing_imports = true
 
 [tool.mypy-pytz]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "volttron-lib-boptest-integration"
-version = "0.1.1rc1"
+version = "0.1.1rc2"
 description = "A Volttron library for boptest simulation integration."
 authors = ["Kefei Mo <kefei.mo@pnnl.gov>"]
 license = "Apache-2.0"
 maintainers = ["Volttron Team <volttron@pnnl.gov>"]
 readme = "README.md"
 homepage = "https://github.com/eclipse-volttron/volttron-boptest"
 repository = "https://github.com/eclipse-volttron/volttron-boptest"
```

### Comparing `volttron_lib_boptest_integration-0.1.1rc1/src/boptest_integration/boptest_integration.py` & `volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/boptest_integration.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1rc1/src/boptest_integration/controllers/controller.py` & `volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1rc1/src/boptest_integration/controllers/pid.py` & `volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/controllers/pid.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1rc1/src/boptest_integration/controllers/pidTwoZones.py` & `volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/controllers/pidTwoZones.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1rc1/src/boptest_integration/controllers/sup.py` & `volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/controllers/sup.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1rc1/src/boptest_integration/interface.py` & `volttron_lib_boptest_integration-0.1.1rc2/src/boptest_integration/interface.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_boptest_integration-0.1.1rc1/PKG-INFO` & `volttron_lib_boptest_integration-0.1.1rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volttron-lib-boptest-integration
-Version: 0.1.1rc1
+Version: 0.1.1rc2
 Summary: A Volttron library for boptest simulation integration.
 Home-page: https://github.com/eclipse-volttron/volttron-boptest
 License: Apache-2.0
 Keywords: volttron,boptest,simulation,integration
 Author: Kefei Mo
 Author-email: kefei.mo@pnnl.gov
 Maintainer: Volttron Team
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: volttron-lib-boptest-integration Version: 0.1.1rc1
+Metadata-Version: 2.1 Name: volttron-lib-boptest-integration Version: 0.1.1rc2
 Summary: A Volttron library for boptest simulation integration. Home-page:
 https://github.com/eclipse-volttron/volttron-boptest License: Apache-2.0
 Keywords: volttron,boptest,simulation,integration Author: Kefei Mo Author-
 email: kefei.mo@pnnl.gov Maintainer: Volttron Team Maintainer-email:
 volttron@pnnl.gov Requires-Python: >=3.10,<4.0 Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
```

