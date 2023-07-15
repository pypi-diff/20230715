# Comparing `tmp/huawei-solar-2.2.8b1.tar.gz` & `tmp/huawei-solar-2.2.8b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huawei-solar-2.2.8b1.tar", last modified: Mon Jul 10 13:26:01 2023, max compression
+gzip compressed data, was "huawei-solar-2.2.8b2.tar", last modified: Sat Jul 15 07:18:32 2023, max compression
```

## Comparing `huawei-solar-2.2.8b1.tar` & `huawei-solar-2.2.8b2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:26:01.566200 huawei-solar-2.2.8b1/
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/.codecov.yml
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1326 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/.yamllint
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     7719 2023-07-10 13:26:01.566200 huawei-solar-2.2.8b1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7163 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1002 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/bridge_tst.py
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/requirements_test.txt
--rw-rw-rw-   0 root         (0) root         (0)      936 2023-07-10 13:26:01.567200 huawei-solar-2.2.8b1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:26:01.559200 huawei-solar-2.2.8b1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:26:01.564200 huawei-solar-2.2.8b1/src/huawei_solar/
--rw-rw-rw-   0 root         (0) root         (0)      737 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18705 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/bridge.py
--rw-rw-rw-   0 root         (0) root         (0)     1764 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    11325 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/files.py
--rw-rw-rw-   0 root         (0) root         (0)    25023 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/huawei_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     6983 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/modbus.py
--rw-rw-rw-   0 root         (0) root         (0)    18080 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/register_names.py
--rw-rw-rw-   0 root         (0) root         (0)    22487 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/register_values.py
--rw-rw-rw-   0 root         (0) root         (0)    42677 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/registers.py
--rw-rw-rw-   0 root         (0) root         (0)      194 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/src/huawei_solar/utils.py
--rw-r--r--   0 root         (0) root         (0)      148 2023-07-10 13:26:01.000000 huawei-solar-2.2.8b1/src/huawei_solar/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:26:01.565200 huawei-solar-2.2.8b1/src/huawei_solar.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7719 2023-07-10 13:26:01.000000 huawei-solar-2.2.8b1/src/huawei_solar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      891 2023-07-10 13:26:01.000000 huawei-solar-2.2.8b1/src/huawei_solar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 13:26:01.000000 huawei-solar-2.2.8b1/src/huawei_solar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-07-10 13:26:01.000000 huawei-solar-2.2.8b1/src/huawei_solar.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-10 13:26:01.000000 huawei-solar-2.2.8b1/src/huawei_solar.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     3578 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 13:26:01.566200 huawei-solar-2.2.8b1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2611 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/tests/mock_huawei_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     3531 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/tests/test__registers__peak_periods.py
--rw-rw-rw-   0 root         (0) root         (0)     6245 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/tests/test__registers__time_of_use.py
--rw-rw-rw-   0 root         (0) root         (0)    16324 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/tests/test_huawei_solar.py
--rw-rw-rw-   0 root         (0) root         (0)      945 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/tests/test_registers.py
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-07-10 13:25:47.000000 huawei-solar-2.2.8b1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:18:32.480639 huawei-solar-2.2.8b2/
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/.codecov.yml
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/.yamllint
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     7719 2023-07-15 07:18:32.480639 huawei-solar-2.2.8b2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7163 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/bridge_tst.py
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/requirements_test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      936 2023-07-15 07:18:32.481639 huawei-solar-2.2.8b2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:18:32.472639 huawei-solar-2.2.8b2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:18:32.478639 huawei-solar-2.2.8b2/src/huawei_solar/
+-rw-rw-rw-   0 root         (0) root         (0)      737 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/src/huawei_solar/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18975 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/src/huawei_solar/bridge.py
+-rw-rw-rw-   0 root         (0) root         (0)     1764 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/src/huawei_solar/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    11325 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/src/huawei_solar/files.py
+-rw-rw-rw-   0 root         (0) root         (0)    25435 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/src/huawei_solar/huawei_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     6983 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/src/huawei_solar/modbus.py
+-rw-rw-rw-   0 root         (0) root         (0)    18080 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/src/huawei_solar/register_names.py
+-rw-rw-rw-   0 root         (0) root         (0)    22487 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/src/huawei_solar/register_values.py
+-rw-rw-rw-   0 root         (0) root         (0)    42677 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/src/huawei_solar/registers.py
+-rw-rw-rw-   0 root         (0) root         (0)      194 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/src/huawei_solar/utils.py
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-15 07:18:32.000000 huawei-solar-2.2.8b2/src/huawei_solar/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:18:32.479639 huawei-solar-2.2.8b2/src/huawei_solar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7719 2023-07-15 07:18:32.000000 huawei-solar-2.2.8b2/src/huawei_solar.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      891 2023-07-15 07:18:32.000000 huawei-solar-2.2.8b2/src/huawei_solar.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 07:18:32.000000 huawei-solar-2.2.8b2/src/huawei_solar.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-07-15 07:18:32.000000 huawei-solar-2.2.8b2/src/huawei_solar.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-15 07:18:32.000000 huawei-solar-2.2.8b2/src/huawei_solar.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3578 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:18:32.480639 huawei-solar-2.2.8b2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2611 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/tests/mock_huawei_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     3531 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/tests/test__registers__peak_periods.py
+-rw-rw-rw-   0 root         (0) root         (0)     6245 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/tests/test__registers__time_of_use.py
+-rw-rw-rw-   0 root         (0) root         (0)    16324 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/tests/test_huawei_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)      945 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/tests/test_registers.py
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-07-15 07:18:18.000000 huawei-solar-2.2.8b2/tox.ini
```

### Comparing `huawei-solar-2.2.8b1/.gitignore` & `huawei-solar-2.2.8b2/.gitignore`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/.gitlab-ci.yml` & `huawei-solar-2.2.8b2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/.pre-commit-config.yaml` & `huawei-solar-2.2.8b2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/LICENSE.md` & `huawei-solar-2.2.8b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/PKG-INFO` & `huawei-solar-2.2.8b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huawei-solar
-Version: 2.2.8b1
+Version: 2.2.8b2
 Summary: A Python wrapper for the Huawei Inverter modbus TCP API
 Home-page: https://gitlab.com/EmilV2/huawei-solar
 Author: Emil Vanherp
 Author-email: emil@vanherp.me
 License: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `huawei-solar-2.2.8b1/README.md` & `huawei-solar-2.2.8b2/README.md`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/bridge_tst.py` & `huawei-solar-2.2.8b2/bridge_tst.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/pyproject.toml` & `huawei-solar-2.2.8b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/setup.cfg` & `huawei-solar-2.2.8b2/setup.cfg`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/src/huawei_solar/__init__.py` & `huawei-solar-2.2.8b2/src/huawei_solar/__init__.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/src/huawei_solar/bridge.py` & `huawei-solar-2.2.8b2/src/huawei_solar/bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,14 +209,17 @@
 
         result = {}
         async with self.update_lock:
             if self.battery_type != rv.StorageProductModel.NONE:
                 result.update(await self._get_multiple_to_dict(ENERGY_STORAGE_CONFIGURATION_PARAMETERS_1))
                 result.update(await self._get_multiple_to_dict(ENERGY_STORAGE_CONFIGURATION_PARAMETERS_2))
                 result.update(await self._get_multiple_to_dict(ENERGY_STORAGE_CONFIGURATION_PARAMETERS_3))
+
+                # We have no way of knowing if a backup box is installed, so always fetch these registers
+                result.update(await self._get_multiple_to_dict(BACKUP_POWER_REGISTERS))
             if self.supports_capacity_control:
                 result.update(await self._get_multiple_to_dict(CAPACITY_CONTROL_REGISTERS))
         return result
 
     async def _read_file(self, file_type, customized_data=None) -> bytes:
         """
         Wraps `get_file` from `AsyncHuaweiSolar` in a retry-logic for when
@@ -485,7 +488,11 @@
 ]
 
 CAPACITY_CONTROL_REGISTERS = [
     rn.STORAGE_CAPACITY_CONTROL_MODE,
     rn.STORAGE_CAPACITY_CONTROL_SOC_PEAK_SHAVING,
     rn.STORAGE_CAPACITY_CONTROL_PERIODS,
 ]
+
+BACKUP_POWER_REGISTERS = [
+    rn.STORAGE_BACKUP_POWER_STATE_OF_CHARGE,
+]
```

### Comparing `huawei-solar-2.2.8b1/src/huawei_solar/exceptions.py` & `huawei-solar-2.2.8b2/src/huawei_solar/exceptions.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/src/huawei_solar/files.py` & `huawei-solar-2.2.8b2/src/huawei_solar/files.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/src/huawei_solar/huawei_solar.py` & `huawei-solar-2.2.8b2/src/huawei_solar/huawei_solar.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,16 @@
 
     return hmac.digest(key=hashed_password, msg=seed, digest=sha256)
 
 
 class AsyncHuaweiSolar:
     """Async interface to the Huawei solar inverter"""
 
+    _reconnect_task: asyncio.Task | None = None
+
     def __init__(
         self,
         client: t.Union[AsyncHuaweiSolarModbusSerialClient, AsyncHuaweiSolarModbusTcpClient],
         slave: int = DEFAULT_SLAVE,
         timeout: int = DEFAULT_TIMEOUT,
         cooldown_time: float = DEFAULT_COOLDOWN_TIME,
     ):
@@ -130,15 +132,21 @@
                 raise rerr
 
     @asynccontextmanager
     async def _communication_lock(self):
         async with self.__communication_lock:
             if not self._client.connected_event.is_set():
                 LOGGER.info("Waiting for connection ...")
-            await asyncio.wait_for(self._client.connected_event.wait(), WAIT_FOR_CONNECTION_TIMEOUT)
+
+            try:
+                await asyncio.wait_for(self._client.connected_event.wait(), WAIT_FOR_CONNECTION_TIMEOUT)
+            except asyncio.TimeoutError as err:
+                LOGGER.exception("Timeout while waiting for connection. Reconnecting...")
+                self._reconnect_task = asyncio.create_task(self._reconnect())
+                raise err
 
             await self.__cooled_down.wait()
             self.__cooled_down.clear()
 
             try:
                 yield
             finally:
@@ -206,14 +214,17 @@
             # if an error occurs, we need to make sure that the Modbus-client is stopped,
             # otherwise it can stay active and cause even more problems ...
             LOGGER.exception("Aborting client creation due to error.")
             raise ConnectionException from err
 
     async def stop(self):
         """Stop the modbus client."""
+        if self._reconnect_task:
+            self._reconnect_task.cancel()
+
         self._client.close()
 
     async def _reconnect(self):
         """Reconnect to the inverter"""
         self._client.close()
         await self._client.connect()
 
@@ -293,15 +304,15 @@
                 sys.exc_info()[0],
                 details["wait"],
                 details["tries"],
             )
 
         def on_backoff_with_reconnect(details):
             if details["tries"] % 3 == 0:
-                asyncio.create_task(self._reconnect())
+                self._reconnect_task = asyncio.create_task(self._reconnect())
                 LOGGER.debug(
                     "Received %s: reconnecting and backing off reading for %0.1f seconds after %d tries",
                     sys.exc_info()[0],
                     details["wait"],
                     details["tries"],
                 )
             else:
@@ -313,23 +324,23 @@
                 )
 
         def backoff_giveup(details):
             raise ReadException(f"Failed to read register {register} after {details['tries']} tries")
 
         @backoff.on_exception(
             backoff.expo,
-            (asyncio.TimeoutError),
+            (asyncio.TimeoutError, ConnectionInterruptedException),
             max_tries=6,
             jitter=None,
             on_backoff=on_backoff_with_reconnect,
             on_giveup=backoff_giveup,
         )
         @backoff.on_exception(
             backoff.expo,
-            (SlaveBusyException, SlaveFailureException, ConnectionInterruptedException),
+            (SlaveBusyException, SlaveFailureException),
             max_tries=6,
             jitter=None,
             on_backoff=on_backoff,
             on_giveup=backoff_giveup,
         )
         async def _do_read():
             if not self._client.connected:
```

### Comparing `huawei-solar-2.2.8b1/src/huawei_solar/modbus.py` & `huawei-solar-2.2.8b2/src/huawei_solar/modbus.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/src/huawei_solar/register_names.py` & `huawei-solar-2.2.8b2/src/huawei_solar/register_names.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/src/huawei_solar/register_values.py` & `huawei-solar-2.2.8b2/src/huawei_solar/register_values.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/src/huawei_solar/registers.py` & `huawei-solar-2.2.8b2/src/huawei_solar/registers.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/src/huawei_solar.egg-info/PKG-INFO` & `huawei-solar-2.2.8b2/src/huawei_solar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huawei-solar
-Version: 2.2.8b1
+Version: 2.2.8b2
 Summary: A Python wrapper for the Huawei Inverter modbus TCP API
 Home-page: https://gitlab.com/EmilV2/huawei-solar
 Author: Emil Vanherp
 Author-email: emil@vanherp.me
 License: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `huawei-solar-2.2.8b1/src/huawei_solar.egg-info/SOURCES.txt` & `huawei-solar-2.2.8b2/src/huawei_solar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/test.py` & `huawei-solar-2.2.8b2/test.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/tests/conftest.py` & `huawei-solar-2.2.8b2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/tests/mock_huawei_solar.py` & `huawei-solar-2.2.8b2/tests/mock_huawei_solar.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/tests/test__registers__peak_periods.py` & `huawei-solar-2.2.8b2/tests/test__registers__peak_periods.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/tests/test__registers__time_of_use.py` & `huawei-solar-2.2.8b2/tests/test__registers__time_of_use.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/tests/test_huawei_solar.py` & `huawei-solar-2.2.8b2/tests/test_huawei_solar.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/tests/test_registers.py` & `huawei-solar-2.2.8b2/tests/test_registers.py`

 * *Files identical despite different names*

### Comparing `huawei-solar-2.2.8b1/tox.ini` & `huawei-solar-2.2.8b2/tox.ini`

 * *Files identical despite different names*

