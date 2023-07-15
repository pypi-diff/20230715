# Comparing `tmp/ac_infinity_ble-0.4.1.tar.gz` & `tmp/ac_infinity_ble-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ac_infinity_ble-0.4.1.tar", max compression
+gzip compressed data, was "ac_infinity_ble-0.4.2.tar", max compression
```

## Comparing `ac_infinity_ble-0.4.1.tar` & `ac_infinity_ble-0.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-07-14 23:26:48.157786 ac_infinity_ble-0.4.1/LICENSE
--rw-r--r--   0        0        0     3538 2023-07-14 23:26:48.157786 ac_infinity_ble-0.4.1/README.md
--rw-r--r--   0        0        0     2182 2023-07-14 23:26:48.897791 ac_infinity_ble-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      322 2023-07-14 23:26:48.869791 ac_infinity_ble-0.4.1/src/ac_infinity_ble/__init__.py
--rw-r--r--   0        0        0      405 2023-07-14 23:26:48.157786 ac_infinity_ble-0.4.1/src/ac_infinity_ble/const.py
--rw-r--r--   0        0        0    16366 2023-07-14 23:26:48.157786 ac_infinity_ble-0.4.1/src/ac_infinity_ble/device.py
--rw-r--r--   0        0        0       96 2023-07-14 23:26:48.157786 ac_infinity_ble-0.4.1/src/ac_infinity_ble/exceptions.py
--rw-r--r--   0        0        0      591 2023-07-14 23:26:48.157786 ac_infinity_ble-0.4.1/src/ac_infinity_ble/models.py
--rw-r--r--   0        0        0     3239 2023-07-14 23:26:48.157786 ac_infinity_ble-0.4.1/src/ac_infinity_ble/protocol.py
--rw-r--r--   0        0        0        0 2023-07-14 23:26:48.157786 ac_infinity_ble-0.4.1/src/ac_infinity_ble/py.typed
--rw-r--r--   0        0        0      756 2023-07-14 23:26:48.157786 ac_infinity_ble-0.4.1/src/ac_infinity_ble/util.py
--rw-r--r--   0        0        0     4659 1970-01-01 00:00:00.000000 ac_infinity_ble-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-15 20:04:57.989342 ac_infinity_ble-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3538 2023-07-15 20:04:57.989342 ac_infinity_ble-0.4.2/README.md
+-rw-r--r--   0        0        0     2182 2023-07-15 20:04:58.825353 ac_infinity_ble-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      322 2023-07-15 20:04:58.797352 ac_infinity_ble-0.4.2/src/ac_infinity_ble/__init__.py
+-rw-r--r--   0        0        0      427 2023-07-15 20:04:57.989342 ac_infinity_ble-0.4.2/src/ac_infinity_ble/const.py
+-rw-r--r--   0        0        0    16307 2023-07-15 20:04:57.989342 ac_infinity_ble-0.4.2/src/ac_infinity_ble/device.py
+-rw-r--r--   0        0        0       96 2023-07-15 20:04:57.989342 ac_infinity_ble-0.4.2/src/ac_infinity_ble/exceptions.py
+-rw-r--r--   0        0        0      591 2023-07-15 20:04:57.989342 ac_infinity_ble-0.4.2/src/ac_infinity_ble/models.py
+-rw-r--r--   0        0        0     3239 2023-07-15 20:04:57.989342 ac_infinity_ble-0.4.2/src/ac_infinity_ble/protocol.py
+-rw-r--r--   0        0        0        0 2023-07-15 20:04:57.989342 ac_infinity_ble-0.4.2/src/ac_infinity_ble/py.typed
+-rw-r--r--   0        0        0      756 2023-07-15 20:04:57.989342 ac_infinity_ble-0.4.2/src/ac_infinity_ble/util.py
+-rw-r--r--   0        0        0     4659 1970-01-01 00:00:00.000000 ac_infinity_ble-0.4.2/PKG-INFO
```

### Comparing `ac_infinity_ble-0.4.1/LICENSE` & `ac_infinity_ble-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.4.1/README.md` & `ac_infinity_ble-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.4.1/pyproject.toml` & `ac_infinity_ble-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ac-infinity-ble"
-version = "0.4.1"
+version = "0.4.2"
 description = "AC Infinity BLE Controller"
 authors = ["Jason Hunter <hunterjm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/hunterjm/ac-infinity-ble"
 documentation = "https://ac-infinity-ble.readthedocs.io"
 classifiers = [
```

### Comparing `ac_infinity_ble-0.4.1/src/ac_infinity_ble/device.py` & `ac_infinity_ble-0.4.2/src/ac_infinity_ble/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         self._write_char: BleakGATTCharacteristic | None = None
         self._disconnect_timer: asyncio.TimerHandle | None = None
         self._client: BleakClientWithServiceCache | None = None
         self._protocol: Protocol = Protocol()
         self._expected_disconnect = False
         self.loop = asyncio.get_running_loop()
         self._callbacks: list[Callable[[DeviceInfo, CallbackType], None]] = []
+        self._notify_future: asyncio.Future[bytearray] | None = None
         self._sequence = 1
 
     def set_ble_device_and_advertisement_data(
         self, ble_device: BLEDevice, advertisement_data: AdvertisementData
     ) -> None:
         """Set the ble device."""
         self._ble_device = ble_device
@@ -78,14 +79,15 @@
             self._state, **{k: v for k, v in asdict(info).items() if v is not None}
         )
         if self._state.fan:
             if self._state.level_off or 0 > self._state.fan:
                 self._state.level_off = self._state.fan
             if self._state.level_on or 10 < self._state.fan:
                 self._state.level_on = self._state.fan
+        self._fire_callbacks(CallbackType.ADVERTISEMENT)
 
     @property
     def address(self) -> str:
         """Return the address."""
         return self._ble_device.address
 
     @property
@@ -136,33 +138,27 @@
         if self._sequence == 65535:
             self._sequence = 0
         self._sequence += 1
         return self._sequence
 
     async def update(self) -> None:
         """Update the controller."""
-        events = {
-            CallbackType.NOTIFICATION: asyncio.Event(),
-            CallbackType.UPDATE_RESPONSE: asyncio.Event(),
-        }
-
-        def on_event(_: DeviceInfo, type: CallbackType) -> None:
-            events[type].set()
-
-        cancel_callback = self.register_callback(on_event)
-
         await self._ensure_connected()
         _LOGGER.debug("%s: Updating", self.name)
         command = self._protocol.get_model_data(self._state.type, 0, self.sequence)
-        await self._send_command([command])
-
-        async with async_timeout.timeout(5):
-            await events[CallbackType.NOTIFICATION].wait()
-            await events[CallbackType.UPDATE_RESPONSE].wait()
-        cancel_callback()
+        if data := await self._send_command(command):
+            self._state.work_type = data[12]
+            self._state.level_off = data[15]
+            self._state.level_on = data[18]
+            if self._state.work_type == 1:
+                self._state.fan = self._state.level_off
+            if self._state.work_type == 2:
+                self._state.fan = self._state.level_on
+            self._fire_callbacks(CallbackType.UPDATE_RESPONSE)
+        await self._execute_disconnect()
 
     async def turn_on(self, speed: int | None = None) -> None:
         """Turn on the controller."""
         await self._ensure_connected()
         _LOGGER.debug("%s: Turn on", self.name)
         self._state.work_type = 2
         if speed is not None:
@@ -171,42 +167,45 @@
         else:
             self._state.fan = self._state.level_on or 10
             self._state.level_on = self._state.fan
 
         command = self._protocol.set_level(
             self._state.type, 2, self._state.level_on, 0, self.sequence
         )
-        await self._send_command([command])
+        await self._send_command(command)
+        await self._execute_disconnect()
 
     async def turn_off(self) -> None:
         """Turn off the controller."""
         await self._ensure_connected()
         _LOGGER.debug("%s: Turn off", self.name)
         self._state.work_type = 1
         self._state.fan = self._state.level_off or 0
         self._state.level_off = self._state.fan
         command = self._protocol.set_level(
             self._state.type, 1, self._state.level_off, 0, self.sequence
         )
-        await self._send_command([command])
+        await self._send_command(command)
+        await self._execute_disconnect()
 
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
             self._state.type, self._state.work_type, speed, 0, self.sequence
         )
-        await self._send_command([command])
+        await self._send_command(command)
+        await self._execute_disconnect()
 
     async def stop(self) -> None:
         """Stop the controller."""
         _LOGGER.debug("%s: Stop", self.name)
         await self._execute_disconnect()
 
     def _fire_callbacks(self, type: CallbackType) -> None:
@@ -263,14 +262,17 @@
                 "%s: Subscribe to notifications; RSSI: %s", self.name, self.rssi
             )
             await client.start_notify(self._read_char, self._notification_handler)
 
     def _notification_handler(self, _sender: int, data: bytearray) -> None:
         """Handle notification responses."""
         _LOGGER.debug("%s: Notification received: %s", self.name, data.hex())
+        if self._notify_future and not self._notify_future.done():
+            self._notify_future.set_result(data)
+            return
 
         if data[0] == 0x1E and data[1] == 0xFF:
             self._state.is_degree = get_bit(data[6], 0)
             self._state.tmp_state = get_bits(data[6], 1, 2)
             self._state.hum_state = get_bits(data[6], 3, 2)
             self._state.vpd_state = get_bits(data[6], 5, 2)
             self._state.choose_port = get_bits(data[7], 4, 4)
@@ -279,24 +281,14 @@
             self._state.vpd = get_short(data, 12) / 100
             self._state.fan_type = get_short(data, 14)
             self._state.fan_state = get_bits(data[16], 0, 2)
             # self._state.fan = get_bits(data[17], 0, 4) # Not accurate
             self._state.work_type = get_bits(data[17], 4, 4)
             self._fire_callbacks(CallbackType.NOTIFICATION)
 
-        if data[0] == 0xA5 and data[1] == 0x17 and len(data) == 63:
-            self._state.work_type = data[12]
-            self._state.level_off = data[15]
-            self._state.level_on = data[18]
-            if self._state.work_type == 1:
-                self._state.fan = self._state.level_off
-            if self._state.work_type == 2:
-                self._state.fan = self._state.level_on
-            self._fire_callbacks(CallbackType.UPDATE_RESPONSE)
-
     def _reset_disconnect_timer(self) -> None:
         """Reset disconnect timer."""
         if self._disconnect_timer:
             self._disconnect_timer.cancel()
         self._expected_disconnect = False
         self._disconnect_timer = self.loop.call_later(
             DISCONNECT_DELAY, self._disconnect
@@ -339,18 +331,18 @@
             self._read_char = None
             self._write_char = None
             if client and client.is_connected:
                 await client.stop_notify(read_char)
                 await client.disconnect()
 
     @retry_bluetooth_connection_error(DEFAULT_ATTEMPTS)
-    async def _send_command_locked(self, commands: list[bytes]) -> None:
+    async def _send_command_locked(self, command: bytes) -> bytes | None:
         """Send command to device and read response."""
         try:
-            await self._execute_command_locked(commands)
+            return await self._execute_command_locked(command)
         except BleakDBusError as ex:
             # Disconnect so we can reset state and try again
             await asyncio.sleep(BLEAK_BACKOFF_TIME)
             _LOGGER.debug(
                 "%s: RSSI: %s; Backing off %ss; Disconnecting due to error: %s",
                 self.name,
                 self.rssi,
@@ -364,41 +356,38 @@
             _LOGGER.debug(
                 "%s: RSSI: %s; Disconnecting due to error: %s", self.name, self.rssi, ex
             )
             await self._execute_disconnect()
             raise
 
     async def _send_command(
-        self, commands: list[bytes] | bytes, retry: int | None = None
-    ) -> None:
+        self, command: bytes, retry: int | None = None
+    ) -> bytes | None:
         """Send command to device and read response."""
         await self._ensure_connected()
-        if not isinstance(commands, list):
-            commands = [commands]
-        await self._send_command_while_connected(commands, retry)
+        return await self._send_command_while_connected(command, retry)
 
     async def _send_command_while_connected(
-        self, commands: list[bytes], retry: int | None = None
-    ) -> None:
+        self, command: bytes, retry: int | None = None
+    ) -> bytes | None:
         """Send command to device and read response."""
         _LOGGER.debug(
-            "%s: Sending commands %s",
+            "%s: Sending command %s",
             self.name,
-            [command.hex() for command in commands],
+            command.hex(),
         )
         if self._operation_lock.locked():
             _LOGGER.debug(
                 "%s: Operation already in progress, waiting; RSSI: %s",
                 self.name,
                 self.rssi,
             )
         async with self._operation_lock:
             try:
-                await self._send_command_locked(commands)
-                return
+                return await self._send_command_locked(command)
             except BleakNotFoundError:
                 _LOGGER.error(
                     "%s: device not found, no longer in range, or poor RSSI: %s",
                     self.name,
                     self.rssi,
                     exc_info=True,
                 )
@@ -414,23 +403,31 @@
                 raise
             except BLEAK_EXCEPTIONS:
                 _LOGGER.debug("%s: communication failed", self.name, exc_info=True)
                 raise
 
         raise RuntimeError("Unreachable")
 
-    async def _execute_command_locked(self, commands: list[bytes]) -> None:
+    async def _execute_command_locked(self, command: bytes) -> bytes:
         """Execute command and read response."""
         assert self._client is not None  # nosec
         if not self._read_char:
             raise CharacteristicMissingError("Read characteristic missing")
         if not self._write_char:
             raise CharacteristicMissingError("Write characteristic missing")
-        for command in commands:
-            await self._client.write_gatt_char(self._write_char, command, False)
+
+        self._notify_future = asyncio.Future()
+        await self._client.write_gatt_char(self._write_char, command, False)
+
+        notify_msg = None
+        async with async_timeout.timeout(5):
+            notify_msg = await self._notify_future
+
+        self._notify_future = None
+        return notify_msg
 
     def _resolve_characteristics(self, services: BleakGATTServiceCollection) -> bool:
         """Resolve characteristics."""
         for characteristic in POSSIBLE_READ_CHARACTERISTIC_UUIDS:
             if char := services.get_characteristic(characteristic):
                 self._read_char = char
                 break
```

### Comparing `ac_infinity_ble-0.4.1/src/ac_infinity_ble/models.py` & `ac_infinity_ble-0.4.2/src/ac_infinity_ble/models.py`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.4.1/src/ac_infinity_ble/protocol.py` & `ac_infinity_ble-0.4.2/src/ac_infinity_ble/protocol.py`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.4.1/src/ac_infinity_ble/util.py` & `ac_infinity_ble-0.4.2/src/ac_infinity_ble/util.py`

 * *Files identical despite different names*

### Comparing `ac_infinity_ble-0.4.1/PKG-INFO` & `ac_infinity_ble-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ac-infinity-ble
-Version: 0.4.1
+Version: 0.4.2
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
-Metadata-Version: 2.1 Name: ac-infinity-ble Version: 0.4.1 Summary: AC Infinity
+Metadata-Version: 2.1 Name: ac-infinity-ble Version: 0.4.2 Summary: AC Infinity
 BLE Controller Home-page: https://github.com/hunterjm/ac-infinity-ble License:
 MIT Author: Jason Hunter Author-email: hunterjm@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

