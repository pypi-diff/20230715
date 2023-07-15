# Comparing `tmp/miauw-base-service-0.3.0.tar.gz` & `tmp/miauw-base-service-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miauw-base-service-0.3.0.tar", last modified: Fri Jul 14 10:12:08 2023, max compression
+gzip compressed data, was "miauw-base-service-1.0.0.tar", last modified: Sat Jul 15 12:56:43 2023, max compression
```

## Comparing `miauw-base-service-0.3.0.tar` & `miauw-base-service-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-14 10:12:08.369837 miauw-base-service-0.3.0/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-14 10:12:08.366504 miauw-base-service-0.3.0/PKG-INFO
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-14 10:12:08.366504 miauw-base-service-0.3.0/base_service/
--rw-r--r--   0 leo       (1000) leo       (1000)       63 2023-07-13 05:13:50.000000 miauw-base-service-0.3.0/base_service/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1850 2023-07-13 09:02:41.000000 miauw-base-service-0.3.0/base_service/service.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1879 2023-07-14 10:06:11.000000 miauw-base-service-0.3.0/base_service/worker.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-14 10:12:08.366504 miauw-base-service-0.3.0/miauw_base_service.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-14 10:12:08.000000 miauw-base-service-0.3.0/miauw_base_service.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-14 10:12:08.000000 miauw-base-service-0.3.0/miauw_base_service.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-14 10:12:08.000000 miauw-base-service-0.3.0/miauw_base_service.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-14 10:12:08.000000 miauw-base-service-0.3.0/miauw_base_service.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-14 10:12:08.000000 miauw-base-service-0.3.0/miauw_base_service.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-14 10:04:54.000000 miauw-base-service-0.3.0/pyproject.toml
--rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-14 10:12:08.369837 miauw-base-service-0.3.0/setup.cfg
--rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-14 10:11:27.000000 miauw-base-service-0.3.0/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-15 12:56:43.864951 miauw-base-service-1.0.0/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-15 12:56:43.864951 miauw-base-service-1.0.0/PKG-INFO
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-15 12:56:43.861617 miauw-base-service-1.0.0/base_service/
+-rw-r--r--   0 leo       (1000) leo       (1000)       63 2023-07-13 05:13:50.000000 miauw-base-service-1.0.0/base_service/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2091 2023-07-15 12:45:55.000000 miauw-base-service-1.0.0/base_service/service.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1879 2023-07-14 10:06:11.000000 miauw-base-service-1.0.0/base_service/worker.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-15 12:56:43.864951 miauw-base-service-1.0.0/miauw_base_service.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-15 12:56:43.000000 miauw-base-service-1.0.0/miauw_base_service.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-15 12:56:43.000000 miauw-base-service-1.0.0/miauw_base_service.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-15 12:56:43.000000 miauw-base-service-1.0.0/miauw_base_service.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-15 12:56:43.000000 miauw-base-service-1.0.0/miauw_base_service.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-15 12:56:43.000000 miauw-base-service-1.0.0/miauw_base_service.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-15 12:52:38.000000 miauw-base-service-1.0.0/pyproject.toml
+-rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-15 12:56:43.864951 miauw-base-service-1.0.0/setup.cfg
+-rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-15 12:52:28.000000 miauw-base-service-1.0.0/setup.py
```

### Comparing `miauw-base-service-0.3.0/base_service/service.py` & `miauw-base-service-1.0.0/base_service/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from base_service import RabbitMQWorker
 from collections import defaultdict
 import asyncio
 import typing
 import logging
 
-class Service:
+class BaseService:
     """creates the base service class"""
     def __init__(self, name: str, url: str, logfile: str = None, worker_log: bool = True):
         self.worker = RabbitMQWorker(url)
         self.events: list[str] = []
         self.m: dict[str, typing.Callable[[dict], typing.Awaitable[dict]]] = defaultdict()
         self.name = name
         self.logger = logging.getLogger(name)
@@ -34,7 +34,14 @@
 
 
     def add_event_handler(self, event: str, handler: typing.Callable[[dict], typing.Awaitable[dict]]) -> None:
         """adds a new event handler for service"""
         self.logger.debug(f"add handler {handler} for event '{event}'")
         self.events.append(event)
         self.m[event] = handler
+
+
+    def event(self, event: str):
+        """adds a new event handler for event"""
+        def wrapper(handler: typing.Callable[[dict], typing.Awaitable[dict]]):
+            self.add_event_handler(event, handler)
+        return wrapper
```

### Comparing `miauw-base-service-0.3.0/base_service/worker.py` & `miauw-base-service-1.0.0/base_service/worker.py`

 * *Files identical despite different names*

