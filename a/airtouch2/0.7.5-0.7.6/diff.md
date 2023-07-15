# Comparing `tmp/airtouch2-0.7.5.tar.gz` & `tmp/airtouch2-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtouch2-0.7.5.tar", last modified: Tue Jul 11 11:36:57 2023, max compression
+gzip compressed data, was "airtouch2-0.7.6.tar", last modified: Sat Jul 15 03:49:24 2023, max compression
```

## Comparing `airtouch2-0.7.5.tar` & `airtouch2-0.7.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.201552 airtouch2-0.7.5/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1076 2023-01-10 07:31:33.000000 airtouch2-0.7.5/LICENSE
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2281 2023-07-11 11:36:57.201552 airtouch2-0.7.5/PKG-INFO
--rw-r--r--   0 nathan    (1000) nathan    (1000)      271 2023-01-10 07:31:33.000000 airtouch2-0.7.5/README.md
--rw-r--r--   0 nathan    (1000) nathan    (1000)      852 2023-07-11 11:35:30.000000 airtouch2-0.7.5/pyproject.toml
--rw-r--r--   0 nathan    (1000) nathan    (1000)       38 2023-07-11 11:36:57.201552 airtouch2-0.7.5/setup.cfg
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/airtouch2/
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/airtouch2/at2/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     5511 2023-06-28 10:35:59.000000 airtouch2-0.7.5/src/airtouch2/at2/At2Aircon.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3713 2023-07-10 10:06:21.000000 airtouch2-0.7.5/src/airtouch2/at2/At2Client.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3301 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/at2/At2Group.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      204 2023-07-10 10:42:42.000000 airtouch2-0.7.5/src/airtouch2/at2/__init__.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/airtouch2/at2plus/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2789 2023-06-28 10:35:27.000000 airtouch2-0.7.5/src/airtouch2/at2plus/At2PlusAircon.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     8381 2023-07-11 11:17:00.000000 airtouch2-0.7.5/src/airtouch2/at2plus/At2PlusClient.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      190 2023-07-10 11:17:26.000000 airtouch2-0.7.5/src/airtouch2/at2plus/__init__.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/airtouch2/common/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2457 2023-07-11 11:20:25.000000 airtouch2-0.7.5/src/airtouch2/common/Buffer.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     4764 2023-07-10 10:07:01.000000 airtouch2-0.7.5/src/airtouch2/common/NetClient.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/common/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      428 2023-07-09 02:16:01.000000 airtouch2-0.7.5/src/airtouch2/common/interfaces.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/airtouch2/helpers/
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/helpers/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      541 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/helpers/diff_bytes.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/airtouch2/protocol/
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-03-19 07:06:23.000000 airtouch2-0.7.5/src/airtouch2/protocol/__init__.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/airtouch2/protocol/at2/
--rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2584 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/constants.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2773 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/conversions.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      647 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/enums.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      865 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/lookups.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      308 2023-07-11 11:17:00.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/message_common.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/
--rw-r--r--   0 nathan    (1000) nathan    (1000)      849 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/RequestState.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     5046 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/ResponseMessage.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)      339 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/__init__.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2861 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/ac_commands.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1867 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/group_commands.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.201552 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/
--rw-r--r--   0 nathan    (1000) nathan    (1000)      148 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/constants.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2768 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/control_status_common.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1128 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/conversions.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2359 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/crc16_modbus.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1560 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/enums.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1113 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/extended_common.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3942 2023-07-11 11:17:00.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/message_common.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.201552 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/messages/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     6156 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     3167 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/messages/AcControl.py
--rw-r--r--   0 nathan    (1000) nathan    (1000)     4119 2023-06-25 08:46:07.000000 airtouch2-0.7.5/src/airtouch2/protocol/at2plus/messages/AcStatus.py
-drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-11 11:36:57.197552 airtouch2-0.7.5/src/airtouch2.egg-info/
--rw-r--r--   0 nathan    (1000) nathan    (1000)     2281 2023-07-11 11:36:57.000000 airtouch2-0.7.5/src/airtouch2.egg-info/PKG-INFO
--rw-r--r--   0 nathan    (1000) nathan    (1000)     1649 2023-07-11 11:36:57.000000 airtouch2-0.7.5/src/airtouch2.egg-info/SOURCES.txt
--rw-r--r--   0 nathan    (1000) nathan    (1000)        1 2023-07-11 11:36:57.000000 airtouch2-0.7.5/src/airtouch2.egg-info/dependency_links.txt
--rw-r--r--   0 nathan    (1000) nathan    (1000)       10 2023-07-11 11:36:57.000000 airtouch2-0.7.5/src/airtouch2.egg-info/top_level.txt
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.555294 airtouch2-0.7.6/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1076 2023-01-10 07:31:33.000000 airtouch2-0.7.6/LICENSE
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2281 2023-07-15 03:49:24.555294 airtouch2-0.7.6/PKG-INFO
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      271 2023-01-10 07:31:33.000000 airtouch2-0.7.6/README.md
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      852 2023-07-15 03:47:27.000000 airtouch2-0.7.6/pyproject.toml
+-rw-r--r--   0 nathan    (1000) nathan    (1000)       38 2023-07-15 03:49:24.555294 airtouch2-0.7.6/setup.cfg
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/airtouch2/
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/airtouch2/at2/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     5511 2023-06-28 10:35:59.000000 airtouch2-0.7.6/src/airtouch2/at2/At2Aircon.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3515 2023-07-15 03:40:22.000000 airtouch2-0.7.6/src/airtouch2/at2/At2Client.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3301 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/at2/At2Group.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      204 2023-07-10 10:42:42.000000 airtouch2-0.7.6/src/airtouch2/at2/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/airtouch2/at2plus/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2789 2023-07-15 03:31:26.000000 airtouch2-0.7.6/src/airtouch2/at2plus/At2PlusAircon.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     8423 2023-07-15 03:40:27.000000 airtouch2-0.7.6/src/airtouch2/at2plus/At2PlusClient.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      190 2023-07-10 11:17:26.000000 airtouch2-0.7.6/src/airtouch2/at2plus/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/airtouch2/common/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2457 2023-07-11 11:20:25.000000 airtouch2-0.7.6/src/airtouch2/common/Buffer.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     4810 2023-07-15 03:40:27.000000 airtouch2-0.7.6/src/airtouch2/common/NetClient.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/common/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      428 2023-07-09 02:16:01.000000 airtouch2-0.7.6/src/airtouch2/common/interfaces.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/airtouch2/helpers/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/helpers/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      541 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/helpers/diff_bytes.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/airtouch2/protocol/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-03-19 07:06:23.000000 airtouch2-0.7.6/src/airtouch2/protocol/__init__.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/airtouch2/protocol/at2/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        0 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2584 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/constants.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2773 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/conversions.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      647 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/enums.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      865 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/lookups.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      308 2023-07-11 11:17:00.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/message_common.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      849 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/RequestState.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     5046 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/ResponseMessage.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      339 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/__init__.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2861 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/ac_commands.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1867 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/group_commands.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.555294 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      148 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/constants.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2768 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/control_status_common.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1128 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/conversions.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2359 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/crc16_modbus.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1560 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/enums.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1113 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/extended_common.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3942 2023-07-11 11:17:00.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/message_common.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.555294 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/messages/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     6156 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     3167 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/messages/AcControl.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     4119 2023-06-25 08:46:07.000000 airtouch2-0.7.6/src/airtouch2/protocol/at2plus/messages/AcStatus.py
+drwxr-xr-x   0 nathan    (1000) nathan    (1000)        0 2023-07-15 03:49:24.551294 airtouch2-0.7.6/src/airtouch2.egg-info/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     2281 2023-07-15 03:49:24.000000 airtouch2-0.7.6/src/airtouch2.egg-info/PKG-INFO
+-rw-r--r--   0 nathan    (1000) nathan    (1000)     1649 2023-07-15 03:49:24.000000 airtouch2-0.7.6/src/airtouch2.egg-info/SOURCES.txt
+-rw-r--r--   0 nathan    (1000) nathan    (1000)        1 2023-07-15 03:49:24.000000 airtouch2-0.7.6/src/airtouch2.egg-info/dependency_links.txt
+-rw-r--r--   0 nathan    (1000) nathan    (1000)       10 2023-07-15 03:49:24.000000 airtouch2-0.7.6/src/airtouch2.egg-info/top_level.txt
```

### Comparing `airtouch2-0.7.5/LICENSE` & `airtouch2-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/PKG-INFO` & `airtouch2-0.7.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtouch2
-Version: 0.7.5
+Version: 0.7.6
 Summary: API for the monitoring and control of a Polyaire Airtouch 2 system over the local network
 Author-email: Nathan Van der Hoek <nathan.vanderhoek@student.adelaide.edu.au>
 License: MIT License
         
         Copyright (c) 2022 Nathan Van der Hoek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `airtouch2-0.7.5/pyproject.toml` & `airtouch2-0.7.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=64"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "airtouch2"
 description = "API for the monitoring and control of a Polyaire Airtouch 2 system over the local network"
-version = "0.7.5"
+version = "0.7.6"
 authors = [{ name = "Nathan Van der Hoek", email = "nathan.vanderhoek@student.adelaide.edu.au" }]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `airtouch2-0.7.5/src/airtouch2/at2/At2Aircon.py` & `airtouch2-0.7.6/src/airtouch2/at2/At2Aircon.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/at2/At2Client.py` & `airtouch2-0.7.6/src/airtouch2/at2/At2Client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import asyncio
 from datetime import datetime
-import errno
 import logging
-from airtouch2.common.NetClient import NetClient
 
+from airtouch2.common.NetClient import NetClient
 from airtouch2.protocol.at2.constants import MessageLength
 from airtouch2.protocol.at2.messages import RequestState, ResponseMessage
 from airtouch2.at2.At2Aircon import At2Aircon
 from airtouch2.at2.At2Group import At2Group
 from airtouch2.common.interfaces import Callback, Serializable, TaskCreator
 
 _LOGGER = logging.getLogger(__name__)
 
-NetworkOrHostDownErrors = (errno.EHOSTUNREACH, errno.ECONNREFUSED,  errno.ETIMEDOUT,
-                           errno.ENETDOWN, errno.ENETUNREACH, errno.ENETRESET, errno.ECONNABORTED)
-
 
 class At2Client:
     def __init__(self, host: str, dump_responses: bool = False, task_creator: TaskCreator = asyncio.create_task):
         # public
         self.aircons: list[At2Aircon] = []
         self.groups: list[At2Group] = []
         self.system_name: str = "UNKNOWN"
```

### Comparing `airtouch2-0.7.5/src/airtouch2/at2/At2Group.py` & `airtouch2-0.7.6/src/airtouch2/at2/At2Group.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/at2plus/At2PlusAircon.py` & `airtouch2-0.7.6/src/airtouch2/at2plus/At2PlusAircon.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/at2plus/At2PlusClient.py` & `airtouch2-0.7.6/src/airtouch2/at2plus/At2PlusClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 from datetime import datetime
 import logging
+
 from airtouch2.at2plus.At2PlusAircon import At2PlusAircon
 from airtouch2.common.NetClient import NetClient
 from airtouch2.protocol.at2plus.control_status_common import ControlStatusSubHeader, ControlStatusSubType
 from airtouch2.protocol.at2plus.extended_common import ExtendedMessageSubType, ExtendedSubHeader
 from airtouch2.protocol.at2plus.message_common import HEADER_LENGTH, HEADER_MAGIC, Header, Message, MessageType
 from airtouch2.protocol.at2plus.messages.AcAbilityMessage import AcAbility, AcAbilityMessage, RequestAcAbilityMessage
 from airtouch2.protocol.at2plus.messages.AcStatus import AcStatusMessage
@@ -144,26 +145,26 @@
     async def _on_connect(self) -> None:
         # request AcStatus
         await self._client.send(AcStatusMessage([]))
 
     async def _handle_status_message(self, message: AcStatusMessage):
         _LOGGER.debug("Handling status message")
         for status in message.statuses:
-            if status.id in self.aircons_by_id.keys():
-                self.aircons_by_id[status.id]._update_status(status)
-                _LOGGER.debug(f"Updated AC {status.id} with value {status}")
-            else:
+            if status.id not in self.aircons_by_id.keys():
                 _LOGGER.debug(f"New AC ({status.id}) found")
                 self.aircons_by_id[status.id] = At2PlusAircon(status, self)
                 for callback in self._new_ac_callbacks:
                     callback()
                 ability = await self._request_ac_ability(status.id)
                 while not ability:
                     ability = await self._request_ac_ability(status.id)
                 self.aircons_by_id[status.id]._set_ability(ability)
+                _LOGGER.debug(f"Set ability of AC{status.id}")
+            self.aircons_by_id[status.id]._update_status(status)
+            _LOGGER.debug(f"Updated AC {status.id} with value {status}")
         _LOGGER.debug("Finished handling status message")
 
     async def _request_ac_ability(self, id: int) -> AcAbility | None:
         _LOGGER.debug(f"Requesting ability of AC{id}")
         await self._client.send(RequestAcAbilityMessage(id))
         _LOGGER.debug("Waiting for ability message response...")
         ac_ability = await self._ability_message_queue.get()
```

### Comparing `airtouch2-0.7.5/src/airtouch2/common/Buffer.py` & `airtouch2-0.7.6/src/airtouch2/common/Buffer.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/common/NetClient.py` & `airtouch2-0.7.6/src/airtouch2/common/NetClient.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,14 +67,15 @@
     async def send(self, message: Serializable) -> None:
         """Send the serializable 'message'"""
         if self._writer is None:
             raise RuntimeError("Client is not connected - call connect() first")
         else:
             bytes_to_write = message.to_bytes()
             _LOGGER.debug(f"Sending {message.__class__.__name__} with data: {bytes_to_write.hex(':')}")
+            _LOGGER.debug(f"{repr(message)}")
             self._writer.write(bytes_to_write)
             drained: bool = False
             while not drained:
                 try:
                     await self._writer.drain()
                     drained = True
                 except (ConnectionResetError, asyncio.IncompleteReadError) as e:
```

### Comparing `airtouch2-0.7.5/src/airtouch2/helpers/diff_bytes.py` & `airtouch2-0.7.6/src/airtouch2/helpers/diff_bytes.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/protocol/at2/constants.py` & `airtouch2-0.7.6/src/airtouch2/protocol/at2/constants.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/protocol/at2/conversions.py` & `airtouch2-0.7.6/src/airtouch2/protocol/at2/conversions.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/protocol/at2/enums.py` & `airtouch2-0.7.6/src/airtouch2/protocol/at2/enums.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/protocol/at2/lookups.py` & `airtouch2-0.7.6/src/airtouch2/protocol/at2/lookups.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/RequestState.py` & `airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/RequestState.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/ResponseMessage.py` & `airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/ResponseMessage.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/ac_commands.py` & `airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/ac_commands.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/protocol/at2/messages/group_commands.py` & `airtouch2-0.7.6/src/airtouch2/protocol/at2/messages/group_commands.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/protocol/at2plus/control_status_common.py` & `airtouch2-0.7.6/src/airtouch2/protocol/at2plus/control_status_common.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/protocol/at2plus/conversions.py` & `airtouch2-0.7.6/src/airtouch2/protocol/at2plus/conversions.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/protocol/at2plus/crc16_modbus.py` & `airtouch2-0.7.6/src/airtouch2/protocol/at2plus/crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/protocol/at2plus/enums.py` & `airtouch2-0.7.6/src/airtouch2/protocol/at2plus/enums.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/protocol/at2plus/extended_common.py` & `airtouch2-0.7.6/src/airtouch2/protocol/at2plus/extended_common.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/protocol/at2plus/message_common.py` & `airtouch2-0.7.6/src/airtouch2/protocol/at2plus/message_common.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py` & `airtouch2-0.7.6/src/airtouch2/protocol/at2plus/messages/AcAbilityMessage.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/protocol/at2plus/messages/AcControl.py` & `airtouch2-0.7.6/src/airtouch2/protocol/at2plus/messages/AcControl.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2/protocol/at2plus/messages/AcStatus.py` & `airtouch2-0.7.6/src/airtouch2/protocol/at2plus/messages/AcStatus.py`

 * *Files identical despite different names*

### Comparing `airtouch2-0.7.5/src/airtouch2.egg-info/PKG-INFO` & `airtouch2-0.7.6/src/airtouch2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airtouch2
-Version: 0.7.5
+Version: 0.7.6
 Summary: API for the monitoring and control of a Polyaire Airtouch 2 system over the local network
 Author-email: Nathan Van der Hoek <nathan.vanderhoek@student.adelaide.edu.au>
 License: MIT License
         
         Copyright (c) 2022 Nathan Van der Hoek
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `airtouch2-0.7.5/src/airtouch2.egg-info/SOURCES.txt` & `airtouch2-0.7.6/src/airtouch2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

