# Comparing `tmp/pyacaia_async-0.0.3.tar.gz` & `tmp/pyacaia_async-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacaia_async-0.0.3.tar", last modified: Thu Jul 13 11:04:30 2023, max compression
+gzip compressed data, was "pyacaia_async-0.0.4.tar", last modified: Sat Jul 15 09:41:28 2023, max compression
```

## Comparing `pyacaia_async-0.0.3.tar` & `pyacaia_async-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:30.916785 pyacaia_async-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-13 11:04:08.000000 pyacaia_async-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-13 11:04:30.916785 pyacaia_async-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-13 11:04:08.000000 pyacaia_async-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:30.916785 pyacaia_async-0.0.3/pyacaia_async/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 11:04:08.000000 pyacaia_async-0.0.3/pyacaia_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-07-13 11:04:08.000000 pyacaia_async-0.0.3/pyacaia_async/acaiascale.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-13 11:04:08.000000 pyacaia_async-0.0.3/pyacaia_async/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-07-13 11:04:08.000000 pyacaia_async-0.0.3/pyacaia_async/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-13 11:04:08.000000 pyacaia_async-0.0.3/pyacaia_async/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-13 11:04:08.000000 pyacaia_async-0.0.3/pyacaia_async/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:04:30.916785 pyacaia_async-0.0.3/pyacaia_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-13 11:04:30.000000 pyacaia_async-0.0.3/pyacaia_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-13 11:04:30.000000 pyacaia_async-0.0.3/pyacaia_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:04:30.000000 pyacaia_async-0.0.3/pyacaia_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-13 11:04:30.000000 pyacaia_async-0.0.3/pyacaia_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-13 11:04:30.000000 pyacaia_async-0.0.3/pyacaia_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 11:04:30.916785 pyacaia_async-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-13 11:04:08.000000 pyacaia_async-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:41:28.138112 pyacaia_async-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 09:41:11.000000 pyacaia_async-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-15 09:41:28.138112 pyacaia_async-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-15 09:41:11.000000 pyacaia_async-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:41:28.138112 pyacaia_async-0.0.4/pyacaia_async/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-15 09:41:11.000000 pyacaia_async-0.0.4/pyacaia_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-07-15 09:41:11.000000 pyacaia_async-0.0.4/pyacaia_async/acaiascale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-15 09:41:11.000000 pyacaia_async-0.0.4/pyacaia_async/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-15 09:41:11.000000 pyacaia_async-0.0.4/pyacaia_async/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-15 09:41:11.000000 pyacaia_async-0.0.4/pyacaia_async/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-15 09:41:11.000000 pyacaia_async-0.0.4/pyacaia_async/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:41:28.138112 pyacaia_async-0.0.4/pyacaia_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-15 09:41:28.000000 pyacaia_async-0.0.4/pyacaia_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-15 09:41:28.000000 pyacaia_async-0.0.4/pyacaia_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 09:41:28.000000 pyacaia_async-0.0.4/pyacaia_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-15 09:41:28.000000 pyacaia_async-0.0.4/pyacaia_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-15 09:41:28.000000 pyacaia_async-0.0.4/pyacaia_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 09:41:28.138112 pyacaia_async-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-15 09:41:11.000000 pyacaia_async-0.0.4/setup.py
```

### Comparing `pyacaia_async-0.0.3/LICENSE` & `pyacaia_async-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyacaia_async-0.0.3/PKG-INFO` & `pyacaia_async-0.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacaia_async
-Version: 0.0.3
+Version: 0.0.4
 Summary: An async implementation of PyAcaia
 Home-page: https://github.com/zweckj/pyacaia_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -23,14 +23,30 @@
 import asyncio
 from pyacaia_async import AcaiaScale
 from pyacaia_async.helpers import find_acaia_devices
 
 async def main()
   addresses = await find_acaia_devices()
   address = addresses[0]
-  scale = await AcaiaScale.create(mac=address, isPyxisStyle=False)
+  scale = await AcaiaScale.create(mac=address, is_new_style_scale=False)
   await scale.tare()
   await scale.startStopTimer()
   await scale.resetTimer()
 
 asyncio.run(main())
 ```
+
+# Callback
+Weight and settings are available, if you pass a callback function to the constructor. 
+In that callback you will either receive objects of type `Message` or `Settings`. A sample notification handler can look like this and can also be found in `decode.py`
+
+```python
+def notification_handler(sender, data) -> None:
+    msg = decode(data)[0]
+    if isinstance(msg, Settings):
+        print(f"Battery: {msg.battery}")
+        print(f"Unit: {msg.unit}")
+    elif isinstance(msg, Message):
+        print(f"Weight: {msg.value}")
+
+scale = await AcaiaScale.create(mac=address, callback=notification_handler)
+```
```

### Comparing `pyacaia_async-0.0.3/pyacaia_async/decode.py` & `pyacaia_async-0.0.4/pyacaia_async/decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,9 +144,10 @@
     return (None,bytes[messageEnd:])
 
 
 def notification_handler(sender, data) -> None:
     msg = decode(data)[0]
     if isinstance(msg, Settings):
         print(f"Battery: {msg.battery}")
+        print(f"Units: {msg.units}")
     elif isinstance(msg, Message):
-        pass
+        print(f"Weight: {msg.value}")
```

### Comparing `pyacaia_async-0.0.3/pyacaia_async/helpers.py` & `pyacaia_async-0.0.4/pyacaia_async/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,29 +63,25 @@
     if isPyxisStyle:
         payload = bytearray([0x30,0x31,0x32,0x33,0x34,0x35,0x36,0x37,0x38,0x39,0x30,0x31,0x32,0x33,0x34])
     else:
         payload = bytearray([0x2d,0x2d,0x2d,0x2d,0x2d,0x2d,0x2d,0x2d,0x2d,0x2d,0x2d,0x2d,0x2d,0x2d,0x2d])
     return encode(11,payload)
 
 
-def encodeEventData(payload) -> bytearray:
-    bytes= bytearray(len(payload)+1)
-    bytes[0] = len(payload) + 1
-
-    for i in range(len(payload)):
-        bytes[i+1]=payload[i] & 0xff
-
-    return encode(12,bytes)
-
-
 def encodeNotificationRequest() -> bytearray:
     payload=[
     	0,  # weight
     	1,  # weight argument
     	1,  # battery
     	2,  # battery argument
     	2,  # timer
     	5,  # timer argument (number heartbeats between timer messages)
     	3,  # key
     	4   # setting
     ]
-    return encodeEventData(payload)
+    bytes= bytearray(len(payload)+1)
+    bytes[0] = len(payload) + 1
+
+    for i in range(len(payload)):
+        bytes[i+1]=payload[i] & 0xff
+
+    return encode(12,bytes)
```

### Comparing `pyacaia_async-0.0.3/pyacaia_async.egg-info/PKG-INFO` & `pyacaia_async-0.0.4/pyacaia_async.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyacaia-async
-Version: 0.0.3
+Version: 0.0.4
 Summary: An async implementation of PyAcaia
 Home-page: https://github.com/zweckj/pyacaia_async
 Author: Josef Zweck
 Author-email: 24647999+zweckj@users.noreply.github.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -23,14 +23,30 @@
 import asyncio
 from pyacaia_async import AcaiaScale
 from pyacaia_async.helpers import find_acaia_devices
 
 async def main()
   addresses = await find_acaia_devices()
   address = addresses[0]
-  scale = await AcaiaScale.create(mac=address, isPyxisStyle=False)
+  scale = await AcaiaScale.create(mac=address, is_new_style_scale=False)
   await scale.tare()
   await scale.startStopTimer()
   await scale.resetTimer()
 
 asyncio.run(main())
 ```
+
+# Callback
+Weight and settings are available, if you pass a callback function to the constructor. 
+In that callback you will either receive objects of type `Message` or `Settings`. A sample notification handler can look like this and can also be found in `decode.py`
+
+```python
+def notification_handler(sender, data) -> None:
+    msg = decode(data)[0]
+    if isinstance(msg, Settings):
+        print(f"Battery: {msg.battery}")
+        print(f"Unit: {msg.unit}")
+    elif isinstance(msg, Message):
+        print(f"Weight: {msg.value}")
+
+scale = await AcaiaScale.create(mac=address, callback=notification_handler)
+```
```

### Comparing `pyacaia_async-0.0.3/setup.py` & `pyacaia_async-0.0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setuptools.setup(
     name="pyacaia_async",
-    version="0.0.3",
+    version="0.0.4",
     description="An async implementation of PyAcaia",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/zweckj/pyacaia_async",
     author="Josef Zweck",
     author_email="24647999+zweckj@users.noreply.github.com",
     license="MIT",
```

