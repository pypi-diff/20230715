# Comparing `tmp/ac_infinity_ble-0.3.0.tar.gz` & `tmp/ac_infinity_ble-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ac_infinity_ble-0.3.0.tar", max compression
+gzip compressed data, was "ac_infinity_ble-0.4.0.tar", max compression
```

## Comparing `ac_infinity_ble-0.3.0.tar` & `ac_infinity_ble-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-07-14 21:09:32.979167 ac_infinity_ble-0.3.0/LICENSE
--rw-r--r--   0        0        0     3538 2023-07-14 21:09:32.979167 ac_infinity_ble-0.3.0/README.md
--rw-r--r--   0        0        0     2182 2023-07-14 21:09:33.771173 ac_infinity_ble-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      322 2023-07-14 21:09:33.743172 ac_infinity_ble-0.3.0/src/ac_infinity_ble/__init__.py
--rw-r--r--   0        0        0      405 2023-07-14 21:09:32.983168 ac_infinity_ble-0.3.0/src/ac_infinity_ble/const.py
--rw-r--r--   0        0        0    16046 2023-07-14 21:09:32.983168 ac_infinity_ble-0.3.0/src/ac_infinity_ble/device.py
--rw-r--r--   0        0        0       96 2023-07-14 21:09:32.983168 ac_infinity_ble-0.3.0/src/ac_infinity_ble/exceptions.py
--rw-r--r--   0        0        0      591 2023-07-14 21:09:32.983168 ac_infinity_ble-0.3.0/src/ac_infinity_ble/models.py
--rw-r--r--   0        0        0     3150 2023-07-14 21:09:32.983168 ac_infinity_ble-0.3.0/src/ac_infinity_ble/protocol.py
--rw-r--r--   0        0        0        0 2023-07-14 21:09:32.983168 ac_infinity_ble-0.3.0/src/ac_infinity_ble/py.typed
--rw-r--r--   0        0        0      756 2023-07-14 21:09:32.983168 ac_infinity_ble-0.3.0/src/ac_infinity_ble/util.py
--rw-r--r--   0        0        0     4659 1970-01-01 00:00:00.000000 ac_infinity_ble-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 23:08:49.306084 ac_infinity_ble-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3538 2023-07-14 23:08:49.306084 ac_infinity_ble-0.4.0/README.md
+-rw-r--r--   0        0        0     2182 2023-07-14 23:08:50.126084 ac_infinity_ble-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      322 2023-07-14 23:08:50.098084 ac_infinity_ble-0.4.0/src/ac_infinity_ble/__init__.py
+-rw-r--r--   0        0        0      405 2023-07-14 23:08:49.306084 ac_infinity_ble-0.4.0/src/ac_infinity_ble/const.py
+-rw-r--r--   0        0        0    16300 2023-07-14 23:08:49.306084 ac_infinity_ble-0.4.0/src/ac_infinity_ble/device.py
+-rw-r--r--   0        0        0       96 2023-07-14 23:08:49.310084 ac_infinity_ble-0.4.0/src/ac_infinity_ble/exceptions.py
+-rw-r--r--   0        0        0      591 2023-07-14 23:08:49.310084 ac_infinity_ble-0.4.0/src/ac_infinity_ble/models.py
+-rw-r--r--   0        0        0     3239 2023-07-14 23:08:49.310084 ac_infinity_ble-0.4.0/src/ac_infinity_ble/protocol.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:08:49.310084 ac_infinity_ble-0.4.0/src/ac_infinity_ble/py.typed
+-rw-r--r--   0        0        0      756 2023-07-14 23:08:49.310084 ac_infinity_ble-0.4.0/src/ac_infinity_ble/util.py
+-rw-r--r--   0        0        0     4659 1970-01-01 00:00:00.000000 ac_infinity_ble-0.4.0/PKG-INFO
```

### Comparing `ac_infinity_ble-0.3.0/LICENSE` & `ac_infinity_ble-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.3.0/README.md` & `ac_infinity_ble-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.3.0/pyproject.toml` & `ac_infinity_ble-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ac-infinity-ble"
-version = "0.3.0"
+version = "0.4.0"
 description = "AC Infinity BLE Controller"
 authors = ["Jason Hunter <hunterjm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/hunterjm/ac-infinity-ble"
 documentation = "https://ac-infinity-ble.readthedocs.io"
 classifiers = [
```

### Comparing `ac_infinity_ble-0.3.0/src/ac_infinity_ble/device.py` & `ac_infinity_ble-0.4.0/src/ac_infinity_ble/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,46 +154,55 @@
         await self._send_command([command])
 
         async with async_timeout.timeout(5):
             await events[CallbackType.NOTIFICATION].wait()
             await events[CallbackType.UPDATE_RESPONSE].wait()
         cancel_callback()
 
-    async def turn_on(self) -> None:
+    async def turn_on(self, speed: int | None = None) -> None:
         """Turn on the controller."""
         await self._ensure_connected()
         _LOGGER.debug("%s: Turn on", self.name)
         self._state.work_type = 2
-        self._state.fan = self._state.level_on or 10
-        self._state.level_on = self._state.fan
-        command = self._protocol.set_level(2, self._state.level_on, 0, self.sequence)
+        if speed is not None:
+            self._state.fan = speed
+            self._state.level_on = speed
+        else:
+            self._state.fan = self._state.level_on or 10
+            self._state.level_on = self._state.fan
+
+        command = self._protocol.set_level(
+            self._state.type, 2, self._state.level_on, 0, self.sequence
+        )
         await self._send_command([command])
 
     async def turn_off(self) -> None:
         """Turn off the controller."""
         await self._ensure_connected()
         _LOGGER.debug("%s: Turn off", self.name)
         self._state.work_type = 1
         self._state.fan = self._state.level_off or 0
         self._state.level_off = self._state.fan
-        command = self._protocol.set_level(1, self._state.level_off, 0, self.sequence)
+        command = self._protocol.set_level(
+            self._state.type, 1, self._state.level_off, 0, self.sequence
+        )
         await self._send_command([command])
 
     async def set_speed(self, speed: int) -> None:
         """Set the speed of the controller."""
         await self._ensure_connected()
         _LOGGER.debug("%s: Set speed to %s", self.name, speed)
         self._state.work_type = 2 if speed > 0 else 1
         self.state.fan = speed
         if self._state.work_type == 1:
             self._state.level_off = speed
         else:
             self._state.level_on = speed
         command = self._protocol.set_level(
-            self._state.work_type, speed, 0, self.sequence
+            self._state.type, self._state.work_type, speed, 0, self.sequence
         )
         await self._send_command([command])
 
     async def stop(self) -> None:
         """Stop the controller."""
         _LOGGER.debug("%s: Stop", self.name)
         await self._execute_disconnect()
```

### Comparing `ac_infinity_ble-0.3.0/src/ac_infinity_ble/models.py` & `ac_infinity_ble-0.4.0/src/ac_infinity_ble/models.py`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.3.0/src/ac_infinity_ble/protocol.py` & `ac_infinity_ble-0.4.0/src/ac_infinity_ble/protocol.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,15 +93,19 @@
 
     def get_model_data(self, type: int, b: int, sequence: int) -> bytes:
         command = [16, 17, 18, 19, 20, 21, 22, 23]
         if type in [7, 9, 11, 12]:
             command += [255, b]
         return self._add_head(command, 1, sequence)
 
-    def set_level(self, work_type: int, level: int, b: int, sequence: int) -> bytes:
+    def set_level(
+        self, type: int, work_type: int, level: int, b: int, sequence: int
+    ) -> bytes:
         if work_type not in [1, 2]:
             raise ValueError("Work type must be 1 (off) or 2 (on)")
         if level not in range(0, 11):
             raise ValueError("Level must be between 0 and 10")
-        return self._add_head(
-            [16, 1, work_type, work_type + 16, 1, level, 255, b], 3, sequence
-        )
+
+        command = [16, 1, work_type, work_type + 16, 1, level]
+        if type in [7, 9, 11, 12]:
+            command += [255, b]
+        return self._add_head(command, 3, sequence)
```

### Comparing `ac_infinity_ble-0.3.0/src/ac_infinity_ble/util.py` & `ac_infinity_ble-0.4.0/src/ac_infinity_ble/util.py`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.3.0/PKG-INFO` & `ac_infinity_ble-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ac-infinity-ble
-Version: 0.3.0
+Version: 0.4.0
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
-Metadata-Version: 2.1 Name: ac-infinity-ble Version: 0.3.0 Summary: AC Infinity
+Metadata-Version: 2.1 Name: ac-infinity-ble Version: 0.4.0 Summary: AC Infinity
 BLE Controller Home-page: https://github.com/hunterjm/ac-infinity-ble License:
 MIT Author: Jason Hunter Author-email: hunterjm@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

