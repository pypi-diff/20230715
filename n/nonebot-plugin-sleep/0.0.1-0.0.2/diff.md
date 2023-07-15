# Comparing `tmp/nonebot-plugin-sleep-0.0.1.tar.gz` & `tmp/nonebot-plugin-sleep-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-sleep-0.0.1.tar", last modified: Sun Apr  2 06:30:49 2023, max compression
+gzip compressed data, was "nonebot-plugin-sleep-0.0.2.tar", last modified: Sat Jul 15 13:19:06 2023, max compression
```

## Comparing `nonebot-plugin-sleep-0.0.1.tar` & `nonebot-plugin-sleep-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-02 06:30:49.478974 nonebot-plugin-sleep-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-04-02 06:30:40.000000 nonebot-plugin-sleep-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2750 2023-04-02 06:30:49.478974 nonebot-plugin-sleep-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2304 2023-04-02 06:30:40.000000 nonebot-plugin-sleep-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-02 06:30:49.478974 nonebot-plugin-sleep-0.0.1/nonebot_plugin_sleep/
--rw-r--r--   0 runner    (1001) docker     (122)     1991 2023-04-02 06:30:40.000000 nonebot-plugin-sleep-0.0.1/nonebot_plugin_sleep/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-02 06:30:49.478974 nonebot-plugin-sleep-0.0.1/nonebot_plugin_sleep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2750 2023-04-02 06:30:49.000000 nonebot-plugin-sleep-0.0.1/nonebot_plugin_sleep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-04-02 06:30:49.000000 nonebot-plugin-sleep-0.0.1/nonebot_plugin_sleep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-02 06:30:49.000000 nonebot-plugin-sleep-0.0.1/nonebot_plugin_sleep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-04-02 06:30:49.000000 nonebot-plugin-sleep-0.0.1/nonebot_plugin_sleep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-02 06:30:49.000000 nonebot-plugin-sleep-0.0.1/nonebot_plugin_sleep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-02 06:30:49.478974 nonebot-plugin-sleep-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-04-02 06:30:40.000000 nonebot-plugin-sleep-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 13:19:06.710360 nonebot-plugin-sleep-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-15 13:18:54.000000 nonebot-plugin-sleep-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-07-15 13:19:06.710360 nonebot-plugin-sleep-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2310 2023-07-15 13:18:54.000000 nonebot-plugin-sleep-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 13:19:06.710360 nonebot-plugin-sleep-0.0.2/nonebot_plugin_sleep/
+-rw-r--r--   0 runner    (1001) docker     (122)     1991 2023-07-15 13:18:54.000000 nonebot-plugin-sleep-0.0.2/nonebot_plugin_sleep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 13:19:06.710360 nonebot-plugin-sleep-0.0.2/nonebot_plugin_sleep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-07-15 13:19:06.000000 nonebot-plugin-sleep-0.0.2/nonebot_plugin_sleep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-07-15 13:19:06.000000 nonebot-plugin-sleep-0.0.2/nonebot_plugin_sleep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-15 13:19:06.000000 nonebot-plugin-sleep-0.0.2/nonebot_plugin_sleep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-07-15 13:19:06.000000 nonebot-plugin-sleep-0.0.2/nonebot_plugin_sleep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-15 13:19:06.000000 nonebot-plugin-sleep-0.0.2/nonebot_plugin_sleep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-15 13:19:06.710360 nonebot-plugin-sleep-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1044 2023-07-15 13:18:54.000000 nonebot-plugin-sleep-0.0.2/setup.py
```

### Comparing `nonebot-plugin-sleep-0.0.1/LICENSE` & `nonebot-plugin-sleep-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sleep-0.0.1/PKG-INFO` & `nonebot-plugin-sleep-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sleep
-Version: 0.0.1
+Version: 0.0.2
 Summary: 来一份精致的睡眠套餐
 Home-page: https://github.com/mas-alone/nonebot-plugin-sleep
 Author: A M D
 Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -88,9 +88,9 @@
 否则只回复晚安。且无法禁言管理员！
 
 ## 🎉 使用
 ### 指令表
 `/sleep`<br>
 禁言发指令的用户8小时，bot回复晚安。<br><br>
 `/sleep 10`<br>
-禁言发指令的用户10小时，bot回复晚安。<br>
-sleep后面带数字的话就禁言对应的时长，最多24也就是1天，如果超过24则也禁言1天，最小1也就是1小时，如果是0.1这样的也算作1。不带数字就是第一个例子了默认8小时。
+禁言发指令的用户10小时，bot回复晚安。<br><br>
+ **sleep** 后面带数字的话就禁言对应的时长，必须为整数， **最多24** 也就是1天，如果超过24则也禁言1天， **最小1** 也就是1小时，不带数字就是第一个例子了默认8小时。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sleep Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sleep Version: 0.0.2 Summary:
 æ¥ä¸ä»½ç²¾è´çç¡ç å¥é¤ Home-page: https://github.com/mas-alone/nonebot-
 plugin-sleep Author: A M D Author-email: mas_alone@qq.com Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 GNU Affero General Public License v3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
@@ -20,8 +20,11 @@
 ["nonebot_plugin_sleep"]  ## âï¸ æ³¨æ botå¿é¡»ä¸º ç®¡çå/ç¾¤ä¸»
 ææç¦è¨çæé å¦ååªåå¤æå®ãä¸æ æ³ç¦è¨ç®¡çåï¼ ##
 ð ä½¿ç¨ ### æä»¤è¡¨ `/sleep`
 ç¦è¨åæä»¤çç¨æ·8å°æ¶ï¼botåå¤æå®ã
 
 `/sleep 10`
 ç¦è¨åæä»¤çç¨æ·10å°æ¶ï¼botåå¤æå®ã
-sleepåé¢å¸¦æ°å­çè¯å°±ç¦è¨å¯¹åºçæ¶é¿ï¼æå¤24ä¹å°±æ¯1å¤©ï¼å¦æè¶è¿24åä¹ç¦è¨1å¤©ï¼æå°1ä¹å°±æ¯1å°æ¶ï¼å¦ææ¯0.1è¿æ ·çä¹ç®ä½1ãä¸å¸¦æ°å­å°±æ¯ç¬¬ä¸ä¸ªä¾å­äºé»è®¤8å°æ¶ã
+
+**sleep** åé¢å¸¦æ°å­çè¯å°±ç¦è¨å¯¹åºçæ¶é¿ï¼å¿é¡»ä¸ºæ´æ°ï¼
+**æå¤24** ä¹å°±æ¯1å¤©ï¼å¦æè¶è¿24åä¹ç¦è¨1å¤©ï¼ **æå°1**
+ä¹å°±æ¯1å°æ¶ï¼ä¸å¸¦æ°å­å°±æ¯ç¬¬ä¸ä¸ªä¾å­äºé»è®¤8å°æ¶ã
```

### Comparing `nonebot-plugin-sleep-0.0.1/README.md` & `nonebot-plugin-sleep-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -75,9 +75,9 @@
 否则只回复晚安。且无法禁言管理员！
 
 ## 🎉 使用
 ### 指令表
 `/sleep`<br>
 禁言发指令的用户8小时，bot回复晚安。<br><br>
 `/sleep 10`<br>
-禁言发指令的用户10小时，bot回复晚安。<br>
-sleep后面带数字的话就禁言对应的时长，最多24也就是1天，如果超过24则也禁言1天，最小1也就是1小时，如果是0.1这样的也算作1。不带数字就是第一个例子了默认8小时。
+禁言发指令的用户10小时，bot回复晚安。<br><br>
+ **sleep** 后面带数字的话就禁言对应的时长，必须为整数， **最多24** 也就是1天，如果超过24则也禁言1天， **最小1** 也就是1小时，不带数字就是第一个例子了默认8小时。
```

#### html2text {}

```diff
@@ -14,8 +14,11 @@
 ["nonebot_plugin_sleep"]  ## âï¸ æ³¨æ botå¿é¡»ä¸º ç®¡çå/ç¾¤ä¸»
 ææç¦è¨çæé å¦ååªåå¤æå®ãä¸æ æ³ç¦è¨ç®¡çåï¼ ##
 ð ä½¿ç¨ ### æä»¤è¡¨ `/sleep`
 ç¦è¨åæä»¤çç¨æ·8å°æ¶ï¼botåå¤æå®ã
 
 `/sleep 10`
 ç¦è¨åæä»¤çç¨æ·10å°æ¶ï¼botåå¤æå®ã
-sleepåé¢å¸¦æ°å­çè¯å°±ç¦è¨å¯¹åºçæ¶é¿ï¼æå¤24ä¹å°±æ¯1å¤©ï¼å¦æè¶è¿24åä¹ç¦è¨1å¤©ï¼æå°1ä¹å°±æ¯1å°æ¶ï¼å¦ææ¯0.1è¿æ ·çä¹ç®ä½1ãä¸å¸¦æ°å­å°±æ¯ç¬¬ä¸ä¸ªä¾å­äºé»è®¤8å°æ¶ã
+
+**sleep** åé¢å¸¦æ°å­çè¯å°±ç¦è¨å¯¹åºçæ¶é¿ï¼å¿é¡»ä¸ºæ´æ°ï¼
+**æå¤24** ä¹å°±æ¯1å¤©ï¼å¦æè¶è¿24åä¹ç¦è¨1å¤©ï¼ **æå°1**
+ä¹å°±æ¯1å°æ¶ï¼ä¸å¸¦æ°å­å°±æ¯ç¬¬ä¸ä¸ªä¾å­äºé»è®¤8å°æ¶ã
```

### Comparing `nonebot-plugin-sleep-0.0.1/nonebot_plugin_sleep/__init__.py` & `nonebot-plugin-sleep-0.0.2/nonebot_plugin_sleep/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     usage='sleep[数字]',
     config={},
     extra={}
 )
 
 sleep = on_command(
     'sleep',
-    priority=0,
+    priority=1,
     block=False
 )
 
 
 @sleep.handle()
 async def _(bot: Bot, event: GroupMessageEvent, args: Message = CommandArg()):
     sleep_time = str(args).strip()
```

### Comparing `nonebot-plugin-sleep-0.0.1/nonebot_plugin_sleep.egg-info/PKG-INFO` & `nonebot-plugin-sleep-0.0.2/nonebot_plugin_sleep.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sleep
-Version: 0.0.1
+Version: 0.0.2
 Summary: 来一份精致的睡眠套餐
 Home-page: https://github.com/mas-alone/nonebot-plugin-sleep
 Author: A M D
 Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -88,9 +88,9 @@
 否则只回复晚安。且无法禁言管理员！
 
 ## 🎉 使用
 ### 指令表
 `/sleep`<br>
 禁言发指令的用户8小时，bot回复晚安。<br><br>
 `/sleep 10`<br>
-禁言发指令的用户10小时，bot回复晚安。<br>
-sleep后面带数字的话就禁言对应的时长，最多24也就是1天，如果超过24则也禁言1天，最小1也就是1小时，如果是0.1这样的也算作1。不带数字就是第一个例子了默认8小时。
+禁言发指令的用户10小时，bot回复晚安。<br><br>
+ **sleep** 后面带数字的话就禁言对应的时长，必须为整数， **最多24** 也就是1天，如果超过24则也禁言1天， **最小1** 也就是1小时，不带数字就是第一个例子了默认8小时。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sleep Version: 0.0.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sleep Version: 0.0.2 Summary:
 æ¥ä¸ä»½ç²¾è´çç¡ç å¥é¤ Home-page: https://github.com/mas-alone/nonebot-
 plugin-sleep Author: A M D Author-email: mas_alone@qq.com Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 GNU Affero General Public License v3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
@@ -20,8 +20,11 @@
 ["nonebot_plugin_sleep"]  ## âï¸ æ³¨æ botå¿é¡»ä¸º ç®¡çå/ç¾¤ä¸»
 ææç¦è¨çæé å¦ååªåå¤æå®ãä¸æ æ³ç¦è¨ç®¡çåï¼ ##
 ð ä½¿ç¨ ### æä»¤è¡¨ `/sleep`
 ç¦è¨åæä»¤çç¨æ·8å°æ¶ï¼botåå¤æå®ã
 
 `/sleep 10`
 ç¦è¨åæä»¤çç¨æ·10å°æ¶ï¼botåå¤æå®ã
-sleepåé¢å¸¦æ°å­çè¯å°±ç¦è¨å¯¹åºçæ¶é¿ï¼æå¤24ä¹å°±æ¯1å¤©ï¼å¦æè¶è¿24åä¹ç¦è¨1å¤©ï¼æå°1ä¹å°±æ¯1å°æ¶ï¼å¦ææ¯0.1è¿æ ·çä¹ç®ä½1ãä¸å¸¦æ°å­å°±æ¯ç¬¬ä¸ä¸ªä¾å­äºé»è®¤8å°æ¶ã
+
+**sleep** åé¢å¸¦æ°å­çè¯å°±ç¦è¨å¯¹åºçæ¶é¿ï¼å¿é¡»ä¸ºæ´æ°ï¼
+**æå¤24** ä¹å°±æ¯1å¤©ï¼å¦æè¶è¿24åä¹ç¦è¨1å¤©ï¼ **æå°1**
+ä¹å°±æ¯1å°æ¶ï¼ä¸å¸¦æ°å­å°±æ¯ç¬¬ä¸ä¸ªä¾å­äºé»è®¤8å°æ¶ã
```

### Comparing `nonebot-plugin-sleep-0.0.1/setup.py` & `nonebot-plugin-sleep-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-sleep",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.0.1",  # 程序版本
+    version="0.0.2",  # 程序版本
     author="A M D",  # 项目作者
     author_email="mas_alone@qq.com",  # 作者邮件
     description="来一份精致的睡眠套餐",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/mas-alone/nonebot-plugin-sleep",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

