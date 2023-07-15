# Comparing `tmp/nonebot_plugin_cp_broadcast-1.0.0.tar.gz` & `tmp/nonebot_plugin_cp_broadcast-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cp_broadcast-1.0.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_cp_broadcast-1.1.0.tar", max compression
```

## Comparing `nonebot_plugin_cp_broadcast-1.0.0.tar` & `nonebot_plugin_cp_broadcast-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-07-14 13:38:10.859183 nonebot_plugin_cp_broadcast-1.0.0/LICENSE
--rw-r--r--   0        0        0     5298 2023-07-14 13:38:10.859183 nonebot_plugin_cp_broadcast-1.0.0/README.md
--rw-r--r--   0        0        0     8429 2023-07-14 13:38:10.871183 nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/__init__.py
--rw-r--r--   0        0        0     2699 2023-07-14 13:38:10.871183 nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/atcoder.py
--rw-r--r--   0        0        0     3257 2023-07-14 13:38:10.871183 nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/codeforces.py
--rw-r--r--   0        0        0      589 2023-07-14 13:38:10.871183 nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/config.py
--rw-r--r--   0        0        0     2416 2023-07-14 13:38:10.871183 nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/nowcoder.py
--rw-r--r--   0        0        0     6778 2023-07-14 13:38:10.871183 nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/sqlite3.py
--rw-r--r--   0        0        0      732 2023-07-14 13:38:10.871183 nonebot_plugin_cp_broadcast-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6255 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-15 16:52:19.077491 nonebot_plugin_cp_broadcast-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5432 2023-07-15 16:52:19.077491 nonebot_plugin_cp_broadcast-1.1.0/README.md
+-rw-r--r--   0        0        0     8511 2023-07-15 16:52:19.085492 nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/__init__.py
+-rw-r--r--   0        0        0     2699 2023-07-15 16:52:19.085492 nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/atcoder.py
+-rw-r--r--   0        0        0     3665 2023-07-15 16:52:19.085492 nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/codeforces.py
+-rw-r--r--   0        0        0      589 2023-07-15 16:52:19.085492 nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/config.py
+-rw-r--r--   0        0        0     2416 2023-07-15 16:52:19.085492 nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/nowcoder.py
+-rw-r--r--   0        0        0     7803 2023-07-15 16:52:19.085492 nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/sqlite3.py
+-rw-r--r--   0        0        0      732 2023-07-15 16:52:19.085492 nonebot_plugin_cp_broadcast-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6389 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-1.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_cp_broadcast-1.0.0/LICENSE` & `nonebot_plugin_cp_broadcast-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-1.0.0/README.md` & `nonebot_plugin_cp_broadcast-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 | `牛客` or `nc` | 群员 | 否 | 群聊 | 发送最近三场牛客比赛的信息 |
 | `atc` | 群员 | 否 | 群聊 | 发送最近两场 AtCoder 比赛的信息 |
 | `today` | 群员 | 否 | 群聊 | 发送今天的比赛信息 |
 | `next` | 群员 | 否 | 群聊 | 发送今天后的部分比赛信息 |
 | `help` | 群员 | 是 | 群聊 | 发送帮助信息 |
 | `update` | 群员 | 否 | 群聊 | 手动更新比赛信息 |
 | `cf监视` | 群员 | 是 | 群聊 | 监视某人的 rating 变化 |
+| `cf监视移除` | 群员 | 是 | 群聊 | 移除监视某人的 rating 变化 |
 | `cf监视列表` | 群员 | 是 | 群聊 | 展示已经监视了哪些人 |
 | `cf查询` | 群员 | 是 | 群聊 | 查询对应 id 的相关信息 |
 
 
 ### 效果图
 <img src="./docs/cf.JPG" style="zoom:30%;" />
 
@@ -122,10 +123,12 @@
 
 <img src="./docs/help.JPG" style="zoom:30%;" />
 
 <img src="./docs/update.JPG" style="zoom:30%;" />
 
 <img src="./docs/cfjianshi.JPG" style="zoom:30%;" />
 
+<img src="./docs/remove.png" style="zoom:30%;" />
+
 <img src="./docs/cfjianshiliebiao.JPG" style="zoom:30%;" />
 
 <img src="./docs/cfchaxun.JPG" style="zoom:30%;" />
```

#### html2text {}

```diff
@@ -47,13 +47,14 @@
 åéæè¿ä¸åº Codeforces æ¯èµçä¿¡æ¯ | | `çå®¢` or `nc` | ç¾¤å |
 å¦ | ç¾¤è | åéæè¿ä¸åºçå®¢æ¯èµçä¿¡æ¯ | | `atc` | ç¾¤å | å¦
 | ç¾¤è | åéæè¿ä¸¤åº AtCoder æ¯èµçä¿¡æ¯ | | `today` | ç¾¤å |
 å¦ | ç¾¤è | åéä»å¤©çæ¯èµä¿¡æ¯ | | `next` | ç¾¤å | å¦ | ç¾¤è |
 åéä»å¤©åçé¨åæ¯èµä¿¡æ¯ | | `help` | ç¾¤å | æ¯ | ç¾¤è |
 åéå¸®å©ä¿¡æ¯ | | `update` | ç¾¤å | å¦ | ç¾¤è |
 æå¨æ´æ°æ¯èµä¿¡æ¯ | | `cfçè§` | ç¾¤å | æ¯ | ç¾¤è |
-çè§æäººç rating åå | | `cfçè§åè¡¨` | ç¾¤å | æ¯ | ç¾¤è |
-å±ç¤ºå·²ç»çè§äºåªäºäºº | | `cfæ¥è¯¢` | ç¾¤å | æ¯ | ç¾¤è |
-æ¥è¯¢å¯¹åº id çç¸å³ä¿¡æ¯ | ### ææå¾ [./docs/cf.JPG] [./docs/nc.JPG]
-[./docs/atc.JPG] [./docs/today.JPG] [./docs/next.JPG] [./docs/help.JPG] [./
-docs/update.JPG] [./docs/cfjianshi.JPG] [./docs/cfjianshiliebiao.JPG] [./docs/
-cfchaxun.JPG]
+çè§æäººç rating åå | | `cfçè§ç§»é¤` | ç¾¤å | æ¯ | ç¾¤è |
+ç§»é¤çè§æäººç rating åå | | `cfçè§åè¡¨` | ç¾¤å | æ¯ |
+ç¾¤è | å±ç¤ºå·²ç»çè§äºåªäºäºº | | `cfæ¥è¯¢` | ç¾¤å | æ¯ | ç¾¤è
+| æ¥è¯¢å¯¹åº id çç¸å³ä¿¡æ¯ | ### ææå¾ [./docs/cf.JPG] [./docs/
+nc.JPG] [./docs/atc.JPG] [./docs/today.JPG] [./docs/next.JPG] [./docs/help.JPG]
+[./docs/update.JPG] [./docs/cfjianshi.JPG] [./docs/remove.png] [./docs/
+cfjianshiliebiao.JPG] [./docs/cfchaxun.JPG]
```

### Comparing `nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/__init__.py` & `nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,19 @@
 cp_broadcast_updatetime = cp_broadcast_config.cp_broadcast_updatetime
 
 from nonebot.plugin import PluginMetadata
 
 __plugin_meta__ = PluginMetadata(
     name="算法竞赛比赛查询",
     description="可以查询牛客、atcoder、codeforces平台的今天和近几天的比赛信息",
-    usage="cf->查询cf比赛\n"\
+    usage=\
+        "cf->查询cf比赛\n"\
         "@{botname} cf查询+id->查询某人信息\n"\
         "@{botname} cf监视+id->监视某人rating变化\n"\
+        "@{botname} cf监视移除+id->不再监视某人rating变化"\
         "@{botname} cf监视列表->展示已监视的选手id\n"\
         "nc/牛客->查询牛客比赛\n"\
         "atc->查询atcoder比赛\n"\
         "today->查询今天的比赛\n"\
         "next->查询明天之后的部分比赛\n"
         "update->更新比赛数据\n"\
         "about->{botname}的一些信息\n",
```

### Comparing `nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/atcoder.py` & `nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/atcoder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/codeforces.py` & `nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/codeforces.py`

 * *Files 18% similar despite different names*

```diff
@@ -55,14 +55,15 @@
             break
     return f"找到最近的 {tot} 场cf比赛为：\n" + msg
 
 
 
 cf_matcher = on_fullmatch('cf',priority = 80,block=True)
 bind = on_command('cf监视', rule=to_me(), priority=80, block=True)
+bind_remove = on_command('cf监视移除', rule=to_me(), priority=80, block=True)
 bind_list = on_fullmatch('cf监视列表', rule=to_me(), priority=78, block=True)
 query = on_command('cf查询', rule=to_me(), priority=79, block=True)
 
 
 @cf_matcher.handle()
 async def reply_handle():
     msg = await ans_cf()
@@ -76,14 +77,24 @@
         if status:
             await bind.finish(f'监视{cfid}成功！')
         else:
             await bind.finish(f'监视{cfid}失败！请检查该用户是否存在')
     else:
         await bind.finish('绑定失败，请按照格式发起指令！')
 
+@bind_remove.handle()
+async def bind_remove_handle(args: Message = CommandArg()):
+    cfid = args.extract_plain_text()
+    if cfid:
+        status = await removeUser(cfid)
+        if status:
+            await bind_remove.finish(f'{cfid}移除成功')
+        else:
+            await bind_remove.finish(f'{cfid}移除失败')
+
 @bind_list.handle()
 async def bind_list_handle():
     msg = await returnBindList()
     await bind_list.finish(msg)
 
 @query.handle()
 async def query_handle(bot: Bot, event: GroupMessageEvent, args: Message = CommandArg()):
```

### Comparing `nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/config.py` & `nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/nowcoder.py` & `nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/nowcoder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-1.0.0/nonebot_plugin_cp_broadcast/sqlite3.py` & `nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/sqlite3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from .config import cp_broadcast_path, cf_user_info_baseurl
 from nonebot.log import logger
 import sqlite3
 import json
 import datetime
+import time
 from httpx import AsyncClient
 from nonebot.adapters.onebot.v11 import Message, MessageSegment
 import asyncio
 
 if not cp_broadcast_path.exists():
     cp_broadcast_path.mkdir(parents=True, exist_ok=True)
 
@@ -68,14 +69,49 @@
                 user.avatar_url
             ))
             conn.commit()
             return True
     else:
         logger.warning('添加用户失败')
         return False
+    
+async def removeUser(id: str):
+    global cf_user_info_baseurl, cursor, conn
+    cf_user_info_url = cf_user_info_baseurl + id
+
+    try:
+        async with AsyncClient() as client:
+            response = await client.get(cf_user_info_url, timeout=10.0)
+        response.raise_for_status()
+
+        user_data = json.loads(response.text)
+    except Exception as e:
+        logger.warning(e)
+        return False
+    
+    cfid = ''
+    if user_data['status'] == 'OK':
+        resluts = user_data['result']
+
+        for reslut in resluts:
+            cfid = str(reslut['handle'])
+    else:
+        logger.warning(f"cf api查询状态为{user_data['status']}")
+        return False
+
+    conn.execute('SELECT * FROM CF_User WHERE id = ?', (cfid,))
+    data = cursor.fetchall()
+    if data is None:
+        logger.warning(f'监视成员中没有此人:{cfid}')
+        return False
+    
+    conn.execute('DELETE FROM CF_User WHERE id = ?', (cfid,))
+    conn.commit()
+
+    return True
         
 async def updateUser():
     Users = []
     global cf_user_info_baseurl, cursor, conn
 
     cursor.execute('SELECT * FROM CF_User')
     RS = cursor.fetchall()
@@ -114,30 +150,29 @@
                 user.last_rating,
                 user.avatar_url
             ))
                 conn.commit()
         else:
             logger.warning("数据请求失败")
 
-
     return Users
 
 async def returRatingChangeInfo():
     outputlist = []
     Users = await updateUser()
 
     global cursor, conn
     for user in Users:
-        output=f"当前时间：{datetime.datetime.now()}\n"
+        output=f"当前时间：{time.strftime('%Y-%m-%d %H:%M:%S', time.localtime())}\n"
         cursor.execute('SELECT now_rating,last_rating,QQ FROM CF_User WHERE id = ?', (user.id,))
-        row = cursor.fetchone()
+        row = cursor.fetchall()
         now_rating, last_rating, QQ = row
         if last_rating != now_rating:
             change = now_rating - last_rating
-            output += f"cf用户 {user.id} 分数发生变化，从{last_rating} → {now_rating}  变动了{change}分！\n"
+            output += f"cf用户 {user.id} 分数发生变化，从 {last_rating} → {now_rating}，变动了{change}分！\n"
             outputlist.append({'QQ':QQ,'output':output})
 
     return outputlist
 
 
 async def returnBindList():
     global cursor, conn
@@ -185,15 +220,15 @@
             async with AsyncClient() as client:
                 resp = await client.get(avatar_url, timeout=10.0)
             
             pic = resp.content
 
             msg = MessageSegment.image(pic)
             msg += Message(
-                "name: " + name + \
+                "\nname: " + name + \
                 "\nrank: " + rank + \
                 "\nrating: " + str(contest_rating) + \
                 "\nmax rating: " + str(max_rating) + \
                 "\ncontribution: " + str(contribution) + \
                 "\nfriend of: " + str(friend_of) + " users"
             )
```

### Comparing `nonebot_plugin_cp_broadcast-1.0.0/pyproject.toml` & `nonebot_plugin_cp_broadcast-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-cp-broadcast"
-version = "1.0.0"
+version = "1.1.0"
 description = "Codeforces、牛客、AtCoder平台比赛查询，ACMer 必备"
 authors = ["HuParry <huparry@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_cp_broadcast"}]
 homepage = "https://github.com/HuParry/nonebot-plugin-cp-broadcast"
 repository = "https://github.com/HuParry/nonebot-plugin-cp-broadcast"
```

### Comparing `nonebot_plugin_cp_broadcast-1.0.0/PKG-INFO` & `nonebot_plugin_cp_broadcast-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cp-broadcast
-Version: 1.0.0
+Version: 1.1.0
 Summary: Codeforces、牛客、AtCoder平台比赛查询，ACMer 必备
 Home-page: https://github.com/HuParry/nonebot-plugin-cp-broadcast
 License: MIT
 Author: HuParry
 Author-email: huparry@outlook.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -125,14 +125,15 @@
 | `牛客` or `nc` | 群员 | 否 | 群聊 | 发送最近三场牛客比赛的信息 |
 | `atc` | 群员 | 否 | 群聊 | 发送最近两场 AtCoder 比赛的信息 |
 | `today` | 群员 | 否 | 群聊 | 发送今天的比赛信息 |
 | `next` | 群员 | 否 | 群聊 | 发送今天后的部分比赛信息 |
 | `help` | 群员 | 是 | 群聊 | 发送帮助信息 |
 | `update` | 群员 | 否 | 群聊 | 手动更新比赛信息 |
 | `cf监视` | 群员 | 是 | 群聊 | 监视某人的 rating 变化 |
+| `cf监视移除` | 群员 | 是 | 群聊 | 移除监视某人的 rating 变化 |
 | `cf监视列表` | 群员 | 是 | 群聊 | 展示已经监视了哪些人 |
 | `cf查询` | 群员 | 是 | 群聊 | 查询对应 id 的相关信息 |
 
 
 ### 效果图
 <img src="./docs/cf.JPG" style="zoom:30%;" />
 
@@ -146,11 +147,13 @@
 
 <img src="./docs/help.JPG" style="zoom:30%;" />
 
 <img src="./docs/update.JPG" style="zoom:30%;" />
 
 <img src="./docs/cfjianshi.JPG" style="zoom:30%;" />
 
+<img src="./docs/remove.png" style="zoom:30%;" />
+
 <img src="./docs/cfjianshiliebiao.JPG" style="zoom:30%;" />
 
 <img src="./docs/cfchaxun.JPG" style="zoom:30%;" />
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 1.1.0 Summary:
 Codeforcesãçå®¢ãAtCoderå¹³å°æ¯èµæ¥è¯¢ï¼ACMer å¿å¤ Home-page:
 https://github.com/HuParry/nonebot-plugin-cp-broadcast License: MIT Author:
 HuParry Author-email: huparry@outlook.com Requires-Python: >=3.8 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
@@ -60,13 +60,14 @@
 åéæè¿ä¸åº Codeforces æ¯èµçä¿¡æ¯ | | `çå®¢` or `nc` | ç¾¤å |
 å¦ | ç¾¤è | åéæè¿ä¸åºçå®¢æ¯èµçä¿¡æ¯ | | `atc` | ç¾¤å | å¦
 | ç¾¤è | åéæè¿ä¸¤åº AtCoder æ¯èµçä¿¡æ¯ | | `today` | ç¾¤å |
 å¦ | ç¾¤è | åéä»å¤©çæ¯èµä¿¡æ¯ | | `next` | ç¾¤å | å¦ | ç¾¤è |
 åéä»å¤©åçé¨åæ¯èµä¿¡æ¯ | | `help` | ç¾¤å | æ¯ | ç¾¤è |
 åéå¸®å©ä¿¡æ¯ | | `update` | ç¾¤å | å¦ | ç¾¤è |
 æå¨æ´æ°æ¯èµä¿¡æ¯ | | `cfçè§` | ç¾¤å | æ¯ | ç¾¤è |
-çè§æäººç rating åå | | `cfçè§åè¡¨` | ç¾¤å | æ¯ | ç¾¤è |
-å±ç¤ºå·²ç»çè§äºåªäºäºº | | `cfæ¥è¯¢` | ç¾¤å | æ¯ | ç¾¤è |
-æ¥è¯¢å¯¹åº id çç¸å³ä¿¡æ¯ | ### ææå¾ [./docs/cf.JPG] [./docs/nc.JPG]
-[./docs/atc.JPG] [./docs/today.JPG] [./docs/next.JPG] [./docs/help.JPG] [./
-docs/update.JPG] [./docs/cfjianshi.JPG] [./docs/cfjianshiliebiao.JPG] [./docs/
-cfchaxun.JPG]
+çè§æäººç rating åå | | `cfçè§ç§»é¤` | ç¾¤å | æ¯ | ç¾¤è |
+ç§»é¤çè§æäººç rating åå | | `cfçè§åè¡¨` | ç¾¤å | æ¯ |
+ç¾¤è | å±ç¤ºå·²ç»çè§äºåªäºäºº | | `cfæ¥è¯¢` | ç¾¤å | æ¯ | ç¾¤è
+| æ¥è¯¢å¯¹åº id çç¸å³ä¿¡æ¯ | ### ææå¾ [./docs/cf.JPG] [./docs/
+nc.JPG] [./docs/atc.JPG] [./docs/today.JPG] [./docs/next.JPG] [./docs/help.JPG]
+[./docs/update.JPG] [./docs/cfjianshi.JPG] [./docs/remove.png] [./docs/
+cfjianshiliebiao.JPG] [./docs/cfchaxun.JPG]
```

