# Comparing `tmp/onvif-zeep-async-3.1.8.tar.gz` & `tmp/onvif-zeep-async-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-zeep-async-3.1.8.tar", last modified: Wed May 24 14:19:34 2023, max compression
+gzip compressed data, was "onvif-zeep-async-3.1.9.tar", last modified: Thu Jun  1 16:30:14 2023, max compression
```

## Comparing `onvif-zeep-async-3.1.8.tar` & `onvif-zeep-async-3.1.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-24 14:19:34.160561 onvif-zeep-async-3.1.8/
--rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/.pre-commit-config.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.8/CHANGES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.8/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/MANIFEST.in
--rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/Makefile
--rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-24 14:19:34.160641 onvif-zeep-async-3.1.8/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/README.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/bandit.yaml
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-24 14:19:34.150068 onvif-zeep-async-3.1.8/examples/
--rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/examples/events.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/examples/rotate_image.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/examples/streaming.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-24 14:19:34.152464 onvif-zeep-async-3.1.8/onvif/
--rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-05-14 16:23:24.000000 onvif-zeep-async-3.1.8/onvif/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    25053 2023-05-24 14:16:33.000000 onvif-zeep-async-3.1.8/onvif/client.py
--rw-r--r--   0 bdraco     (501) staff       (20)      104 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.8/onvif/const.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/definition.py
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)    12024 2023-05-24 14:18:59.000000 onvif-zeep-async-3.1.8/onvif/managers.py
--rw-r--r--   0 bdraco     (501) staff       (20)      157 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.8/onvif/settings.py
--rw-r--r--   0 bdraco     (501) staff       (20)      563 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.8/onvif/transport.py
--rw-r--r--   0 bdraco     (501) staff       (20)      764 2023-05-14 17:17:16.000000 onvif-zeep-async-3.1.8/onvif/types.py
--rw-r--r--   0 bdraco     (501) staff       (20)     3947 2023-05-24 14:19:06.000000 onvif-zeep-async-3.1.8/onvif/util.py
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-24 14:19:11.000000 onvif-zeep-async-3.1.8/onvif/version.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     2331 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.8/onvif/wrappers.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-24 14:19:34.159251 onvif-zeep-async-3.1.8/onvif/wsdl/
--rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/accesscontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/actionengine.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/addressing
--rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/analytics.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/analyticsdevice.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/b-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/bf-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/bw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/deviceio.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/devicemgmt.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/display.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/doorcontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/envelope
--rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/events.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/imaging.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/include
--rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/media.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/onvif.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/ptz.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/r-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/receiver.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/recording.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/remotediscovery.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/replay.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/rw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/search.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/t-1.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/types.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/ws-addr.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/ws-discovery.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/xml.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/onvif/wsdl/xmlmime
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-24 14:19:34.160135 onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-24 14:19:34.000000 onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     1553 2023-05-24 14:19:34.000000 onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-24 14:19:34.000000 onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-24 14:19:34.000000 onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/entry_points.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/not-zip-safe
--rw-r--r--   0 bdraco     (501) staff       (20)       63 2023-05-24 14:19:34.000000 onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-24 14:19:34.000000 onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/top_level.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/pyproject.toml
--rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-24 14:19:34.160873 onvif-zeep-async-3.1.8/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1836 2023-05-14 17:17:16.000000 onvif-zeep-async-3.1.8/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-24 14:19:34.160350 onvif-zeep-async-3.1.8/tests/
--rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.8/tests/test.py
--rw-r--r--   0 bdraco     (501) staff       (20)     3533 2023-05-24 14:16:33.000000 onvif-zeep-async-3.1.8/tests/test_util.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-06-01 16:30:14.001415 onvif-zeep-async-3.1.9/
+-rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.9/CHANGES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.9/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-06-01 16:30:14.001474 onvif-zeep-async-3.1.9/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/README.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/bandit.yaml
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-06-01 16:30:13.991023 onvif-zeep-async-3.1.9/examples/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/examples/events.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/examples/rotate_image.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/examples/streaming.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-06-01 16:30:13.992800 onvif-zeep-async-3.1.9/onvif/
+-rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-05-14 16:23:24.000000 onvif-zeep-async-3.1.9/onvif/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    25053 2023-05-24 14:16:33.000000 onvif-zeep-async-3.1.9/onvif/client.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      104 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.9/onvif/const.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/definition.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    12304 2023-06-01 16:29:09.000000 onvif-zeep-async-3.1.9/onvif/managers.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      157 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.9/onvif/settings.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      563 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.9/onvif/transport.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      764 2023-05-14 17:17:16.000000 onvif-zeep-async-3.1.9/onvif/types.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3947 2023-05-24 14:19:06.000000 onvif-zeep-async-3.1.9/onvif/util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-06-01 16:29:13.000000 onvif-zeep-async-3.1.9/onvif/version.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     2331 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.9/onvif/wrappers.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-06-01 16:30:14.000197 onvif-zeep-async-3.1.9/onvif/wsdl/
+-rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/accesscontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/actionengine.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/addressing
+-rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/analytics.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/analyticsdevice.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/b-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/bf-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/bw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/deviceio.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/display.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/doorcontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/envelope
+-rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/events.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/imaging.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/include
+-rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/media.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/onvif.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/ptz.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/r-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/receiver.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/recording.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/remotediscovery.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/replay.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/rw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/search.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/t-1.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/types.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/ws-discovery.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/xml.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/onvif/wsdl/xmlmime
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-06-01 16:30:14.000981 onvif-zeep-async-3.1.9/onvif_zeep_async.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-06-01 16:30:13.000000 onvif-zeep-async-3.1.9/onvif_zeep_async.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     1553 2023-06-01 16:30:13.000000 onvif-zeep-async-3.1.9/onvif_zeep_async.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-06-01 16:30:13.000000 onvif-zeep-async-3.1.9/onvif_zeep_async.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-06-01 16:30:13.000000 onvif-zeep-async-3.1.9/onvif_zeep_async.egg-info/entry_points.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-3.1.9/onvif_zeep_async.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)       63 2023-06-01 16:30:13.000000 onvif-zeep-async-3.1.9/onvif_zeep_async.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-06-01 16:30:13.000000 onvif-zeep-async-3.1.9/onvif_zeep_async.egg-info/top_level.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/pyproject.toml
+-rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-06-01 16:30:14.001710 onvif-zeep-async-3.1.9/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1836 2023-05-14 17:17:16.000000 onvif-zeep-async-3.1.9/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-06-01 16:30:14.001196 onvif-zeep-async-3.1.9/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.9/tests/test.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3533 2023-05-24 14:16:33.000000 onvif-zeep-async-3.1.9/tests/test_util.py
```

### Comparing `onvif-zeep-async-3.1.8/.gitignore` & `onvif-zeep-async-3.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/.pre-commit-config.yaml` & `onvif-zeep-async-3.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/LICENSE` & `onvif-zeep-async-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/Makefile` & `onvif-zeep-async-3.1.9/Makefile`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/PKG-INFO` & `onvif-zeep-async-3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 3.1.8
+Version: 3.1.9
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-3.1.8/README.rst` & `onvif-zeep-async-3.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/examples/events.py` & `onvif-zeep-async-3.1.9/examples/events.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/examples/rotate_image.py` & `onvif-zeep-async-3.1.9/examples/rotate_image.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/examples/streaming.py` & `onvif-zeep-async-3.1.9/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/__init__.py` & `onvif-zeep-async-3.1.9/onvif/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/client.py` & `onvif-zeep-async-3.1.9/onvif/client.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/definition.py` & `onvif-zeep-async-3.1.9/onvif/definition.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/exceptions.py` & `onvif-zeep-async-3.1.9/onvif/exceptions.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/managers.py` & `onvif-zeep-async-3.1.9/onvif/managers.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 
 _RENEWAL_PERCENTAGE = 0.8
 
 SUBSCRIPTION_ERRORS = (Fault, asyncio.TimeoutError, TransportError)
 RENEW_ERRORS = (ONVIFError, httpx.RequestError, XMLParseError, *SUBSCRIPTION_ERRORS)
 SUBSCRIPTION_RESTART_INTERVAL_ON_ERROR = dt.timedelta(seconds=40)
 
+# If the camera returns a subscription with a termination time that is less than
+# this value, we will use this value instead to prevent subscribing over and over
+# again.
+MINIMUM_SUBSCRIPTION_SECONDS = 60.0
 
 if TYPE_CHECKING:
     from onvif.client import ONVIFCamera, ONVIFService
 
 
 class BaseManager:
     """Base class for notification and pull point managers."""
@@ -112,15 +116,18 @@
         """Calculate the next renewal call_at."""
         current_time: dt.datetime | None = result.CurrentTime
         termination_time: dt.datetime | None = result.TerminationTime
         if termination_time and current_time:
             delay = termination_time - current_time
         else:
             delay = self._interval
-        delay_seconds = delay.total_seconds() * _RENEWAL_PERCENTAGE
+        delay_seconds = (
+            max(delay.total_seconds(), MINIMUM_SUBSCRIPTION_SECONDS)
+            * _RENEWAL_PERCENTAGE
+        )
         logger.debug(
             "%s: Renew notification subscription in %s seconds",
             self._device.host,
             delay_seconds,
         )
         return self._loop.time() + delay_seconds
 
@@ -137,15 +144,15 @@
         if self._restart_or_renew_task and not self._restart_or_renew_task.done():
             logger.debug("%s: Notify renew already in progress", self._device.host)
             return
         self._restart_or_renew_task = asyncio.create_task(
             self._renew_or_restart_subscription()
         )
 
-    async def _restart_subscription(self) -> bool:
+    async def _restart_subscription(self) -> float:
         """Restart the notify subscription assuming the camera rebooted."""
         self._cancel_renewals()
         return await self._start()
 
     @retry_connection_error()
     async def _call_subscription_renew(self) -> float:
         """Call notify subscription Renew."""
```

### Comparing `onvif-zeep-async-3.1.8/onvif/transport.py` & `onvif-zeep-async-3.1.9/onvif/transport.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/types.py` & `onvif-zeep-async-3.1.9/onvif/types.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/util.py` & `onvif-zeep-async-3.1.9/onvif/util.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wrappers.py` & `onvif-zeep-async-3.1.9/onvif/wrappers.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/accesscontrol.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/actionengine.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/addressing` & `onvif-zeep-async-3.1.9/onvif/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/advancedsecurity.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/analytics.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/analyticsdevice.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/b-2.xsd` & `onvif-zeep-async-3.1.9/onvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/bf-2.xsd` & `onvif-zeep-async-3.1.9/onvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/bw-2.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/deviceio.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/devicemgmt.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/display.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/doorcontrol.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/envelope` & `onvif-zeep-async-3.1.9/onvif/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/events.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/imaging.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/media.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/onvif.xsd` & `onvif-zeep-async-3.1.9/onvif/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/ptz.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/r-2.xsd` & `onvif-zeep-async-3.1.9/onvif/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/receiver.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/recording.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/remotediscovery.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/replay.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/rw-2.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/search.wsdl` & `onvif-zeep-async-3.1.9/onvif/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/t-1.xsd` & `onvif-zeep-async-3.1.9/onvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/types.xsd` & `onvif-zeep-async-3.1.9/onvif/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/ws-addr.xsd` & `onvif-zeep-async-3.1.9/onvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/ws-discovery.xsd` & `onvif-zeep-async-3.1.9/onvif/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/xml.xsd` & `onvif-zeep-async-3.1.9/onvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif/wsdl/xmlmime` & `onvif-zeep-async-3.1.9/onvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/PKG-INFO` & `onvif-zeep-async-3.1.9/onvif_zeep_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 3.1.8
+Version: 3.1.9
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-3.1.8/onvif_zeep_async.egg-info/SOURCES.txt` & `onvif-zeep-async-3.1.9/onvif_zeep_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/pylintrc` & `onvif-zeep-async-3.1.9/pylintrc`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/setup.py` & `onvif-zeep-async-3.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/tests/test.py` & `onvif-zeep-async-3.1.9/tests/test.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.8/tests/test_util.py` & `onvif-zeep-async-3.1.9/tests/test_util.py`

 * *Files identical despite different names*

