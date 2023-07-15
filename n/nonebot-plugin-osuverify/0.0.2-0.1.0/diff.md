# Comparing `tmp/nonebot-plugin-osuverify-0.0.2.tar.gz` & `tmp/nonebot-plugin-osuverify-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-osuverify-0.0.2.tar", last modified: Thu Apr 13 13:09:04 2023, max compression
+gzip compressed data, was "nonebot-plugin-osuverify-0.1.0.tar", last modified: Sat Jul 15 13:14:20 2023, max compression
```

## Comparing `nonebot-plugin-osuverify-0.0.2.tar` & `nonebot-plugin-osuverify-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 13:09:04.371813 nonebot-plugin-osuverify-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-04-13 13:08:54.000000 nonebot-plugin-osuverify-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3172 2023-04-13 13:09:04.371813 nonebot-plugin-osuverify-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2715 2023-04-13 13:08:54.000000 nonebot-plugin-osuverify-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 13:09:04.367813 nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify/
--rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-04-13 13:08:54.000000 nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-13 13:09:04.371813 nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3172 2023-04-13 13:09:04.000000 nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-13 13:09:04.000000 nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-13 13:09:04.000000 nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-04-13 13:09:04.000000 nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-13 13:09:04.000000 nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-13 13:09:04.371813 nonebot-plugin-osuverify-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-04-13 13:08:54.000000 nonebot-plugin-osuverify-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 13:14:20.098896 nonebot-plugin-osuverify-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-15 13:14:08.000000 nonebot-plugin-osuverify-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-07-15 13:14:20.098896 nonebot-plugin-osuverify-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-07-15 13:14:08.000000 nonebot-plugin-osuverify-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 13:14:20.098896 nonebot-plugin-osuverify-0.1.0/nonebot_plugin_osuverify/
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-07-15 13:14:08.000000 nonebot-plugin-osuverify-0.1.0/nonebot_plugin_osuverify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 13:14:20.098896 nonebot-plugin-osuverify-0.1.0/nonebot_plugin_osuverify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3035 2023-07-15 13:14:20.000000 nonebot-plugin-osuverify-0.1.0/nonebot_plugin_osuverify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-07-15 13:14:20.000000 nonebot-plugin-osuverify-0.1.0/nonebot_plugin_osuverify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-15 13:14:20.000000 nonebot-plugin-osuverify-0.1.0/nonebot_plugin_osuverify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-15 13:14:20.000000 nonebot-plugin-osuverify-0.1.0/nonebot_plugin_osuverify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-15 13:14:20.000000 nonebot-plugin-osuverify-0.1.0/nonebot_plugin_osuverify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-15 13:14:20.098896 nonebot-plugin-osuverify-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-07-15 13:14:08.000000 nonebot-plugin-osuverify-0.1.0/setup.py
```

### Comparing `nonebot-plugin-osuverify-0.0.2/LICENSE` & `nonebot-plugin-osuverify-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-osuverify-0.0.2/PKG-INFO` & `nonebot-plugin-osuverify-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-osuverify
-Version: 0.0.2
+Version: 0.1.0
 Summary: 通过osu!账号审核入群功能
 Home-page: https://github.com/mas-alone/nonebot-plugin-sayoroll
 Author: A M D
 Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -90,14 +90,13 @@
 |:-----:|:----:|:----:|:----:|
 | osu_amd | 是 | 无 | 填入osu!官网申请的apiV1 |
 
 申请地址：https://osu.ppy.sh/p/api
 
 填写示例：osu_amd="申请到的api"
 
-请在使用时通过管理群->加群方式->需要身份认证中开启需要回答问题并由管理员审核并将bot设为管理员
 
 ## 🎉 使用
 无图，无指令。
 如果输入的osu!用户名官网查无此人，bot会拒绝，并提示用户输入正确的用户名。
 
 如果验证通过，bot会自动修改用户的Q群备注为osu!用户名。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-osuverify Version: 0.0.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-osuverify Version: 0.1.0 Summary:
 éè¿osu!è´¦å·å®¡æ ¸å¥ç¾¤åè½ Home-page: https://github.com/mas-alone/
 nonebot-plugin-sayoroll Author: A M D Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
 Approved :: GNU Affero General Public License v3 Classifier: Operating System
 :: OS Independent Description-Content-Type: text/markdown License-File: LICENSE
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
@@ -21,13 +21,10 @@
 poetry poetry add nonebot-plugin-osuverify   conda conda install nonebot-
 plugin-osuverify  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml`
 æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot_plugin_osuverify"]  ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | osu_amd | æ¯ | æ  |
 å¡«å¥osu!å®ç½ç³è¯·çapiV1 | ç³è¯·å°åï¼https://osu.ppy.sh/p/api
-å¡«åç¤ºä¾ï¼osu_amd="ç³è¯·å°çapi" è¯·å¨ä½¿ç¨æ¶éè¿ç®¡çç¾¤-
->å ç¾¤æ¹å¼-
->éè¦èº«ä»½è®¤è¯ä¸­å¼å¯éè¦åç­é®é¢å¹¶ç±ç®¡çåå®¡æ ¸å¹¶å°botè®¾ä¸ºç®¡çå
-## ð ä½¿ç¨ æ å¾ï¼æ æä»¤ã
+å¡«åç¤ºä¾ï¼osu_amd="ç³è¯·å°çapi" ## ð ä½¿ç¨ æ å¾ï¼æ æä»¤ã
 å¦æè¾å¥çosu!ç¨æ·åå®ç½æ¥æ æ­¤äººï¼botä¼æç»ï¼å¹¶æç¤ºç¨æ·è¾å¥æ­£ç¡®çç¨æ·åã
 å¦æéªè¯éè¿ï¼botä¼èªå¨ä¿®æ¹ç¨æ·çQç¾¤å¤æ³¨ä¸ºosu!ç¨æ·åã
```

### Comparing `nonebot-plugin-osuverify-0.0.2/README.md` & `nonebot-plugin-osuverify-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -77,14 +77,13 @@
 |:-----:|:----:|:----:|:----:|
 | osu_amd | 是 | 无 | 填入osu!官网申请的apiV1 |
 
 申请地址：https://osu.ppy.sh/p/api
 
 填写示例：osu_amd="申请到的api"
 
-请在使用时通过管理群->加群方式->需要身份认证中开启需要回答问题并由管理员审核并将bot设为管理员
 
 ## 🎉 使用
 无图，无指令。
 如果输入的osu!用户名官网查无此人，bot会拒绝，并提示用户输入正确的用户名。
 
 如果验证通过，bot会自动修改用户的Q群备注为osu!用户名。
```

#### html2text {}

```diff
@@ -15,13 +15,10 @@
 poetry poetry add nonebot-plugin-osuverify   conda conda install nonebot-
 plugin-osuverify  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml`
 æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot_plugin_osuverify"]  ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | osu_amd | æ¯ | æ  |
 å¡«å¥osu!å®ç½ç³è¯·çapiV1 | ç³è¯·å°åï¼https://osu.ppy.sh/p/api
-å¡«åç¤ºä¾ï¼osu_amd="ç³è¯·å°çapi" è¯·å¨ä½¿ç¨æ¶éè¿ç®¡çç¾¤-
->å ç¾¤æ¹å¼-
->éè¦èº«ä»½è®¤è¯ä¸­å¼å¯éè¦åç­é®é¢å¹¶ç±ç®¡çåå®¡æ ¸å¹¶å°botè®¾ä¸ºç®¡çå
-## ð ä½¿ç¨ æ å¾ï¼æ æä»¤ã
+å¡«åç¤ºä¾ï¼osu_amd="ç³è¯·å°çapi" ## ð ä½¿ç¨ æ å¾ï¼æ æä»¤ã
 å¦æè¾å¥çosu!ç¨æ·åå®ç½æ¥æ æ­¤äººï¼botä¼æç»ï¼å¹¶æç¤ºç¨æ·è¾å¥æ­£ç¡®çç¨æ·åã
 å¦æéªè¯éè¿ï¼botä¼èªå¨ä¿®æ¹ç¨æ·çQç¾¤å¤æ³¨ä¸ºosu!ç¨æ·åã
```

### Comparing `nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify/__init__.py` & `nonebot-plugin-osuverify-0.1.0/nonebot_plugin_osuverify/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     description='osu!账户自动审批入群申请！',
     usage="",
     config={},
     extra={}
 )
 
 join_group = on_request(
-    priority=0,
+    priority=1,
     block=True
 )
 
 async def check_comment(comment):
     k = nonebot.get_driver().config.dict().get('osu_amd')
     if k:
         verify_api = 'https://osu.ppy.sh/api/get_user?k={}&u={}'.format(k, comment)
```

### Comparing `nonebot-plugin-osuverify-0.0.2/nonebot_plugin_osuverify.egg-info/PKG-INFO` & `nonebot-plugin-osuverify-0.1.0/nonebot_plugin_osuverify.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-osuverify
-Version: 0.0.2
+Version: 0.1.0
 Summary: 通过osu!账号审核入群功能
 Home-page: https://github.com/mas-alone/nonebot-plugin-sayoroll
 Author: A M D
 Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -90,14 +90,13 @@
 |:-----:|:----:|:----:|:----:|
 | osu_amd | 是 | 无 | 填入osu!官网申请的apiV1 |
 
 申请地址：https://osu.ppy.sh/p/api
 
 填写示例：osu_amd="申请到的api"
 
-请在使用时通过管理群->加群方式->需要身份认证中开启需要回答问题并由管理员审核并将bot设为管理员
 
 ## 🎉 使用
 无图，无指令。
 如果输入的osu!用户名官网查无此人，bot会拒绝，并提示用户输入正确的用户名。
 
 如果验证通过，bot会自动修改用户的Q群备注为osu!用户名。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-osuverify Version: 0.0.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-osuverify Version: 0.1.0 Summary:
 éè¿osu!è´¦å·å®¡æ ¸å¥ç¾¤åè½ Home-page: https://github.com/mas-alone/
 nonebot-plugin-sayoroll Author: A M D Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8 Classifier: License :: OSI
 Approved :: GNU Affero General Public License v3 Classifier: Operating System
 :: OS Independent Description-Content-Type: text/markdown License-File: LICENSE
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
@@ -21,13 +21,10 @@
 poetry poetry add nonebot-plugin-osuverify   conda conda install nonebot-
 plugin-osuverify  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml`
 æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot_plugin_osuverify"]  ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | osu_amd | æ¯ | æ  |
 å¡«å¥osu!å®ç½ç³è¯·çapiV1 | ç³è¯·å°åï¼https://osu.ppy.sh/p/api
-å¡«åç¤ºä¾ï¼osu_amd="ç³è¯·å°çapi" è¯·å¨ä½¿ç¨æ¶éè¿ç®¡çç¾¤-
->å ç¾¤æ¹å¼-
->éè¦èº«ä»½è®¤è¯ä¸­å¼å¯éè¦åç­é®é¢å¹¶ç±ç®¡çåå®¡æ ¸å¹¶å°botè®¾ä¸ºç®¡çå
-## ð ä½¿ç¨ æ å¾ï¼æ æä»¤ã
+å¡«åç¤ºä¾ï¼osu_amd="ç³è¯·å°çapi" ## ð ä½¿ç¨ æ å¾ï¼æ æä»¤ã
 å¦æè¾å¥çosu!ç¨æ·åå®ç½æ¥æ æ­¤äººï¼botä¼æç»ï¼å¹¶æç¤ºç¨æ·è¾å¥æ­£ç¡®çç¨æ·åã
 å¦æéªè¯éè¿ï¼botä¼èªå¨ä¿®æ¹ç¨æ·çQç¾¤å¤æ³¨ä¸ºosu!ç¨æ·åã
```

### Comparing `nonebot-plugin-osuverify-0.0.2/setup.py` & `nonebot-plugin-osuverify-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-osuverify",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.0.2",  # 程序版本
+    version="0.1.0",  # 程序版本
     author="A M D",  # 项目作者
     author_email="mas_alone@qq.com",  # 作者邮件
     description="通过osu!账号审核入群功能",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/mas-alone/nonebot-plugin-sayoroll",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

