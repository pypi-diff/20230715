# Comparing `tmp/indipydriver-0.0.6.tar.gz` & `tmp/indipydriver-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipydriver-0.0.6.tar", last modified: Sun Jul  9 10:55:57 2023, max compression
+gzip compressed data, was "indipydriver-0.0.7.tar", last modified: Fri Jul 14 22:05:16 2023, max compression
```

## Comparing `indipydriver-0.0.6.tar` & `indipydriver-0.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-05-04 20:13:36.000000 indipydriver-0.0.6/LICENSE
--rw-r--r--   0        0        0     2261 2023-06-17 14:59:33.000000 indipydriver-0.0.6/README.md
--rw-r--r--   0        0        0      573 2023-07-08 14:17:28.000000 indipydriver-0.0.6/indipydriver/__init__.py
--rw-r--r--   0        0        0    17081 2023-07-09 09:46:38.000000 indipydriver-0.0.6/indipydriver/comms.py
--rw-r--r--   0        0        0    21067 2023-07-09 10:33:24.000000 indipydriver-0.0.6/indipydriver/events.py
--rw-r--r--   0        0        0    20883 2023-07-09 10:29:51.000000 indipydriver-0.0.6/indipydriver/ipydriver.py
--rw-r--r--   0        0        0     8206 2023-07-09 10:17:52.000000 indipydriver-0.0.6/indipydriver/ipyserver.py
--rw-r--r--   0        0        0    11759 2023-07-09 08:25:23.000000 indipydriver-0.0.6/indipydriver/propertymembers.py
--rw-r--r--   0        0        0    42713 2023-07-08 21:53:53.000000 indipydriver-0.0.6/indipydriver/propertyvectors.py
--rw-r--r--   0        0        0      814 2023-07-08 14:16:54.000000 indipydriver-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 indipydriver-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-04 20:13:36.000000 indipydriver-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2411 2023-07-11 05:27:01.000000 indipydriver-0.0.7/README.md
+-rw-r--r--   0        0        0      573 2023-07-14 21:34:04.000000 indipydriver-0.0.7/indipydriver/__init__.py
+-rw-r--r--   0        0        0    17081 2023-07-09 09:46:38.000000 indipydriver-0.0.7/indipydriver/comms.py
+-rw-r--r--   0        0        0    21067 2023-07-09 10:33:24.000000 indipydriver-0.0.7/indipydriver/events.py
+-rw-r--r--   0        0        0    21510 2023-07-13 19:40:55.000000 indipydriver-0.0.7/indipydriver/ipydriver.py
+-rw-r--r--   0        0        0    10816 2023-07-13 20:27:03.000000 indipydriver-0.0.7/indipydriver/ipyserver.py
+-rw-r--r--   0        0        0    11759 2023-07-09 08:25:23.000000 indipydriver-0.0.7/indipydriver/propertymembers.py
+-rw-r--r--   0        0        0    42713 2023-07-08 21:53:53.000000 indipydriver-0.0.7/indipydriver/propertyvectors.py
+-rw-r--r--   0        0        0      814 2023-07-14 21:33:48.000000 indipydriver-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 indipydriver-0.0.7/PKG-INFO
```

### Comparing `indipydriver-0.0.6/LICENSE` & `indipydriver-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `indipydriver-0.0.6/README.md` & `indipydriver-0.0.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,34 +2,44 @@
 
 This is a pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver.
 
 INDI - Instrument Neutral Distributed Interface.
 
 See https://en.wikipedia.org/wiki/Instrument_Neutral_Distributed_Interface
 
-Typically the driver created with this package interfaces between your code which controls an instrument, or GPIO pins on the computer itself, and the INDI protocol which communicates to an INDI client. The protocol defines the format of the data sent, such as light, number, text or switch, and the client can send commands to control the instrument.  The client can be general purpose - communicating with any INDI driver, and taking the format of switches, numbers etc., from the protocol.
+Typically the driver created with this package interfaces between your code which controls an instrument, or GPIO pins on the computer itself, and the INDI protocol which communicates to an INDI client.
 
-INDI is normally used with astronomical instruments, but is a general purpose protocol which can be used for any instrument control providing drivers are available. This package is aimed at making drivers easy to write.
+This package can be used to create the drivers, it does not include client functions. The INDI protocol is defined so that drivers should operate with any INDI client.
+
+The protocol defines the format of the data sent, such as light, number, text or switch, and the client can send commands to control the instrument.  The client can be general purpose, taking the format of switches, numbers etc., from the protocol.
+
+INDI is often used with astronomical instruments, but is a general purpose protocol which can be used for any instrument control providing drivers are available.
 
 The driver object created contains 'device' objects, each of which can contain 'vector' objects, such as a SwitchVector or LightVector. These Vector objects can contain one or more 'members', such as a number of 'switches', or a number of 'lights'.
 
 Typically you would create a subclass of IPyDriver.
 
-The driver has two methods which should be overwritten.
+The driver has methods which should be overwritten.
 
 async def clientevent(self, event)
 
-This is called whenever data is received, the event object describes the received data, and you provide the code which then controls your instrument.
+This is called whenever data is received from the client, typically to set an instrument parameter. The event object describes the received data, and you provide the code which then controls your instrument.
 
 async def hardware(self)
 
-This should be a contuously running coroutine which you can use to poll your instruments, and if required send updates to the client.
+This should be a contuously running coroutine which you can use to operate your instruments, and if required send updates to the client.
+
+async def snoopevent(self, event)
 
-Finally you would run the driver asyncrun() method which runs the driver, typically called using:
+This is only used if one device is monitoring (snooping) on other devices.
+
+Having created an instance of your IPyDriver subclass, you would run the driver using:
 
 asyncio.run(driver.asyncrun())
 
-The driver can transmit/receive either by stdin/stdout, or by a port, typically localhost:7624 which is the INDI port number, and to which a client typically connects. If this is the only driver on the network, then the 'indiserver' (debian package indi-bin) software - which connects multiple drivers to a port - is not needed.
+The driver can transmit/receive either by stdin/stdout, or by a port.
+
+A further class provided in the package, IPyServer can operate with multiple driver instances, and serves them all via a port, a connected client can then control all the drivers.
 
 Documentation at https://indipydriver.readthedocs.io
 
 Installation from https://pypi.org/project/indipydriver
```

### Comparing `indipydriver-0.0.6/indipydriver/__init__.py` & `indipydriver-0.0.7/indipydriver/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 
 from .ipydriver import IPyDriver, Device
 from .propertyvectors import SwitchVector, LightVector, TextVector, BLOBVector, NumberVector
 from .propertymembers import SwitchMember, LightMember, TextMember, BLOBMember, NumberMember
 from .events import getProperties, enableBLOB, newSwitchVector, newTextVector, newNumberVector, newBLOBVector, Message, delProperty, defSwitchVector, defTextVector, defNumberVector, defLightVector, defBLOBVector, setSwitchVector, setTextVector, setNumberVector, setLightVector, setBLOBVector
 from .ipyserver import IPyServer
 
-version = "0.0.6"
+version = "0.0.7"
```

### Comparing `indipydriver-0.0.6/indipydriver/comms.py` & `indipydriver-0.0.7/indipydriver/comms.py`

 * *Files identical despite different names*

### Comparing `indipydriver-0.0.6/indipydriver/events.py` & `indipydriver-0.0.7/indipydriver/events.py`

 * *Files identical despite different names*

### Comparing `indipydriver-0.0.6/indipydriver/ipydriver.py` & `indipydriver-0.0.7/indipydriver/ipydriver.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,14 +96,21 @@
         self.snoopque = asyncio.Queue(4)
         # data for each device is passed to each device dataque
 
         # An object for communicating can be set, if not set, then
         # self.comms = STDINOUT() will be set in the asyncrun call
         self.comms = None
 
+        # These set the remote traffic which this driver is snooping
+        # initially the driver is not snooping anything, until it sends
+        # a getProperties
+        self.snoopall = False           # gets set to True if it is snooping everything
+        self.snoopdevices = set()       # gets set to a set of device names
+        self.snoopvectors = set()       # gets set to a set of (devicename,vectorname) tuples
+
 
     def _reporterror(self, message):
         "Prints message to stderr"
         print(message, file=sys.stderr)
 
     def listen(self, host="localhost", port=7624):
         """If called, listens on the given host and port. Only one connection is accepted,
@@ -250,24 +257,29 @@
     async def send_getProperties(self, devicename=None, vectorname=None):
         """Sends a getProperties request - which is used to snoop data from other devices
            on the network, if devicename given, it must not be a device of this driver as
            the point of this is to snoop on remote devices."""
         xmldata = ET.Element('getProperties')
         if devicename is None:
             await self.send(xmldata)
+            self.snoopall = True
             return
         if devicename in self.devices:
             self._reporterror("Cannot snoop on a device already controlled by this driver")
             return
         xmldata.set("device", devicename)
         if vectorname is None:
             await self.send(xmldata)
+            self.snoopdevices.add(devicename)
             return
         xmldata.set("name", vectorname)
         await self.send(xmldata)
+        # adds tuple (devicename,vectorname) to self.snoopvectors
+        self.snoopvectors.add((devicename,vectorname))
+
 
     async def hardware(self):
         """Override this to operate device hardware, and transmit updates
 
         For example: call your own code to operate hardware
         then update the appropriate vectors, and send updated
         values to the client using
```

### Comparing `indipydriver-0.0.6/indipydriver/ipyserver.py` & `indipydriver-0.0.7/indipydriver/ipyserver.py`

 * *Files 17% similar despite different names*

```diff
@@ -56,15 +56,21 @@
 
         self.connectionpool = []
         for clientconnection in range(0, maxconnections):
             self.connectionpool.append(_ClientConnection(self.devices, self.serverreaderque))
 
         for driver in drivers:
             # an instance of _DriverComms is created for each driver
-            driver.comms = _DriverComms(self.serverwriterque, self.connectionpool)
+            # each _DriverComms object has a list of drivers, not including its own driver
+            # these will be used to send snooping traffic, sent by its own driver
+            otherdrivers = [ d for d in drivers if not d is driver]
+            driver.comms = _DriverComms(self.serverwriterque, self.connectionpool, otherdrivers)
+
+        for driver in drivers:
+            driver.comms.otherdrivers = [ d for d in drivers if not d is driver]
 
         self.drivers = drivers
         self.host = host
         self.port = port
 
     async def runserver(self):
         "Runs the server on the given host and port"
@@ -99,19 +105,38 @@
 
 
     async def copyreceivedtodriversrxque(self):
         "For every driver, get rxque and copy data into it from serverreaderque"
         while True:
             await asyncio.sleep(0)
             xmldata = await self.serverreaderque.get()
-            for driver in self.drivers:
-                # should check data is for the driver
+            devicename = xmldata.get("device")
+            propertyname = xmldata.get("name")
+            if devicename is None:
+                # if no devicename - goes to every driver (getproperties)
+                for driver in self.drivers:
+                    await driver.comms.rxque.put(xmldata)
+            elif devicename in self.devices:
+                # self.devices is a dictionary of device name to device
+                driver = self.devices[devicename].driver
+                # data is intended for this driver
                 await driver.comms.rxque.put(xmldata)
+            else:
+                # devicename is unknown, check if driver is snooping on this device, vector
+                for driver in self.drivers:
+                    if driver.snoopall:
+                        await driver.comms.rxque.put(xmldata)
+                    elif devicename in driver.snoopdevices:
+                        await driver.comms.rxque.put(xmldata)
+                    elif not propertyname is None:
+                        if (devicename, propertyname) in driver.snoopvectors:
+                            await driver.comms.rxque.put(xmldata)
+                    # else not snooping, so don't bother sending it to the driver
             self.serverreaderque.task_done()
-            # now every driver.comms object has this xmldata in its rxque
+            # now every driver.comms object which needs it has this xmldata in its rxque
 
 
     async def copytransmittedtoclienttxque(self):
         "For every clientconnection, get txque and copy data into it from serverwriterque"
         while True:
             await asyncio.sleep(0)
             xmldata = await self.serverwriterque.get()
@@ -127,28 +152,31 @@
 
     """An instance of this is created for each driver, which calls the __call__
        method, expecting xmldata to be received from the client and placed
        in readerque, and any data the driver wishes to be sent should
        be taken from the writerque and transmitted to the client by placing it
        into the serverwriterque"""
 
-    def __init__(self, serverwriterque, connectionpool):
+    def __init__(self, serverwriterque, connectionpool, otherdrivers):
 
         # self.rxque will have data received from the network
         # inserted into it from the IPyServer.copyreceivedtodriversrxque()
         # method
         self.rxque = asyncio.Queue(6)
         self.serverwriterque = serverwriterque
         # connectionpool is a list of ClientConnection objects, which is used
         # to test if a client is connected
         self.connectionpool = connectionpool
         # self.connected is read by the driver, and in this case is always True
         # as the driver is connected to IPyServer, which handles snooping traffic,
         # even if no client is connected
         self.connected = True
+        # self.otherdrivers is set to a list of drivers, not including the driver
+        # this object is attached to.
+        self.otherdrivers = otherdrivers
 
 
     async def __call__(self, readerque, writerque):
         "Called by the driver, should run continuously to add and read the queues"
         await asyncio.gather(self.handleread(readerque),
                              self.handlewrite(writerque))
 
@@ -157,36 +185,50 @@
         while True:
             await asyncio.sleep(0)
             xmldata = await self.rxque.get()
             await readerque.put(xmldata)
             # task completed
             self.rxque.task_done()
 
-
     async def handlewrite(self, writerque):
         "reads writerque from the driver, and sends xml data to the network"
         while True:
             await asyncio.sleep(0)
             xmldata = await writerque.get()
-            # should check if this driver wants to snoop
-
+            # Check if other drivers wants to snoop this traffic
+            devicename = xmldata.get("device")
+            propertyname = xmldata.get("name")
+            if devicename is None:
+                # if no devicename - goes to every other driver (getproperties)
+                for driver in self.otherdrivers:
+                    await driver.comms.rxque.put(xmldata)
+            else:
+                for driver in self.otherdrivers:
+                    if driver.snoopall:
+                        await driver.comms.rxque.put(xmldata)
+                    elif devicename in driver.snoopdevices:
+                        await driver.comms.rxque.put(xmldata)
+                    elif not propertyname is None:
+                        if (devicename, propertyname) in driver.snoopvectors:
+                            await driver.comms.rxque.put(xmldata)
+            # traffic from one driver has been sent to other drivers if they want to snoop
+            # the traffic must also now be sent to the clients
             # If no clients are connected, do not put this data into
             # the serverwriterque
             for clientconnection in self.connectionpool:
                 if clientconnection.connected:
                     # at least one is connected, so this data is put into
                     # serverwriterque, and is then sent to each client by
                     # the copytransmittedtoclienttxque method.
                     await self.serverwriterque.put(xmldata)
                     break
             # task completed
             writerque.task_done()
 
 
-
 class _ClientConnection:
 
     "Handles a client connection"
 
     def __init__(self, devices, serverreaderque):
         # self.txque will have data to be transmitted
         # inserted into it from the IPyServer.copytransmittedtoclienttxque()
```

### Comparing `indipydriver-0.0.6/indipydriver/propertymembers.py` & `indipydriver-0.0.7/indipydriver/propertymembers.py`

 * *Files identical despite different names*

### Comparing `indipydriver-0.0.6/indipydriver/propertyvectors.py` & `indipydriver-0.0.7/indipydriver/propertyvectors.py`

 * *Files identical despite different names*

### Comparing `indipydriver-0.0.6/pyproject.toml` & `indipydriver-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipydriver"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.0.6"
+version = "0.0.7"
 description="Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'driver', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipydriver.readthedocs.io"
```

### Comparing `indipydriver-0.0.6/PKG-INFO` & `indipydriver-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipydriver
-Version: 0.0.6
+Version: 0.0.7
 Summary: Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver.
 Keywords: indi,driver,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -17,35 +17,45 @@
 
 This is a pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver.
 
 INDI - Instrument Neutral Distributed Interface.
 
 See https://en.wikipedia.org/wiki/Instrument_Neutral_Distributed_Interface
 
-Typically the driver created with this package interfaces between your code which controls an instrument, or GPIO pins on the computer itself, and the INDI protocol which communicates to an INDI client. The protocol defines the format of the data sent, such as light, number, text or switch, and the client can send commands to control the instrument.  The client can be general purpose - communicating with any INDI driver, and taking the format of switches, numbers etc., from the protocol.
+Typically the driver created with this package interfaces between your code which controls an instrument, or GPIO pins on the computer itself, and the INDI protocol which communicates to an INDI client.
 
-INDI is normally used with astronomical instruments, but is a general purpose protocol which can be used for any instrument control providing drivers are available. This package is aimed at making drivers easy to write.
+This package can be used to create the drivers, it does not include client functions. The INDI protocol is defined so that drivers should operate with any INDI client.
+
+The protocol defines the format of the data sent, such as light, number, text or switch, and the client can send commands to control the instrument.  The client can be general purpose, taking the format of switches, numbers etc., from the protocol.
+
+INDI is often used with astronomical instruments, but is a general purpose protocol which can be used for any instrument control providing drivers are available.
 
 The driver object created contains 'device' objects, each of which can contain 'vector' objects, such as a SwitchVector or LightVector. These Vector objects can contain one or more 'members', such as a number of 'switches', or a number of 'lights'.
 
 Typically you would create a subclass of IPyDriver.
 
-The driver has two methods which should be overwritten.
+The driver has methods which should be overwritten.
 
 async def clientevent(self, event)
 
-This is called whenever data is received, the event object describes the received data, and you provide the code which then controls your instrument.
+This is called whenever data is received from the client, typically to set an instrument parameter. The event object describes the received data, and you provide the code which then controls your instrument.
 
 async def hardware(self)
 
-This should be a contuously running coroutine which you can use to poll your instruments, and if required send updates to the client.
+This should be a contuously running coroutine which you can use to operate your instruments, and if required send updates to the client.
+
+async def snoopevent(self, event)
 
-Finally you would run the driver asyncrun() method which runs the driver, typically called using:
+This is only used if one device is monitoring (snooping) on other devices.
+
+Having created an instance of your IPyDriver subclass, you would run the driver using:
 
 asyncio.run(driver.asyncrun())
 
-The driver can transmit/receive either by stdin/stdout, or by a port, typically localhost:7624 which is the INDI port number, and to which a client typically connects. If this is the only driver on the network, then the 'indiserver' (debian package indi-bin) software - which connects multiple drivers to a port - is not needed.
+The driver can transmit/receive either by stdin/stdout, or by a port.
+
+A further class provided in the package, IPyServer can operate with multiple driver instances, and serves them all via a port, a connected client can then control all the drivers.
 
 Documentation at https://indipydriver.readthedocs.io
 
 Installation from https://pypi.org/project/indipydriver
```

