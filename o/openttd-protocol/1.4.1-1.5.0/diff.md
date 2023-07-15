# Comparing `tmp/openttd-protocol-1.4.1.tar.gz` & `tmp/openttd-protocol-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openttd-protocol-1.4.1.tar", last modified: Sun Oct 17 09:06:22 2021, max compression
+gzip compressed data, was "openttd-protocol-1.5.0.tar", last modified: Sat Jul 15 11:11:45 2023, max compression
```

## Comparing `openttd-protocol-1.4.1.tar` & `openttd-protocol-1.5.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 09:06:22.531988 openttd-protocol-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)    26521 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       35 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2950 2021-10-17 09:06:22.531988 openttd-protocol-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2039 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-10-17 09:06:22.000000 openttd-protocol-1.4.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 09:06:22.531988 openttd-protocol-1.4.1/openttd_protocol/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/openttd_protocol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 09:06:22.531988 openttd-protocol-1.4.1/openttd_protocol/protocol/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/openttd_protocol/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9581 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/openttd_protocol/protocol/content.py
--rw-r--r--   0 runner    (1001) docker     (121)    21389 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/openttd_protocol/protocol/coordinator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6169 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/openttd_protocol/protocol/game.py
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/openttd_protocol/protocol/stun.py
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/openttd_protocol/protocol/turn.py
--rw-r--r--   0 runner    (1001) docker     (121)      863 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/openttd_protocol/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 09:06:22.531988 openttd-protocol-1.4.1/openttd_protocol/wire/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/openttd_protocol/wire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      661 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/openttd_protocol/wire/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2710 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/openttd_protocol/wire/read.py
--rw-r--r--   0 runner    (1001) docker     (121)      795 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/openttd_protocol/wire/source.py
--rw-r--r--   0 runner    (1001) docker     (121)     7984 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/openttd_protocol/wire/tcp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1459 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/openttd_protocol/wire/test_read.py
--rw-r--r--   0 runner    (1001) docker     (121)     3880 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/openttd_protocol/wire/test_tcp.py
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/openttd_protocol/wire/test_write.py
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/openttd_protocol/wire/write.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-17 09:06:22.531988 openttd-protocol-1.4.1/openttd_protocol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2950 2021-10-17 09:06:22.000000 openttd-protocol-1.4.1/openttd_protocol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      788 2021-10-17 09:06:22.000000 openttd-protocol-1.4.1/openttd_protocol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-17 09:06:22.000000 openttd-protocol-1.4.1/openttd_protocol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-10-17 09:06:22.000000 openttd-protocol-1.4.1/openttd_protocol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-17 09:06:22.531988 openttd-protocol-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      752 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2021-10-17 09:06:12.000000 openttd-protocol-1.4.1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:11:45.925711 openttd-protocol-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26521 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-15 11:11:45.921711 openttd-protocol-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-15 11:11:45.000000 openttd-protocol-1.5.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:11:45.921711 openttd-protocol-1.5.0/openttd_protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:11:45.921711 openttd-protocol-1.5.0/openttd_protocol/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/protocol/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20789 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/protocol/coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/protocol/game.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/protocol/stun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/protocol/turn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:11:45.921711 openttd-protocol-1.5.0/openttd_protocol/wire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/wire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/wire/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/wire/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/wire/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7704 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/wire/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/wire/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/wire/test_tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/wire/test_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/openttd_protocol/wire/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:11:45.921711 openttd-protocol-1.5.0/openttd_protocol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-15 11:11:45.000000 openttd-protocol-1.5.0/openttd_protocol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-15 11:11:45.000000 openttd-protocol-1.5.0/openttd_protocol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 11:11:45.000000 openttd-protocol-1.5.0/openttd_protocol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-15 11:11:45.000000 openttd-protocol-1.5.0/openttd_protocol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 11:11:45.925711 openttd-protocol-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-15 11:11:34.000000 openttd-protocol-1.5.0/version.py
```

### Comparing `openttd-protocol-1.4.1/LICENSE` & `openttd-protocol-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.4.1/PKG-INFO` & `openttd-protocol-1.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openttd-protocol
-Version: 1.4.1
+Version: 1.5.0
 Summary: OpenTTD network protocol for Python
 Home-page: https://github.com/OpenTTD/py-protocol
 Author: OpenTTD Dev Team
 Author-email: info@openttd.org
 License: UNKNOWN
 Description: # openttd-protocol
```

### Comparing `openttd-protocol-1.4.1/README.md` & `openttd-protocol-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.4.1/openttd_protocol/protocol/content.py` & `openttd-protocol-1.5.0/openttd_protocol/protocol/content.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import enum
 import logging
 import struct
 
-from .. import tracer
 from ..wire.exceptions import PacketInvalidData
 from ..wire.read import (
     read_string,
     read_uint8,
     read_uint16,
     read_uint32,
 )
@@ -68,15 +67,14 @@
 
 
 class ContentProtocol(TCPProtocol):
     PacketType = PacketContentType
     PACKET_END = PacketContentType.PACKET_CONTENT_END
 
     @staticmethod
-    @tracer.traced("content")
     def receive_PACKET_CONTENT_CLIENT_INFO_LIST(source, data):
         content_type, data = read_uint8(data)
         openttd_version, data = read_uint32(data)
 
         # Since OpenTTD 12.0 we extended this packet to include multiple
         # branches and their versions, so patchpacks can filter the list
         # based on their version. This is indicated by sending an
@@ -139,64 +137,59 @@
                 content_info["md5sum"] = md5sum
 
             content_infos.append(ContentInfo(**content_info))
 
         return content_infos, data
 
     @classmethod
-    @tracer.traced("content")
     def receive_PACKET_CONTENT_CLIENT_INFO_ID(cls, source, data):
         count, data = read_uint16(data)
 
         content_infos, data = cls._receive_client_info(data, count, has_content_id=True)
 
         if len(data) != 0:
             raise PacketInvalidData("more bytes than expected; remaining: ", len(data))
 
         return {"content_infos": content_infos}
 
     @classmethod
-    @tracer.traced("content")
     def receive_PACKET_CONTENT_CLIENT_INFO_EXTID(cls, source, data):
         count, data = read_uint8(data)
 
         content_infos, data = cls._receive_client_info(data, count, has_content_type_and_unique_id=True)
 
         if len(data) != 0:
             raise PacketInvalidData("more bytes than expected; remaining: ", len(data))
 
         return {"content_infos": content_infos}
 
     @classmethod
-    @tracer.traced("content")
     def receive_PACKET_CONTENT_CLIENT_INFO_EXTID_MD5(cls, source, data):
         count, data = read_uint8(data)
 
         content_infos, data = cls._receive_client_info(
             data, count, has_content_type_and_unique_id=True, has_md5sum=True
         )
 
         if len(data) != 0:
             raise PacketInvalidData("more bytes than expected; remaining: ", len(data))
 
         return {"content_infos": content_infos}
 
     @classmethod
-    @tracer.traced("content")
     def receive_PACKET_CONTENT_CLIENT_CONTENT(cls, source, data):
         count, data = read_uint16(data)
 
         content_infos, data = cls._receive_client_info(data, count, has_content_id=True)
 
         if len(data) != 0:
             raise PacketInvalidData("more bytes than expected; remaining: ", len(data))
 
         return {"content_infos": content_infos}
 
-    @tracer.traced("content")
     async def send_PACKET_CONTENT_SERVER_INFO(
         self, content_type, content_id, filesize, name, version, url, description, unique_id, md5sum, dependencies, tags
     ):
         data = write_init(PacketContentType.PACKET_CONTENT_SERVER_INFO)
 
         write_uint8(data, content_type.value)
         write_uint32(data, content_id)
@@ -230,15 +223,14 @@
         write_uint8(data, len(tags))
         for tag in tags:
             write_string(data, tag)
 
         write_presend(data, SEND_TCP_COMPAT_MTU)
         await self.send_packet(data)
 
-    @tracer.traced("content")
     async def send_PACKET_CONTENT_SERVER_CONTENT(self, content_type, content_id, filesize, filename, stream):
         # First, send a packet to tell the client it will be receiving a file
         data = write_init(PacketContentType.PACKET_CONTENT_SERVER_CONTENT)
 
         write_uint8(data, content_type.value)
         write_uint32(data, content_id)
```

### Comparing `openttd-protocol-1.4.1/openttd_protocol/protocol/coordinator.py` & `openttd-protocol-1.5.0/openttd_protocol/protocol/coordinator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import enum
 import logging
 
-from .. import tracer
 from ..wire.exceptions import PacketInvalidData
 from ..wire.read import (
     read_bytes,
     read_string,
     read_uint8,
     read_uint16,
     read_uint32,
@@ -91,15 +90,14 @@
 
 
 class CoordinatorProtocol(TCPProtocol):
     PacketType = PacketCoordinatorType
     PACKET_END = PacketCoordinatorType.PACKET_COORDINATOR_END
 
     @staticmethod
-    @tracer.traced("coordinator")
     def receive_PACKET_COORDINATOR_SERVER_REGISTER(source, data):
         protocol_version, data = read_uint8(data)
 
         if protocol_version < 1 or protocol_version > 6:
             raise PacketInvalidData("unknown protocol version: ", protocol_version)
 
         game_type, data = read_uint8(data)
@@ -126,15 +124,14 @@
             "game_type": game_type,
             "server_port": server_port,
             "invite_code": invite_code,
             "invite_code_secret": invite_code_secret,
         }
 
     @staticmethod
-    @tracer.traced("coordinator")
     def receive_PACKET_COORDINATOR_SERVER_UPDATE(source, data):
         protocol_version, data = read_uint8(data)
 
         if protocol_version < 1 or protocol_version > 6:
             raise PacketInvalidData("unknown protocol version: ", protocol_version)
 
         game_info_version, data = read_uint8(data)
@@ -239,15 +236,14 @@
             "map_height": map_height,
             "map_type": map_type,
             "gamescript_version": gamescript_version,
             "gamescript_name": gamescript_name,
         }
 
     @staticmethod
-    @tracer.traced("coordinator")
     def receive_PACKET_COORDINATOR_CLIENT_LISTING(source, data):
         protocol_version, data = read_uint8(data)
 
         if protocol_version < 1 or protocol_version > 6:
             raise PacketInvalidData("unknown protocol version: ", protocol_version)
 
         game_info_version, data = read_uint8(data)
@@ -268,15 +264,14 @@
             "protocol_version": protocol_version,
             "game_info_version": game_info_version,
             "openttd_version": openttd_version,
             "newgrf_lookup_table_cursor": newgrf_lookup_table_cursor,
         }
 
     @staticmethod
-    @tracer.traced("coordinator")
     def receive_PACKET_COORDINATOR_CLIENT_CONNECT(source, data):
         protocol_version, data = read_uint8(data)
 
         if protocol_version < 2 or protocol_version > 6:
             raise PacketInvalidData("unknown protocol version: ", protocol_version)
 
         invite_code, data = read_string(data)
@@ -286,15 +281,14 @@
 
         return {
             "protocol_version": protocol_version,
             "invite_code": invite_code,
         }
 
     @staticmethod
-    @tracer.traced("coordinator")
     def receive_PACKET_COORDINATOR_SERCLI_CONNECT_FAILED(source, data):
         protocol_version, data = read_uint8(data)
 
         if protocol_version < 2 or protocol_version > 6:
             raise PacketInvalidData("unknown protocol version: ", protocol_version)
 
         token, data = read_string(data)
@@ -306,15 +300,14 @@
         return {
             "protocol_version": protocol_version,
             "token": token,
             "tracking_number": tracking_number,
         }
 
     @staticmethod
-    @tracer.traced("coordinator")
     def receive_PACKET_COORDINATOR_CLIENT_CONNECTED(source, data):
         protocol_version, data = read_uint8(data)
 
         if protocol_version < 2 or protocol_version > 6:
             raise PacketInvalidData("unknown protocol version: ", protocol_version)
 
         token, data = read_string(data)
@@ -324,15 +317,14 @@
 
         return {
             "protocol_version": protocol_version,
             "token": token,
         }
 
     @staticmethod
-    @tracer.traced("coordinator")
     def receive_PACKET_COORDINATOR_SERCLI_STUN_RESULT(source, data):
         protocol_version, data = read_uint8(data)
 
         if protocol_version < 3 or protocol_version > 6:
             raise PacketInvalidData("unknown protocol version: ", protocol_version)
 
         token, data = read_string(data)
@@ -345,15 +337,14 @@
         return {
             "protocol_version": protocol_version,
             "token": token,
             "interface_number": interface_number,
             "result": result,
         }
 
-    @tracer.traced("coordinator")
     async def send_PACKET_COORDINATOR_GC_ERROR(self, protocol_version, error_no, error_detail):
         data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_ERROR)
 
         # Older protocol versions didn't know "REUSE_OF_INVITE_CODE" yet. So
         # replace it with the next best thing: "REGISTRATION_FAILED".
         if (
             protocol_version < 6
@@ -363,15 +354,14 @@
 
         write_uint8(data, error_no.value)
         write_string(data, error_detail)
 
         write_presend(data, SEND_TCP_MTU)
         await self.send_packet(data)
 
-    @tracer.traced("coordinator")
     async def send_PACKET_COORDINATOR_GC_REGISTER_ACK(
         self, protocol_version, connection_type, invite_code, invite_code_secret
     ):
         data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_REGISTER_ACK)
 
         if protocol_version > 1:
             write_string(data, invite_code)
@@ -402,15 +392,14 @@
                 yield count, data
                 data = bytearray()
                 count = 0
 
         if count != 0:
             yield count, data
 
-    @tracer.traced("coordinator")
     async def send_PACKET_COORDINATOR_GC_NEWGRF_LOOKUP(
         self, protocol_version, newgrf_lookup_table_cursor, newgrf_lookup_table
     ):
         cursor = max(newgrf_lookup_table.keys())
 
         for count, body in self._fill_NEWGRF_LOOKUP_PACKET(newgrf_lookup_table_cursor, newgrf_lookup_table):
             data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_NEWGRF_LOOKUP)
@@ -420,15 +409,14 @@
             write_uint32(data, cursor)
             write_uint16(data, count)
             write_bytes(data, body)
 
             write_presend(data, SEND_TCP_MTU)
             await self.send_packet(data)
 
-    @tracer.traced("coordinator")
     async def send_PACKET_COORDINATOR_GC_LISTING(
         self, protocol_version, game_info_version, servers, newgrf_lookup_table
     ):
         for server in servers:
             if server.game_type != ServerGameType.SERVER_GAME_TYPE_PUBLIC:
                 continue
             if len(server.info) == 0:
@@ -499,70 +487,64 @@
 
         # Send a final packet with 0 servers to indicate end-of-list.
         data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_LISTING)
         write_uint16(data, 0)
         write_presend(data, SEND_TCP_MTU)
         await self.send_packet(data)
 
-    @tracer.traced("coordinator")
     async def send_PACKET_COORDINATOR_GC_CONNECTING(self, protocol_version, token, invite_code):
         data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_CONNECTING)
 
         write_string(data, token)
         write_string(data, invite_code)
 
         write_presend(data, SEND_TCP_MTU)
         await self.send_packet(data)
 
-    @tracer.traced("coordinator")
     async def send_PACKET_COORDINATOR_GC_CONNECT_FAILED(self, protocol_version, token):
         data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_CONNECT_FAILED)
 
         write_string(data, token)
 
         write_presend(data, SEND_TCP_MTU)
         await self.send_packet(data)
 
-    @tracer.traced("coordinator")
     async def send_PACKET_COORDINATOR_GC_DIRECT_CONNECT(self, protocol_version, token, tracking_number, hostname, port):
         data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_DIRECT_CONNECT)
 
         write_string(data, token)
         write_uint8(data, tracking_number)
         write_string(data, hostname)
         write_uint16(data, port)
 
         write_presend(data, SEND_TCP_MTU)
         await self.send_packet(data)
 
-    @tracer.traced("coordinator")
     async def send_PACKET_COORDINATOR_GC_STUN_REQUEST(self, protocol_version, token):
         data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_STUN_REQUEST)
 
         write_string(data, token)
 
         write_presend(data, SEND_TCP_MTU)
         await self.send_packet(data)
 
-    @tracer.traced("coordinator")
     async def send_PACKET_COORDINATOR_GC_STUN_CONNECT(
         self, protocol_version, token, tracking_number, interface_number, hostname, port
     ):
         data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_STUN_CONNECT)
 
         write_string(data, token)
         write_uint8(data, tracking_number)
         write_uint8(data, interface_number)
         write_string(data, hostname)
         write_uint16(data, port)
 
         write_presend(data, SEND_TCP_MTU)
         await self.send_packet(data)
 
-    @tracer.traced("coordinator")
     async def send_PACKET_COORDINATOR_GC_TURN_CONNECT(
         self, protocol_version, token, tracking_number, ticket, connection_string
     ):
         data = write_init(PacketCoordinatorType.PACKET_COORDINATOR_GC_TURN_CONNECT)
 
         write_string(data, token)
         write_uint8(data, tracking_number)
```

### Comparing `openttd-protocol-1.4.1/openttd_protocol/protocol/game.py` & `openttd-protocol-1.5.0/openttd_protocol/protocol/game.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import enum
 import logging
 
-from .. import tracer
 from ..wire.exceptions import PacketInvalidData
 from ..wire.read import (
     read_bytes,
     read_string,
     read_uint8,
     read_uint16,
     read_uint32,
@@ -50,15 +49,14 @@
 
 
 class GameProtocol(TCPProtocol):
     PacketType = PacketGameType
     PACKET_END = PacketGameType.PACKET_END
 
     @staticmethod
-    @tracer.traced("game")
     def receive_PACKET_SERVER_GAME_INFO(source, data):
         game_info_version, data = read_uint8(data)
 
         if game_info_version < 1 or game_info_version > 6:
             raise PacketInvalidData("unknown game info version: ", game_info_version)
 
         if game_info_version >= 6:
@@ -156,19 +154,17 @@
             "map_height": map_height,
             "map_type": map_type,
             "gamescript_version": gamescript_version,
             "gamescript_name": gamescript_name,
         }
 
     @staticmethod
-    @tracer.traced("game")
     def receive_PACKET_SERVER_SHUTDOWN(source, data):
         if len(data) != 0:
             raise PacketInvalidData("more bytes than expected in SERVER_SHUTDOWN; remaining: ", len(data))
 
         return {}
 
-    @tracer.traced("game")
     async def send_PACKET_CLIENT_GAME_INFO(self):
         data = write_init(PacketGameType.PACKET_CLIENT_GAME_INFO)
         write_presend(data, SEND_TCP_MTU)
         await self.send_packet(data)
```

### Comparing `openttd-protocol-1.4.1/openttd_protocol/protocol/stun.py` & `openttd-protocol-1.5.0/openttd_protocol/protocol/stun.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import enum
 import logging
 
-from .. import tracer
 from ..wire.exceptions import PacketInvalidData
 from ..wire.read import (
     read_string,
     read_uint8,
 )
 from ..wire.tcp import TCPProtocol
 
@@ -18,15 +17,14 @@
 
 
 class StunProtocol(TCPProtocol):
     PacketType = PacketStunType
     PACKET_END = PacketStunType.PACKET_STUN_END
 
     @staticmethod
-    @tracer.traced("stun")
     def receive_PACKET_STUN_SERCLI_STUN(source, data):
         protocol_version, data = read_uint8(data)
 
         if protocol_version < 3 or protocol_version > 6:
             raise PacketInvalidData("unknown protocol version: ", protocol_version)
 
         token, data = read_string(data)
```

### Comparing `openttd-protocol-1.4.1/openttd_protocol/protocol/turn.py` & `openttd-protocol-1.5.0/openttd_protocol/protocol/turn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import enum
 import logging
 
-from .. import tracer
 from ..wire.exceptions import PacketInvalidData
 from ..wire.read import (
     read_string,
     read_uint8,
 )
 from ..wire.tcp import TCPProtocol
 from ..wire.write import (
@@ -26,29 +25,27 @@
 
 
 class TurnProtocol(TCPProtocol):
     PacketType = PacketTurnType
     PACKET_END = PacketTurnType.PACKET_TURN_END
 
     @staticmethod
-    @tracer.traced("turn")
     def receive_PACKET_TURN_SERCLI_CONNECT(source, data):
         protocol_version, data = read_uint8(data)
 
         if protocol_version < 5 or protocol_version > 6:
             raise PacketInvalidData("unknown protocol version: ", protocol_version)
 
         ticket, data = read_string(data)
 
         if len(data) != 0:
             raise PacketInvalidData("more bytes than expected; remaining: ", len(data))
 
         return {"protocol_version": protocol_version, "ticket": ticket}
 
-    @tracer.traced("turn")
     async def send_PACKET_TURN_TURN_CONNECTED(self, protocol_version, hostname):
         data = write_init(PacketTurnType.PACKET_TURN_TURN_CONNECTED)
 
         write_string(data, hostname)
 
         write_presend(data, SEND_TCP_MTU)
         await self.send_packet(data)
```

### Comparing `openttd-protocol-1.4.1/openttd_protocol/wire/exceptions.py` & `openttd-protocol-1.5.0/openttd_protocol/wire/exceptions.py`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.4.1/openttd_protocol/wire/read.py` & `openttd-protocol-1.5.0/openttd_protocol/wire/read.py`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.4.1/openttd_protocol/wire/source.py` & `openttd-protocol-1.5.0/openttd_protocol/wire/source.py`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.4.1/openttd_protocol/wire/tcp.py` & `openttd-protocol-1.5.0/openttd_protocol/wire/tcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     SocketClosed,
 )
 from .read import (
     read_uint8,
     read_uint16,
 )
 from .source import Source
-from .. import tracer
 
 log = logging.getLogger(__name__)
 
 
 class TCPProtocol(asyncio.Protocol):
     proxy_protocol = False
     PacketType = None
@@ -170,25 +169,22 @@
     async def _process_queue(self):
         data = await self._queue.get()
 
         if hasattr(self._callback, "receive_raw"):
             if await self._callback.receive_raw(self.source, data):
                 return
 
-        with tracer.tracer("tcp.receive-packet"):
-            try:
-                packet_type, kwargs = self.receive_packet(self.source, data)
-            except PacketInvalid as err:
-                log.info("Dropping invalid packet from %s:%d: %r", self.source.ip, self.source.port, err)
-                raise SocketClosed
+        try:
+            packet_type, kwargs = self.receive_packet(self.source, data)
+        except PacketInvalid as err:
+            log.info("Dropping invalid packet from %s:%d: %r", self.source.ip, self.source.port, err)
+            raise SocketClosed
 
-            with tracer.tracer("tcp.packet-handler"):
-                await getattr(self._callback, f"receive_{packet_type.name}")(self.source, **kwargs)
+        await getattr(self._callback, f"receive_{packet_type.name}")(self.source, **kwargs)
 
-    @tracer.traced("tcp")
     def receive_packet(self, source, data):
         # Check length of packet
         length, data = read_uint16(data)
         if length != len(data) + 2:
             raise PacketInvalidSize(len(data) + 2, length)
 
         # Check if type is in range
@@ -198,21 +194,18 @@
 
         # Check if we expect this packet
         packet_type = self.PacketType(packet_type)
         func = getattr(self, f"receive_{packet_type.name}", None)
         if func is None:
             raise PacketInvalidType(packet_type)
 
-        tracer.add_trace_field("command", f"receive.{packet_type.name}")
-
         # Process this packet
         kwargs = func(source, data)
         return packet_type, kwargs
 
-    @tracer.traced("tcp")
     async def send_packet(self, data):
         await self._can_write.wait()
 
         # When a socket is closed on the other side, and due to the nature of
         # how asyncio is doing writes, we never receive an exception. So,
         # instead, check every time we send something if we are not closed.
         # If we are, inform our caller, which should cleanup the socket next.
```

### Comparing `openttd-protocol-1.4.1/openttd_protocol/wire/test_read.py` & `openttd-protocol-1.5.0/openttd_protocol/wire/test_read.py`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.4.1/openttd_protocol/wire/test_tcp.py` & `openttd-protocol-1.5.0/openttd_protocol/wire/test_tcp.py`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.4.1/openttd_protocol/wire/test_write.py` & `openttd-protocol-1.5.0/openttd_protocol/wire/test_write.py`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.4.1/openttd_protocol/wire/write.py` & `openttd-protocol-1.5.0/openttd_protocol/wire/write.py`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.4.1/openttd_protocol.egg-info/PKG-INFO` & `openttd-protocol-1.5.0/openttd_protocol.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openttd-protocol
-Version: 1.4.1
+Version: 1.5.0
 Summary: OpenTTD network protocol for Python
 Home-page: https://github.com/OpenTTD/py-protocol
 Author: OpenTTD Dev Team
 Author-email: info@openttd.org
 License: UNKNOWN
 Description: # openttd-protocol
```

### Comparing `openttd-protocol-1.4.1/openttd_protocol.egg-info/SOURCES.txt` & `openttd-protocol-1.5.0/openttd_protocol.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 VERSION
 setup.py
 version.py
 openttd_protocol/__init__.py
-openttd_protocol/tracer.py
 openttd_protocol.egg-info/PKG-INFO
 openttd_protocol.egg-info/SOURCES.txt
 openttd_protocol.egg-info/dependency_links.txt
 openttd_protocol.egg-info/top_level.txt
 openttd_protocol/protocol/__init__.py
 openttd_protocol/protocol/content.py
 openttd_protocol/protocol/coordinator.py
```

### Comparing `openttd-protocol-1.4.1/setup.py` & `openttd-protocol-1.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `openttd-protocol-1.4.1/version.py` & `openttd-protocol-1.5.0/version.py`

 * *Files identical despite different names*

