# Comparing `tmp/terminal_manager-0.5.0.tar.gz` & `tmp/terminal_manager-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_manager-0.5.0.tar", last modified: Thu Jul 13 09:55:54 2023, max compression
+gzip compressed data, was "terminal_manager-0.6.0.tar", last modified: Sat Jul 15 08:24:50 2023, max compression
```

## Comparing `terminal_manager-0.5.0.tar` & `terminal_manager-0.6.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 09:55:54.545664 terminal_manager-0.5.0/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.5.0/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-13 09:55:54.541665 terminal_manager-0.5.0/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.5.0/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      706 2023-07-13 09:45:59.000000 terminal_manager-0.5.0/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-13 09:55:54.545664 terminal_manager-0.5.0/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 09:55:54.537665 terminal_manager-0.5.0/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 09:55:54.541665 terminal_manager-0.5.0/src/terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     6542 2023-07-13 07:25:37.000000 terminal_manager-0.5.0/src/terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-13 07:22:57.000000 terminal_manager-0.5.0/src/terminal_manager/collection.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5082 2023-07-13 09:29:31.000000 terminal_manager-0.5.0/src/terminal_manager/command.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 09:55:54.541665 terminal_manager-0.5.0/src/terminal_manager/default_collections/
--rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-13 07:22:57.000000 terminal_manager-0.5.0/src/terminal_manager/default_collections/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1084 2023-07-13 07:25:10.000000 terminal_manager-0.5.0/src/terminal_manager/default_collections/const.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     4114 2023-07-13 07:26:17.000000 terminal_manager-0.5.0/src/terminal_manager/default_collections/linux.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5208 2023-07-13 07:28:16.000000 terminal_manager-0.5.0/src/terminal_manager/default_collections/windows_cmd.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     5418 2023-07-13 08:58:44.000000 terminal_manager-0.5.0/src/terminal_manager/default_collections/windows_ps.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-13 07:22:57.000000 terminal_manager-0.5.0/src/terminal_manager/errors.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-13 07:22:57.000000 terminal_manager-0.5.0/src/terminal_manager/event.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-13 07:22:57.000000 terminal_manager-0.5.0/src/terminal_manager/helpers.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8336 2023-07-13 09:29:54.000000 terminal_manager-0.5.0/src/terminal_manager/sensor.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-07-13 07:22:57.000000 terminal_manager-0.5.0/src/terminal_manager/synchronizer.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 09:55:54.541665 terminal_manager-0.5.0/src/terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-13 09:55:54.000000 terminal_manager-0.5.0/src/terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-07-13 09:55:54.000000 terminal_manager-0.5.0/src/terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-13 09:55:54.000000 terminal_manager-0.5.0/src/terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-07-13 09:55:54.000000 terminal_manager-0.5.0/src/terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-07-13 09:55:54.000000 terminal_manager-0.5.0/src/terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-15 08:24:50.356202 terminal_manager-0.6.0/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:30.000000 terminal_manager-0.6.0/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-15 08:24:50.356202 terminal_manager-0.6.0/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      107 2023-07-11 04:42:30.000000 terminal_manager-0.6.0/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      706 2023-07-15 08:17:22.000000 terminal_manager-0.6.0/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-15 08:24:50.356202 terminal_manager-0.6.0/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-15 08:24:50.328201 terminal_manager-0.6.0/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-15 08:24:50.344201 terminal_manager-0.6.0/src/terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     7058 2023-07-14 02:57:27.000000 terminal_manager-0.6.0/src/terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     3352 2023-07-13 07:22:57.000000 terminal_manager-0.6.0/src/terminal_manager/collection.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5805 2023-07-15 07:05:41.000000 terminal_manager-0.6.0/src/terminal_manager/command.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-15 08:24:50.356202 terminal_manager-0.6.0/src/terminal_manager/default_collections/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      161 2023-07-13 07:22:57.000000 terminal_manager-0.6.0/src/terminal_manager/default_collections/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1084 2023-07-13 07:25:10.000000 terminal_manager-0.6.0/src/terminal_manager/default_collections/const.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     4074 2023-07-15 03:35:59.000000 terminal_manager-0.6.0/src/terminal_manager/default_collections/linux.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5206 2023-07-14 05:28:35.000000 terminal_manager-0.6.0/src/terminal_manager/default_collections/windows_cmd.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     5374 2023-07-15 03:36:09.000000 terminal_manager-0.6.0/src/terminal_manager/default_collections/windows_ps.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)       94 2023-07-13 07:22:57.000000 terminal_manager-0.6.0/src/terminal_manager/errors.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      617 2023-07-13 07:22:57.000000 terminal_manager-0.6.0/src/terminal_manager/event.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      222 2023-07-13 07:22:57.000000 terminal_manager-0.6.0/src/terminal_manager/helpers.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8394 2023-07-14 07:44:55.000000 terminal_manager-0.6.0/src/terminal_manager/sensor.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     1248 2023-07-13 07:22:57.000000 terminal_manager-0.6.0/src/terminal_manager/synchronizer.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-15 08:24:50.348202 terminal_manager-0.6.0/src/terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      681 2023-07-15 08:24:50.000000 terminal_manager-0.6.0/src/terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      776 2023-07-15 08:24:50.000000 terminal_manager-0.6.0/src/terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-15 08:24:50.000000 terminal_manager-0.6.0/src/terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       22 2023-07-15 08:24:50.000000 terminal_manager-0.6.0/src/terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       17 2023-07-15 08:24:50.000000 terminal_manager-0.6.0/src/terminal_manager.egg-info/top_level.txt
```

### Comparing `terminal_manager-0.5.0/LICENSE` & `terminal_manager-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.5.0/PKG-INFO` & `terminal_manager-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: terminal_manager
-Version: 0.5.0
+Version: 0.6.0
 Summary: Use terminal commands to control and monitor devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,command line
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Terminal Manager
 
 ## Initialize
```

### Comparing `terminal_manager-0.5.0/pyproject.toml` & `terminal_manager-0.6.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "terminal_manager"
-version = "0.5.0"
+version = "0.6.0"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Use terminal commands to control and monitor devices"
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 classifiers = [
-  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 keywords = [ 
   "terminal", 
   "command line",
 ]
```

### Comparing `terminal_manager-0.5.0/src/terminal_manager/__init__.py` & `terminal_manager-0.6.0/src/terminal_manager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Terminal manager."""
 from __future__ import annotations
 
 import logging
 from collections.abc import Sequence
 from dataclasses import dataclass
+from time import time
 from typing import Any
 
 from .collection import Collection
 from .command import ActionCommand, Command, SensorCommand
 from .default_collections import ActionKey, SensorKey
 from .errors import CommandError
 from .event import Event
@@ -86,14 +87,29 @@
             return sensor.last_known_value
 
     @property
     def wake_on_lan(self) -> bool | None:
         if sensor := self.sensors_by_key.get(SensorKey.WAKE_ON_LAN):
             return sensor.last_known_value
 
+    async def async_update_sensor_commands(self, force: bool = False) -> None:
+        """Update the sensor commands.
+
+        Execute sensor commands that passed their `interval` or
+        all sensor commands with `force=True`.
+
+        """
+        for command in self.sensor_commands:
+            if not (force or command.should_update):
+                return
+            try:
+                await self.async_execute_command(command)
+            except CommandError:
+                pass
+
     async def async_execute_command_string(
         self, string: str, command_timeout: int | None = None
     ) -> CommandOutput:
         """Execute a command string.
 
         Raises:
             CommandError
```

### Comparing `terminal_manager-0.5.0/src/terminal_manager/collection.py` & `terminal_manager-0.6.0/src/terminal_manager/collection.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.5.0/src/terminal_manager/default_collections/const.py` & `terminal_manager-0.6.0/src/terminal_manager/default_collections/const.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.5.0/src/terminal_manager/default_collections/linux.py` & `terminal_manager-0.6.0/src/terminal_manager/default_collections/linux.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,45 +14,45 @@
         ActionCommand(
             "/sbin/shutdown -r now",
             ActionName.RESTART,
             ActionKey.RESTART,
         ),
     ],
     [
+        # TODO: OS_ARCHITECTURE
+        SensorCommand(
+            "/sbin/route -n | awk '/^0.0.0.0/ {print $NF}'",
+            sensors=[
+                TextSensor(
+                    SensorName.NETWORK_INTERFACE,
+                    SensorKey.NETWORK_INTERFACE,
+                )
+            ],
+        ),
         SensorCommand(
-            "cat /sys/class/net/{network_interface}/address",
+            "cat /sys/class/net/@sensor{network_interface}/address",
             sensors=[
                 TextSensor(
                     SensorName.MAC_ADDRESS,
                     SensorKey.MAC_ADDRESS,
                 )
             ],
         ),
         SensorCommand(
-            "file=/sys/class/net/{network_interface}/device/power/wakeup; "
+            "file=/sys/class/net/@sensor{network_interface}/device/power/wakeup; "
             + "[[ ! -f $file ]] || cat $file",
             sensors=[
                 BinarySensor(
                     SensorName.WAKE_ON_LAN,
                     SensorKey.WAKE_ON_LAN,
-                    payload_on="enabled",
                 )
             ],
         ),
         SensorCommand(
-            "/sbin/route -n | awk '/^0.0.0.0/ {{print $NF}}'",
-            sensors=[
-                TextSensor(
-                    SensorName.NETWORK_INTERFACE,
-                    SensorKey.NETWORK_INTERFACE,
-                )
-            ],
-        ),
-        SensorCommand(
-            "uname -a | awk '{{print $1; print $2; print $3; print $(NF-1)}}'",
+            "uname -a | awk '{print $1; print $2; print $3; print $(NF-1)}'",
             sensors=[
                 TextSensor(
                     SensorName.OS_NAME,
                     SensorKey.OS_NAME,
                 ),
                 TextSensor(
                     SensorName.HOSTNAME,
@@ -64,51 +64,50 @@
                 ),
                 TextSensor(
                     SensorName.MACHINE_TYPE,
                     SensorKey.MACHINE_TYPE,
                 ),
             ],
         ),
-        # TODO: OS_ARCHITECTURE
         SensorCommand(
-            "free -k | awk '/^Mem:/ {{print $2}}'",
+            "free -k | awk '/^Mem:/ {print $2}'",
             sensors=[
                 NumberSensor(
                     SensorName.TOTAL_MEMORY,
                     SensorKey.TOTAL_MEMORY,
                     unit="KiB",
                 )
             ],
         ),
         SensorCommand(
-            "free -k | awk '/^Mem:/ {{print $4}}'",
+            "free -k | awk '/^Mem:/ {print $4}'",
             interval=30,
             sensors=[
                 NumberSensor(
                     SensorName.FREE_MEMORY,
                     SensorKey.FREE_MEMORY,
                     unit="KiB",
                 )
             ],
         ),
         SensorCommand(
-            "df -k | awk '/^\\/dev\\// {{print $6 \"|\" $4}}'",
+            "df -k | awk '/^\\/dev\\// {print $6 \"|\" $4}'",
             interval=60,
             sensors=[
                 NumberSensor(
                     SensorName.FREE_DISK_SPACE,
                     SensorKey.FREE_DISK_SPACE,
                     dynamic=True,
                     separator="|",
                     unit="KiB",
                 )
             ],
         ),
         SensorCommand(
-            "top -bn1 | awk 'NR<4 && tolower($0)~/cpu/ {{print 100-$8}}'",
+            "top -bn1 | awk 'NR<4 && tolower($0)~/cpu/ {print 100-$8}'",
             interval=30,
             sensors=[
                 NumberSensor(
                     SensorName.CPU_LOAD,
                     SensorKey.CPU_LOAD,
                     unit="%",
                 )
```

### Comparing `terminal_manager-0.5.0/src/terminal_manager/default_collections/windows_cmd.py` & `terminal_manager-0.6.0/src/terminal_manager/default_collections/windows_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         SensorCommand(
             "for /f %i in ('wmic path win32_ip4routetable "
             + "where \"Destination='0.0.0.0'\" "
             + "get InterfaceIndex ^| "
             + 'findstr /r "\\<[0-9][0-9]*\\>"\') do '
             + '@for /f "skip=2 tokens=2,3 delims=," %j in (\'wmic nic '
             + 'where "InterfaceIndex=%i" '
-            + "get MACAddress^, NetConnectionID /format:csv') do "
+            + "get MACAddress^,NetConnectionID /format:csv') do "
             + "@echo %j & @echo %k",
             sensors=[
                 TextSensor(
                     SensorName.MAC_ADDRESS,
                     SensorKey.MAC_ADDRESS,
                 ),
                 TextSensor(
@@ -109,15 +109,15 @@
                     SensorKey.FREE_MEMORY,
                     unit="kB",
                 ),
             ],
         ),
         SensorCommand(
             'for /f "tokens=1,2" %i in (\'wmic LogicalDisk '
-            + "get DeviceID^, FreeSpace ^| "
+            + "get DeviceID^,FreeSpace ^| "
             + 'findstr ":"\') do '
             + "@echo %i^|%j",
             interval=60,
             sensors=[
                 NumberSensor(
                     SensorName.FREE_DISK_SPACE,
                     SensorKey.FREE_DISK_SPACE,
```

### Comparing `terminal_manager-0.5.0/src/terminal_manager/default_collections/windows_ps.py` & `terminal_manager-0.6.0/src/terminal_manager/default_collections/windows_ps.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,33 +16,32 @@
             ActionName.RESTART,
             ActionKey.RESTART,
         ),
     ],
     [
         SensorCommand(
             "$x = Get-NetAdapterPowerManagement "
-            + '-Name "{network_interface}" | '
+            + '-Name "@sensor{network_interface}" | '
             + "Select WakeOnMagicPacket; "
             + "$x.WakeOnMagicPacket",
             sensors=[
                 BinarySensor(
                     SensorName.WAKE_ON_LAN,
                     SensorKey.WAKE_ON_LAN,
-                    payload_on="Enabled",
                 )
             ],
         ),
         SensorCommand(
             "$y = Get-CimInstance Win32_IP4RouteTable "
             + "-Filter \"Destination='0.0.0.0'\" | "
             + "Select InterfaceIndex; "
             + "$x = Get-CimInstance Win32_NetworkAdapter "
             + "-Property NetConnectionID, InterfaceIndex, MACAddress "
             + '-Filter "InterfaceIndex=$($y.InterfaceIndex)" | '
-            + "Select MACAddress, NetConnectionID; "
+            + "Select MACAddress,NetConnectionID; "
             + "$x.MACAddress; "
             + "$x.NetConnectionID",
             sensors=[
                 TextSensor(
                     SensorName.MAC_ADDRESS,
                     SensorKey.MAC_ADDRESS,
                 ),
@@ -50,15 +49,15 @@
                     SensorName.NETWORK_INTERFACE,
                     SensorKey.NETWORK_INTERFACE,
                 ),
             ],
         ),
         SensorCommand(
             "$x = Get-CimInstance Win32_ComputerSystem | "
-            + "Select Name, SystemType; "
+            + "Select Name,SystemType; "
             + "$x.Name; "
             + "$x.SystemType",
             sensors=[
                 TextSensor(
                     SensorName.HOSTNAME,
                     SensorKey.HOSTNAME,
                 ),
@@ -66,15 +65,15 @@
                     SensorName.MACHINE_TYPE,
                     SensorKey.MACHINE_TYPE,
                 ),
             ],
         ),
         SensorCommand(
             "$x = Get-CimInstance Win32_OperatingSystem | "
-            + "Select Caption, Version, OSArchitecture; "
+            + "Select Caption,Version,OSArchitecture; "
             + "$x.Caption; "
             + "$x.Version; "
             + "$x.OSArchitecture",
             sensors=[
                 TextSensor(
                     SensorName.OS_NAME,
                     SensorKey.OS_NAME,
@@ -112,16 +111,16 @@
                     SensorKey.FREE_MEMORY,
                     unit="kB",
                 )
             ],
         ),
         SensorCommand(
             "Get-CimInstance Win32_LogicalDisk | "
-            + "Select DeviceID, FreeSpace | ForEach-Object "
-            + '{{$_.DeviceID + "|" + $_.FreeSpace}}',
+            + "Select DeviceID,FreeSpace | "
+            + 'ForEach-Object {$_.DeviceID + "|" + $_.FreeSpace}',
             interval=60,
             sensors=[
                 NumberSensor(
                     SensorName.FREE_DISK_SPACE,
                     SensorKey.FREE_DISK_SPACE,
                     dynamic=True,
                     separator="|",
@@ -153,15 +152,15 @@
                     SensorName.TEMPERATURE,
                     SensorKey.TEMPERATURE,
                     unit="°C",
                 )
             ],
         ),
         SensorCommand(
-            "Get-Process | Measure | ForEach-Object {{$_.Count}}",
+            "Get-Process | Measure | ForEach-Object {$_.Count}",
             interval=60,
             sensors=[
                 NumberSensor(
                     SensorName.PROCESSES,
                     SensorKey.PROCESSES,
                 )
             ],
```

### Comparing `terminal_manager-0.5.0/src/terminal_manager/event.py` & `terminal_manager-0.6.0/src/terminal_manager/event.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.5.0/src/terminal_manager/sensor.py` & `terminal_manager-0.6.0/src/terminal_manager/sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,29 +68,31 @@
         return value_string
 
     def _validate(self, value: Any) -> None:
         ...
 
     def _update_value(self, manager: Manager, data: str | None) -> None:
         if data is None:
-            manager.logger.info("%s: %s => %s", manager.name, self.key, self.value)
             self.value = None
+            manager.logger.info(
+                "[%s] Sensor: %s => %s", manager.name, self.key, self.value
+            )
             return
 
         try:
             value_string = self._render(data)
             value = self._convert(value_string)
             self._validate(value)
         except Exception as exc:  # pylint: disable=broad-except
-            manager.logger.info("%s: %s => %s", manager.name, self.key, exc)
             self.value = None
+            manager.logger.info("[%s] Sensor: %s => %s", manager.name, self.key, exc)
             return
 
         self.value = self.last_known_value = value
-        manager.logger.info("%s: %s => %s", manager.name, self.key, self.value)
+        manager.logger.info("[%s] Sensor: %s => %s", manager.name, self.key, self.value)
 
     def _update_child_sensors(self, manager: Manager, data: list[str] | None) -> None:
         if data is None:
             for child in self.child_sensors:
                 child.update(manager, None)
             return
 
@@ -241,15 +243,15 @@
 
         if value_string.lower() in TRUE_STRINGS:
             return True
 
         if value_string.lower() in FALSE_STRINGS:
             return False
 
-        raise ValueError("Can't generate bool from {value_string}")
+        raise ValueError(f"Can't generate bool from {value_string}")
 
     def _validate(self, value: Any) -> None:
         if not isinstance(value, bool):
             raise TypeError(f"{value} is {type(value)} and not {bool}")
 
 
 class DynamicData:
```

### Comparing `terminal_manager-0.5.0/src/terminal_manager/synchronizer.py` & `terminal_manager-0.6.0/src/terminal_manager/synchronizer.py`

 * *Files identical despite different names*

### Comparing `terminal_manager-0.5.0/src/terminal_manager.egg-info/PKG-INFO` & `terminal_manager-0.6.0/src/terminal_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: terminal-manager
-Version: 0.5.0
+Version: 0.6.0
 Summary: Use terminal commands to control and monitor devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/terminal-manager/issues
 Keywords: terminal,command line
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Terminal Manager
 
 ## Initialize
```

### Comparing `terminal_manager-0.5.0/src/terminal_manager.egg-info/SOURCES.txt` & `terminal_manager-0.6.0/src/terminal_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

