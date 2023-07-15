# Comparing `tmp/pyrainbird-2.1.1.tar.gz` & `tmp/pyrainbird-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrainbird-2.1.1.tar", last modified: Sat Jul 15 02:43:30 2023, max compression
+gzip compressed data, was "pyrainbird-3.0.0.tar", last modified: Sat Jul 15 18:00:31 2023, max compression
```

## Comparing `pyrainbird-2.1.1.tar` & `pyrainbird-3.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:30.275490 pyrainbird-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-15 02:43:30.275490 pyrainbird-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:30.271490 pyrainbird-2.1.1/pyrainbird/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    21075 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/rainbird.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:30.271490 pyrainbird-2.1.1/pyrainbird/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/resources/models.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/resources/sipcommands.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/pyrainbird/timeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:30.275490 pyrainbird-2.1.1/pyrainbird.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-15 02:43:30.000000 pyrainbird-2.1.1/pyrainbird.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-15 02:43:30.000000 pyrainbird-2.1.1/pyrainbird.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 02:43:30.000000 pyrainbird-2.1.1/pyrainbird.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-15 02:43:30.000000 pyrainbird-2.1.1/pyrainbird.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-15 02:43:30.000000 pyrainbird-2.1.1/pyrainbird.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-15 02:43:30.275490 pyrainbird-2.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:30.275490 pyrainbird-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    46176 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/tests/test_async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-15 02:43:18.000000 pyrainbird-2.1.1/tests/test_rainbird.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:00:31.010426 pyrainbird-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-15 18:00:17.000000 pyrainbird-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-15 18:00:31.014426 pyrainbird-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-15 18:00:17.000000 pyrainbird-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:00:31.010426 pyrainbird-3.0.0/pyrainbird/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-15 18:00:17.000000 pyrainbird-3.0.0/pyrainbird/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-07-15 18:00:17.000000 pyrainbird-3.0.0/pyrainbird/async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-15 18:00:17.000000 pyrainbird-3.0.0/pyrainbird/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21246 2023-07-15 18:00:17.000000 pyrainbird-3.0.0/pyrainbird/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-07-15 18:00:17.000000 pyrainbird-3.0.0/pyrainbird/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-15 18:00:17.000000 pyrainbird-3.0.0/pyrainbird/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-07-15 18:00:17.000000 pyrainbird-3.0.0/pyrainbird/rainbird.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:00:31.010426 pyrainbird-3.0.0/pyrainbird/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-15 18:00:17.000000 pyrainbird-3.0.0/pyrainbird/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-15 18:00:17.000000 pyrainbird-3.0.0/pyrainbird/resources/models.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-07-15 18:00:17.000000 pyrainbird-3.0.0/pyrainbird/resources/sipcommands.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-15 18:00:17.000000 pyrainbird-3.0.0/pyrainbird/timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:00:31.010426 pyrainbird-3.0.0/pyrainbird.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-15 18:00:30.000000 pyrainbird-3.0.0/pyrainbird.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-15 18:00:31.000000 pyrainbird-3.0.0/pyrainbird.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 18:00:30.000000 pyrainbird-3.0.0/pyrainbird.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-15 18:00:30.000000 pyrainbird-3.0.0/pyrainbird.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-15 18:00:30.000000 pyrainbird-3.0.0/pyrainbird.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-15 18:00:31.014426 pyrainbird-3.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-07-15 18:00:17.000000 pyrainbird-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:00:31.010426 pyrainbird-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    46176 2023-07-15 18:00:17.000000 pyrainbird-3.0.0/tests/test_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-15 18:00:17.000000 pyrainbird-3.0.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-15 18:00:17.000000 pyrainbird-3.0.0/tests/test_rainbird.py
```

### Comparing `pyrainbird-2.1.1/LICENSE` & `pyrainbird-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.1/PKG-INFO` & `pyrainbird-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pyrainbird
-Version: 2.1.1
+Version: 3.0.0
 Summary: Rain Bird Controller
 Home-page: https://github.com/allenporter/pyrainbird
 Author: J.J.Barrancos
 Author-email: jordy@fusion-ict.nl
 License: MIT
 Keywords: Rain Bird
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Python module for interacting with [WiFi LNK](https://www.rainbird.com/products/module-wi-fi-lnk) module of the Rain Bird Irrigation system. This project has no affiliation with Rain Bird.
 
 This module communicates directly towards the IP Address of the WiFi module. You can start/stop the irrigation, get the currently active zone, and other controller settings. This library currently only has very limited cloud support. Also there are a number of Rain Bird devices with very different command APIs.
```

### Comparing `pyrainbird-2.1.1/README.md` & `pyrainbird-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.1/pyrainbird/async_client.py` & `pyrainbird-3.0.0/pyrainbird/async_client.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.1/pyrainbird/const.py` & `pyrainbird-3.0.0/pyrainbird/const.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.1/pyrainbird/data.py` & `pyrainbird-3.0.0/pyrainbird/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 from collections.abc import Iterable
 from dataclasses import dataclass
 from enum import IntEnum
 from typing import Any, Optional
 
 from ical.iter import MergedIterable, SortableItem
 from ical.timespan import Timespan
-from pydantic import BaseModel, Field, root_validator, validator
+try:
+    from pydantic.v1 import BaseModel, Field, root_validator, validator
+except ImportError:
+    from pydantic import BaseModel, Field, root_validator, validator
 
 from .const import DayOfWeek, ProgramFrequency
 from .resources import RAINBIRD_MODELS
 from .timeline import ProgramEvent, ProgramTimeline, create_recurrence, ProgramId
 
 _LOGGER = logging.getLogger(__name__)
 
@@ -93,15 +96,17 @@
     def model_name(self) -> str:
         """The device model name."""
         return self.model_info.name
 
     @property
     def model_info(self) -> ModelInfo:
         """Return details about a device model capabilities."""
-        return ModelInfo(**RAINBIRD_MODELS["%04x" % self.model])
+        key = f"{self.model:04x}"
+        data = RAINBIRD_MODELS.get(key, RAINBIRD_MODELS["UNKNOWN"])
+        return ModelInfo(**data)
 
     def __str__(self):
         return "model: %04X (%s), version: %d.%d" % (
             self.model,
             self.model_name,
             self.major,
             self.minor,
```

### Comparing `pyrainbird-2.1.1/pyrainbird/encryption.py` & `pyrainbird-3.0.0/pyrainbird/encryption.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.1/pyrainbird/rainbird.py` & `pyrainbird-3.0.0/pyrainbird/rainbird.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.1/pyrainbird/resources/__init__.py` & `pyrainbird-3.0.0/pyrainbird/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.1/pyrainbird/resources/models.yaml` & `pyrainbird-3.0.0/pyrainbird/resources/models.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -69,14 +69,21 @@
 - device_id: "0099"
   code: TBOS_BT
   name: TBOS-BT
   supports_water_budget: true
   max_programs: 3
   max_run_times: 8
 
+- device_id: "0100"
+  code: TBOS_BT
+  name: TBOS-BT
+  supports_water_budget: true
+  max_programs: 3
+  max_run_times: 8
+
 - device_id: "0107"
   code: ESP_MEv2
   name: ESP-Me
   supports_water_budget: true
   max_programs: 4
   max_run_times: 6
   retries: true
@@ -85,12 +92,27 @@
   code: ESP_RZXe2
   name: ESP-RZXe2
   supports_water_budget: false
   max_programs: 8
   max_run_times: 6
 
 - device_id: "0812"
+  code: RC2
+  name: RC2
+  supports_water_budget: true
+  max_programs: 3
+  max_run_times: 4
+
+- device_id: "0813"
   code: ARC8
   name: ARC8
   supports_water_budget: true
   max_programs: 3
   max_run_times: 4
+
+- device_id: "UNKNOWN"
+  code: UNKNOWN
+  name: Unknown
+  supports_water_budget: false
+  max_programs: 0
+  max_run_times: 0
+  retries: false
```

### Comparing `pyrainbird-2.1.1/pyrainbird/resources/sipcommands.yaml` & `pyrainbird-3.0.0/pyrainbird/resources/sipcommands.yaml`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.1/pyrainbird/timeline.py` & `pyrainbird-3.0.0/pyrainbird/timeline.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.1/pyrainbird.egg-info/PKG-INFO` & `pyrainbird-3.0.0/pyrainbird.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pyrainbird
-Version: 2.1.1
+Version: 3.0.0
 Summary: Rain Bird Controller
 Home-page: https://github.com/allenporter/pyrainbird
 Author: J.J.Barrancos
 Author-email: jordy@fusion-ict.nl
 License: MIT
 Keywords: Rain Bird
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Python module for interacting with [WiFi LNK](https://www.rainbird.com/products/module-wi-fi-lnk) module of the Rain Bird Irrigation system. This project has no affiliation with Rain Bird.
 
 This module communicates directly towards the IP Address of the WiFi module. You can start/stop the irrigation, get the currently active zone, and other controller settings. This library currently only has very limited cloud support. Also there are a number of Rain Bird devices with very different command APIs.
```

### Comparing `pyrainbird-2.1.1/pyrainbird.egg-info/SOURCES.txt` & `pyrainbird-3.0.0/pyrainbird.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.1/setup.cfg` & `pyrainbird-3.0.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [metadata]
 name = pyrainbird
-version = 2.1.1
+version = 3.0.0
 description = Rain Bird Controller
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/pyrainbird
 author = J.J.Barrancos
 author_email = jordy@fusion-ict.nl
 license = MIT
 license_file = LICENSE
 keywords = Rain Bird
 
 [options]
 packages = find:
-python_requires > = 3.9
+python_requires = >=3.10
 install_requires = 
 	pycryptodome>=3.16.0
 	requests>=2.22.0
 	PyYAML>=5.4
 	pydantic>=1.10.4
 	python-dateutil>=2.8.2
 	ical>=4.2.9
```

### Comparing `pyrainbird-2.1.1/tests/test_async_client.py` & `pyrainbird-3.0.0/tests/test_async_client.py`

 * *Files identical despite different names*

### Comparing `pyrainbird-2.1.1/tests/test_data.py` & `pyrainbird-3.0.0/tests/test_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import unittest
+from typing import Any
 
+import pytest
 from parameterized import parameterized
 
-from pyrainbird.data import States
+from pyrainbird.data import States, ModelAndVersion
 
 
 def encode_name_func(testcase_func, param_num, param):
     return "%s_%s_%s" % (
         testcase_func.__name__,
         param_num,
         parameterized.to_safe_name(param.args[0]),
@@ -50,7 +52,30 @@
         i = 1
         print(states.active_set)
         for bit in expected:
             print(bit)
             active = i in states.active_set
             assert active == bit
             i = i + 1
+
+@pytest.mark.parametrize(
+    ("response", "expected_name"),
+    [
+        (
+            {'modelID': 2067, 'protocolRevisionMajor': 2, 'protocolRevisionMinor': 12},
+            "ARC8"
+        ),
+        (
+            {'modelID': 9999, 'protocolRevisionMajor': 2, 'protocolRevisionMinor': 12},
+            "Unknown"
+        ),
+    ],
+)
+def test_model_info(response: dict[str, Any], expected_name: str) -> None:
+    """Test parsing of ModelInfo responses."""
+    mv = ModelAndVersion(
+        response["modelID"],
+        response["protocolRevisionMajor"],
+        response["protocolRevisionMinor"],
+    )
+    assert mv.model_name == expected_name
+    assert mv.model_info.name == expected_name
```

### Comparing `pyrainbird-2.1.1/tests/test_rainbird.py` & `pyrainbird-3.0.0/tests/test_rainbird.py`

 * *Files identical despite different names*

