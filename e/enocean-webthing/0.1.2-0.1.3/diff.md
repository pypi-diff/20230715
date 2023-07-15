# Comparing `tmp/enocean_webthing-0.1.2.tar.gz` & `tmp/enocean_webthing-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/enocean_webthing-0.1.2.tar", last modified: Thu Apr 14 05:44:21 2022, max compression
+gzip compressed data, was "dist/enocean_webthing-0.1.3.tar", last modified: Sat Jul 15 13:23:26 2023, max compression
```

## Comparing `enocean_webthing-0.1.2.tar` & `enocean_webthing-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 05:44:21.000000 enocean_webthing-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     2833 2022-04-14 05:44:21.000000 enocean_webthing-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1980 2022-04-14 05:44:12.000000 enocean_webthing-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 05:44:21.000000 enocean_webthing-0.1.2/enocean_webthing/
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-04-14 05:44:12.000000 enocean_webthing-0.1.2/enocean_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6619 2022-04-14 05:44:12.000000 enocean_webthing-0.1.2/enocean_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     3229 2022-04-14 05:44:12.000000 enocean_webthing-0.1.2/enocean_webthing/enocean_ting.py
--rw-r--r--   0 runner    (1001) docker     (121)     4028 2022-04-14 05:44:12.000000 enocean_webthing-0.1.2/enocean_webthing/enocean_webthing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 05:44:21.000000 enocean_webthing-0.1.2/enocean_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2833 2022-04-14 05:44:20.000000 enocean_webthing-0.1.2/enocean_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-04-14 05:44:20.000000 enocean_webthing-0.1.2/enocean_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-14 05:44:20.000000 enocean_webthing-0.1.2/enocean_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-04-14 05:44:20.000000 enocean_webthing-0.1.2/enocean_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-04-14 05:44:20.000000 enocean_webthing-0.1.2/enocean_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-04-14 05:44:20.000000 enocean_webthing-0.1.2/enocean_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-14 05:44:21.000000 enocean_webthing-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-04-14 05:44:12.000000 enocean_webthing-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-15 13:23:11.000000 enocean_webthing-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/enocean_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-15 13:23:11.000000 enocean_webthing-0.1.3/enocean_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-15 13:23:11.000000 enocean_webthing-0.1.3/enocean_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-07-15 13:23:11.000000 enocean_webthing-0.1.3/enocean_webthing/enocean_ting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-15 13:23:11.000000 enocean_webthing-0.1.3/enocean_webthing/enocean_webthing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/enocean_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/enocean_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/enocean_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/enocean_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/enocean_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/enocean_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/enocean_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-15 13:23:11.000000 enocean_webthing-0.1.3/setup.py
```

### Comparing `enocean_webthing-0.1.2/PKG-INFO` & `enocean_webthing-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enocean_webthing
-Version: 0.1.2
+Version: 0.1.3
 Summary: A web connected enocean gateway
 Home-page: https://github.com/grro/enocean_webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: UNKNOWN
 Description: # enocean_webthing
         A web connected enocean gateway. This project provides a [webthing API](https://iot.mozilla.org/wot/) to an enocean gateway such as the  [EnOcean USB 300 USB-Gateway](https://www.enocean.com/de/produkt/usb-300-500u-400j/)
```

### Comparing `enocean_webthing-0.1.2/README.md` & `enocean_webthing-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `enocean_webthing-0.1.2/enocean_webthing/__init__.py` & `enocean_webthing-0.1.3/enocean_webthing/__init__.py`

 * *Files identical despite different names*

### Comparing `enocean_webthing-0.1.2/enocean_webthing/app.py` & `enocean_webthing-0.1.3/enocean_webthing/app.py`

 * *Files identical despite different names*

### Comparing `enocean_webthing-0.1.2/enocean_webthing/enocean_webthing.py` & `enocean_webthing-0.1.3/enocean_webthing/enocean_webthing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from time import sleep
 from typing import List
 from webthing import (MultipleThings, Property, Thing, Value, WebThingServer)
-from enocean_webthing.enocean_ting import Enocean, WindowHandle
+from enocean_webthing.enocean_ting import Enocean, WindowHandle, DeviceListener
 import logging
 import tornado.ioloop
 
 
-class WindowHandleWebThing(Thing):
+class WindowHandleWebThing(Thing, DeviceListener):
 
     # regarding capabilities refer https://iot.mozilla.org/schemas
     # there is also another schema registry http://iotschema.org/docs/full.html not used by webthing
 
     def __init__(self, description: str, name: str, eep_id: str, enocean_id: str):
         Thing.__init__(
             self,
@@ -18,15 +18,15 @@
             'WindowHandle ' + name,
             ['MultiLevelSensor'],
             description
         )
 
         self.ioloop = tornado.ioloop.IOLoop.current()
 
-        self.device = WindowHandle(eep_id, enocean_id, self.on_state_updated)
+        self.device = WindowHandle(eep_id, enocean_id, self)
 
         self.eepid = Value(eep_id)
         self.add_property(
             Property(self,
                      'eep_id',
                      self.eepid,
                      metadata={
@@ -68,26 +68,20 @@
                      metadata={
                          'title': 'State Description',
                          "type": "string",
                          'description': 'The state description',
                          'readOnly': True,
                      }))
 
-    def on_state_updated(self, new_state: int):
-        self.ioloop.add_callback(self.__update_state, new_state)
-
-    def __update_state(self, new_state: int):
-        self.state.notify_of_external_update(new_state)
-        if new_state == 1:
-            self.state_text.notify_of_external_update("TILTED")
-        elif new_state == 2:
-            self.state_text.notify_of_external_update("OPEN")
-        else:
-            self.state_text.notify_of_external_update("CLOSED")
+    def on_updated(self, device: WindowHandle):
+        self.ioloop.add_callback(self.__update_state, device)
 
+    def __update_state(self, device: WindowHandle):
+        self.state.notify_of_external_update(device.state)
+        self.state_text.notify_of_external_update(device.state_text)
 
 def run_server(port: int, description: str, path: str, addresses: List[str]):
     enocean_webthings = []
     for address in sorted(addresses):
         name, eep_id, enocean_id = address.split("/")
         if WindowHandle.supports(eep_id):
             enocean_webthings.append(WindowHandleWebThing(description, name, eep_id, enocean_id))
```

### Comparing `enocean_webthing-0.1.2/enocean_webthing.egg-info/PKG-INFO` & `enocean_webthing-0.1.3/enocean_webthing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enocean-webthing
-Version: 0.1.2
+Version: 0.1.3
 Summary: A web connected enocean gateway
 Home-page: https://github.com/grro/enocean_webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: UNKNOWN
 Description: # enocean_webthing
         A web connected enocean gateway. This project provides a [webthing API](https://iot.mozilla.org/wot/) to an enocean gateway such as the  [EnOcean USB 300 USB-Gateway](https://www.enocean.com/de/produkt/usb-300-500u-400j/)
```

### Comparing `enocean_webthing-0.1.2/setup.py` & `enocean_webthing-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             ENTRY_POINT + '=' + PACKAGENAME + ':main'
         ]
     },
     keywords=[
         'webthings', 'home automation', 'enocean', 'gateway'
     ],
     install_requires=[
-        'webthing==0.15.0',  'enocean==0.60.1'
+        'webthing==0.15.0',  'enocean==0.60.1', 'redzoo'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Development Status :: 3 - Alpha"
     ],
```

