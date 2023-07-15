# Comparing `tmp/nonebot-plugin-blocker-0.1.8.tar.gz` & `tmp/nonebot-plugin-blocker-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-blocker-0.1.8.tar", last modified: Fri Jul 14 12:04:28 2023, max compression
+gzip compressed data, was "nonebot-plugin-blocker-0.2.0.tar", last modified: Sat Jul 15 14:51:59 2023, max compression
```

## Comparing `nonebot-plugin-blocker-0.1.8.tar` & `nonebot-plugin-blocker-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:04:28.575801 nonebot-plugin-blocker-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-14 12:04:28.575801 nonebot-plugin-blocker-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-14 12:04:07.000000 nonebot-plugin-blocker-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:04:28.575801 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-14 12:04:07.000000 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-14 12:04:07.000000 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-14 12:04:07.000000 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:04:28.575801 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-14 12:04:28.000000 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-14 12:04:28.000000 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:04:28.000000 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-14 12:04:28.000000 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 12:04:28.000000 nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-14 12:04:07.000000 nonebot-plugin-blocker-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:04:28.575801 nonebot-plugin-blocker-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:51:59.398855 nonebot-plugin-blocker-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-15 14:51:59.398855 nonebot-plugin-blocker-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-15 14:51:35.000000 nonebot-plugin-blocker-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:51:59.394855 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-15 14:51:35.000000 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-15 14:51:35.000000 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-15 14:51:35.000000 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:51:59.398855 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-15 14:51:59.000000 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-15 14:51:59.000000 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 14:51:59.000000 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-15 14:51:59.000000 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 14:51:59.000000 nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-15 14:51:35.000000 nonebot-plugin-blocker-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 14:51:59.398855 nonebot-plugin-blocker-0.2.0/setup.cfg
```

### Comparing `nonebot-plugin-blocker-0.1.8/PKG-INFO` & `nonebot-plugin-blocker-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-blocker
-Version: 0.1.8
-Summary: Message Blocker
-Author-email: MerCuJerry <mercujerry@gmail.com>
-License: MIT
-Project-URL: homepage, https://github.com/MerCuJerry/nonebot-plugin-blocker
-Requires-Python: <4.0,>=3.8
-Description-Content-Type: text/markdown
-
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
@@ -50,15 +40,23 @@
 
     plugins = ["nonebot-plugin-blocker"]
 
 </details>
 
 ## ⚙️ 配置
 
-插件的配置文件位于 `data/blocker/blocker_reply.json` 里
+### 常规配置项，位于.env文件里
+
+```ini
+#本配置项不是必填配置项
+blocker_trigger={"%BotQQ号%":{"on":"%开启命令%","off":"%关闭命令%"}}
+```
+
+### 其他配置项
+插件的回复配置文件位于 `data/blocker/blocker_reply.json` 里
 ```jsonc
     {
         "reply_on":{
             "type":"text"
             "data":{
                 "text":"在本群开启"
             }
@@ -77,8 +75,8 @@
 
 指令只有管理员，群主以及Bot的SUPERUSER能够使用
 
 ### .bot on在该群开启bot
 
 ### .bot off在该群关闭bot
 
-### 在上述指令后at特定bot将关闭使用了本插件的特定Bot，不会影响使用本插件的其他Bot
+### 在上述指令后at特定bot将关闭使用了本插件的特定Bot，不会影响使用本插件的其他Bot
```

#### html2text {}

```diff
@@ -1,23 +1,21 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.8 Summary:
-Message Blocker Author-email: MerCuJerry
-gmail.com> License: MIT Project-URL: homepage, https://github.com/MerCuJerry/
-nonebot-plugin-blocker Requires-Python: <4.0,>=3.8 Description-Content-Type:
-text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
                                    [python]
 ## ð ä»ç» è¿æ¯ä¸ä¸ª nonebot2
 æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­ ## ð¿ å®è£
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-blocker  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot-plugin-blocker"]  ## âï¸ éç½® æä»¶çéç½®æä»¶ä½äº `data/
-blocker/blocker_reply.json` é ```jsonc { "reply_on":{ "type":"text" "data":
-{ "text":"å¨æ¬ç¾¤å¼å¯" } }, "reply_off":{ "type":"text" "data":{ "text":
+["nonebot-plugin-blocker"]  ## âï¸ éç½® ###
+å¸¸è§éç½®é¡¹ï¼ä½äº.envæä»¶é ```ini #æ¬éç½®é¡¹ä¸æ¯å¿å¡«éç½®é¡¹
+blocker_trigger={"%BotQQå·%":{"on":"%å¼å¯å½ä»¤%","off":"%å³é­å½ä»¤%"}}
+``` ### å¶ä»éç½®é¡¹ æä»¶çåå¤éç½®æä»¶ä½äº `data/blocker/
+blocker_reply.json` é ```jsonc { "reply_on":{ "type":"text" "data":{ "text":
+"å¨æ¬ç¾¤å¼å¯" } }, "reply_off":{ "type":"text" "data":{ "text":
 "å¨æ¬ç¾¤å³é­" } } } ``` `data/blocker/blocklist.json`
 éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
 ## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
 ### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot ###
 å¨ä¸è¿°æä»¤åatç¹å®botå°å³é­ä½¿ç¨äºæ¬æä»¶çç¹å®Botï¼ä¸ä¼å½±åä½¿ç¨æ¬æä»¶çå¶ä»Bot
```

### Comparing `nonebot-plugin-blocker-0.1.8/README.md` & `nonebot-plugin-blocker-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: nonebot-plugin-blocker
+Version: 0.2.0
+Summary: Message Blocker
+Author-email: MerCuJerry <mercujerry@gmail.com>
+License: MIT
+Project-URL: homepage, https://github.com/MerCuJerry/nonebot-plugin-blocker
+Requires-Python: <4.0,>=3.8
+Description-Content-Type: text/markdown
+
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
@@ -40,15 +50,23 @@
 
     plugins = ["nonebot-plugin-blocker"]
 
 </details>
 
 ## ⚙️ 配置
 
-插件的配置文件位于 `data/blocker/blocker_reply.json` 里
+### 常规配置项，位于.env文件里
+
+```ini
+#本配置项不是必填配置项
+blocker_trigger={"%BotQQ号%":{"on":"%开启命令%","off":"%关闭命令%"}}
+```
+
+### 其他配置项
+插件的回复配置文件位于 `data/blocker/blocker_reply.json` 里
 ```jsonc
     {
         "reply_on":{
             "type":"text"
             "data":{
                 "text":"在本群开启"
             }
@@ -67,8 +85,8 @@
 
 指令只有管理员，群主以及Bot的SUPERUSER能够使用
 
 ### .bot on在该群开启bot
 
 ### .bot off在该群关闭bot
 
-### 在上述指令后at特定bot将关闭使用了本插件的特定Bot，不会影响使用本插件的其他Bot
+### 在上述指令后at特定bot将关闭使用了本插件的特定Bot，不会影响使用本插件的其他Bot
```

#### html2text {}

```diff
@@ -1,18 +1,26 @@
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.2.0 Summary:
+Message Blocker Author-email: MerCuJerry
+gmail.com> License: MIT Project-URL: homepage, https://github.com/MerCuJerry/
+nonebot-plugin-blocker Requires-Python: <4.0,>=3.8 Description-Content-Type:
+text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
                                    [python]
 ## ð ä»ç» è¿æ¯ä¸ä¸ª nonebot2
 æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­ ## ð¿ å®è£
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-blocker  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot-plugin-blocker"]  ## âï¸ éç½® æä»¶çéç½®æä»¶ä½äº `data/
-blocker/blocker_reply.json` é ```jsonc { "reply_on":{ "type":"text" "data":
-{ "text":"å¨æ¬ç¾¤å¼å¯" } }, "reply_off":{ "type":"text" "data":{ "text":
+["nonebot-plugin-blocker"]  ## âï¸ éç½® ###
+å¸¸è§éç½®é¡¹ï¼ä½äº.envæä»¶é ```ini #æ¬éç½®é¡¹ä¸æ¯å¿å¡«éç½®é¡¹
+blocker_trigger={"%BotQQå·%":{"on":"%å¼å¯å½ä»¤%","off":"%å³é­å½ä»¤%"}}
+``` ### å¶ä»éç½®é¡¹ æä»¶çåå¤éç½®æä»¶ä½äº `data/blocker/
+blocker_reply.json` é ```jsonc { "reply_on":{ "type":"text" "data":{ "text":
+"å¨æ¬ç¾¤å¼å¯" } }, "reply_off":{ "type":"text" "data":{ "text":
 "å¨æ¬ç¾¤å³é­" } } } ``` `data/blocker/blocklist.json`
 éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
 ## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
 ### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot ###
 å¨ä¸è¿°æä»¤åatç¹å®botå°å³é­ä½¿ç¨äºæ¬æä»¶çç¹å®Botï¼ä¸ä¼å½±åä½¿ç¨æ¬æä»¶çå¶ä»Bot
```

### Comparing `nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker/config.py` & `nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             self.blocklist[str(qid)].append(gid)
         except KeyError:
             self.blocklist.setdefault(str(qid),[gid])
         
     def del_blocker(self,gid: int, qid: int):
         try:
             self.blocklist[str(qid)].remove(gid)
-        except ValueError:
+        except:
             pass
         
     def check_blocker(self,gid: int, qid: int) -> bool:
         try:
             self.blocklist[str(qid)].index(gid)
         except:
             return False
```

### Comparing `nonebot-plugin-blocker-0.1.8/nonebot_plugin_blocker.egg-info/PKG-INFO` & `nonebot-plugin-blocker-0.2.0/nonebot_plugin_blocker.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.1.8
+Version: 0.2.0
 Summary: Message Blocker
 Author-email: MerCuJerry <mercujerry@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/MerCuJerry/nonebot-plugin-blocker
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
 
@@ -50,15 +50,23 @@
 
     plugins = ["nonebot-plugin-blocker"]
 
 </details>
 
 ## ⚙️ 配置
 
-插件的配置文件位于 `data/blocker/blocker_reply.json` 里
+### 常规配置项，位于.env文件里
+
+```ini
+#本配置项不是必填配置项
+blocker_trigger={"%BotQQ号%":{"on":"%开启命令%","off":"%关闭命令%"}}
+```
+
+### 其他配置项
+插件的回复配置文件位于 `data/blocker/blocker_reply.json` 里
 ```jsonc
     {
         "reply_on":{
             "type":"text"
             "data":{
                 "text":"在本群开启"
             }
```

#### html2text {}

```diff
@@ -1,23 +1,26 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.1.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.2.0 Summary:
 Message Blocker Author-email: MerCuJerry
 gmail.com> License: MIT Project-URL: homepage, https://github.com/MerCuJerry/
 nonebot-plugin-blocker Requires-Python: <4.0,>=3.8 Description-Content-Type:
 text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
                                    [python]
 ## ð ä»ç» è¿æ¯ä¸ä¸ª nonebot2
 æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­ ## ð¿ å®è£
 ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-blocker  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot-plugin-blocker"]  ## âï¸ éç½® æä»¶çéç½®æä»¶ä½äº `data/
-blocker/blocker_reply.json` é ```jsonc { "reply_on":{ "type":"text" "data":
-{ "text":"å¨æ¬ç¾¤å¼å¯" } }, "reply_off":{ "type":"text" "data":{ "text":
+["nonebot-plugin-blocker"]  ## âï¸ éç½® ###
+å¸¸è§éç½®é¡¹ï¼ä½äº.envæä»¶é ```ini #æ¬éç½®é¡¹ä¸æ¯å¿å¡«éç½®é¡¹
+blocker_trigger={"%BotQQå·%":{"on":"%å¼å¯å½ä»¤%","off":"%å³é­å½ä»¤%"}}
+``` ### å¶ä»éç½®é¡¹ æä»¶çåå¤éç½®æä»¶ä½äº `data/blocker/
+blocker_reply.json` é ```jsonc { "reply_on":{ "type":"text" "data":{ "text":
+"å¨æ¬ç¾¤å¼å¯" } }, "reply_off":{ "type":"text" "data":{ "text":
 "å¨æ¬ç¾¤å³é­" } } } ``` `data/blocker/blocklist.json`
 éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
 ## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
 ### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot ###
 å¨ä¸è¿°æä»¤åatç¹å®botå°å³é­ä½¿ç¨äºæ¬æä»¶çç¹å®Botï¼ä¸ä¼å½±åä½¿ç¨æ¬æä»¶çå¶ä»Bot
```

