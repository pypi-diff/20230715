# Comparing `tmp/mqttapi-0.1.1.tar.gz` & `tmp/mqttapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqttapi-0.1.1.tar", last modified: Sat Jul 15 03:57:12 2023, max compression
+gzip compressed data, was "mqttapi-0.1.2.tar", last modified: Sat Jul 15 04:27:39 2023, max compression
```

## Comparing `mqttapi-0.1.1.tar` & `mqttapi-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 davi      (1000) davi      (1000)        0 2023-07-15 03:57:12.949657 mqttapi-0.1.1/
--rw-r--r--   0 davi      (1000) davi      (1000)     1066 2023-07-14 19:20:24.000000 mqttapi-0.1.1/LICENSE
--rw-r--r--   0 davi      (1000) davi      (1000)      629 2023-07-15 03:57:12.948658 mqttapi-0.1.1/PKG-INFO
-drwxr-xr-x   0 davi      (1000) davi      (1000)        0 2023-07-15 03:57:12.931099 mqttapi-0.1.1/mqttapi/
--rw-r--r--   0 davi      (1000) davi      (1000)      183 2023-07-15 03:51:16.000000 mqttapi-0.1.1/mqttapi/__init__.py
--rw-r--r--   0 davi      (1000) davi      (1000)       22 2023-07-15 03:51:38.000000 mqttapi-0.1.1/mqttapi/__version__.py
--rw-r--r--   0 davi      (1000) davi      (1000)     1050 2023-07-14 19:38:55.000000 mqttapi-0.1.1/mqttapi/bd_manipulator.py
--rw-r--r--   0 davi      (1000) davi      (1000)      559 2023-07-14 19:38:55.000000 mqttapi-0.1.1/mqttapi/json_manipulator.py
--rw-r--r--   0 davi      (1000) davi      (1000)     1597 2023-07-15 03:37:20.000000 mqttapi-0.1.1/mqttapi/main.py
--rw-r--r--   0 davi      (1000) davi      (1000)     1472 2023-07-14 19:38:55.000000 mqttapi-0.1.1/mqttapi/mqtt_communicator.py
--rw-r--r--   0 davi      (1000) davi      (1000)     2257 2023-07-15 03:40:38.000000 mqttapi-0.1.1/mqttapi/websocket_server.py
-drwxr-xr-x   0 davi      (1000) davi      (1000)        0 2023-07-15 03:57:12.947656 mqttapi-0.1.1/mqttapi.egg-info/
--rw-r--r--   0 davi      (1000) davi      (1000)      629 2023-07-15 03:57:12.000000 mqttapi-0.1.1/mqttapi.egg-info/PKG-INFO
--rw-r--r--   0 davi      (1000) davi      (1000)      340 2023-07-15 03:57:12.000000 mqttapi-0.1.1/mqttapi.egg-info/SOURCES.txt
--rw-r--r--   0 davi      (1000) davi      (1000)        1 2023-07-15 03:57:12.000000 mqttapi-0.1.1/mqttapi.egg-info/dependency_links.txt
--rw-r--r--   0 davi      (1000) davi      (1000)       43 2023-07-15 03:57:12.000000 mqttapi-0.1.1/mqttapi.egg-info/requires.txt
--rw-r--r--   0 davi      (1000) davi      (1000)        8 2023-07-15 03:57:12.000000 mqttapi-0.1.1/mqttapi.egg-info/top_level.txt
--rw-r--r--   0 davi      (1000) davi      (1000)       38 2023-07-15 03:57:12.949657 mqttapi-0.1.1/setup.cfg
--rw-r--r--   0 davi      (1000) davi      (1000)     1171 2023-07-15 03:53:03.000000 mqttapi-0.1.1/setup.py
+drwxr-xr-x   0 davi      (1000) davi      (1000)        0 2023-07-15 04:27:39.822895 mqttapi-0.1.2/
+-rw-r--r--   0 davi      (1000) davi      (1000)     1066 2023-07-15 04:13:08.000000 mqttapi-0.1.2/LICENSE
+-rw-r--r--   0 davi      (1000) davi      (1000)      629 2023-07-15 04:27:39.821895 mqttapi-0.1.2/PKG-INFO
+drwxr-xr-x   0 davi      (1000) davi      (1000)        0 2023-07-15 04:27:39.813359 mqttapi-0.1.2/mqttapi/
+-rw-r--r--   0 davi      (1000) davi      (1000)      183 2023-07-15 04:20:29.000000 mqttapi-0.1.2/mqttapi/__init__.py
+-rw-r--r--   0 davi      (1000) davi      (1000)       22 2023-07-15 04:26:59.000000 mqttapi-0.1.2/mqttapi/__version__.py
+-rw-r--r--   0 davi      (1000) davi      (1000)     1050 2023-07-15 04:13:08.000000 mqttapi-0.1.2/mqttapi/bd_manipulator.py
+-rw-r--r--   0 davi      (1000) davi      (1000)      559 2023-07-15 04:13:08.000000 mqttapi-0.1.2/mqttapi/json_manipulator.py
+-rw-r--r--   0 davi      (1000) davi      (1000)     1597 2023-07-15 04:13:08.000000 mqttapi-0.1.2/mqttapi/main.py
+-rw-r--r--   0 davi      (1000) davi      (1000)     1472 2023-07-15 04:13:08.000000 mqttapi-0.1.2/mqttapi/mqtt_communicator.py
+-rw-r--r--   0 davi      (1000) davi      (1000)     2275 2023-07-15 04:23:34.000000 mqttapi-0.1.2/mqttapi/websocket_server.py
+drwxr-xr-x   0 davi      (1000) davi      (1000)        0 2023-07-15 04:27:39.821895 mqttapi-0.1.2/mqttapi.egg-info/
+-rw-r--r--   0 davi      (1000) davi      (1000)      629 2023-07-15 04:27:39.000000 mqttapi-0.1.2/mqttapi.egg-info/PKG-INFO
+-rw-r--r--   0 davi      (1000) davi      (1000)      340 2023-07-15 04:27:39.000000 mqttapi-0.1.2/mqttapi.egg-info/SOURCES.txt
+-rw-r--r--   0 davi      (1000) davi      (1000)        1 2023-07-15 04:27:39.000000 mqttapi-0.1.2/mqttapi.egg-info/dependency_links.txt
+-rw-r--r--   0 davi      (1000) davi      (1000)       47 2023-07-15 04:27:39.000000 mqttapi-0.1.2/mqttapi.egg-info/requires.txt
+-rw-r--r--   0 davi      (1000) davi      (1000)        8 2023-07-15 04:27:39.000000 mqttapi-0.1.2/mqttapi.egg-info/top_level.txt
+-rw-r--r--   0 davi      (1000) davi      (1000)       38 2023-07-15 04:27:39.822895 mqttapi-0.1.2/setup.cfg
+-rw-r--r--   0 davi      (1000) davi      (1000)     1182 2023-07-15 04:23:13.000000 mqttapi-0.1.2/setup.py
```

### Comparing `mqttapi-0.1.1/LICENSE` & `mqttapi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mqttapi-0.1.1/PKG-INFO` & `mqttapi-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqttapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: simplified mqtt library
 Home-page: https://github.com/davifurao/mqttapi
 Author: Davi Luna
 Author-email: Sdavi738@gmail.com
 Keywords: mqtt api,mosquitto api,real-time,messaging,simplified mqtt,paho-mqtt api
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `mqttapi-0.1.1/mqttapi/bd_manipulator.py` & `mqttapi-0.1.2/mqttapi/bd_manipulator.py`

 * *Files identical despite different names*

### Comparing `mqttapi-0.1.1/mqttapi/json_manipulator.py` & `mqttapi-0.1.2/mqttapi/json_manipulator.py`

 * *Files identical despite different names*

### Comparing `mqttapi-0.1.1/mqttapi/main.py` & `mqttapi-0.1.2/mqttapi/main.py`

 * *Files identical despite different names*

### Comparing `mqttapi-0.1.1/mqttapi/mqtt_communicator.py` & `mqttapi-0.1.2/mqttapi/mqtt_communicator.py`

 * *Files identical despite different names*

### Comparing `mqttapi-0.1.1/mqttapi/websocket_server.py` & `mqttapi-0.1.2/mqttapi/websocket_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import asyncio
 import json
 import threading
 import websockets
+import websocket
+
 
 
 class WebSocketServer:
     def __init__(self, host, port):
         self.host = host
         self.port = port
         self.connected_clients = set()
```

### Comparing `mqttapi-0.1.1/mqttapi.egg-info/PKG-INFO` & `mqttapi-0.1.2/mqttapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqttapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: simplified mqtt library
 Home-page: https://github.com/davifurao/mqttapi
 Author: Davi Luna
 Author-email: Sdavi738@gmail.com
 Keywords: mqtt api,mosquitto api,real-time,messaging,simplified mqtt,paho-mqtt api
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `mqttapi-0.1.1/setup.py` & `mqttapi-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     author='Davi Luna',
     author_email='Sdavi738@gmail.com',
     packages=['mqttapi'],
     install_requires=[
     'pymysql',
     'paho-mqtt',
     'asyncio',
-    'websocket-client'
+    'websockets',
+    'websocket'
     ],
     keywords=[
         "mqtt api",
         "mosquitto api",
         "real-time",
         "messaging",
         "simplified mqtt",
```

