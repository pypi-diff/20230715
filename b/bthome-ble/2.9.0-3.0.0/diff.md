# Comparing `tmp/bthome_ble-2.9.0.tar.gz` & `tmp/bthome_ble-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bthome_ble-2.9.0.tar", max compression
+gzip compressed data, was "bthome_ble-3.0.0.tar", max compression
```

## Comparing `bthome_ble-2.9.0.tar` & `bthome_ble-3.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-03-12 18:06:38.418232 bthome_ble-2.9.0/LICENSE
--rw-r--r--   0        0        0     3675 2023-03-12 18:06:38.418232 bthome_ble-2.9.0/README.md
--rw-r--r--   0        0        0     2379 2023-03-12 18:06:39.210245 bthome_ble-2.9.0/pyproject.toml
--rw-r--r--   0        0        0      610 2023-03-12 18:06:39.174244 bthome_ble-2.9.0/src/bthome_ble/__init__.py
--rw-r--r--   0        0        0     3588 2023-03-12 18:06:38.418232 bthome_ble-2.9.0/src/bthome_ble/bthome_v1_encryption.py
--rw-r--r--   0        0        0     3739 2023-03-12 18:06:38.418232 bthome_ble-2.9.0/src/bthome_ble/bthome_v2_encryption.py
--rw-r--r--   0        0        0    10015 2023-03-12 18:06:38.418232 bthome_ble-2.9.0/src/bthome_ble/const.py
--rw-r--r--   0        0        0      649 2023-03-12 18:06:38.418232 bthome_ble-2.9.0/src/bthome_ble/event.py
--rw-r--r--   0        0        0    20586 2023-03-12 18:06:38.418232 bthome_ble-2.9.0/src/bthome_ble/parser.py
--rw-r--r--   0        0        0        0 2023-03-12 18:06:38.418232 bthome_ble-2.9.0/src/bthome_ble/py.typed
--rw-r--r--   0        0        0     5129 1970-01-01 00:00:00.000000 bthome_ble-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-15 21:51:51.949743 bthome_ble-3.0.0/LICENSE
+-rw-r--r--   0        0        0     3675 2023-07-15 21:51:51.949743 bthome_ble-3.0.0/README.md
+-rw-r--r--   0        0        0     2395 2023-07-15 21:51:52.753757 bthome_ble-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      610 2023-07-15 21:51:52.721756 bthome_ble-3.0.0/src/bthome_ble/__init__.py
+-rw-r--r--   0        0        0     3604 2023-07-15 21:51:51.949743 bthome_ble-3.0.0/src/bthome_ble/bthome_v1_encryption.py
+-rw-r--r--   0        0        0     3765 2023-07-15 21:51:51.949743 bthome_ble-3.0.0/src/bthome_ble/bthome_v2_encryption.py
+-rw-r--r--   0        0        0    10458 2023-07-15 21:51:51.949743 bthome_ble-3.0.0/src/bthome_ble/const.py
+-rw-r--r--   0        0        0      649 2023-07-15 21:51:51.949743 bthome_ble-3.0.0/src/bthome_ble/event.py
+-rw-r--r--   0        0        0    22304 2023-07-15 21:51:51.949743 bthome_ble-3.0.0/src/bthome_ble/parser.py
+-rw-r--r--   0        0        0        0 2023-07-15 21:51:51.949743 bthome_ble-3.0.0/src/bthome_ble/py.typed
+-rw-r--r--   0        0        0     5167 1970-01-01 00:00:00.000000 bthome_ble-3.0.0/PKG-INFO
```

### Comparing `bthome_ble-2.9.0/LICENSE` & `bthome_ble-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bthome_ble-2.9.0/README.md` & `bthome_ble-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `bthome_ble-2.9.0/pyproject.toml` & `bthome_ble-3.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bthome-ble"
-version = "2.9.0"
+version = "3.0.0"
 description = "BThome BLE support"
 authors = ["Ernst Klamer <e.klamer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/bthome-ble"
 documentation = "https://bthome-ble.readthedocs.io"
 classifiers = [
@@ -26,17 +26,18 @@
 python = "^3.9"
 
 # Documentation Dependencies
 Sphinx = {version = "^5.0", optional = true}
 sphinx-rtd-theme = {version = "^1.0", optional = true}
 myst-parser = {version = "^0.18", optional = true}
 bluetooth-sensor-state-data = ">=1.6.1"
-pycryptodomex = ">=3.15.0"
-sensor-state-data = ">=2.14.0"
+sensor-state-data = ">=2.16.1"
 bluetooth-data-tools = ">=0.1.2"
+pytz = "^2023.3"
+cryptography = ">=40.0.0"
 
 [tool.poetry.extras]
 docs = [
     "myst-parser",
     "sphinx",
     "sphinx-rtd-theme",
 ]
```

### Comparing `bthome_ble-2.9.0/src/bthome_ble/__init__.py` & `bthome_ble-3.0.0/src/bthome_ble/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     SensorUpdate,
     SensorValue,
     Units,
 )
 
 from .parser import BTHomeBluetoothDeviceData
 
-__version__ = "2.9.0"
+__version__ = "3.0.0"
 
 __all__ = [
     "BinarySensorDeviceClass",
     "BTHomeBluetoothDeviceData",
     "DeviceClass",
     "DeviceKey",
     "SensorDescription",
```

### Comparing `bthome_ble-2.9.0/src/bthome_ble/bthome_v1_encryption.py` & `bthome_ble-3.0.0/src/bthome_ble/bthome_v1_encryption.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Example showing encoding and decoding of BTHome v1 advertisement"""
 from __future__ import annotations
 
 import binascii
 
-from Cryptodome.Cipher import AES
+from cryptography.hazmat.primitives.ciphers.aead import AESCCM
 
 
 def parse_value(data: bytes) -> dict[str, float]:
     """Parse decrypted payload to readable BTHome data"""
     vlength = len(data)
     if vlength >= 3:
         temp = round(int.from_bytes(data[2:4], "little", signed=False) * 0.01, 2)
@@ -21,20 +21,19 @@
 def decrypt_payload(
     payload: bytes, mic: bytes, key: bytes, nonce: bytes
 ) -> dict[str, float] | None:
     """Decrypt payload."""
     print("Nonce:", nonce.hex())
     print("CryptData:", payload.hex())
     print("Mic:", mic.hex())
-    cipher = AES.new(key, AES.MODE_CCM, nonce=nonce, mac_len=4)
-    cipher.update(b"\x11")
+    cipher = AESCCM(key, tag_length=4)
     print()
     print("Starting Decryption data")
     try:
-        data = cipher.decrypt_and_verify(payload, mic)
+        data = cipher.decrypt(nonce, payload + mic, b"\x11")
     except ValueError as error:
         print()
         print("Decryption failed:", error)
         return None
     print("Decryption succeeded, decrypted data:", data.hex())
     print()
     return parse_value(data=data)
@@ -60,17 +59,19 @@
 
 
 def encrypt_payload(
     data: bytes, mac: bytes, uuid16: bytes, count_id: bytes, key: bytes
 ) -> bytes:
     """Encrypt payload."""
     nonce = b"".join([mac, uuid16, count_id])  # 6+2+4 = 12 bytes
-    cipher = AES.new(key, AES.MODE_CCM, nonce=nonce, mac_len=4)
-    cipher.update(b"\x11")
-    ciphertext, mic = cipher.encrypt_and_digest(data)
+    cipher = AESCCM(key, tag_length=4)
+    associated_data = b"\x11"
+    result = cipher.encrypt(nonce, data, associated_data)
+    ciphertext = result[:-4]
+    mic = result[-4:]
     print("MAC:", mac.hex())
     print("Binkey:", key.hex())
     print("Data:", data.hex())
     print("Nonce:", nonce.hex())
     print("CryptData:", ciphertext.hex(), "Mic:", mic.hex())
     return b"".join([uuid16, ciphertext, count_id, mic])
```

### Comparing `bthome_ble-2.9.0/src/bthome_ble/bthome_v2_encryption.py` & `bthome_ble-3.0.0/src/bthome_ble/bthome_v2_encryption.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Example showing encoding and decoding of BTHome v2 advertisement"""
 from __future__ import annotations
 
 import binascii
 
-from Cryptodome.Cipher import AES
+from cryptography.hazmat.primitives.ciphers.aead import AESCCM
 
 
 def parse_value(data: bytes) -> dict[str, float]:
     """Parse decrypted payload to readable BTHome data"""
     vlength = len(data)
     if vlength >= 3:
         temp = round(int.from_bytes(data[1:3], "little", signed=False) * 0.01, 2)
@@ -21,19 +21,19 @@
 def decrypt_payload(
     payload: bytes, mic: bytes, key: bytes, nonce: bytes
 ) -> dict[str, float] | None:
     """Decrypt payload."""
     print("Nonce:", nonce.hex())
     print("Ciphertext:", payload.hex())
     print("MIC:", mic.hex())
-    cipher = AES.new(key, AES.MODE_CCM, nonce=nonce, mac_len=4)
+    cipher = AESCCM(key, tag_length=4)
     print()
     print("Starting Decryption data")
     try:
-        data = cipher.decrypt_and_verify(payload, mic)
+        data = cipher.decrypt(nonce, payload + mic, None)
     except ValueError as error:
         print()
         print("Decryption failed:", error)
         return None
     print("Decryption succeeded, decrypted data:", data.hex())
     print()
     return parse_value(data=data)
@@ -65,16 +65,18 @@
     uuid16: bytes,
     sw_version: bytes,
     count_id: bytes,
     key: bytes,
 ) -> bytes:
     """Encrypt payload."""
     nonce = b"".join([mac, uuid16, sw_version, count_id])  # 6+2+1+4 = 13 bytes
-    cipher = AES.new(key, AES.MODE_CCM, nonce=nonce, mac_len=4)
-    ciphertext, mic = cipher.encrypt_and_digest(data)
+    cipher = AESCCM(key, tag_length=4)
+    result = cipher.encrypt(nonce, data, None)
+    ciphertext = result[:-4]
+    mic = result[-4:]
     print("MAC:", mac.hex())
     print("Binkey:", key.hex())
     print("Data:", data.hex())
     print("Nonce:", nonce.hex())
     print("Ciphertext:", ciphertext.hex())
     print("MIC:", mic.hex())
     return b"".join([uuid16, sw_version, ciphertext, count_id, mic])
```

### Comparing `bthome_ble-2.9.0/src/bthome_ble/const.py` & `bthome_ble-3.0.0/src/bthome_ble/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -338,8 +338,23 @@
         factor=0.001,
     ),
     0x4F: MeasTypes(
         meas_format=SensorLibrary.WATER__VOLUME_LITERS,
         data_length=4,
         factor=0.001,
     ),
+    0x50: MeasTypes(
+        meas_format=SensorLibrary.TIMESTAMP__NONE,
+        data_length=4,
+        data_format="timestamp",
+    ),
+    0x51: MeasTypes(
+        meas_format=SensorLibrary.ACCELERATION__ACCELERATION_METERS_PER_SQUARE_SECOND,
+        data_length=2,
+        factor=0.001,
+    ),
+    0x52: MeasTypes(
+        meas_format=SensorLibrary.GYROSCOPE__GYROSCOPE_DEGREES_PER_SECOND,
+        data_length=2,
+        factor=0.001,
+    ),
 }
```

### Comparing `bthome_ble-2.9.0/src/bthome_ble/event.py` & `bthome_ble-3.0.0/src/bthome_ble/event.py`

 * *Files identical despite different names*

### Comparing `bthome_ble-2.9.0/src/bthome_ble/parser.py` & `bthome_ble-3.0.0/src/bthome_ble/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,34 +9,36 @@
 MIT License applies.
 """
 from __future__ import annotations
 
 import logging
 import struct
 import sys
+from datetime import datetime
 from enum import Enum
 from typing import Any
 
+import pytz
 from bluetooth_data_tools import short_address
 from bluetooth_sensor_state_data import BluetoothData
-from Cryptodome.Cipher import AES
+from cryptography.exceptions import InvalidTag
+from cryptography.hazmat.primitives.ciphers.aead import AESCCM
 from home_assistant_bluetooth import BluetoothServiceInfo
 from sensor_state_data.description import (
     BaseBinarySensorDescription,
     BaseSensorDescription,
 )
 
 from .const import MEAS_TYPES
 from .event import BUTTON_EVENTS, DIMMER_EVENTS, EventDeviceKeys
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class EncryptionScheme(Enum):
-
     # No encryption is needed to use this device
     NONE = "none"
 
     # 16 byte encryption key expected
     BTHOME_BINDKEY = "bthome_bindkey"
 
 
@@ -77,20 +79,27 @@
 
 
 def parse_string(data_obj: bytes) -> str:
     """Convert bytes to string."""
     return data_obj.decode("UTF-8")
 
 
+def parse_timestamp(data_obj: bytes) -> datetime:
+    """Convert bytes to a datetime object."""
+    value = datetime.utcfromtimestamp(int.from_bytes(data_obj, "little", signed=False))
+    _LOGGER.error("time %s", value)
+    return pytz.utc.localize(value)
+
+
 def parse_event_type(event_device: str, data_obj: int) -> str | None:
     """Convert bytes to event type."""
     if event_device == "dimmer":
-        event_type = DIMMER_EVENTS[data_obj]
+        event_type = DIMMER_EVENTS.get(data_obj)
     elif event_device == "button":
-        event_type = BUTTON_EVENTS[data_obj]
+        event_type = BUTTON_EVENTS.get(data_obj)
     else:
         event_type = None
     return event_type
 
 
 def parse_event_properties(
     event_device: str, data_obj: bytes
@@ -104,42 +113,53 @@
 
 
 class BTHomeBluetoothDeviceData(BluetoothData):
     """Data for BTHome Bluetooth devices."""
 
     def __init__(self, bindkey: bytes | None = None) -> None:
         super().__init__()
-        self.bindkey = bindkey
+        self.set_bindkey(bindkey)
 
         # Data that we know how to parse but don't yet map to the SensorData model.
         self.unhandled: dict[str, Any] = {}
 
         # Encryption to expect, based on flags in the UUID.
         self.encryption_scheme = EncryptionScheme.NONE
 
-        # If true, then we know the actual MAC of the device.
+        # If True, then we know the actual MAC of the device.
         # On macOS, we don't unless the device includes it in the advertisement
         # (CoreBluetooth uses UUID's generated by CoreBluetooth instead of the MAC)
         self.mac_known = sys.platform != "darwin"
 
-        # If true then we have used the provided encryption key to decrypt at least
+        # If True then we have used the provided encryption key to decrypt at least
         # one payload.
-        # If false then we have either not seen an encrypted payload, the key is wrong
+        # If False then we have either not seen an encrypted payload, the key is wrong
         # or encryption is not in use
         self.bindkey_verified = False
 
         # If this is True, then we have not seen an advertisement with a payload
         # Until we see a payload, we can't tell if this device is encrypted or not
         self.pending = True
 
         # The last service_info we saw that had a payload
         # We keep this to help in reauth flows where we want to reprocess and old
         # value with a new bindkey.
         self.last_service_info: BluetoothServiceInfo | None = None
 
+        # If this is True, the device is not sending advertisements in a regular interval
+        self.sleepy_device = False
+
+    def set_bindkey(self, bindkey: bytes | None) -> None:
+        """Set the bindkey."""
+        self.bindkey = bindkey
+        if bindkey:
+            self.cipher: AESCCM | None = AESCCM(bindkey, tag_length=4)
+        else:
+            self.cipher = None
+
     def supported(self, data: BluetoothServiceInfo) -> bool:
         if not super().supported(data):
             return False
 
         # Where a device uses encryption we need to know its actual MAC address.
         # As the encryption uses it as part of the nonce.
         # On macOS, we instead only know its CoreBluetooth UUID.
@@ -251,14 +271,27 @@
         # Determine if encryption is used
         encryption = adv_info & (1 << 0)  # bit 0
         if encryption == 1:
             self.encryption_scheme = EncryptionScheme.BTHOME_BINDKEY
         else:
             self.encryption_scheme = EncryptionScheme.NONE
 
+        # If True, the first 6 bytes contain the mac address
+        mac_included = adv_info & (1 << 1)  # bit 1
+        if mac_included:
+            bthome_mac_reversed = data[1:7]
+            mac_readable = to_mac(bthome_mac_reversed[::-1])
+            payload = data[7:]
+        else:
+            mac_readable = service_info.address
+            payload = data[1:]
+
+        # If True, the device is only updating when triggered
+        self.sleepy_device = bool(adv_info & (1 << 2))  # bit 2
+
         # Check BTHome version
         sw_version = (adv_info >> 5) & 7  # 3 bits (5-7)
         if sw_version == 2:
             if self.encryption_scheme == EncryptionScheme.BTHOME_BINDKEY:
                 self.set_device_sw_version(f"BTHome BLE v{sw_version} (encrypted)")
             else:
                 self.set_device_sw_version(f"BTHome BLE v{sw_version}")
@@ -269,49 +302,53 @@
                 sw_version,
             )
             return False
 
         # Try to get manufacturer based on the name
         if name.startswith(("ATC", "LYWSD03MMC")):
             manufacturer = "Xiaomi"
+            device_type = "Temperature/Humidity sensor"
         elif name.startswith("prst"):
             manufacturer = "b-parasite"
             name = "b-parasite"
+            device_type = "Plant sensor"
+        elif name.startswith("SBBT"):
+            manufacturer = "Shelly"
+            name = "Shelly BLU Button1"
+            device_type = "BLU Button1"
+        elif name.startswith("SBDW"):
+            manufacturer = "Shelly"
+            name = "Shelly BLU Door/Window"
+            device_type = "BLU Door/Window"
         else:
             manufacturer = None
+            device_type = "BTHome sensor"
 
         if manufacturer:
             self.set_device_manufacturer(manufacturer)
 
         # Get device information from local name and identifier
         self.set_device_name(f"{name} {identifier}")
         self.set_title(f"{name} {identifier}")
-        self.set_device_type("BTHome sensor")
-
-        mac_included = adv_info & (1 << 1)  # bit 1
-        if mac_included:
-            bthome_mac_reversed = data[1:7]
-            mac_readable = to_mac(bthome_mac_reversed[::-1])
-            payload = data[7:]
-        else:
-            mac_readable = service_info.address
-            payload = data[1:]
+        self.set_device_type(device_type)
 
         if self.encryption_scheme == EncryptionScheme.BTHOME_BINDKEY:
             if len(mac_readable) != 17 and mac_readable[2] != ":":
                 # On macOS, we get a UUID, which is useless for BTHome sensors
                 # Unless the MAC address is specified in the payload
                 self.mac_known = False
                 return False
             else:
                 self.mac_known = True
             bthome_mac = bytes.fromhex(mac_readable.replace(":", ""))
             # Decode encrypted payload
             try:
-                payload = self._decrypt_bthome(payload, bthome_mac, sw_version)
+                payload = self._decrypt_bthome(
+                    payload, bthome_mac, sw_version, adv_info
+                )
             except (ValueError, TypeError):
                 return True
 
         return self._parse_payload(payload, sw_version)
 
     def _parse_payload(self, payload: bytes, sw_version: int) -> bool:
         payload_length = len(payload)
@@ -405,24 +442,25 @@
                 # Add a postfix for advertisements with multiple measurements of the same type
                 postfix_counter = postfix_dict.get(meas_format, 0) + 1
                 postfix_dict[meas_format] = postfix_counter
                 postfix = f"_{postfix_counter}"
             else:
                 postfix = ""
 
-            value: None | str | int | float
-
+            value: None | str | int | float | datetime
             if meas["data format"] == 0 or meas["data format"] == "unsigned_integer":
                 value = parse_uint(meas["measurement data"], meas_factor)
             elif meas["data format"] == 1 or meas["data format"] == "signed_integer":
                 value = parse_int(meas["measurement data"], meas_factor)
             elif meas["data format"] == 2 or meas["data format"] == "float":
                 value = parse_float(meas["measurement data"], meas_factor)
             elif meas["data format"] == 3 or meas["data format"] == "string":
                 value = parse_string(meas["measurement data"])
+            elif meas["data format"] == 5 or meas["data format"] == "timestamp":
+                value = parse_timestamp(meas["measurement data"])
             else:
                 _LOGGER.error(
                     "UNKNOWN dataobject in BTHome BLE payload! Adv: %s",
                     payload.hex(),
                 )
                 continue
 
@@ -469,15 +507,17 @@
                 )
 
         if not result:
             return False
 
         return True
 
-    def _decrypt_bthome(self, data: bytes, bthome_mac: bytes, sw_version: int) -> bytes:
+    def _decrypt_bthome(
+        self, data: bytes, bthome_mac: bytes, sw_version: int, adv_info: int = 65
+    ) -> bytes:
         """Decrypt encrypted BTHome BLE advertisements"""
         if not self.bindkey:
             self.bindkey_verified = False
             _LOGGER.debug("Encryption key not set and adv is encrypted")
             raise ValueError
 
         if not self.bindkey or len(self.bindkey) != 16:
@@ -490,29 +530,33 @@
             _LOGGER.debug("Invalid data length (for decryption), adv: %s", data.hex())
             raise ValueError
 
         # prepare the data for decryption
         if sw_version == 1:
             uuid = b"\x1e\x18"
         else:
-            uuid = b"\xd2\xfc\x41"
+            uuid = b"\xd2\xfc" + bytes([adv_info])
         encrypted_payload = data[:-8]
         count_id = data[-8:-4]
         mic = data[-4:]
 
         # nonce: mac [6], uuid16 [2 (v1) or 3 (v2)], count_id [4]
         nonce = b"".join([bthome_mac, uuid, count_id])
-        cipher = AES.new(self.bindkey, AES.MODE_CCM, nonce=nonce, mac_len=4)
+
+        associated_data = None
         if sw_version == 1:
-            cipher.update(b"\x11")
+            associated_data = b"\x11"
 
+        assert self.cipher is not None  # nosec
         # decrypt the data
         try:
-            decrypted_payload = cipher.decrypt_and_verify(encrypted_payload, mic)
-        except ValueError as error:
+            decrypted_payload = self.cipher.decrypt(
+                nonce, encrypted_payload + mic, associated_data
+            )
+        except InvalidTag as error:
             self.bindkey_verified = False
             _LOGGER.warning("Decryption failed: %s", error)
             _LOGGER.debug("mic: %s", mic.hex())
             _LOGGER.debug("nonce: %s", nonce.hex())
             _LOGGER.debug("encrypted_payload: %s", encrypted_payload.hex())
             raise ValueError
         if decrypted_payload is None:
```

### Comparing `bthome_ble-2.9.0/PKG-INFO` & `bthome_ble-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bthome-ble
-Version: 2.9.0
+Version: 3.0.0
 Summary: BThome BLE support
 Home-page: https://github.com/bluetooth-devices/bthome-ble
 License: MIT
 Author: Ernst Klamer
 Author-email: e.klamer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -17,17 +17,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=5.0,<6.0) ; extra == "docs"
 Requires-Dist: bluetooth-data-tools (>=0.1.2)
 Requires-Dist: bluetooth-sensor-state-data (>=1.6.1)
+Requires-Dist: cryptography (>=40.0.0)
 Requires-Dist: myst-parser (>=0.18,<0.19) ; extra == "docs"
-Requires-Dist: pycryptodomex (>=3.15.0)
-Requires-Dist: sensor-state-data (>=2.14.0)
+Requires-Dist: pytz (>=2023.3,<2024.0)
+Requires-Dist: sensor-state-data (>=2.16.1)
 Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0) ; extra == "docs"
 Project-URL: Bug Tracker, https://github.com/bluetooth-devices/bthome-ble/issues
 Project-URL: Changelog, https://github.com/bluetooth-devices/bthome-ble/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://bthome-ble.readthedocs.io
 Project-URL: Repository, https://github.com/bluetooth-devices/bthome-ble
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: bthome-ble Version: 2.9.0 Summary: BThome BLE
+Metadata-Version: 2.1 Name: bthome-ble Version: 3.0.0 Summary: BThome BLE
 support Home-page: https://github.com/bluetooth-devices/bthome-ble License: MIT
 Author: Ernst Klamer Author-email: e.klamer@gmail.com Requires-Python:
 >=3.9,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Software Development :: Libraries Provides-Extra: docs Requires-Dist:
 Sphinx (>=5.0,<6.0) ; extra == "docs" Requires-Dist: bluetooth-data-tools
 (>=0.1.2) Requires-Dist: bluetooth-sensor-state-data (>=1.6.1) Requires-Dist:
-myst-parser (>=0.18,<0.19) ; extra == "docs" Requires-Dist: pycryptodomex
-(>=3.15.0) Requires-Dist: sensor-state-data (>=2.14.0) Requires-Dist: sphinx-
-rtd-theme (>=1.0,<2.0) ; extra == "docs" Project-URL: Bug Tracker, https://
-github.com/bluetooth-devices/bthome-ble/issues Project-URL: Changelog, https://
-github.com/bluetooth-devices/bthome-ble/blob/main/CHANGELOG.md Project-URL:
-Documentation, https://bthome-ble.readthedocs.io Project-URL: Repository,
-https://github.com/bluetooth-devices/bthome-ble Description-Content-Type: text/
-markdown # BTHome BLE
+cryptography (>=40.0.0) Requires-Dist: myst-parser (>=0.18,<0.19) ; extra ==
+"docs" Requires-Dist: pytz (>=2023.3,<2024.0) Requires-Dist: sensor-state-data
+(>=2.16.1) Requires-Dist: sphinx-rtd-theme (>=1.0,<2.0) ; extra == "docs"
+Project-URL: Bug Tracker, https://github.com/bluetooth-devices/bthome-ble/
+issues Project-URL: Changelog, https://github.com/bluetooth-devices/bthome-ble/
+blob/main/CHANGELOG.md Project-URL: Documentation, https://bthome-
+ble.readthedocs.io Project-URL: Repository, https://github.com/bluetooth-
+devices/bthome-ble Description-Content-Type: text/markdown # BTHome BLE
          [CI_Status] [Documentation_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 BLE parser for sensors that support the BTHome BLE format (V1 and V2). ##
 Installation Install this via pip (or your favourite package manager): `pip
 install bthome-ble` ## BThome BLE format More detailed information about the
 BTHome BLE format can be found on the [usage page](https://bthome.io/) ##
```

