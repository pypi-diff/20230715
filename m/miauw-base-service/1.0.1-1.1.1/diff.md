# Comparing `tmp/miauw-base-service-1.0.1.tar.gz` & `tmp/miauw-base-service-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miauw-base-service-1.0.1.tar", last modified: Sat Jul 15 13:06:21 2023, max compression
+gzip compressed data, was "miauw-base-service-1.1.1.tar", last modified: Sat Jul 15 16:10:34 2023, max compression
```

## Comparing `miauw-base-service-1.0.1.tar` & `miauw-base-service-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-15 13:06:21.114938 miauw-base-service-1.0.1/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-15 13:06:21.111605 miauw-base-service-1.0.1/PKG-INFO
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-15 13:06:21.111605 miauw-base-service-1.0.1/base_service/
--rw-r--r--   0 leo       (1000) leo       (1000)       67 2023-07-15 13:04:36.000000 miauw-base-service-1.0.1/base_service/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2091 2023-07-15 12:45:55.000000 miauw-base-service-1.0.1/base_service/service.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1879 2023-07-14 10:06:11.000000 miauw-base-service-1.0.1/base_service/worker.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-15 13:06:21.111605 miauw-base-service-1.0.1/miauw_base_service.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-15 13:06:21.000000 miauw-base-service-1.0.1/miauw_base_service.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-15 13:06:21.000000 miauw-base-service-1.0.1/miauw_base_service.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-15 13:06:21.000000 miauw-base-service-1.0.1/miauw_base_service.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-15 13:06:21.000000 miauw-base-service-1.0.1/miauw_base_service.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-15 13:06:21.000000 miauw-base-service-1.0.1/miauw_base_service.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-15 13:05:35.000000 miauw-base-service-1.0.1/pyproject.toml
--rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-15 13:06:21.114938 miauw-base-service-1.0.1/setup.cfg
--rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-15 13:05:30.000000 miauw-base-service-1.0.1/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-15 16:10:34.851368 miauw-base-service-1.1.1/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-15 16:10:34.848034 miauw-base-service-1.1.1/PKG-INFO
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-15 16:10:34.848034 miauw-base-service-1.1.1/base_service/
+-rw-r--r--   0 leo       (1000) leo       (1000)       67 2023-07-15 13:04:36.000000 miauw-base-service-1.1.1/base_service/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2026 2023-07-15 15:57:46.000000 miauw-base-service-1.1.1/base_service/service.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1997 2023-07-15 16:03:21.000000 miauw-base-service-1.1.1/base_service/worker.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2023-07-15 16:10:34.848034 miauw-base-service-1.1.1/miauw_base_service.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)      272 2023-07-15 16:10:34.000000 miauw-base-service-1.1.1/miauw_base_service.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-15 16:10:34.000000 miauw-base-service-1.1.1/miauw_base_service.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2023-07-15 16:10:34.000000 miauw-base-service-1.1.1/miauw_base_service.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       23 2023-07-15 16:10:34.000000 miauw-base-service-1.1.1/miauw_base_service.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       31 2023-07-15 16:10:34.000000 miauw-base-service-1.1.1/miauw_base_service.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      304 2023-07-15 16:05:44.000000 miauw-base-service-1.1.1/pyproject.toml
+-rw-r--r--   0 leo       (1000) leo       (1000)       38 2023-07-15 16:10:34.851368 miauw-base-service-1.1.1/setup.cfg
+-rw-r--r--   0 leo       (1000) leo       (1000)      437 2023-07-15 16:05:48.000000 miauw-base-service-1.1.1/setup.py
```

### Comparing `miauw-base-service-1.0.1/base_service/service.py` & `miauw-base-service-1.1.1/base_service/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import logging
 
 class BaseService:
     """creates the base service class"""
     def __init__(self, name: str, url: str, logfile: str = None, worker_log: bool = True):
         self.worker = RabbitMQWorker(url)
         self.events: list[str] = []
-        self.m: dict[str, typing.Callable[[dict], typing.Awaitable[dict]]] = defaultdict()
+        self.m: dict[str, typing.Callable[[typing.Any], typing.Awaitable[typing.Any]]] = defaultdict()
         self.name = name
+        # logging
         self.logger = logging.getLogger(name)
-        # self.log_formatter = logging.Formatter("[%(asctime)s] - %(name)s - %(levelname)s - %(message)s")
         self.log_formatter = logging.Formatter("[%(asctime)s] - %(name)s - %(message)s")
         self.log_filehandler = logging.FileHandler(logfile or "service.log")
         self.log_streamhandler = logging.StreamHandler()
         self.logger.setLevel(logging.DEBUG)
         self.log_filehandler.setLevel(logging.DEBUG)
         self.log_streamhandler.setLevel(logging.INFO)
         self.log_filehandler.setFormatter(self.log_formatter)
@@ -29,15 +29,15 @@
         self.logger.info("starting")
         loop = asyncio.get_event_loop()
         for ev in self.events:
             self.logger.info(f"listening for event '{ev}'")
         loop.run_until_complete(asyncio.gather(*[self.worker.listen(k,v) for k,v in self.m.items()]))
 
 
-    def add_event_handler(self, event: str, handler: typing.Callable[[dict], typing.Awaitable[dict]]) -> None:
+    def add_event_handler(self, event: str, handler: typing.Callable[[typing.Any], typing.Awaitable[typing.Any]]) -> None:
         """adds a new event handler for service"""
         self.logger.debug(f"add handler {handler} for event '{event}'")
         self.events.append(event)
         self.m[event] = handler
 
 
     def event(self, event: str):
```

### Comparing `miauw-base-service-1.0.1/base_service/worker.py` & `miauw-base-service-1.1.1/base_service/worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,25 +21,28 @@
         return self
 
     async def send_basic(self, queue_name: str, data: bytes) -> None:
         """sends something to queue"""
         await self.ex.publish(aio_pika.Message(data), routing_key=queue_name)
 
     async def listen(
-        self, queue_name: str, worker_function: Callable[[dict], Awaitable[dict]]
+        self, queue_name: str, worker_function: Callable[[Any], Awaitable[Any]]
     ):
         await self.setup()
         queue = await self.channel.declare_queue(queue_name)
         async with queue.iterator() as qi:
             message: aio_pika.abc.AbstractMessage
             async for message in qi:
                 try:
                     async with message.process(requeue=False):
                         assert message.reply_to is not None
-                        data: dict = json.loads(message.body)
+                        if type(data) is dict:
+                            data = json.loads(message.body)
+                        else:
+                            data = str(data)
                         res = await worker_function(data)
                         await self.ex.publish(
                             aio_pika.Message(
                                 body=json.dumps(res).encode("utf-8"),
                                 correlation_id=message.correlation_id,
                             ),
                             routing_key=message.reply_to,
```

