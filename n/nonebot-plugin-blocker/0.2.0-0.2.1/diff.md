# Comparing `tmp/nonebot-plugin-blocker-0.2.0.tar.gz` & `tmp/nonebot-plugin-blocker-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-blocker-0.2.0.tar", last modified: Sat Jul 15 14:51:59 2023, max compression
+gzip compressed data, was "nonebot-plugin-blocker-0.2.1.tar", last modified: Sat Jul 15 18:18:57 2023, max compression
```

## Comparing `nonebot-plugin-blocker-0.2.0.tar` & `nonebot-plugin-blocker-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:51:59.398855 nonebot-plugin-blocker-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-15 14:51:59.398855 nonebot-plugin-blocker-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-15 14:51:35.000000 nonebot-plugin-blocker-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:51:59.394855 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-15 14:51:35.000000 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-15 14:51:35.000000 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-15 14:51:35.000000 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:51:59.398855 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-15 14:51:59.000000 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-15 14:51:59.000000 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 14:51:59.000000 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-15 14:51:59.000000 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 14:51:59.000000 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-15 14:51:35.000000 nonebot-plugin-blocker-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 14:51:59.398855 nonebot-plugin-blocker-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:18:57.176221 nonebot-plugin-blocker-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-15 18:18:57.176221 nonebot-plugin-blocker-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-15 18:18:40.000000 nonebot-plugin-blocker-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:18:57.176221 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-15 18:18:40.000000 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-15 18:18:40.000000 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-15 18:18:40.000000 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:18:57.176221 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-15 18:18:57.000000 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-15 18:18:57.000000 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 18:18:57.000000 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-15 18:18:57.000000 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 18:18:57.000000 nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-15 18:18:40.000000 nonebot-plugin-blocker-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 18:18:57.176221 nonebot-plugin-blocker-0.2.1/setup.cfg
```

### Comparing `nonebot-plugin-blocker-0.2.0/PKG-INFO` & `nonebot-plugin-blocker-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.2.0
+Version: 0.2.1
 Summary: Message Blocker
 Author-email: MerCuJerry <mercujerry@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/MerCuJerry/nonebot-plugin-blocker
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.2.1 Summary:
 Message Blocker Author-email: MerCuJerry
 gmail.com> License: MIT Project-URL: homepage, https://github.com/MerCuJerry/
 nonebot-plugin-blocker Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
```

### Comparing `nonebot-plugin-blocker-0.2.0/README.md` & `nonebot-plugin-blocker-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker/__main__.py` & `nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,52 +17,48 @@
 blocker_trigger: dict
     
 @driver.on_startup
 async def load_blocker_on_start():
     global blockerlist, blocker_trigger
     blockerlist = BlockerList()
     try:
-        blocker_trigger = get_driver().config.blocker_trigger
+        blocker_trigger = driver.config.blocker_trigger
     except AttributeError:
         blocker_trigger = {}
 
 
 @driver.on_shutdown
 async def save_blocker_on_shut():
     global blockerlist
     del blockerlist
     
-def msg_checker(msg: str,uid: str):
+def msg_checker(msg: str,uid: str) -> bool|None:
     try:
         if re.match(blocker_trigger[uid]['on']+'$', msg) is not None:
-            return True, True
+            return True
         elif re.match(blocker_trigger[uid]['off']+'$', msg) is not None:
-            return True, False
+            return False
     except (KeyError,TypeError):
-        if re.match('[.。]bot (on|off)\s?(|\[at:qq=\d+\])', msg) is not None:
-            if msg.find('on') != -1:
-                return True, True
-            elif msg.find('off') != -1:
-                return True, False
-    return False, False
+        if re.match('[.。]bot on\s?(|\[at:qq=\d+\])', msg) is not None:
+            return True
+        elif re.match('[.。]bot off\s?(|\[at:qq=\d+\])', msg) is not None:
+            return False
+    return None
 
 async def msg_checker_rule(event: GroupMessageEvent, state: T_State) -> bool:
-    if event.get_plaintext().find('qq') != -1 and not event.is_tome():
+    if (event.get_plaintext().find('qq') != -1 and not event.is_tome()) or event.user_id == event.self_id:
         return False
-    if event.user_id == event.self_id:
-        return False
-    state['blocker_passthrough'], state['blocker_state'] = msg_checker(event.get_plaintext(), str(event.self_id))
-    return state['blocker_passthrough']
+    state['blocker_state'] = msg_checker(event.get_plaintext(), str(event.self_id))
+    return True if state['blocker_state'] is not None else False
     
 blocker = on_message(rule=msg_checker_rule, permission=GROUP_ADMIN | GROUP_OWNER | SUPERUSER, priority=2, block=True)
 
 @run_preprocessor
 async def blocker_hook(matcher: Matcher, event: GroupMessageEvent):
-    blocker_pass, tmp = msg_checker(event.get_plaintext(), str(event.self_id))
-    if blockerlist.check_blocker(event.group_id, event.self_id) and not blocker_pass:
+    if blockerlist.check_blocker(event.group_id, event.self_id) and msg_checker(event.get_plaintext(), str(event.self_id)) is None:
         logger.info('[Blocker]Your Message is Blocked By Blocker.')
         await matcher.finish()
         
 @blocker.handle()
 async def blocker_msg_handle(matcher: Matcher, event: GroupMessageEvent, state: T_State):
     if state['blocker_state']:
         msg_type, msg_data = blockerlist.get_on_reply()
```

### Comparing `nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker/config.py` & `nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker.egg-info/PKG-INFO` & `nonebot-plugin-blocker-0.2.1/nonebot_plugin_blocker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.2.0
+Version: 0.2.1
 Summary: Message Blocker
 Author-email: MerCuJerry <mercujerry@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/MerCuJerry/nonebot-plugin-blocker
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.2.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.2.1 Summary:
 Message Blocker Author-email: MerCuJerry
 gmail.com> License: MIT Project-URL: homepage, https://github.com/MerCuJerry/
 nonebot-plugin-blocker Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
```

