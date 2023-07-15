# Comparing `tmp/ssh_terminal_manager-0.5.0.tar.gz` & `tmp/ssh_terminal_manager-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh_terminal_manager-0.5.0.tar", last modified: Thu Jul 13 09:58:08 2023, max compression
+gzip compressed data, was "ssh_terminal_manager-0.6.0.tar", last modified: Sat Jul 15 08:27:42 2023, max compression
```

## Comparing `ssh_terminal_manager-0.5.0.tar` & `ssh_terminal_manager-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 09:58:08.174756 ssh_terminal_manager-0.5.0/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.5.0/LICENSE
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-13 09:58:08.170756 ssh_terminal_manager-0.5.0/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.5.0/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      802 2023-07-13 09:53:35.000000 ssh_terminal_manager-0.5.0/pyproject.toml
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-13 09:58:08.174756 ssh_terminal_manager-0.5.0/setup.cfg
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 09:58:08.166756 ssh_terminal_manager-0.5.0/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 09:58:08.170756 ssh_terminal_manager-0.5.0/src/ssh_terminal_manager/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     8398 2023-07-13 09:29:07.000000 ssh_terminal_manager-0.5.0/src/ssh_terminal_manager/__init__.py
--rw-r--r--   0 adrian    (1000) adrian    (1000)      383 2023-07-13 07:22:57.000000 ssh_terminal_manager-0.5.0/src/ssh_terminal_manager/errors.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-13 09:58:08.170756 ssh_terminal_manager-0.5.0/src/ssh_terminal_manager.egg-info/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-13 09:58:08.000000 ssh_terminal_manager-0.5.0/src/ssh_terminal_manager.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      343 2023-07-13 09:58:08.000000 ssh_terminal_manager-0.5.0/src/ssh_terminal_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-13 09:58:08.000000 ssh_terminal_manager-0.5.0/src/ssh_terminal_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       70 2023-07-13 09:58:08.000000 ssh_terminal_manager-0.5.0/src/ssh_terminal_manager.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-07-13 09:58:08.000000 ssh_terminal_manager-0.5.0/src/ssh_terminal_manager.egg-info/top_level.txt
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-15 08:27:42.525275 ssh_terminal_manager-0.6.0/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)     1063 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.6.0/LICENSE
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-15 08:27:42.525275 ssh_terminal_manager-0.6.0/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      223 2023-07-11 04:42:39.000000 ssh_terminal_manager-0.6.0/README.md
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      802 2023-07-15 08:16:29.000000 ssh_terminal_manager-0.6.0/pyproject.toml
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2023-07-15 08:27:42.525275 ssh_terminal_manager-0.6.0/setup.cfg
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-15 08:27:42.521275 ssh_terminal_manager-0.6.0/src/
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-15 08:27:42.521275 ssh_terminal_manager-0.6.0/src/ssh_terminal_manager/
+-rw-r--r--   0 adrian    (1000) adrian    (1000)     8370 2023-07-14 05:16:44.000000 ssh_terminal_manager-0.6.0/src/ssh_terminal_manager/__init__.py
+-rw-r--r--   0 adrian    (1000) adrian    (1000)      393 2023-07-14 04:14:01.000000 ssh_terminal_manager-0.6.0/src/ssh_terminal_manager/errors.py
+drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2023-07-15 08:27:42.525275 ssh_terminal_manager-0.6.0/src/ssh_terminal_manager.egg-info/
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      820 2023-07-15 08:27:42.000000 ssh_terminal_manager-0.6.0/src/ssh_terminal_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)      343 2023-07-15 08:27:42.000000 ssh_terminal_manager-0.6.0/src/ssh_terminal_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2023-07-15 08:27:42.000000 ssh_terminal_manager-0.6.0/src/ssh_terminal_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       70 2023-07-15 08:27:42.000000 ssh_terminal_manager-0.6.0/src/ssh_terminal_manager.egg-info/requires.txt
+-rw-rw-r--   0 adrian    (1000) adrian    (1000)       21 2023-07-15 08:27:42.000000 ssh_terminal_manager-0.6.0/src/ssh_terminal_manager.egg-info/top_level.txt
```

### Comparing `ssh_terminal_manager-0.5.0/LICENSE` & `ssh_terminal_manager-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ssh_terminal_manager-0.5.0/PKG-INFO` & `ssh_terminal_manager-0.6.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ssh_terminal_manager
-Version: 0.5.0
+Version: 0.6.0
 Summary: Use terminal commands to control and monitor remote devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
 Keywords: ssh,terminal,command line
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SSH Terminal Manager
 
 ## Initialize
```

### Comparing `ssh_terminal_manager-0.5.0/pyproject.toml` & `ssh_terminal_manager-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ssh_terminal_manager"
-version = "0.5.0"
+version = "0.6.0"
 authors = [
   { name="zhbjsh", email="zhbjsh@outlook.com" },
 ]
 description = "Use terminal commands to control and monitor remote devices"
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
   "ssh", 
   "terminal", 
   "command line",
 ]
 dependencies = [
   "icmplib >= 3.0",
   "paramiko >= 3.2.0",
-  "terminal-manager >= 0.5.0",
+  "terminal-manager >= 0.6.0",
   "wakeonlan >= 3.0.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/zhbjsh/ssh-terminal-manager"
 "Bug Tracker" = "https://github.com/zhbjsh/ssh-terminal-manager/issues"
```

### Comparing `ssh_terminal_manager-0.5.0/src/ssh_terminal_manager/__init__.py` & `ssh_terminal_manager-0.6.0/src/ssh_terminal_manager/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,20 @@
     Sensor,
     SensorCommand,
     TextSensor,
     default_collections,
 )
 from terminal_manager.default_collections import ActionKey, SensorKey
 
-from .errors import OfflineError, SSHAuthError, SSHConnectError, SSHHostKeyUnknownError
+from .errors import (
+    OfflineError,
+    SSHAuthenticationError,
+    SSHConnectError,
+    SSHHostKeyUnknownError,
+)
 
 _LOGGER = logging.getLogger(__name__)
 _TEST_COMMAND = Command("echo ''")
 
 ONLINE = "online"
 CONNECTED = "connected"
 
@@ -41,15 +46,15 @@
 DEFAULT_ADD_HOST_KEYS = False
 
 
 class CustomRejectPolicy(paramiko.MissingHostKeyPolicy):
     def missing_host_key(
         self, client: paramiko.SSHClient, hostname: str, key: paramiko.PKey
     ) -> None:
-        raise SSHHostKeyUnknownError("Host key is unknown")
+        raise SSHHostKeyUnknownError(f"SSH host key of {hostname} is unknown")
 
 
 class State:
     online: bool = False
     connected: bool = False
 
     def __init__(self, manager: SSHManager) -> None:
@@ -57,15 +62,17 @@
         self.on_change = Event()
 
     def update(self, name, value) -> None:
         if getattr(self, name) == value:
             return
 
         setattr(self, name, value)
-        self._manager.logger.info("%s: %s is %s", self._manager.name, name, value)
+        self._manager.logger.info(
+            "[%s] State: %s => %s", self._manager.name, name, value
+        )
         self.on_change.notify(self)
 
 
 class SSHManager(Manager):
     def __init__(
         self,
         host: str,
@@ -122,53 +129,53 @@
         try:
             stdin, stdout, stderr = self.client.exec_command(
                 string,
                 timeout=float(timeout),
             )
         except Exception as exc:
             self._disconnect()
-            raise CommandError("Disconnected before execution") from exc
+            raise CommandError(f"Disconnected before execution ({exc})") from exc
 
         try:
             return CommandOutput(
                 time(),
                 ["".join(line.splitlines()) for line in stdout],
                 ["".join(line.splitlines()) for line in stderr],
                 stdout.channel.recv_exit_status(),
             )
         except TimeoutError as exc:
             stdin.channel.close()
-            raise CommandError(f"Timeout ({timeout} s)") from exc
+            raise CommandError(f"Timeout of {timeout} seconds reached") from exc
         except Exception as exc:
             self._disconnect()
-            raise CommandError("Disconnected during execution") from exc
+            raise CommandError(f"Disconnected during execution ({exc})") from exc
 
     def _connect(self) -> None:
         if self.state.connected:
             return
 
         try:
             self.client.connect(
                 self.host,
                 self.port,
                 self.username,
                 self.password,
                 key_filename=self.key_filename,
-                timeout=self.ssh_timeout,  # TCP connect timeout
+                timeout=self.ssh_timeout,
                 allow_agent=False,
             )
         except SSHHostKeyUnknownError:
             self._disconnect()
             raise
         except paramiko.AuthenticationException as exc:
             self._disconnect()
-            raise SSHAuthError("SSH authentication failed") from exc
+            raise SSHAuthenticationError(f"SSH authentication failed ({exc})") from exc
         except Exception as exc:
             self._disconnect()
-            raise SSHConnectError("SSH connection failed") from exc
+            raise SSHConnectError(f"SSH connection failed ({exc})") from exc
 
         self.state.update(CONNECTED, True)
 
     def _disconnect(self) -> None:
         if not self.state.connected:
             return
 
@@ -184,49 +191,43 @@
         loop = asyncio.get_running_loop()
         timeout = command_timeout or self.command_timeout
         return await loop.run_in_executor(
             None, self._execute_command_string, string, timeout
         )
 
     async def async_connect(self) -> None:
-        """Connect to the SSH server.
+        """Connect the SSH client.
 
         Set `state.connected` to `True` and update all sensor
         commands if successful, otherwise raise an error.
 
         Raises:
             SSHHostKeyUnknownError
-            SSHAuthError
+            SSHAuthenticationError
             SSHConnectError
         """
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(None, self._connect)
-
-        for command in self.sensor_commands:
-            try:
-                await self.async_execute_command(command)
-            except CommandError:
-                pass
+        await self.async_update_sensor_commands(force=True)
 
     async def async_disconnect(self) -> None:
         """Disconnect the SSH client.
 
-        Set `state.connected` to `False` and update all sensor
-        commands with `None`.
+        Set `state.connected` to `False`.
         """
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(None, self._disconnect)
 
     async def async_update_state(self, *, raise_errors: bool = False) -> None:
         """Update state.
 
         Raises:
             OfflineError (only with `raise_errors=True`)
             SSHHostKeyUnknownError
-            SSHAuthError
+            SSHAuthenticationError
             SSHConnectError (only with `raise_errors=True`)
         """
         if self.state.connected:
             try:
                 await self.async_execute_command(_TEST_COMMAND)
                 return
             except CommandError:
@@ -236,22 +237,22 @@
             host = await icmplib.async_ping(
                 self.host,
                 count=1,
                 timeout=self.ping_timeout,
                 privileged=False,
             )
         except Exception as exc:  # pylint: disable=broad-except
-            self.logger.info("%s: Ping request failed (%s)", self.name, exc)
+            self.logger.info("[%s] Ping request failed (%s)", self.name, exc)
             self.state.update(ONLINE, False)
         else:
             self.state.update(ONLINE, host.is_alive)
 
         if not self.state.online:
             if raise_errors:
-                raise OfflineError("Host is offline")
+                raise OfflineError(f"Host is offline")
             return
 
         try:
             await self.async_connect()
         except SSHConnectError:
             if raise_errors:
                 raise
```

### Comparing `ssh_terminal_manager-0.5.0/src/ssh_terminal_manager.egg-info/PKG-INFO` & `ssh_terminal_manager-0.6.0/src/ssh_terminal_manager.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: ssh-terminal-manager
-Version: 0.5.0
+Version: 0.6.0
 Summary: Use terminal commands to control and monitor remote devices
 Author-email: zhbjsh <zhbjsh@outlook.com>
 Project-URL: Homepage, https://github.com/zhbjsh/ssh-terminal-manager
 Project-URL: Bug Tracker, https://github.com/zhbjsh/ssh-terminal-manager/issues
 Keywords: ssh,terminal,command line
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SSH Terminal Manager
 
 ## Initialize
```

