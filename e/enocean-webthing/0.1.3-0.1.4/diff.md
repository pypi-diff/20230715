# Comparing `tmp/enocean_webthing-0.1.3.tar.gz` & `tmp/enocean_webthing-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/enocean_webthing-0.1.3.tar", last modified: Sat Jul 15 13:23:26 2023, max compression
+gzip compressed data, was "dist/enocean_webthing-0.1.4.tar", last modified: Sat Jul 15 13:32:50 2023, max compression
```

## Comparing `enocean_webthing-0.1.3.tar` & `enocean_webthing-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-15 13:23:11.000000 enocean_webthing-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/enocean_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-15 13:23:11.000000 enocean_webthing-0.1.3/enocean_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-15 13:23:11.000000 enocean_webthing-0.1.3/enocean_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-07-15 13:23:11.000000 enocean_webthing-0.1.3/enocean_webthing/enocean_ting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-15 13:23:11.000000 enocean_webthing-0.1.3/enocean_webthing/enocean_webthing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/enocean_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/enocean_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/enocean_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/enocean_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/enocean_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/enocean_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/enocean_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 13:23:26.000000 enocean_webthing-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-15 13:23:11.000000 enocean_webthing-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:32:50.000000 enocean_webthing-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-15 13:32:50.000000 enocean_webthing-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-15 13:32:35.000000 enocean_webthing-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:32:50.000000 enocean_webthing-0.1.4/enocean_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-15 13:32:35.000000 enocean_webthing-0.1.4/enocean_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6619 2023-07-15 13:32:35.000000 enocean_webthing-0.1.4/enocean_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-15 13:32:35.000000 enocean_webthing-0.1.4/enocean_webthing/enocean_thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-15 13:32:35.000000 enocean_webthing-0.1.4/enocean_webthing/enocean_webthing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:32:50.000000 enocean_webthing-0.1.4/enocean_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-07-15 13:32:49.000000 enocean_webthing-0.1.4/enocean_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-15 13:32:50.000000 enocean_webthing-0.1.4/enocean_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 13:32:49.000000 enocean_webthing-0.1.4/enocean_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-15 13:32:49.000000 enocean_webthing-0.1.4/enocean_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-15 13:32:49.000000 enocean_webthing-0.1.4/enocean_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-15 13:32:49.000000 enocean_webthing-0.1.4/enocean_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 13:32:50.000000 enocean_webthing-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-15 13:32:35.000000 enocean_webthing-0.1.4/setup.py
```

### Comparing `enocean_webthing-0.1.3/PKG-INFO` & `enocean_webthing-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enocean_webthing
-Version: 0.1.3
+Version: 0.1.4
 Summary: A web connected enocean gateway
 Home-page: https://github.com/grro/enocean_webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: UNKNOWN
 Description: # enocean_webthing
         A web connected enocean gateway. This project provides a [webthing API](https://iot.mozilla.org/wot/) to an enocean gateway such as the  [EnOcean USB 300 USB-Gateway](https://www.enocean.com/de/produkt/usb-300-500u-400j/)
```

### Comparing `enocean_webthing-0.1.3/README.md` & `enocean_webthing-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `enocean_webthing-0.1.3/enocean_webthing/__init__.py` & `enocean_webthing-0.1.4/enocean_webthing/__init__.py`

 * *Files identical despite different names*

### Comparing `enocean_webthing-0.1.3/enocean_webthing/app.py` & `enocean_webthing-0.1.4/enocean_webthing/app.py`

 * *Files identical despite different names*

### Comparing `enocean_webthing-0.1.3/enocean_webthing/enocean_ting.py` & `enocean_webthing-0.1.4/enocean_webthing/enocean_thing.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,16 +29,17 @@
 
 class WindowHandle(Device):
 
     @staticmethod
     def supports(eep_id: str) -> bool:
         return eep_id.upper() == 'F6:10:00'
 
-    def __init__(self, eep_id: str, enocean_id: str, listener: DeviceListener):
+    def __init__(self, name: str, eep_id: str, enocean_id: str, listener: DeviceListener):
         self.listener = listener
+        self.name = name
         self.db = SimpleDB("processing_state_" + eep_id + "_" + enocean_id)
         self.sender = enocean_id.upper()
         self.sender_hex_string: List[int] = enocean.utils.from_hex_string(self.sender)
         self.eep_id = eep_id.upper()
         self.eep_id_hex_string: List[int] = enocean.utils.from_hex_string(self.eep_id)
         logging.info("window handle (eep_id: " + eep_id + ", enocean_id: " + enocean_id +")")
 
@@ -59,14 +60,15 @@
         is_handled = False
         try:
             if self.eep_id_hex_string[0] == 0xf6 and packet.packet_type == PACKET.RADIO_ERP1 and packet.rorg == RORG.RPS:
                 packet.parse_eep(self.eep_id_hex_string[1], self.eep_id_hex_string[2])
                 state = packet.parsed['WIN']['raw_value']  #  WIN: {'description': 'Window handle', 'unit': '', 'value': 'Moved from vertical to down', 'raw_value': 3}
                 if self.sender == packet.sender_hex:
                     self.db.put("state", state)
+                    logging.info(self.name + " state updated " + self.state_text)
                     self.listener.on_updated(self)
                     is_handled = True
         except Exception as e:
             logging.warning("error occurred by handling packet", e)
         return is_handled
```

### Comparing `enocean_webthing-0.1.3/enocean_webthing/enocean_webthing.py` & `enocean_webthing-0.1.4/enocean_webthing/enocean_webthing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from time import sleep
 from typing import List
 from webthing import (MultipleThings, Property, Thing, Value, WebThingServer)
-from enocean_webthing.enocean_ting import Enocean, WindowHandle, DeviceListener
+from enocean_webthing.enocean_thing import Enocean, WindowHandle, DeviceListener
 import logging
 import tornado.ioloop
 
 
 class WindowHandleWebThing(Thing, DeviceListener):
 
     # regarding capabilities refer https://iot.mozilla.org/schemas
@@ -18,15 +18,27 @@
             'WindowHandle ' + name,
             ['MultiLevelSensor'],
             description
         )
 
         self.ioloop = tornado.ioloop.IOLoop.current()
 
-        self.device = WindowHandle(eep_id, enocean_id, self)
+        self.device = WindowHandle(name, eep_id, enocean_id, self)
+
+        self.name = Value(name)
+        self.add_property(
+            Property(self,
+                     'name',
+                     self.name,
+                     metadata={
+                         'title': 'name',
+                         "type": "string",
+                         'description': '"The name',
+                         'readOnly': True,
+                     }))
 
         self.eepid = Value(eep_id)
         self.add_property(
             Property(self,
                      'eep_id',
                      self.eepid,
                      metadata={
```

### Comparing `enocean_webthing-0.1.3/enocean_webthing.egg-info/PKG-INFO` & `enocean_webthing-0.1.4/enocean_webthing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enocean-webthing
-Version: 0.1.3
+Version: 0.1.4
 Summary: A web connected enocean gateway
 Home-page: https://github.com/grro/enocean_webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: UNKNOWN
 Description: # enocean_webthing
         A web connected enocean gateway. This project provides a [webthing API](https://iot.mozilla.org/wot/) to an enocean gateway such as the  [EnOcean USB 300 USB-Gateway](https://www.enocean.com/de/produkt/usb-300-500u-400j/)
```

### Comparing `enocean_webthing-0.1.3/setup.py` & `enocean_webthing-0.1.4/setup.py`

 * *Files identical despite different names*

