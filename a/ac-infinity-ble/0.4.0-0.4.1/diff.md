# Comparing `tmp/ac_infinity_ble-0.4.0.tar.gz` & `tmp/ac_infinity_ble-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ac_infinity_ble-0.4.0.tar", max compression
+gzip compressed data, was "ac_infinity_ble-0.4.1.tar", max compression
```

## Comparing `ac_infinity_ble-0.4.0.tar` & `ac_infinity_ble-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-07-14 23:08:49.306084 ac_infinity_ble-0.4.0/LICENSE
--rw-r--r--   0        0        0     3538 2023-07-14 23:08:49.306084 ac_infinity_ble-0.4.0/README.md
--rw-r--r--   0        0        0     2182 2023-07-14 23:08:50.126084 ac_infinity_ble-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      322 2023-07-14 23:08:50.098084 ac_infinity_ble-0.4.0/src/ac_infinity_ble/__init__.py
--rw-r--r--   0        0        0      405 2023-07-14 23:08:49.306084 ac_infinity_ble-0.4.0/src/ac_infinity_ble/const.py
--rw-r--r--   0        0        0    16300 2023-07-14 23:08:49.306084 ac_infinity_ble-0.4.0/src/ac_infinity_ble/device.py
--rw-r--r--   0        0        0       96 2023-07-14 23:08:49.310084 ac_infinity_ble-0.4.0/src/ac_infinity_ble/exceptions.py
--rw-r--r--   0        0        0      591 2023-07-14 23:08:49.310084 ac_infinity_ble-0.4.0/src/ac_infinity_ble/models.py
--rw-r--r--   0        0        0     3239 2023-07-14 23:08:49.310084 ac_infinity_ble-0.4.0/src/ac_infinity_ble/protocol.py
--rw-r--r--   0        0        0        0 2023-07-14 23:08:49.310084 ac_infinity_ble-0.4.0/src/ac_infinity_ble/py.typed
--rw-r--r--   0        0        0      756 2023-07-14 23:08:49.310084 ac_infinity_ble-0.4.0/src/ac_infinity_ble/util.py
--rw-r--r--   0        0        0     4659 1970-01-01 00:00:00.000000 ac_infinity_ble-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 23:26:48.157786 ac_infinity_ble-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3538 2023-07-14 23:26:48.157786 ac_infinity_ble-0.4.1/README.md
+-rw-r--r--   0        0        0     2182 2023-07-14 23:26:48.897791 ac_infinity_ble-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      322 2023-07-14 23:26:48.869791 ac_infinity_ble-0.4.1/src/ac_infinity_ble/__init__.py
+-rw-r--r--   0        0        0      405 2023-07-14 23:26:48.157786 ac_infinity_ble-0.4.1/src/ac_infinity_ble/const.py
+-rw-r--r--   0        0        0    16366 2023-07-14 23:26:48.157786 ac_infinity_ble-0.4.1/src/ac_infinity_ble/device.py
+-rw-r--r--   0        0        0       96 2023-07-14 23:26:48.157786 ac_infinity_ble-0.4.1/src/ac_infinity_ble/exceptions.py
+-rw-r--r--   0        0        0      591 2023-07-14 23:26:48.157786 ac_infinity_ble-0.4.1/src/ac_infinity_ble/models.py
+-rw-r--r--   0        0        0     3239 2023-07-14 23:26:48.157786 ac_infinity_ble-0.4.1/src/ac_infinity_ble/protocol.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:26:48.157786 ac_infinity_ble-0.4.1/src/ac_infinity_ble/py.typed
+-rw-r--r--   0        0        0      756 2023-07-14 23:26:48.157786 ac_infinity_ble-0.4.1/src/ac_infinity_ble/util.py
+-rw-r--r--   0        0        0     4659 1970-01-01 00:00:00.000000 ac_infinity_ble-0.4.1/PKG-INFO
```

### Comparing `ac_infinity_ble-0.4.0/LICENSE` & `ac_infinity_ble-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.4.0/README.md` & `ac_infinity_ble-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.4.0/pyproject.toml` & `ac_infinity_ble-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ac-infinity-ble"
-version = "0.4.0"
+version = "0.4.1"
 description = "AC Infinity BLE Controller"
 authors = ["Jason Hunter <hunterjm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/hunterjm/ac-infinity-ble"
 documentation = "https://ac-infinity-ble.readthedocs.io"
 classifiers = [
```

### Comparing `ac_infinity_ble-0.4.0/src/ac_infinity_ble/device.py` & `ac_infinity_ble-0.4.1/src/ac_infinity_ble/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,17 @@
     ) -> None:
         """Set the ble device."""
         self._ble_device = ble_device
         self._advertisement_data = advertisement_data
         info = parse_manufacturer_data(
             advertisement_data.manufacturer_data[MANUFACTURER_ID]
         )
-        self._state = replace(self._state, **asdict(info))
+        self._state = replace(
+            self._state, **{k: v for k, v in asdict(info).items() if v is not None}
+        )
         if self._state.fan:
             if self._state.level_off or 0 > self._state.fan:
                 self._state.level_off = self._state.fan
             if self._state.level_on or 10 < self._state.fan:
                 self._state.level_on = self._state.fan
 
     @property
```

### Comparing `ac_infinity_ble-0.4.0/src/ac_infinity_ble/models.py` & `ac_infinity_ble-0.4.1/src/ac_infinity_ble/models.py`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.4.0/src/ac_infinity_ble/protocol.py` & `ac_infinity_ble-0.4.1/src/ac_infinity_ble/protocol.py`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.4.0/src/ac_infinity_ble/util.py` & `ac_infinity_ble-0.4.1/src/ac_infinity_ble/util.py`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.4.0/PKG-INFO` & `ac_infinity_ble-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ac-infinity-ble
-Version: 0.4.0
+Version: 0.4.1
 Summary: AC Infinity BLE Controller
 Home-page: https://github.com/hunterjm/ac-infinity-ble
 License: MIT
 Author: Jason Hunter
 Author-email: hunterjm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ac-infinity-ble Version: 0.4.0 Summary: AC Infinity
+Metadata-Version: 2.1 Name: ac-infinity-ble Version: 0.4.1 Summary: AC Infinity
 BLE Controller Home-page: https://github.com/hunterjm/ac-infinity-ble License:
 MIT Author: Jason Hunter Author-email: hunterjm@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

