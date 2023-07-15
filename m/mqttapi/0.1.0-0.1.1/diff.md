# Comparing `tmp/mqttapi-0.1.0.tar.gz` & `tmp/mqttapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqttapi-0.1.0.tar", last modified: Fri Jul 14 20:12:18 2023, max compression
+gzip compressed data, was "mqttapi-0.1.1.tar", last modified: Sat Jul 15 03:57:12 2023, max compression
```

## Comparing `mqttapi-0.1.0.tar` & `mqttapi-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 davi      (1000) davi      (1000)        0 2023-07-14 20:12:18.411528 mqttapi-0.1.0/
--rw-r--r--   0 davi      (1000) davi      (1000)     1066 2023-07-14 19:20:24.000000 mqttapi-0.1.0/LICENSE
--rw-r--r--   0 davi      (1000) davi      (1000)      589 2023-07-14 20:12:18.410527 mqttapi-0.1.0/PKG-INFO
-drwxr-xr-x   0 davi      (1000) davi      (1000)        0 2023-07-14 20:12:18.398640 mqttapi-0.1.0/mqttapi/
--rw-r--r--   0 davi      (1000) davi      (1000)       22 2023-07-14 19:53:13.000000 mqttapi-0.1.0/mqttapi/__init__.py
--rw-r--r--   0 davi      (1000) davi      (1000)     1050 2023-07-14 19:38:55.000000 mqttapi-0.1.0/mqttapi/bd_manipulator.py
--rw-r--r--   0 davi      (1000) davi      (1000)      559 2023-07-14 19:38:55.000000 mqttapi-0.1.0/mqttapi/json_manipulator.py
--rw-r--r--   0 davi      (1000) davi      (1000)     1597 2023-07-14 19:38:55.000000 mqttapi-0.1.0/mqttapi/main.py
--rw-r--r--   0 davi      (1000) davi      (1000)     1472 2023-07-14 19:38:55.000000 mqttapi-0.1.0/mqttapi/mqtt_communicator.py
--rw-r--r--   0 davi      (1000) davi      (1000)     1352 2023-07-14 19:38:55.000000 mqttapi-0.1.0/mqttapi/websocket-server.py
-drwxr-xr-x   0 davi      (1000) davi      (1000)        0 2023-07-14 20:12:18.410527 mqttapi-0.1.0/mqttapi.egg-info/
--rw-r--r--   0 davi      (1000) davi      (1000)      589 2023-07-14 20:12:18.000000 mqttapi-0.1.0/mqttapi.egg-info/PKG-INFO
--rw-r--r--   0 davi      (1000) davi      (1000)      317 2023-07-14 20:12:18.000000 mqttapi-0.1.0/mqttapi.egg-info/SOURCES.txt
--rw-r--r--   0 davi      (1000) davi      (1000)        1 2023-07-14 20:12:18.000000 mqttapi-0.1.0/mqttapi.egg-info/dependency_links.txt
--rw-r--r--   0 davi      (1000) davi      (1000)       43 2023-07-14 20:12:18.000000 mqttapi-0.1.0/mqttapi.egg-info/requires.txt
--rw-r--r--   0 davi      (1000) davi      (1000)        8 2023-07-14 20:12:18.000000 mqttapi-0.1.0/mqttapi.egg-info/top_level.txt
--rw-r--r--   0 davi      (1000) davi      (1000)       38 2023-07-14 20:12:18.411528 mqttapi-0.1.0/setup.cfg
--rw-r--r--   0 davi      (1000) davi      (1000)     1128 2023-07-14 19:59:47.000000 mqttapi-0.1.0/setup.py
+drwxr-xr-x   0 davi      (1000) davi      (1000)        0 2023-07-15 03:57:12.949657 mqttapi-0.1.1/
+-rw-r--r--   0 davi      (1000) davi      (1000)     1066 2023-07-14 19:20:24.000000 mqttapi-0.1.1/LICENSE
+-rw-r--r--   0 davi      (1000) davi      (1000)      629 2023-07-15 03:57:12.948658 mqttapi-0.1.1/PKG-INFO
+drwxr-xr-x   0 davi      (1000) davi      (1000)        0 2023-07-15 03:57:12.931099 mqttapi-0.1.1/mqttapi/
+-rw-r--r--   0 davi      (1000) davi      (1000)      183 2023-07-15 03:51:16.000000 mqttapi-0.1.1/mqttapi/__init__.py
+-rw-r--r--   0 davi      (1000) davi      (1000)       22 2023-07-15 03:51:38.000000 mqttapi-0.1.1/mqttapi/__version__.py
+-rw-r--r--   0 davi      (1000) davi      (1000)     1050 2023-07-14 19:38:55.000000 mqttapi-0.1.1/mqttapi/bd_manipulator.py
+-rw-r--r--   0 davi      (1000) davi      (1000)      559 2023-07-14 19:38:55.000000 mqttapi-0.1.1/mqttapi/json_manipulator.py
+-rw-r--r--   0 davi      (1000) davi      (1000)     1597 2023-07-15 03:37:20.000000 mqttapi-0.1.1/mqttapi/main.py
+-rw-r--r--   0 davi      (1000) davi      (1000)     1472 2023-07-14 19:38:55.000000 mqttapi-0.1.1/mqttapi/mqtt_communicator.py
+-rw-r--r--   0 davi      (1000) davi      (1000)     2257 2023-07-15 03:40:38.000000 mqttapi-0.1.1/mqttapi/websocket_server.py
+drwxr-xr-x   0 davi      (1000) davi      (1000)        0 2023-07-15 03:57:12.947656 mqttapi-0.1.1/mqttapi.egg-info/
+-rw-r--r--   0 davi      (1000) davi      (1000)      629 2023-07-15 03:57:12.000000 mqttapi-0.1.1/mqttapi.egg-info/PKG-INFO
+-rw-r--r--   0 davi      (1000) davi      (1000)      340 2023-07-15 03:57:12.000000 mqttapi-0.1.1/mqttapi.egg-info/SOURCES.txt
+-rw-r--r--   0 davi      (1000) davi      (1000)        1 2023-07-15 03:57:12.000000 mqttapi-0.1.1/mqttapi.egg-info/dependency_links.txt
+-rw-r--r--   0 davi      (1000) davi      (1000)       43 2023-07-15 03:57:12.000000 mqttapi-0.1.1/mqttapi.egg-info/requires.txt
+-rw-r--r--   0 davi      (1000) davi      (1000)        8 2023-07-15 03:57:12.000000 mqttapi-0.1.1/mqttapi.egg-info/top_level.txt
+-rw-r--r--   0 davi      (1000) davi      (1000)       38 2023-07-15 03:57:12.949657 mqttapi-0.1.1/setup.cfg
+-rw-r--r--   0 davi      (1000) davi      (1000)     1171 2023-07-15 03:53:03.000000 mqttapi-0.1.1/setup.py
```

### Comparing `mqttapi-0.1.0/LICENSE` & `mqttapi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mqttapi-0.1.0/PKG-INFO` & `mqttapi-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: mqttapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: simplified mqtt library
+Home-page: https://github.com/davifurao/mqttapi
 Author: Davi Luna
 Author-email: Sdavi738@gmail.com
 Keywords: mqtt api,mosquitto api,real-time,messaging,simplified mqtt,paho-mqtt api
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
```

### Comparing `mqttapi-0.1.0/mqttapi/bd_manipulator.py` & `mqttapi-0.1.1/mqttapi/bd_manipulator.py`

 * *Files identical despite different names*

### Comparing `mqttapi-0.1.0/mqttapi/json_manipulator.py` & `mqttapi-0.1.1/mqttapi/json_manipulator.py`

 * *Files identical despite different names*

### Comparing `mqttapi-0.1.0/mqttapi/main.py` & `mqttapi-0.1.1/mqttapi/main.py`

 * *Files identical despite different names*

### Comparing `mqttapi-0.1.0/mqttapi/mqtt_communicator.py` & `mqttapi-0.1.1/mqttapi/mqtt_communicator.py`

 * *Files identical despite different names*

### Comparing `mqttapi-0.1.0/mqttapi/websocket-server.py` & `mqttapi-0.1.1/mqttapi/websocket_server.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import asyncio
+import json
+import threading
 import websockets
 
+
 class WebSocketServer:
     def __init__(self, host, port):
         self.host = host
         self.port = port
         self.connected_clients = set()
         self.server = None
 
@@ -33,7 +36,34 @@
         asyncio.get_event_loop().run_until_complete(self.server)
         asyncio.get_event_loop().run_forever()
 
     def stop_server(self):
         if self.server:
             self.server.close()
             
+    def send_message_to_websocket(topic, payload):
+        if websocket and websocket.sock and websocket.sock.connected:
+            message = {
+                'topic': topic,
+                'payload': payload
+            }
+            websocket.send(json.dumps(message))
+            
+    def connect_to_websocket(self):
+        global websocket
+        websocket_server = f"ws://{self.host}:{self.port}/"
+        websocket = websocket.WebSocketApp(websocket_server, on_message=self.on_message)
+        websocket.run_forever()
+        
+    def on_message(ws, message):
+        data = json.loads(message)
+        topic = data['topic']
+        payload = data['payload']
+
+    def start_websocket_thread(self):
+        websocket_thread = threading.Thread(target=self.connect_to_websocket)
+        websocket_thread.daemon = True
+        websocket_thread.start()
+
+
+
+
```

### Comparing `mqttapi-0.1.0/mqttapi.egg-info/PKG-INFO` & `mqttapi-0.1.1/mqttapi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: mqttapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: simplified mqtt library
+Home-page: https://github.com/davifurao/mqttapi
 Author: Davi Luna
 Author-email: Sdavi738@gmail.com
 Keywords: mqtt api,mosquitto api,real-time,messaging,simplified mqtt,paho-mqtt api
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
```

### Comparing `mqttapi-0.1.0/setup.py` & `mqttapi-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 import os
 
 def read_version():
     here = os.path.abspath(os.path.dirname(__file__))
-    version_file = os.path.join(here, 'mqttapi', '__init__.py')
+    version_file = os.path.join(here, 'mqttapi', '__version__.py')
     namespace = {}
     with open(version_file, 'r') as f:
         exec(f.read(), namespace)
     return namespace['__version__']
 
 setup(
     name='mqttapi',
@@ -27,16 +27,17 @@
         "mosquitto api",
         "real-time",
         "messaging",
         "simplified mqtt",
         "paho-mqtt api",
         ],
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
+        'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
+    url='https://github.com/davifurao/mqttapi',
 )
```

