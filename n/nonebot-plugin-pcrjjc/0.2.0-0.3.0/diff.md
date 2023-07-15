# Comparing `tmp/nonebot-plugin-pcrjjc-0.2.0.tar.gz` & `tmp/nonebot-plugin-pcrjjc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-pcrjjc-0.2.0.tar", last modified: Wed Jun 14 13:19:53 2023, max compression
+gzip compressed data, was "nonebot-plugin-pcrjjc-0.3.0.tar", last modified: Sat Jul 15 05:00:50 2023, max compression
```

## Comparing `nonebot-plugin-pcrjjc-0.2.0.tar` & `nonebot-plugin-pcrjjc-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 13:19:52.938463 nonebot-plugin-pcrjjc-0.2.0/
--rw-rw-rw-   0        0        0    35171 2023-06-10 05:18:04.000000 nonebot-plugin-pcrjjc-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     2702 2023-06-14 13:19:52.937615 nonebot-plugin-pcrjjc-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1838 2023-06-14 13:19:25.000000 nonebot-plugin-pcrjjc-0.2.0/README.md
--rw-rw-rw-   0        0        0     1583 2023-06-14 10:44:30.000000 nonebot-plugin-pcrjjc-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 13:19:52.938463 nonebot-plugin-pcrjjc-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-14 13:19:52.882614 nonebot-plugin-pcrjjc-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-14 13:19:52.908614 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/
--rw-rw-rw-   0        0        0    39835 2023-06-13 07:52:32.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/__init__.py
--rw-rw-rw-   0        0        0     2785 2023-06-08 22:14:57.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/aiorequests.py
--rw-rw-rw-   0        0        0     6022 2023-06-14 11:47:54.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/bsgamesdk.py
--rw-rw-rw-   0        0        0      856 2023-06-14 10:44:45.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/config.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:19:52.924438 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/fonts/
--rw-rw-rw-   0        0        0  8390148 2023-03-11 01:34:30.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf
--rw-rw-rw-   0        0        0     9200 2023-06-10 08:05:10.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/pcrclient.py
--rw-rw-rw-   0        0        0     8186 2023-06-14 11:47:48.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/query.py
--rw-rw-rw-   0        0        0      438 2023-06-09 05:01:11.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/rsacr.py
--rw-rw-rw-   0        0        0     2357 2023-06-08 23:35:29.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/text2img.py
-drwxrwxrwx   0        0        0        0 2023-06-14 13:19:52.921217 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc.egg-info/
--rw-rw-rw-   0        0        0     2702 2023-06-14 13:19:52.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      636 2023-06-14 13:19:52.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 13:19:52.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2023-06-14 13:19:52.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-06-14 13:19:52.000000 nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 05:00:50.442149 nonebot-plugin-pcrjjc-0.3.0/
+-rw-rw-rw-   0        0        0    35171 2023-06-10 05:18:04.000000 nonebot-plugin-pcrjjc-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2961 2023-07-15 05:00:50.440122 nonebot-plugin-pcrjjc-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2096 2023-07-09 09:05:19.000000 nonebot-plugin-pcrjjc-0.3.0/README.md
+-rw-rw-rw-   0        0        0     1583 2023-07-09 23:19:30.000000 nonebot-plugin-pcrjjc-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-15 05:00:50.442149 nonebot-plugin-pcrjjc-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-15 05:00:50.047826 nonebot-plugin-pcrjjc-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-15 05:00:50.266615 nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/
+-rw-rw-rw-   0        0        0    41044 2023-07-15 03:57:15.000000 nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/__init__.py
+-rw-rw-rw-   0        0        0     2785 2023-06-08 22:14:57.000000 nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/aiorequests.py
+-rw-rw-rw-   0        0        0     6022 2023-06-16 01:23:13.000000 nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/bsgamesdk.py
+-rw-rw-rw-   0        0        0      956 2023-07-09 09:05:18.000000 nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/config.py
+drwxrwxrwx   0        0        0        0 2023-07-15 05:00:50.315633 nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/fonts/
+-rw-rw-rw-   0        0        0  8390148 2023-03-11 01:34:30.000000 nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf
+-rw-rw-rw-   0        0        0     9192 2023-07-09 09:03:51.000000 nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/pcrclient.py
+-rw-rw-rw-   0        0        0     8728 2023-07-09 23:30:30.000000 nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/query.py
+-rw-rw-rw-   0        0        0      438 2023-06-09 05:01:11.000000 nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/rsacr.py
+-rw-rw-rw-   0        0        0     2357 2023-06-08 23:35:29.000000 nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/text2img.py
+drwxrwxrwx   0        0        0        0 2023-07-15 05:00:50.309621 nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc.egg-info/
+-rw-rw-rw-   0        0        0     2961 2023-07-15 05:00:49.000000 nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      636 2023-07-15 05:00:49.000000 nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 05:00:49.000000 nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2023-07-15 05:00:49.000000 nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-15 05:00:49.000000 nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc.egg-info/top_level.txt
```

### Comparing `nonebot-plugin-pcrjjc-0.2.0/LICENSE` & `nonebot-plugin-pcrjjc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.2.0/PKG-INFO` & `nonebot-plugin-pcrjjc-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pcrjjc
-Version: 0.2.0
+Version: 0.3.0
 Summary: pcrjjc排名监测插件
 Author-email: reine-ishyanami <2402979195@qq.com>
 License: AGPL-3
 Project-URL: Homepage, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc
 Project-URL: Bug Tracker, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -51,18 +51,19 @@
 
 
 
 ### 配置项
 
 **在nonebot2项目中的`.env`开头的文件添加下表配置项，其中非必填项可不填**
 
-|     配置项     |   类型    | 是否必填 |   默认值   |              说明              |
-| :------------: | :-------: | :------: |:-------:| :----------------------------: |
-|   SUPERUSERS   | list[str] |   True   |         | 超级用户QQ号，示例：["114514"] |
-|      OTTO      |   bool    |  False   |  True   | 是否自动过验证码（不建议修改） |
-|    VERSION     |    str    |  False   | "6.2.0" |          客户端版本号          |
-|    MAX_PRI     |    int    |  False   |    0    |          最大私聊人数          |
-|   MAX_PCRID    |    int    |  False   |    8    |       每人绑定的最大数量       |
-|  MAX_HISTORY   |    int    |  False   |   50    |        单人最多历史记录        |
-| NOTICE_CD_MIN  |    int    |  False   |   10    |  上线提醒时间间隔（单位：分）  |
-| REFRESH_SECOND |    int    |  False   |    3    |    排名刷新频率（单位：秒）    |
+|     配置项     |   类型    | 是否必填 | 默认值  |                     说明                     |
+| :------------: | :-------: | :------: | :-----: | :------------------------------------------: |
+|   SUPERUSERS   | list[str] |   True   |         |        超级用户QQ号，示例：["114514"]        |
+|  PCRJJC_GROUP  |    str    |  False   |  None   | 当私聊不可用时，使用指定群聊推送要私聊的消息 |
+|      OTTO      |   bool    |  False   |  True   |        是否自动过验证码（不建议修改）        |
+|    VERSION     |    str    |  False   | "6.2.0" |                 客户端版本号                 |
+|    MAX_PRI     |    int    |  False   |    0    |                 最大私聊人数                 |
+|   MAX_PCRID    |    int    |  False   |    8    |              每人绑定的最大数量              |
+|  MAX_HISTORY   |    int    |  False   |   50    |               单人最多历史记录               |
+| NOTICE_CD_MIN  |    int    |  False   |   10    |         上线提醒时间间隔（单位：分）         |
+| REFRESH_SECOND |    int    |  False   |    3    |           排名刷新频率（单位：秒）           |
```

### Comparing `nonebot-plugin-pcrjjc-0.2.0/README.md` & `nonebot-plugin-pcrjjc-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -32,18 +32,19 @@
 
 
 
 ### 配置项
 
 **在nonebot2项目中的`.env`开头的文件添加下表配置项，其中非必填项可不填**
 
-|     配置项     |   类型    | 是否必填 |   默认值   |              说明              |
-| :------------: | :-------: | :------: |:-------:| :----------------------------: |
-|   SUPERUSERS   | list[str] |   True   |         | 超级用户QQ号，示例：["114514"] |
-|      OTTO      |   bool    |  False   |  True   | 是否自动过验证码（不建议修改） |
-|    VERSION     |    str    |  False   | "6.2.0" |          客户端版本号          |
-|    MAX_PRI     |    int    |  False   |    0    |          最大私聊人数          |
-|   MAX_PCRID    |    int    |  False   |    8    |       每人绑定的最大数量       |
-|  MAX_HISTORY   |    int    |  False   |   50    |        单人最多历史记录        |
-| NOTICE_CD_MIN  |    int    |  False   |   10    |  上线提醒时间间隔（单位：分）  |
-| REFRESH_SECOND |    int    |  False   |    3    |    排名刷新频率（单位：秒）    |
+|     配置项     |   类型    | 是否必填 | 默认值  |                     说明                     |
+| :------------: | :-------: | :------: | :-----: | :------------------------------------------: |
+|   SUPERUSERS   | list[str] |   True   |         |        超级用户QQ号，示例：["114514"]        |
+|  PCRJJC_GROUP  |    str    |  False   |  None   | 当私聊不可用时，使用指定群聊推送要私聊的消息 |
+|      OTTO      |   bool    |  False   |  True   |        是否自动过验证码（不建议修改）        |
+|    VERSION     |    str    |  False   | "6.2.0" |                 客户端版本号                 |
+|    MAX_PRI     |    int    |  False   |    0    |                 最大私聊人数                 |
+|   MAX_PCRID    |    int    |  False   |    8    |              每人绑定的最大数量              |
+|  MAX_HISTORY   |    int    |  False   |   50    |               单人最多历史记录               |
+| NOTICE_CD_MIN  |    int    |  False   |   10    |         上线提醒时间间隔（单位：分）         |
+| REFRESH_SECOND |    int    |  False   |    3    |           排名刷新频率（单位：秒）           |
```

### Comparing `nonebot-plugin-pcrjjc-0.2.0/pyproject.toml` & `nonebot-plugin-pcrjjc-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-pcrjjc"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
     {name="reine-ishyanami", email="2402979195@qq.com"}
 ]
 description = "pcrjjc排名监测插件"
 readme = "README.md"
 license = { text = "AGPL-3" }
 requires-python = ">=3.10, <4.0"
```

### Comparing `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/__init__.py` & `nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,27 +71,28 @@
 #只绑定1个uid时，绑定的序号可以不填。
 [绑定的序号]1~{MAX_PCRID}对应绑定的第1~{MAX_PCRID}个uid，序号0表示全部
 1）竞技场绑定[uid][昵称]（昵称可省略）
 2）删除竞技场绑定[绑定的序号]（这里序号不可省略）
 3）开启/关闭竞技场推送（不会删除绑定）
 4）清空竞技场绑定
 5）竞技场查询[uid]（uid可省略）
-6）竞技场订阅状态
-7）竞技场修改昵称 [绑定的序号] [新昵称] 
-8）竞技场设置[开启/关闭][订阅内容][绑定的序号]
-9）竞技场/击剑记录[绑定的序号]（序号可省略）
-10）竞技场设置11110[绑定的序号]
+6）竞技场查询#[绑定的序号]
+7）竞技场订阅状态
+8）竞技场修改昵称 [绑定的序号] [新昵称] 
+9）竞技场设置[开启/关闭][订阅内容][绑定的序号]
+10）竞技场/击剑记录[绑定的序号]（序号可省略）
+11）竞技场设置11110[绑定的序号]
 #0表示关闭，1表示开启
 #5个数字依次代表jjc、pjjc、排名上升、at、上线提醒
 #例如：“竞技场设置10111 2” “竞技场设置11110 0”
 #上线提醒：第5位表示上线提醒等级，可以写0~3
 0表示关闭，1表示{NOTICE_CD_MIN}分钟cd，仅在2点半~3点报，
 2表示{NOTICE_CD_MIN}分钟cd，全天报；3表示1分钟cd全天报。
 每天5点会把上线提醒等级3改成2，有需要的可以再次手动开启。
-11）在本群推送（限群聊发送，无需好友）
+12）在本群推送（限群聊发送，无需好友）
 '''
 sv_help_adm = '''------------------------------------------------
 管理员帮助：
 1）pcrjjc负载查询
 2）pcrjjc删除绑定[qq号]
 3）pcrjjc关闭私聊推送
 4）pcrjjc关闭排名上升
@@ -130,22 +131,22 @@
 
 # ========================================查询========================================
 
 @on_fullmatch(msg='查询群数').handle()
 async def _(bot: Bot, event: GroupMessageEvent):
     global bind_cache, lck
     gid = event.group_id
+    sid = bot.self_id
     async with lck:
-        for sid in get_bots():
-            gl = await bot.get_group_list()
-            gl = [g['group_id'] for g in gl]
-            try:
-                await bot.send_group_msg(group_id=gid, message=f"本Bot目前正在为【{len(gl)}】个群服务")
-            except Exception:
-                logger.info('bot账号{}不在群{}中，将忽略该消息', sid, gid)
+        gl = await bot.get_group_list()
+        gl = [g['group_id'] for g in gl]
+        try:
+            await bot.send_group_msg(group_id=gid, message=f"本Bot目前正在为【{len(gl)}】个群服务")
+        except Exception:
+            logger.info('bot账号{}不在群{}中，将忽略该消息', sid, gid)
 
 
 @on_fullmatch(msg='查询竞技场订阅数').handle()
 async def _(matcher: Matcher):
     global bind_cache, lck
     async with lck:
         await matcher.finish(f'当前竞技场已订阅的账号数量为【{len(bind_cache)}】个')
@@ -164,19 +165,42 @@
             manual_query_list_name = [None]
     except TypeError:  # 只捕获强转异常
         if qid in bind_cache:
             manual_query_list = bind_cache[qid]["pcrid"]
             manual_query_list_name = bind_cache[qid]["pcrName"]
         else:
             await matcher.finish('木有找到绑定信息，查询时不能省略13位uid！')
+    logger.debug("manual_query_list: {}", manual_query_list)
     for i in range(len(manual_query_list)):
         query_cache[event.user_id] = []
         pcrid = manual_query_list[i]
         await queue.put((3, (
             jjc_query, pcrid, {"bot": bot, "event": event, "list": manual_query_list_name, "index": i, "uid": pcrid})))
+        
+
+@on_regex(pattern=r'^竞技场查询\# ?(\d+)$').handle()
+async def _(bot: Bot, event: MessageEvent, matcher: Matcher, group: tuple = RegexGroup()):
+    global bind_cache, lck
+    qid = str(event.user_id)
+    lid = int(group[0])
+    if qid in bind_cache:
+        qid_pcrid_list = bind_cache[qid]["pcrid"]
+        if 0 < lid <= len(qid_pcrid_list):
+            manual_query_list = [bind_cache[qid]["pcrid"][lid-1]]
+            manual_query_list_name = [bind_cache[qid]["pcrName"][lid-1]]
+        else:
+            await matcher.finish('序号超出范围，请检查您绑定的竞技场列表')
+    else:
+        await matcher.finish('木有找到绑定信息，查询时不能省略13位uid！')
+    logger.debug("manual_query_list: {}", manual_query_list)
+    for i in range(len(manual_query_list)):
+        query_cache[event.user_id] = []
+        pcrid = manual_query_list[i]
+        await queue.put((3, (
+            jjc_query, pcrid, {"bot": bot, "event": event, "list": manual_query_list_name, "index": i, "uid": pcrid, "only": lid - 1})))
 
 
 @on_fullmatch(msg='竞技场订阅状态').handle()
 async def _(bot: Bot, event: GroupMessageEvent, matcher: Matcher):
     global bind_cache
     qid = str(event.user_id)
     gid = event.group_id
@@ -540,18 +564,15 @@
     await matcher.finish(reply)
 
 
 @on_regex(pattern=r'^(开启|关闭)竞技场推送$').handle()
 async def _(bot: Bot, event: GroupMessageEvent, matcher: Matcher, group: tuple = RegexGroup()):
     global bind_cache, lck, friend_list, pri_user, admin
     qid = str(event.user_id)
-    try:
-        turn_on = True if group[0] == '开启' else False
-    except:
-        await matcher.finish('出错了，请联系管理员！')
+    turn_on = True if group[0] == '开启' else False
     async with lck:
         if qid in bind_cache:
             if bind_cache[qid]["notice_on"] == turn_on:
                 await matcher.finish(f'您的竞技场推送，已经是{group[0]}状态，不要重复{group[0]}！')
             else:
                 if turn_on:
                     if len(friend_list):
@@ -721,27 +742,28 @@
         last_login_min = int(res["last_login_time"]) % 3600 // 60
         last_login_min = '%02d' % last_login_min  # 分钟补零，变成2位
         if manual_query_list_name[i]:
             res["user_name"] = manual_query_list_name[i]
         extra = ''
         if pcrid in cache:
             extra = f'''上升: {cache[pcrid][3]}次 / {cache[pcrid][4]}次\n'''
+        i = i if data.get("only") is None else data.get("only")  # 如果是查询单个，修改其序号
         query = f'【{i + 1:02}】{res["user_name"]}\n{res["arena_rank"]}({res["arena_group"]}场) / {res["grand_arena_rank"]}({res["grand_arena_group"]}场)\n{extra}最近上号{last_login_hour}：{last_login_min}\n\n'
         async with lck:
             query_list.append(query)
             if len(query_list) == len(manual_query_list_name):
                 query_list.sort()
                 pic = image_draw(''.join(query_list))
                 for sid in get_bots():
                     try:
                         await bot.send_group_msg(self_id=sid, group_id=int(ev.group_id),
                                                  message=MessageSegment.image(pic))
                         break
-                    except Exception:
-                        pass
+                    except Exception as e:
+                        logger.debug(e)
     except KeyError:
         await bot.send_group_msg(group_id=int(ev.group_id), message=f'找不到这个uid，大概率是你输错了！')
 
 
 async def member_add_sub(data):
     global bind_cache, lck, friend_list, MAX_PCRID
     bot = data["bot"]
@@ -800,16 +822,16 @@
             save_binds()
     except KeyError:
         reply = f'找不到这个uid，大概率是你输错了！'
     for sid in get_bots():
         try:
             await bot.send_group_msg(self_id=sid, group_id=int(ev.group_id), message=reply)
             break
-        except Exception:
-            pass
+        except Exception as e:
+            logger.debug(e)
 
 
 async def send_notice(new: int, old: int, pcrid: int, notice_type: int):  # noticeType：1:jjc排名变动   2:pjjc排名变动  3:登录时间刷新
     global bind_cache, timeStamp, jjc_log, today_notice, NOTICE_CD_MIN
     bot = get_bot()
     if notice_type == 3:
         change = f'''上线了！[{time.strftime("%H:%M", time.localtime(new))}]'''
@@ -863,16 +885,16 @@
                     else:
                         if atNotice:
                             msg.append(MessageSegment.at(qid))
                         for sid in get_bots():
                             try:
                                 await bot.send_group_msg(self_id=sid, group_id=int(bind_cache[qid]["gid"]), message=msg)
                                 break
-                            except Exception:
-                                pass
+                            except Exception as e:
+                                logger.debug(e)
                 break
 
 
 # ========================================AUTO========================================
 
 @driver.on_bot_connect
 async def _():
```

### Comparing `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/aiorequests.py` & `nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/aiorequests.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/bsgamesdk.py` & `nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/bsgamesdk.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/config.py` & `nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 class Config(BaseModel, extra=Extra.ignore):
     """Plugin Config Here"""
     apscheduler_log_level: int = 30
     data_path: str = join("data", "pcrjjc")  # 数据存储目录
     superusers: list[str]  # 超级用户列表，建议只填一个，填多个可能导致后续用户指令失效
+    pcrjjc_group: str = None  # 当私聊不可用时，使用指定群聊推送要私聊的消息
     otto: bool = True  # 是否自动过验证码，因自动过码失效，改为手动过码
     version: str = "6.2.0"  # 游戏版本号
     max_pri: int = 0  # 最大私聊人数
     max_pcrid: int = 8  # 每个QQ号绑定的最多数量
     max_history: int = 50  # 每个QQ号保存的最多击剑记录
     notice_cd_min: int = 10  # 上线推送频率
     refresh_second: int = 3  # 刷新频率，可按自身服务器性能输入其他数值，可支持整数、小数
```

### Comparing `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf` & `nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/fonts/SourceHanSansCN-Medium.otf`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/pcrclient.py` & `nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/pcrclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from asyncio import sleep
 from base64 import b64encode, b64decode
 from datetime import datetime
 from hashlib import md5
 from json import loads
-from os.path import dirname, join, exists
+from os.path import join, exists
 from pathlib import Path
 from random import randint
 from re import search
 
 from Crypto.Cipher import AES
 from dateutil.parser import parse
 from msgpack import packb, unpackb
@@ -16,15 +16,15 @@
 from .aiorequests import post
 from .bsgamesdk import login
 from .config import Config
 
 driver = get_driver()
 config = Config.parse_obj(driver.config)
 
-api_root = 'https://l3-prod-all-gs-gzlj.bilibiligame.net'
+api_root = 'https://le1-prod-all-gs-gzlj.bilibiligame.net'
 debugging = 1
 
 data_path = config.data_path
 path = join(str(Path()), data_path)
 version_txt = join(path, 'version.txt')
 version = config.version
```

### Comparing `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/query.py` & `nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import os.path
 import traceback
+import types
 from asyncio import Lock
 from json import load, loads, dump
 from os.path import join
 from pathlib import Path
 
 from nonebot import get_driver, logger, on_regex
 from nonebot.adapters.onebot.v11 import Bot
@@ -18,14 +19,15 @@
 driver = get_driver()
 config = Config.parse_obj(driver.config)
 
 bot: Bot | None = None
 captcha_lck = Lock()
 queue = asyncio.PriorityQueue()
 otto = config.otto
+pcrjjc_group = config.pcrjjc_group
 ordd = 'x'
 validate = None
 validating = False
 ac_first = False
 client = None
 captcha_cnt = 0
 admin = int(config.superusers[0]) if len(config.superusers) > 0 else 0
@@ -53,28 +55,36 @@
 async def _():
     await load_config()
 
 
 @driver.on_bot_connect
 async def _(b: Bot):
     global bot, ac_info, binds_info
+    b.send_admin_msg_of_pcrjjc = types.MethodType(send_admin_msg_of_pcrjjc, b)
     bot = b
     try:
-        while i := ac_info.__iter__().__next__():
+        while i := next(iter(ac_info)):
             b_client = BSdkClient(i, captcha_verifier)
             pcr_client = PcrClient(b_client)
             loop = asyncio.get_event_loop()
             loop.create_task(query(pcr_client))
             if binds_info == {} or binds_info["arena_bind"] == {}:
                 loop.create_task(first_login(pcr_client))
             ac_info.remove(i)  # 遍历删除集合元素，防止有第二个bot对象连接时触发登录事件
     except StopIteration:
         pass
 
 
+async def send_admin_msg_of_pcrjjc(self, user_id: int, group_id: str, message: str):
+    if group_id is None:
+        await self.send_private_msg(user_id=user_id, message=message)
+    else:
+        await self.send_group_msg(group_id=int(group_id), message=message)
+
+
 async def first_login(pcr_client):
     while pcr_client.shouldLogin:
         await pcr_client.login()
 
 
 async def load_config():
     global ac_info, binds_info, path, account_json_template
@@ -94,14 +104,15 @@
     try:
         with open(join(path, binds_json_name)) as fp:
             binds_info = load(fp)
     except FileNotFoundError:
         pass
 
 
+# noinspection PyUnresolvedReferences
 @driver.on_shutdown
 async def _():
     # 清空队列中的任务
     global queue
     while not queue.empty():
         await queue.get()
         queue.task_done()
@@ -110,45 +121,44 @@
 
 @on_regex(pattern=rf'^validate{ordd} ?(\S+)$', permission=SUPERUSER).handle()
 async def validate(group: tuple = RegexGroup()):
     global validate, captcha_lck, otto
     validate = group[0]
     if validate == "manual":
         otto = False
-        await bot.send_private_msg(user_id=admin, message=f'thread{ordd}: Changed to manual')
+        message = f'thread{ordd}: Changed to manual'
+        await bot.send_admin_msg_of_pcrjjc(user_id=admin, group_id=pcrjjc_group, message=message)
     elif validate == "auto":
         otto = True
-        await bot.send_private_msg(user_id=admin, message=f'thread{ordd}: Changed to auto')
+        message = f'thread{ordd}: Changed to auto'
+        await bot.send_admin_msg_of_pcrjjc(user_id=admin, group_id=pcrjjc_group, message=message)
     try:
         captcha_lck.release()
     except:
         pass
 
 
 async def captcha_verifier(gt: str, challenge: str, userid: str):
     global otto, captcha_cnt, ac_first, validating, validate, captcha_lck
-    # global otto, ac_first, validating, validate, captcha_lck
     if not ac_first:
         await captcha_lck.acquire()
         ac_first = True
 
     validating = True
 
     # 非自动过码
     if not otto:
         online_url_head = f"https://help.tencentbot.top/geetest_/?"
         url = f"captcha_type=1&challenge={challenge}&gt={gt}&userid={userid}&gs=1"
-        await bot.send_private_msg(
-            user_id=admin,
-            message=f'pcr账号登录需要验证码，请完成以下链接中的验证内容后将第1个方框的内容点击复制，并加上"validate{ordd} "前缀发送给机器人完成验证'
-                    f'\n示例：validate{ordd} 123456789\n您也可以发送 validate{ordd} auto 命令bot自动过验证码'
-                    f'\n验证链接头：{online_url_head}'
-                    f'\n链接：{url}'
-                    f'\n为避免tx网页安全验证使验证码过期，请手动拼接链接头和链接'
-        )
+        message = f'pcr账号登录需要验证码，请完成以下链接中的验证内容后将第1个方框的内容点击复制，并加上"validate{ordd} "前缀发送给机器人完成验证'
+        f'\n示例：validate{ordd} 123456789\n您也可以发送 validate{ordd} auto 命令bot自动过验证码'
+        f'\n验证链接头：{online_url_head}'
+        f'\n链接：{url}'
+        f'\n为避免tx网页安全验证使验证码过期，请手动拼接链接头和链接'
+        await bot.send_admin_msg_of_pcrjjc(user_id=admin, group_id=pcrjjc_group, message=message)
         await captcha_lck.acquire()
         validating = False
         return challenge, gt, validate
 
     while captcha_cnt < 5:
         captcha_cnt += 1
         try:
@@ -185,17 +195,18 @@
                         return info["challenge"], info["gt_user_id"], info["validate"]
                 if ccnt > 10:
                     raise Exception("Captcha Failed")
         except:
             pass
     if captcha_cnt >= 5:
         otto = False
-        await bot.send_private_msg(user_id=admin,
-                                   message=f'thread{ordd}: 自动过码多次尝试失败，可能为服务器错误，自动切换为手动。\n确实服务器无误后，可发送 validate{ordd} auto重新触发自动过码。')
-        await bot.send_private_msg(user_id=admin, message=f'thread{ordd}: Changed to manual')
+        message1 = f'thread{ordd}: 自动过码多次尝试失败，可能为服务器错误，自动切换为手动。\n确实服务器无误后，可发送 validate{ordd} auto重新触发自动过码。'
+        message2 = f'thread{ordd}: Changed to manual'
+        await bot.send_admin_msg_of_pcrjjc(user_id=admin, group_id=pcrjjc_group, message=message1)
+        await bot.send_admin_msg_of_pcrjjc(user_id=admin, group_id=pcrjjc_group, message=message2)
         validating = False
         return "manual"
 
     logger.info("captchaVerifier: uncaught exception")
     validating = False
     return False
```

### Comparing `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc/text2img.py` & `nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc/text2img.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO` & `nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pcrjjc
-Version: 0.2.0
+Version: 0.3.0
 Summary: pcrjjc排名监测插件
 Author-email: reine-ishyanami <2402979195@qq.com>
 License: AGPL-3
 Project-URL: Homepage, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc
 Project-URL: Bug Tracker, https://github.com/reine-ishyanami/nonebot-plugin-pcrjjc/issues
 Classifier: Framework :: Pydantic
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -51,18 +51,19 @@
 
 
 
 ### 配置项
 
 **在nonebot2项目中的`.env`开头的文件添加下表配置项，其中非必填项可不填**
 
-|     配置项     |   类型    | 是否必填 |   默认值   |              说明              |
-| :------------: | :-------: | :------: |:-------:| :----------------------------: |
-|   SUPERUSERS   | list[str] |   True   |         | 超级用户QQ号，示例：["114514"] |
-|      OTTO      |   bool    |  False   |  True   | 是否自动过验证码（不建议修改） |
-|    VERSION     |    str    |  False   | "6.2.0" |          客户端版本号          |
-|    MAX_PRI     |    int    |  False   |    0    |          最大私聊人数          |
-|   MAX_PCRID    |    int    |  False   |    8    |       每人绑定的最大数量       |
-|  MAX_HISTORY   |    int    |  False   |   50    |        单人最多历史记录        |
-| NOTICE_CD_MIN  |    int    |  False   |   10    |  上线提醒时间间隔（单位：分）  |
-| REFRESH_SECOND |    int    |  False   |    3    |    排名刷新频率（单位：秒）    |
+|     配置项     |   类型    | 是否必填 | 默认值  |                     说明                     |
+| :------------: | :-------: | :------: | :-----: | :------------------------------------------: |
+|   SUPERUSERS   | list[str] |   True   |         |        超级用户QQ号，示例：["114514"]        |
+|  PCRJJC_GROUP  |    str    |  False   |  None   | 当私聊不可用时，使用指定群聊推送要私聊的消息 |
+|      OTTO      |   bool    |  False   |  True   |        是否自动过验证码（不建议修改）        |
+|    VERSION     |    str    |  False   | "6.2.0" |                 客户端版本号                 |
+|    MAX_PRI     |    int    |  False   |    0    |                 最大私聊人数                 |
+|   MAX_PCRID    |    int    |  False   |    8    |              每人绑定的最大数量              |
+|  MAX_HISTORY   |    int    |  False   |   50    |               单人最多历史记录               |
+| NOTICE_CD_MIN  |    int    |  False   |   10    |         上线提醒时间间隔（单位：分）         |
+| REFRESH_SECOND |    int    |  False   |    3    |           排名刷新频率（单位：秒）           |
```

### Comparing `nonebot-plugin-pcrjjc-0.2.0/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt` & `nonebot-plugin-pcrjjc-0.3.0/src/nonebot_plugin_pcrjjc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

