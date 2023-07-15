# Comparing `tmp/tg-botting-2.1.4.tar.gz` & `tmp/tg-botting-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg-botting-2.1.4.tar", last modified: Fri Jul 14 23:18:30 2023, max compression
+gzip compressed data, was "tg-botting-2.1.5.tar", last modified: Sat Jul 15 15:36:19 2023, max compression
```

## Comparing `tg-botting-2.1.4.tar` & `tg-botting-2.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 23:18:30.214655 tg-botting-2.1.4/
--rw-rw-rw-   0        0        0     3407 2023-07-14 23:18:30.213658 tg-botting-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1709 2023-07-12 19:32:58.000000 tg-botting-2.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-14 23:18:30.214655 tg-botting-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0     2624 2023-07-12 19:37:56.000000 tg-botting-2.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 23:18:30.209231 tg-botting-2.1.4/tg_botting/
--rw-rw-rw-   0        0        0      823 2023-07-14 23:18:12.000000 tg-botting-2.1.4/tg_botting/__init__.py
--rw-rw-rw-   0        0        0       39 2023-05-26 21:28:31.000000 tg-botting-2.1.4/tg_botting/_types.py
--rw-rw-rw-   0        0        0      730 2023-07-13 11:59:36.000000 tg-botting-2.1.4/tg_botting/abstract.py
--rw-rw-rw-   0        0        0    19269 2023-07-12 16:28:14.000000 tg-botting-2.1.4/tg_botting/bot.py
--rw-rw-rw-   0        0        0    29574 2023-07-13 23:53:43.000000 tg-botting-2.1.4/tg_botting/client.py
--rw-rw-rw-   0        0        0    12615 2023-05-26 21:34:31.000000 tg-botting-2.1.4/tg_botting/cog.py
--rw-rw-rw-   0        0        0    35621 2023-05-26 21:39:01.000000 tg-botting-2.1.4/tg_botting/commands.py
--rw-rw-rw-   0        0        0     3635 2023-07-13 11:59:36.000000 tg-botting-2.1.4/tg_botting/context.py
--rw-rw-rw-   0        0        0     1361 2023-05-26 21:43:21.000000 tg-botting-2.1.4/tg_botting/context_managers.py
--rw-rw-rw-   0        0        0     1410 2023-05-26 21:35:15.000000 tg-botting-2.1.4/tg_botting/conversions.py
--rw-rw-rw-   0        0        0     3679 2023-05-26 21:31:45.000000 tg-botting-2.1.4/tg_botting/cooldowns.py
--rw-rw-rw-   0        0        0    10433 2023-05-26 21:27:27.000000 tg-botting-2.1.4/tg_botting/exceptions.py
--rw-rw-rw-   0        0        0      902 2023-05-27 14:01:15.000000 tg-botting-2.1.4/tg_botting/general.py
--rw-rw-rw-   0        0        0     9737 2023-05-27 13:35:03.000000 tg-botting-2.1.4/tg_botting/group.py
--rw-rw-rw-   0        0        0      573 2023-07-14 23:16:54.000000 tg-botting-2.1.4/tg_botting/limiters.py
--rw-rw-rw-   0        0        0    19234 2023-07-14 21:40:48.000000 tg-botting-2.1.4/tg_botting/message.py
--rw-rw-rw-   0        0        0    33413 2023-07-14 22:47:31.000000 tg-botting-2.1.4/tg_botting/objects.py
--rw-rw-rw-   0        0        0     3037 2023-07-11 21:05:01.000000 tg-botting-2.1.4/tg_botting/permissions.py
--rw-rw-rw-   0        0        0     1919 2023-07-12 15:17:24.000000 tg-botting-2.1.4/tg_botting/user.py
--rw-rw-rw-   0        0        0     1023 2023-07-13 22:59:13.000000 tg-botting-2.1.4/tg_botting/utils.py
--rw-rw-rw-   0        0        0     4368 2023-05-26 21:44:26.000000 tg-botting-2.1.4/tg_botting/view.py
-drwxrwxrwx   0        0        0        0 2023-07-14 23:18:30.212660 tg-botting-2.1.4/tg_botting.egg-info/
--rw-rw-rw-   0        0        0     3407 2023-07-14 23:18:30.000000 tg-botting-2.1.4/tg_botting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      655 2023-07-14 23:18:30.000000 tg-botting-2.1.4/tg_botting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 23:18:30.000000 tg-botting-2.1.4/tg_botting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-14 23:18:30.000000 tg-botting-2.1.4/tg_botting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-14 23:18:30.000000 tg-botting-2.1.4/tg_botting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 15:36:19.789288 tg-botting-2.1.5/
+-rw-rw-rw-   0        0        0     3407 2023-07-15 15:36:19.789288 tg-botting-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1709 2023-07-12 19:32:58.000000 tg-botting-2.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-15 15:36:19.789288 tg-botting-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     2624 2023-07-12 19:37:56.000000 tg-botting-2.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 15:36:19.773667 tg-botting-2.1.5/tg_botting/
+-rw-rw-rw-   0        0        0      798 2023-07-15 15:34:44.000000 tg-botting-2.1.5/tg_botting/__init__.py
+-rw-rw-rw-   0        0        0       39 2023-05-26 21:28:31.000000 tg-botting-2.1.5/tg_botting/_types.py
+-rw-rw-rw-   0        0        0      730 2023-07-13 11:59:36.000000 tg-botting-2.1.5/tg_botting/abstract.py
+-rw-rw-rw-   0        0        0    19269 2023-07-12 16:28:14.000000 tg-botting-2.1.5/tg_botting/bot.py
+-rw-rw-rw-   0        0        0    31607 2023-07-15 15:34:44.000000 tg-botting-2.1.5/tg_botting/client.py
+-rw-rw-rw-   0        0        0    12615 2023-05-26 21:34:31.000000 tg-botting-2.1.5/tg_botting/cog.py
+-rw-rw-rw-   0        0        0    35621 2023-05-26 21:39:01.000000 tg-botting-2.1.5/tg_botting/commands.py
+-rw-rw-rw-   0        0        0     3635 2023-07-13 11:59:36.000000 tg-botting-2.1.5/tg_botting/context.py
+-rw-rw-rw-   0        0        0     1361 2023-05-26 21:43:21.000000 tg-botting-2.1.5/tg_botting/context_managers.py
+-rw-rw-rw-   0        0        0     1410 2023-05-26 21:35:15.000000 tg-botting-2.1.5/tg_botting/conversions.py
+-rw-rw-rw-   0        0        0     3679 2023-05-26 21:31:45.000000 tg-botting-2.1.5/tg_botting/cooldowns.py
+-rw-rw-rw-   0        0        0    10433 2023-05-26 21:27:27.000000 tg-botting-2.1.5/tg_botting/exceptions.py
+-rw-rw-rw-   0        0        0      902 2023-05-27 14:01:15.000000 tg-botting-2.1.5/tg_botting/general.py
+-rw-rw-rw-   0        0        0     9737 2023-05-27 13:35:03.000000 tg-botting-2.1.5/tg_botting/group.py
+-rw-rw-rw-   0        0        0      578 2023-07-14 23:30:00.000000 tg-botting-2.1.5/tg_botting/limiters.py
+-rw-rw-rw-   0        0        0    18252 2023-07-15 15:34:44.000000 tg-botting-2.1.5/tg_botting/message.py
+-rw-rw-rw-   0        0        0    33413 2023-07-14 22:47:31.000000 tg-botting-2.1.5/tg_botting/objects.py
+-rw-rw-rw-   0        0        0     3037 2023-07-11 21:05:01.000000 tg-botting-2.1.5/tg_botting/permissions.py
+-rw-rw-rw-   0        0        0     1919 2023-07-12 15:17:24.000000 tg-botting-2.1.5/tg_botting/user.py
+-rw-rw-rw-   0        0        0     1023 2023-07-13 22:59:13.000000 tg-botting-2.1.5/tg_botting/utils.py
+-rw-rw-rw-   0        0        0     4368 2023-05-26 21:44:26.000000 tg-botting-2.1.5/tg_botting/view.py
+drwxrwxrwx   0        0        0        0 2023-07-15 15:36:19.789288 tg-botting-2.1.5/tg_botting.egg-info/
+-rw-rw-rw-   0        0        0     3407 2023-07-15 15:36:19.000000 tg-botting-2.1.5/tg_botting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      655 2023-07-15 15:36:19.000000 tg-botting-2.1.5/tg_botting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 15:36:19.000000 tg-botting-2.1.5/tg_botting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-15 15:36:19.000000 tg-botting-2.1.5/tg_botting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-15 15:36:19.000000 tg-botting-2.1.5/tg_botting.egg-info/top_level.txt
```

### Comparing `tg-botting-2.1.4/PKG-INFO` & `tg-botting-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 2.1.4
+Version: 2.1.5
 Summary: A basic package for building async TG bots
 Home-page: https://github.com/2sweetheart2/tg_botting
 Author: Sweetie (Roma Fomkin)
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-2.1.4/README.md` & `tg-botting-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.4/setup.py` & `tg-botting-2.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.4/tg_botting/__init__.py` & `tg-botting-2.1.5/tg_botting/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 _title__ = 'tg_botting'
 __author__ = 'Sweetie'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023-present Sweetie'
-__version__ = '2.1.4'
+__version__ = '2.1.5'
 
 from collections import namedtuple
 import logging
 
 from .bot import Bot
 from .limiters import *
 from .conversions import Converter
 from .message import *
 from .user import *
 from .utils import *
 from .permissions import *
 from .objects import *
-from .commands import *
 
 
 VersionInfo = namedtuple('VersionInfo', 'major minor micro releaselevel serial')
 
 version_info = VersionInfo(major=0, minor=11, micro=0, releaselevel='development', serial=0)
 
 try:
```

### Comparing `tg-botting-2.1.4/tg_botting/abstract.py` & `tg-botting-2.1.5/tg_botting/abstract.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.4/tg_botting/bot.py` & `tg-botting-2.1.5/tg_botting/bot.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.4/tg_botting/client.py` & `tg-botting-2.1.5/tg_botting/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import enum
 import sys
 import textwrap
 import traceback
 import typing
 from typing import TypeVar
-
+import datetime
 import aiohttp
 
 from tg_botting.exceptions import TGException, TGApiError, BadArgument
 from tg_botting.general import convert_params
 from tg_botting.message import Chat, Message, CallbackQuery
 from tg_botting.objects import get_chat_member, MessageEntity, InlineKeyboardMarkup, ReplyKeyboardMarkup, \
     ReplyKeyboardRemove
@@ -60,14 +60,15 @@
         self.force = kwargs.get('force', False)
         self.lang = kwargs.get('lang', None)
         self.loop = asyncio.get_event_loop()
         self.group = None
         self.user = None
         self.key = None
         self.server = None
+        self.offset = 0
         self._listeners = {}
         timeout = aiohttp.ClientTimeout(total=100, connect=10)
         user_agent = kwargs.get('user_agent', None)
         if user_agent:
             headers = {
                 'User-Agent': user_agent
             }
@@ -283,32 +284,35 @@
         res = Message(msg)
         res.bot = self
         return res
 
     def generate_link(self, method: str):
         return f'https://api.telegram.org/bot{self.token}/{method}'
 
-    async def longpoll(self, offset=None):
-        if offset is None:
-            offset = 0
-        payload = {'offset': offset + 1}
+    async def longpoll(self):
+        if self.offset is None:
+            self.offset = 0
+        payload = {'offset': self.offset}
         try:
             res = await self.general_request(self.generate_link("getUpdates"), **payload)
         except asyncio.TimeoutError:
-            return offset, []
+            return self.offset, []
+        print(res)
+
         if res['ok'] is False:
-            offset = 0
+            self.offset = 0
         elif len(res['result']) != 0:
-            offset = res['result'][len(res['result']) - 1]['update_id']
+            self.offset = res['result'][len(res['result']) - 1]['update_id']+1
         updates = res['result']
-        return offset, updates
+        return self.offset, updates
 
     def handle_message(self, message):
         msg = self.build_msg(message)
-
+        if not self.check_date(msg):
+            return
         action = None
         if msg.sticker is not None:
             action = "sticker_new"
         elif msg.audio is not None:
             action = "audio_new"
         elif msg.video is not None:
             action = "video_new"
@@ -325,15 +329,16 @@
         elif msg.new_chat_members is not None:
             action = 'new_chat_members'
         elif msg.successful_payment is not None:
             action = "successful_payment"
 
         if action is not None:
             return self.dispatch(action, msg)
-
+        if msg.text is None:
+            return self.dispatch("something_without_text",msg)
         return self.dispatch('message_new', msg)
 
     def handle_callback_query(self, t, obj):
         event = CallbackQuery(obj)
         event.bot = self
         return self.dispatch(t, event)
 
@@ -357,16 +362,23 @@
         if class_name not in globals():
             return self.dispatch('unknown', update)
 
         klass = globals()[class_name]
         instance = klass(obj)
         return self.dispatch(t, instance)
 
+    def check_date(self, message):
+        date = datetime.datetime.now() - datetime.timedelta(seconds=5)
+        return message.date > date
+
     def handle_update(self, update):
-        update.pop('update_id')
+        try:
+            update.pop('update_id')
+        except Exception:
+            return
         t = list(update.keys())[0]
         obj = update[t]
         on_t = 'on_{}'.format(t)
         used = (t in self._listeners and self._listeners[t]) or (on_t in self.extra_events and self.extra_events[on_t])
         unknown_used = ('unknown' in self._listeners and self._listeners['unknown']) or (
                 'on_unknown' in self.extra_events and self.extra_events['on_unknown'])
         if t == 'message':
@@ -437,14 +449,15 @@
                          ReplyKeyboardMarkup,
                          ReplyKeyboardRemove,
                          None] = None,
                          has_spoiler: typing.Optional[Boolean] = None,
                          ) -> Message:
         reply_markup = reply_markup.dict if reply_markup is not None else None
         caption_entities = [r.dict for r in caption_entities] if caption_entities else None
+        print(parse_mode)
         data = {
             'chat_id':chat_id,
             'photo':photo,
             'caption':caption,
             'parse_mode':parse_mode,
             'caption_entities':caption_entities,
             'message_thread_id':message_thread_id,
@@ -452,15 +465,15 @@
             'protect_content':protect_content,
             'reply_to_message_id':reply_to_message_id,
             'allow_sending_without_reply':allow_sending_without_reply,
             'reply_markup':reply_markup,
             'has_spoiler':has_spoiler
         }
 
-        result = await self.tg_request('dendPhoto', True, **data)
+        result = await self.tg_request('sendPhoto', True, **data)
         return result
 
     @staticmethod
     def prepare_file(payload, files, key, file):
         if isinstance(file, str):
             payload[key] = file
         elif file is not None:
@@ -477,14 +490,43 @@
             except asyncio.CancelledError:
                 pass
 
     def _schedule_event(self, coro, event_name, *args, **kwargs):
         wrapped = self._run_event(coro, event_name, *args, **kwargs)
         return _ClientEventTask(original_coro=coro, event_name=event_name, coro=wrapped, loop=self.loop)
 
+    async def edit_message_text(self,chat_id,text,message_id=None,inline_message_id=None,entities=None,parse_mode	=None,disable_web_page_preview=None,reply_markup=None):
+        params = {'chat_id': chat_id,
+                  'text': text,
+                  'message_id':message_id,
+                  'inline_message_id':inline_message_id,
+                  'parse_mode': parse_mode,
+                  'entities': [r.dict for r in entities] if entities else None,
+                  'disable_web_page_preview': disable_web_page_preview,
+                  'reply_markup': reply_markup.dict if reply_markup else None,
+                  }
+        res = await self.tg_request('editMessageText',**params)
+        if res.get('ok') != True:
+            raise TGApiError('[{error_code}] {description}'.format(**res))
+        return res
+
+    async def edit_message_caption(self,chat_id,caption,message_id=None,inline_message_id=None,caption_entities=None,parse_mode	=None,reply_markup=None):
+        params = {'chat_id': chat_id,
+                  'caption': caption,
+                  'inline_message_id':inline_message_id,
+                  'message_id':message_id,
+                  'parse_mode': parse_mode,
+                  'caption_entities': [r.dict for r in caption_entities] if caption_entities else None,
+                  'reply_markup': reply_markup.dict if reply_markup else None,
+                  }
+        res = await self.tg_request('editMessageCaption',**params)
+        if res.get('ok') != True:
+            raise TGApiError('[{error_code}] {description}'.format(**res))
+        return res
+
     async def send_message(self, chat_id, text, message_thread_id=None, parse_mode=None, disable_web_page_preview=None,
                            disable_notification=None, entities=None,
                            protect_content=None, reply_to_message_id=None, allow_sending_without_reply=None,
                            reply_markup=None, **kwargs):
         as_user = kwargs.pop('as_user', False)
         if kwargs:
             print('Unknown parameters passed to send_message: {}'.format(', '.join(kwargs.keys())), file=sys.stderr)
@@ -541,26 +583,24 @@
         await self.attach_user_token(token)
 
     async def _run(self):
         self.is_group = True
         self.group = await self.get_me()
         self.dispatch('ready')
         updates = []
-        offset = None
         while True:
             try:
-                lp = self.loop.create_task(self.longpoll(offset))
+                lp = self.loop.create_task(self.longpoll())
                 for update in updates:
                     self.handle_update(update)
-                offset, updates = await lp
+                self.offset, updates = await lp
             except Exception as e:
-                if self.use_stack_trace:
-                    traceback.print_exc(file=sys.stderr)
+                traceback.print_exc(file=sys.stderr)
                 print('Ignoring exception in longpoll cycle:\n{}'.format(e), file=sys.stderr)
-                offset+=1
+                self.offset+=1
 
     def run(self, token, user_id=None, user_hash=None):
         self.use_stack_trace = False
         self.token = token
         self.user_id = user_id
         self.user_hash = user_hash
         self.loop.create_task(self._run())
```

### Comparing `tg-botting-2.1.4/tg_botting/cog.py` & `tg-botting-2.1.5/tg_botting/cog.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.4/tg_botting/commands.py` & `tg-botting-2.1.5/tg_botting/commands.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.4/tg_botting/context.py` & `tg-botting-2.1.5/tg_botting/context.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.4/tg_botting/context_managers.py` & `tg-botting-2.1.5/tg_botting/context_managers.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.4/tg_botting/conversions.py` & `tg-botting-2.1.5/tg_botting/conversions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.4/tg_botting/cooldowns.py` & `tg-botting-2.1.5/tg_botting/cooldowns.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.4/tg_botting/exceptions.py` & `tg-botting-2.1.5/tg_botting/exceptions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.4/tg_botting/general.py` & `tg-botting-2.1.5/tg_botting/general.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.4/tg_botting/group.py` & `tg-botting-2.1.5/tg_botting/group.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.4/tg_botting/limiters.py` & `tg-botting-2.1.5/tg_botting/limiters.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from tg_botting import Command
+from tg_botting.commands import *
+
 
 def check(predicate):
 
     def decorator(func):
         if isinstance(func, Command):
             func.checks.append(predicate)
         else:
```

### Comparing `tg-botting-2.1.4/tg_botting/message.py` & `tg-botting-2.1.5/tg_botting/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     __slots__ = ('bot', 'id', 'from_', 'message', 'inline_message_id', 'chat_instance', 'data', 'game_short_name')
 
     def __init__(self, data):
         self._unpack(data)
 
     def _unpack(self, data):
         self.id = data.get('id')
-        self.from_ = data.get('from')
+        self.from_ = User(data.get('from'))
         self.message = Message(data.get('message'))
         self.inline_message_id = data.get('inline_message_id')
         self.chat_instance = data.get('chat_instance')
         self.data = data.get('data')
         self.game_short_name = data.get('game_short_name')
 
     async def _answer(self, text="", show_alert=True, url=None, cache_time=None):
@@ -152,15 +152,15 @@
         self.is_automatic_forward = data.get('is_automatic_forward') if 'is_automatic_forward' in data else False
         self.reply_to_message = Message(data.get('reply_to_message')) if 'reply_to_message' in data else None
         self.via_bot = User(data.get('via_bot')) if 'via_bot' in data else None
         self.edit_date = datetime.fromtimestamp(data.get('edit_date')) if 'edit_date' in data else None
         self.has_protected_content = data.get('has_protected_content') if 'has_protected_content' in data else False
         self.media_group_id = data.get('media_group_id') if 'media_group_id' in data else None
         self.author_signature = data.get('author_signature') if 'author_signature' in data else None
-        self.text = data.get('text') if 'text' in data and data.get('text', None) is not None else None
+        self.text = data.get('text') if 'text' in data else None
         self.entities = [MessageEntity(r) for r in data.get('entities')] if 'entities' in data and data.get('entities',
                                                                                                             None) is not None else []
         self.animation = Animation(data.get('animation')) if 'animation' in data else None
         self.audio = Audio(data.get('audio')) if 'audio' in data else None
         self.document = Document(data.get('document')) if 'document' in data else None
         self.photo = [PhotoSize(r) for r in data.get('photo')] if 'photo' in data else None
         self.sticker = Sticker(data.get('sticker')) if 'sticker' in data else None
@@ -223,36 +223,16 @@
         self.video_chat_ended = VideoChatEnded(data.get('video_chat_ended')) if 'video_chat_ended' in data else None
         self.video_chat_participants_invited = VideoChatParticipantsInvited(
             data.get('video_chat_participants_invited')) if 'video_chat_participants_invited' in data else None
         self.web_app_data = WebAppData(data.get('web_app_data')) if 'web_app_data' in data else None
         self.reply_markup = InlineKeyboardMarkup(data.get('reply_markup')) if 'reply_markup' in data and data.get(
             'reply_markup', None) is not None else None
 
-    async def edit(self, text=None, *, reply_markup: InlineKeyboardMarkup = None, parse_mode: str = None,
-                   entities: ctypes.Array = None, disable_web_page_preview: bool = None, message_id: int = None,
-                   inline_message_id: int = None):
-        params = {
-            'chat_id': self.chat.id,
-            'text': text
-        }
-        if reply_markup:
-            params['reply_markup'] = json.dumps(reply_markup.dict)
-        if parse_mode:
-            params['parse_mode'] = parse_mode
-        if entities:
-            params['entities'] = [r.dict for r in entities]
-        if disable_web_page_preview:
-            params['disable_web_page_preview'] = disable_web_page_preview
-        if message_id:
-            params['message_id'] = message_id
-        if inline_message_id:
-            params['inline_message_id'] = inline_message_id
-        res = await self.bot.tg_request('editMessageText', **params)
-        if 'error' in res.keys():
-            raise TGApiError('[{error_code}] {error_msg}'.format(**res['error']))
+    async def edit_text(self, text: str,**kwargs):
+        res = await self.bot.edit_message_text(self.chat.id,text,**kwargs)
         return res
 
     async def delete(self):
         params = {
             'chat_id': self.chat.id,
             'message_id': self.message_id
         }
@@ -261,17 +241,17 @@
             raise TGApiError('[{error_code}] {error_msg}'.format(**res))
 
 
 
     async def send_photo(self,
                          photo:str,
                          caption: str=None,**kwargs):
-        res = await self.bot.send_photo(self.chat.id,photo,caption,*kwargs)
+        res = await self.bot.send_photo(self.chat.id,photo,caption,**kwargs)
         if res['ok']!=True:
-            raise TGApiError('[{error_code}] {error_msg}'.format(**res))
+            raise TGApiError('[{error_code}] {description}'.format(**res))
         return Message(res['result'])
 
     async def reply(self, text, **kwargs):
         return await self.bot.send_message(text, reply_to_message_id=self.message_id,**kwargs)
 
     async def get_user(self):
         author = await self.bot.get_pages(self.from_id)
```

### Comparing `tg-botting-2.1.4/tg_botting/objects.py` & `tg-botting-2.1.5/tg_botting/objects.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.4/tg_botting/permissions.py` & `tg-botting-2.1.5/tg_botting/permissions.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.4/tg_botting/user.py` & `tg-botting-2.1.5/tg_botting/user.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.4/tg_botting/utils.py` & `tg-botting-2.1.5/tg_botting/utils.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.4/tg_botting/view.py` & `tg-botting-2.1.5/tg_botting/view.py`

 * *Files identical despite different names*

### Comparing `tg-botting-2.1.4/tg_botting.egg-info/PKG-INFO` & `tg-botting-2.1.5/tg_botting.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 2.1.4
+Version: 2.1.5
 Summary: A basic package for building async TG bots
 Home-page: https://github.com/2sweetheart2/tg_botting
 Author: Sweetie (Roma Fomkin)
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-2.1.4/tg_botting.egg-info/SOURCES.txt` & `tg-botting-2.1.5/tg_botting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

