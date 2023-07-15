# Comparing `tmp/tg-botting-2.1.5.tar.gz` & `tmp/tg-botting-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg-botting-2.1.5.tar", last modified: Sat Jul 15 15:36:19 2023, max compression
+gzip compressed data, was "tg-botting-2.1.6.tar", last modified: Sat Jul 15 16:26:52 2023, max compression
```

## Comparing `tg-botting-2.1.5.tar` & `tg-botting-2.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 15:36:19.789288 tg-botting-2.1.5/
--rw-rw-rw-   0        0        0     3407 2023-07-15 15:36:19.789288 tg-botting-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1709 2023-07-12 19:32:58.000000 tg-botting-2.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-15 15:36:19.789288 tg-botting-2.1.5/setup.cfg
--rw-rw-rw-   0        0        0     2624 2023-07-12 19:37:56.000000 tg-botting-2.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 15:36:19.773667 tg-botting-2.1.5/tg_botting/
--rw-rw-rw-   0        0        0      798 2023-07-15 15:34:44.000000 tg-botting-2.1.5/tg_botting/__init__.py
--rw-rw-rw-   0        0        0       39 2023-05-26 21:28:31.000000 tg-botting-2.1.5/tg_botting/_types.py
--rw-rw-rw-   0        0        0      730 2023-07-13 11:59:36.000000 tg-botting-2.1.5/tg_botting/abstract.py
--rw-rw-rw-   0        0        0    19269 2023-07-12 16:28:14.000000 tg-botting-2.1.5/tg_botting/bot.py
--rw-rw-rw-   0        0        0    31607 2023-07-15 15:34:44.000000 tg-botting-2.1.5/tg_botting/client.py
--rw-rw-rw-   0        0        0    12615 2023-05-26 21:34:31.000000 tg-botting-2.1.5/tg_botting/cog.py
--rw-rw-rw-   0        0        0    35621 2023-05-26 21:39:01.000000 tg-botting-2.1.5/tg_botting/commands.py
--rw-rw-rw-   0        0        0     3635 2023-07-13 11:59:36.000000 tg-botting-2.1.5/tg_botting/context.py
--rw-rw-rw-   0        0        0     1361 2023-05-26 21:43:21.000000 tg-botting-2.1.5/tg_botting/context_managers.py
--rw-rw-rw-   0        0        0     1410 2023-05-26 21:35:15.000000 tg-botting-2.1.5/tg_botting/conversions.py
--rw-rw-rw-   0        0        0     3679 2023-05-26 21:31:45.000000 tg-botting-2.1.5/tg_botting/cooldowns.py
--rw-rw-rw-   0        0        0    10433 2023-05-26 21:27:27.000000 tg-botting-2.1.5/tg_botting/exceptions.py
--rw-rw-rw-   0        0        0      902 2023-05-27 14:01:15.000000 tg-botting-2.1.5/tg_botting/general.py
--rw-rw-rw-   0        0        0     9737 2023-05-27 13:35:03.000000 tg-botting-2.1.5/tg_botting/group.py
--rw-rw-rw-   0        0        0      578 2023-07-14 23:30:00.000000 tg-botting-2.1.5/tg_botting/limiters.py
--rw-rw-rw-   0        0        0    18252 2023-07-15 15:34:44.000000 tg-botting-2.1.5/tg_botting/message.py
--rw-rw-rw-   0        0        0    33413 2023-07-14 22:47:31.000000 tg-botting-2.1.5/tg_botting/objects.py
--rw-rw-rw-   0        0        0     3037 2023-07-11 21:05:01.000000 tg-botting-2.1.5/tg_botting/permissions.py
--rw-rw-rw-   0        0        0     1919 2023-07-12 15:17:24.000000 tg-botting-2.1.5/tg_botting/user.py
--rw-rw-rw-   0        0        0     1023 2023-07-13 22:59:13.000000 tg-botting-2.1.5/tg_botting/utils.py
--rw-rw-rw-   0        0        0     4368 2023-05-26 21:44:26.000000 tg-botting-2.1.5/tg_botting/view.py
-drwxrwxrwx   0        0        0        0 2023-07-15 15:36:19.789288 tg-botting-2.1.5/tg_botting.egg-info/
--rw-rw-rw-   0        0        0     3407 2023-07-15 15:36:19.000000 tg-botting-2.1.5/tg_botting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      655 2023-07-15 15:36:19.000000 tg-botting-2.1.5/tg_botting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 15:36:19.000000 tg-botting-2.1.5/tg_botting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-15 15:36:19.000000 tg-botting-2.1.5/tg_botting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-15 15:36:19.000000 tg-botting-2.1.5/tg_botting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 16:26:52.030294 tg-botting-2.1.6/
+-rw-rw-rw-   0        0        0     3407 2023-07-15 16:26:52.030294 tg-botting-2.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1709 2023-07-12 19:32:58.000000 tg-botting-2.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-15 16:26:52.030294 tg-botting-2.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     2624 2023-07-12 19:37:56.000000 tg-botting-2.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:26:52.030294 tg-botting-2.1.6/tg_botting/
+-rw-rw-rw-   0        0        0      798 2023-07-15 16:26:18.000000 tg-botting-2.1.6/tg_botting/__init__.py
+-rw-rw-rw-   0        0        0       39 2023-05-26 21:28:31.000000 tg-botting-2.1.6/tg_botting/_types.py
+-rw-rw-rw-   0        0        0      730 2023-07-13 11:59:36.000000 tg-botting-2.1.6/tg_botting/abstract.py
+-rw-rw-rw-   0        0        0    19269 2023-07-12 16:28:14.000000 tg-botting-2.1.6/tg_botting/bot.py
+-rw-rw-rw-   0        0        0    31560 2023-07-15 16:26:18.000000 tg-botting-2.1.6/tg_botting/client.py
+-rw-rw-rw-   0        0        0    12615 2023-05-26 21:34:31.000000 tg-botting-2.1.6/tg_botting/cog.py
+-rw-rw-rw-   0        0        0    35621 2023-05-26 21:39:01.000000 tg-botting-2.1.6/tg_botting/commands.py
+-rw-rw-rw-   0        0        0     3635 2023-07-13 11:59:36.000000 tg-botting-2.1.6/tg_botting/context.py
+-rw-rw-rw-   0        0        0     1361 2023-05-26 21:43:21.000000 tg-botting-2.1.6/tg_botting/context_managers.py
+-rw-rw-rw-   0        0        0     1410 2023-05-26 21:35:15.000000 tg-botting-2.1.6/tg_botting/conversions.py
+-rw-rw-rw-   0        0        0     3679 2023-05-26 21:31:45.000000 tg-botting-2.1.6/tg_botting/cooldowns.py
+-rw-rw-rw-   0        0        0    10433 2023-05-26 21:27:27.000000 tg-botting-2.1.6/tg_botting/exceptions.py
+-rw-rw-rw-   0        0        0      902 2023-05-27 14:01:15.000000 tg-botting-2.1.6/tg_botting/general.py
+-rw-rw-rw-   0        0        0     9737 2023-05-27 13:35:03.000000 tg-botting-2.1.6/tg_botting/group.py
+-rw-rw-rw-   0        0        0      578 2023-07-14 23:30:00.000000 tg-botting-2.1.6/tg_botting/limiters.py
+-rw-rw-rw-   0        0        0    18252 2023-07-15 15:34:44.000000 tg-botting-2.1.6/tg_botting/message.py
+-rw-rw-rw-   0        0        0    33413 2023-07-14 22:47:31.000000 tg-botting-2.1.6/tg_botting/objects.py
+-rw-rw-rw-   0        0        0     3037 2023-07-11 21:05:01.000000 tg-botting-2.1.6/tg_botting/permissions.py
+-rw-rw-rw-   0        0        0     1919 2023-07-12 15:17:24.000000 tg-botting-2.1.6/tg_botting/user.py
+-rw-rw-rw-   0        0        0     1023 2023-07-13 22:59:13.000000 tg-botting-2.1.6/tg_botting/utils.py
+-rw-rw-rw-   0        0        0     4368 2023-05-26 21:44:26.000000 tg-botting-2.1.6/tg_botting/view.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:26:52.030294 tg-botting-2.1.6/tg_botting.egg-info/
+-rw-rw-rw-   0        0        0     3407 2023-07-15 16:26:51.000000 tg-botting-2.1.6/tg_botting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      655 2023-07-15 16:26:51.000000 tg-botting-2.1.6/tg_botting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 16:26:51.000000 tg-botting-2.1.6/tg_botting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-15 16:26:51.000000 tg-botting-2.1.6/tg_botting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-15 16:26:51.000000 tg-botting-2.1.6/tg_botting.egg-info/top_level.txt
```

### Comparing `tg-botting-2.1.5/PKG-INFO` & `tg-botting-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 2.1.5
+Version: 2.1.6
 Summary: A basic package for building async TG bots
 Home-page: https://github.com/2sweetheart2/tg_botting
 Author: Sweetie (Roma Fomkin)
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-2.1.5/README.md` & `tg-botting-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/setup.py` & `tg-botting-2.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting/__init__.py` & `tg-botting-2.1.6/tg_botting/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 _title__ = 'tg_botting'
 __author__ = 'Sweetie'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023-present Sweetie'
-__version__ = '2.1.5'
+__version__ = '2.1.6'
 
 from collections import namedtuple
 import logging
 
 from .bot import Bot
 from .limiters import *
 from .conversions import Converter
```

### Comparing `tg-botting-2.1.5/tg_botting/abstract.py` & `tg-botting-2.1.6/tg_botting/abstract.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting/bot.py` & `tg-botting-2.1.6/tg_botting/bot.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting/client.py` & `tg-botting-2.1.6/tg_botting/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,14 @@
         if self.offset is None:
             self.offset = 0
         payload = {'offset': self.offset}
         try:
             res = await self.general_request(self.generate_link("getUpdates"), **payload)
         except asyncio.TimeoutError:
             return self.offset, []
-        print(res)
 
         if res['ok'] is False:
             self.offset = 0
         elif len(res['result']) != 0:
             self.offset = res['result'][len(res['result']) - 1]['update_id']+1
         updates = res['result']
         return self.offset, updates
@@ -449,15 +448,14 @@
                          ReplyKeyboardMarkup,
                          ReplyKeyboardRemove,
                          None] = None,
                          has_spoiler: typing.Optional[Boolean] = None,
                          ) -> Message:
         reply_markup = reply_markup.dict if reply_markup is not None else None
         caption_entities = [r.dict for r in caption_entities] if caption_entities else None
-        print(parse_mode)
         data = {
             'chat_id':chat_id,
             'photo':photo,
             'caption':caption,
             'parse_mode':parse_mode,
             'caption_entities':caption_entities,
             'message_thread_id':message_thread_id,
```

### Comparing `tg-botting-2.1.5/tg_botting/cog.py` & `tg-botting-2.1.6/tg_botting/cog.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting/commands.py` & `tg-botting-2.1.6/tg_botting/commands.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting/context.py` & `tg-botting-2.1.6/tg_botting/context.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting/context_managers.py` & `tg-botting-2.1.6/tg_botting/context_managers.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting/conversions.py` & `tg-botting-2.1.6/tg_botting/conversions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting/cooldowns.py` & `tg-botting-2.1.6/tg_botting/cooldowns.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting/exceptions.py` & `tg-botting-2.1.6/tg_botting/exceptions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting/general.py` & `tg-botting-2.1.6/tg_botting/general.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting/group.py` & `tg-botting-2.1.6/tg_botting/group.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting/limiters.py` & `tg-botting-2.1.6/tg_botting/limiters.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting/message.py` & `tg-botting-2.1.6/tg_botting/message.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting/objects.py` & `tg-botting-2.1.6/tg_botting/objects.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting/permissions.py` & `tg-botting-2.1.6/tg_botting/permissions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting/user.py` & `tg-botting-2.1.6/tg_botting/user.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting/utils.py` & `tg-botting-2.1.6/tg_botting/utils.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting/view.py` & `tg-botting-2.1.6/tg_botting/view.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.5/tg_botting.egg-info/PKG-INFO` & `tg-botting-2.1.6/tg_botting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 2.1.5
+Version: 2.1.6
 Summary: A basic package for building async TG bots
 Home-page: https://github.com/2sweetheart2/tg_botting
 Author: Sweetie (Roma Fomkin)
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-2.1.5/tg_botting.egg-info/SOURCES.txt` & `tg-botting-2.1.6/tg_botting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

