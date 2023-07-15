# Comparing `tmp/nonebot_plugin_game_collection-2.3.6.tar.gz` & `tmp/nonebot_plugin_game_collection-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.3.6.tar", last modified: Fri Jul 14 15:20:34 2023, max compression
+gzip compressed data, was "nonebot_plugin_game_collection-2.3.7.tar", last modified: Sat Jul 15 09:53:13 2023, max compression
```

## Comparing `nonebot_plugin_game_collection-2.3.6.tar` & `nonebot_plugin_game_collection-2.3.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 15:20:34.519461 nonebot_plugin_game_collection-2.3.6/
--rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.3.6/LICENSE
--rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.3.6/MANIFEST.in
--rw-rw-rw-   0        0        0      376 2023-07-14 15:20:34.518961 nonebot_plugin_game_collection-2.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 15:20:34.467916 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/
--rw-rw-rw-   0        0        0    21648 2023-07-14 14:56:24.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Account.py
--rw-rw-rw-   0        0        0     2692 2023-07-11 15:32:39.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Alchemy.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:20:34.478926 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Fortress/
--rw-rw-rw-   0        0        0    10093 2023-07-02 07:42:47.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Fortress/core.py
--rw-rw-rw-   0        0        0    73450 2023-07-07 17:09:45.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Game.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:20:34.486433 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/HorseRace/
--rw-rw-rw-   0        0        0    15602 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-rw-rw-   0        0        0     6399 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-rw-rw-   0        0        0     5151 2023-07-01 10:30:51.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-rw-rw-   0        0        0     9182 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/HorseRace/start.py
--rw-rw-rw-   0        0        0    10598 2023-07-13 18:15:22.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Manager.py
--rw-rw-rw-   0        0        0    23104 2023-07-13 19:13:31.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Market.py
--rw-rw-rw-   0        0        0    23596 2023-07-07 16:48:24.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Prop.py
--rw-rw-rw-   0        0        0    32678 2023-07-14 14:30:15.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/__init__.py
--rw-rw-rw-   0        0        0     3733 2023-07-11 14:30:16.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/config.py
--rw-rw-rw-   0        0        0    11300 2023-07-13 19:07:21.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/data.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:20:34.489935 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/
-drwxrwxrwx   0        0        0        0 2023-07-14 15:20:34.509452 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/
--rw-rw-rw-   0        0        0     5488 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-rw-rw-   0        0        0     4549 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-rw-rw-   0        0        0     1757 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-rw-rw-   0        0        0      906 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-rw-rw-   0        0        0     2717 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-rw-rw-   0        0        0     1257 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-rw-rw-   0        0        0    22637 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-rw-rw-   0        0        0     4751 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-rw-rw-   0        0        0     1010 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-rw-rw-   0        0        0     2253 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-rw-rw-   0        0        0    12889 2023-07-11 16:50:54.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/menu_data.json
--rw-rw-rw-   0        0        0     5332 2023-07-07 16:19:38.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/props_library.json
-drwxrwxrwx   0        0        0        0 2023-07-14 15:20:34.511454 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/subprocess/
--rw-rw-rw-   0        0        0     2278 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:20:34.517459 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/utils/
--rw-rw-rw-   0        0        0     1323 2023-06-27 06:06:09.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/utils/avatar.py
--rw-rw-rw-   0        0        0    22338 2023-07-14 15:16:16.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/utils/chart.py
--rw-rw-rw-   0        0        0     1141 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:20:34.477425 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection.egg-info/
--rw-rw-rw-   0        0        0      376 2023-07-14 15:20:34.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1976 2023-07-14 15:20:34.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 15:20:34.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-07-14 15:20:34.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-07-14 15:20:34.000000 nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 15:20:34.519961 nonebot_plugin_game_collection-2.3.6/setup.cfg
--rw-rw-rw-   0        0        0      730 2023-07-14 15:20:30.000000 nonebot_plugin_game_collection-2.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:53:13.185546 nonebot_plugin_game_collection-2.3.7/
+-rw-rw-rw-   0        0        0     1065 2022-08-13 09:26:37.000000 nonebot_plugin_game_collection-2.3.7/LICENSE
+-rw-rw-rw-   0        0        0      193 2022-12-20 21:13:32.000000 nonebot_plugin_game_collection-2.3.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      376 2023-07-15 09:53:13.183544 nonebot_plugin_game_collection-2.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8291 2022-08-13 12:03:08.000000 nonebot_plugin_game_collection-2.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 09:53:13.133001 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/
+-rw-rw-rw-   0        0        0    21570 2023-07-15 08:34:17.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/Account.py
+-rw-rw-rw-   0        0        0     2692 2023-07-11 15:32:39.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/Alchemy.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:53:13.143510 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/Fortress/
+-rw-rw-rw-   0        0        0    10093 2023-07-02 07:42:47.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/Fortress/core.py
+-rw-rw-rw-   0        0        0    73450 2023-07-15 06:50:16.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/Game.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:53:13.150016 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/HorseRace/
+-rw-rw-rw-   0        0        0    15602 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/HorseRace/events_main.py
+-rw-rw-rw-   0        0        0     6399 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/HorseRace/horse.py
+-rw-rw-rw-   0        0        0     5151 2023-07-01 10:30:51.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/HorseRace/race_group.py
+-rw-rw-rw-   0        0        0     9182 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/HorseRace/start.py
+-rw-rw-rw-   0        0        0    10601 2023-07-15 04:46:14.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/Manager.py
+-rw-rw-rw-   0        0        0    24131 2023-07-15 09:45:15.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/Market.py
+-rw-rw-rw-   0        0        0    23596 2023-07-07 16:48:24.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/Prop.py
+-rw-rw-rw-   0        0        0    33417 2023-07-15 09:37:07.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/__init__.py
+-rw-rw-rw-   0        0        0     3733 2023-07-11 14:30:16.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/config.py
+-rw-rw-rw-   0        0        0    12289 2023-07-15 09:28:04.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/data.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:53:13.154519 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/
+drwxrwxrwx   0        0        0        0 2023-07-15 09:53:13.175037 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/
+-rw-rw-rw-   0        0        0     5488 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/Stand.json
+-rw-rw-rw-   0        0        0     4549 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
+-rw-rw-rw-   0        0        0     1757 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
+-rw-rw-rw-   0        0        0      906 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/基础事件.json
+-rw-rw-rw-   0        0        0     2717 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
+-rw-rw-rw-   0        0        0     1257 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
+-rw-rw-rw-   0        0        0    22637 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/群友日常.json
+-rw-rw-rw-   0        0        0     4751 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
+-rw-rw-rw-   0        0        0     1010 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
+-rw-rw-rw-   0        0        0     2253 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
+-rw-rw-rw-   0        0        0    12889 2023-07-11 16:50:54.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/menu_data.json
+-rw-rw-rw-   0        0        0     5332 2023-07-07 16:19:38.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/props_library.json
+drwxrwxrwx   0        0        0        0 2023-07-15 09:53:13.177040 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/subprocess/
+-rw-rw-rw-   0        0        0     2278 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:53:13.181543 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/utils/
+-rw-rw-rw-   0        0        0     1323 2023-06-27 06:06:09.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/utils/avatar.py
+-rw-rw-rw-   0        0        0    22338 2023-07-14 15:16:16.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/utils/chart.py
+-rw-rw-rw-   0        0        0     1141 2023-06-27 04:18:19.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:53:13.141009 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection.egg-info/
+-rw-rw-rw-   0        0        0      376 2023-07-15 09:53:12.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1976 2023-07-15 09:53:13.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 09:53:12.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-07-15 09:53:12.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-07-15 09:53:12.000000 nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 09:53:13.186048 nonebot_plugin_game_collection-2.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      730 2023-07-15 09:52:30.000000 nonebot_plugin_game_collection-2.3.7/setup.py
```

### Comparing `nonebot_plugin_game_collection-2.3.6/LICENSE` & `nonebot_plugin_game_collection-2.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/README.md` & `nonebot_plugin_game_collection-2.3.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Account.py` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/Account.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,15 @@
         return f"你没有足够的金币，无法完成结算。\n——你还有{self_group_account.gold}枚金币。"
 
     if target_group_account.props.get("42001",0):
         fee = 0
         tips = f"『{props_library['42001']['name']}』免手续费"
     else:
         fee = int(gold * 0.02)
+        group_data[self_group_account.group_id].company.bank += fee
         tips = f"扣除2%手续费：{fee}，实际到账金额{gold - fee}"
 
     self_user.gold -= gold
     self_group_account.gold -= gold
     target_user.gold += gold - fee
     target_group_account.gold += gold - fee
 
@@ -460,32 +461,14 @@
     生成总排行榜
     """
     if not (ranklist := Manager.All_ranklist(title)):
         return None
     info = await draw_rank(ranklist, title, 20)
     return MessageSegment.image(info_splicing(info,Manager.BG_path(event.user_id), spacing = 5))
 
-def transfer_fee(amount: int, limit: int) -> int:
-    levels = [[0.02, max_bet_gold * 10],[0.2, max_bet_gold * 40],[0.4, max_bet_gold * 50],[0.6, float('inf')]]
-    fee = 0
-    for n,(level_tax, level_step) in enumerate(levels):
-        if limit >= level_step:
-            limit -= level_step
-            continue
-        levels[n][1] -= limit
-        break
-    for level_tax, level_step in levels[n:]:
-        if amount <= level_step:
-            fee += amount * level_tax
-            break
-        fee += level_step * level_tax
-        amount -= level_step
-
-    return int(fee)
-
 def intergroup_transfer_gold(event:MessageEvent, gold:int, company_name:str):
     """
     跨群转移金币到自己的账户
     """
     user,group_account = Manager.locate_user(event)
     if not group_account:
         return "私聊未关联账户，请发送【关联账户】关联群内账户。"
@@ -498,24 +481,44 @@
         return f"没有 {company_name} 的注册信息"
 
     if company_id in user.group_accounts:
         target_group_account = user.group_accounts[company_id]
     else:
         return f"你在 {company_name} 没有创建账户"
 
-    group_account.gold -= gold
-    ExRate = group_data[group_account.group_id].company.level/group_data[company_id].company.level
-    ExRate = min(ExRate,10) if ExRate else 1.0
-    tgold = int(ExRate * gold + 0.5)
-    fee = transfer_fee(tgold, user.transfer_limit)
-    target_group_account.gold += tgold - fee
-    user.transfer_limit += tgold
-    user.gold -= fee
+    company = group_data[group_account.group_id].company
+    tcompany = group_data[company_id].company
 
-    return f"向 {company_name} 转移{gold}金币。\n汇率：{round(ExRate,2)} 手续费：{fee}({round(100*fee/tgold,2)}%)\n实际到账金额：{tgold - fee}"
+    ExRate = (company.level or 1.0)/tcompany.level
+    ExRate = min(ExRate,10)
+    ExRate = max(ExRate,0.1)
+
+    # 转出税
+    tax = company.transfer_tax(gold, group_account.transfer)
+    company.bank += tax
+    group_account.transfer += gold
+    # 转出
+    user.gold -= gold
+    group_account.gold -= gold
+    # 转入税
+    tgold = int(ExRate * (gold - tax) + 0.5)
+    ttax = tcompany.transfer_tax(tgold, target_group_account.transfer)
+    tcompany.bank += ttax
+    target_group_account.transfer += tgold
+    # 转入
+    tgold -= ttax
+    user.gold += tgold
+    target_group_account.gold += tgold
+
+    return (
+        f"向 {company_name} 转移{gold}金币。\n"
+        f"汇率 {round(ExRate,2)} \n"
+        f"手续费 {tax}({round(100*tax/gold,2)}%){ttax} ({round(100*ttax/(tgold+ttax),2)}%)\n"
+        f"实际到账金额 {tgold}"
+        )
 
 def freeze(target:UserDict):
     target_id = target.user_id
     gold = target.gold
     value = 0.0
     group_accounts = target.group_accounts
     for group_id,group_account in group_accounts.items():
```

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Alchemy.py` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/Alchemy.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Fortress/core.py` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/Fortress/core.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Game.py` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/Game.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/HorseRace/events_main.py` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/HorseRace/events_main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/HorseRace/horse.py` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/HorseRace/horse.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/HorseRace/race_group.py` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/HorseRace/race_group.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/HorseRace/start.py` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/HorseRace/start.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Manager.py` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/Manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from nonebot import get_driver
 from nonebot.log import logger
 
 from .utils.utils import image_url
 from .utils.chart import linecard_to_png, gini_coef, default_BG
 from .utils.avatar import download_url
 from .data import DataBase, UserDict, GroupAccount, GroupDict, Company, props_library
-from .config import revolt_gold, max_bet_gold, lucky_clover, path, BG_image
+from .config import revolt_gold, max_bet_gold, lucky_clover, path, BG_image,bet_gold
 
 driver = get_driver()
 
 # 加载数据
 
 datafile = path / "russian_data.json"
 
@@ -294,15 +294,15 @@
     else:
         return None
 
     rank = [x for x in rank if x[1]]
     rank.sort(key=lambda x:x[1],reverse=True)
     return rank
 
-def Gini(group_id:int, limit:int = revolt_gold[0]) -> float:
+def Gini(group_id:int, limit:int = bet_gold) -> float:
     """
     本群基尼系数
     """
     if group_id in group_data:
         namelist = group_data[group_id].namelist
     else:
         return None
```

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Market.py` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/Market.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     """
     group_id = event.group_id
     company = group_data[group_id].company
     if company.company_name:
         return f"本群已在市场注册，注册名：{company.company_name}"
     if check := check_company_name(company_name):
         return check
-    gold = Manager.group_wealths(group_id)
+    gold = Manager.group_wealths(group_id) + company.bank
     if gold < (limit := 15 * max_bet_gold):
         return f"本群金币（{round(gold,2)}）小于{limit}，注册失败。"
     if (gini := Manager.Gini(group_id)) > 0.56:
         return f"本群基尼系数（{round(gini,3)}）过高，注册失败。"
     company = group_data[group_id].company
     company.company_id = group_id
     company.company_name = company_name
@@ -118,14 +118,33 @@
         if company_id != group_id:
             company = group_data[company_id].company
             unit = company.float_gold / company.issuance
             value += stocks[company_id] * unit
     group_account.value = value
     return value
 
+def bank(event:GroupMessageEvent,sign:int, gold:int):
+    """
+    群金库存取
+    """
+    user,group_account = Manager.locate_user(event)
+    company = group_data[group_account.group_id].company
+    if sign == 1:
+        if company.bank < gold:
+            return f"金币不足。本群金库还有{company.bank}枚金币。"
+        tip = "取出"
+    else:
+        if group_account.gold < gold:
+            return f"金币不足。你还有{group_account.gold}枚金币。"
+        tip = "存入"
+    user.gold += sign*gold
+    group_account.gold += sign*gold
+    company.bank -= sign*gold
+    return f"你{tip}了{gold}金币。"
+
 def buy(event:MessageEvent, buy:int, company_name:str):
     """
     以发行价格购买股票
         buy:购买数量
         company_name:股票名
     """
     if company_name in company_index:
@@ -140,15 +159,15 @@
     company = group_data[company_id].company
     company_name = company.company_name
 
     buy = company.stock if company.stock < buy else buy
     if buy < 1:
         return "已售空，请等待结算或在交易市场购买。"
 
-    group_gold = Manager.group_wealths(company_id,company.level)
+    group_gold = Manager.group_wealths(company_id,company.level) + company.bank
 
     if group_gold < 10 * max_bet_gold:
         return f"【{company_name}】金币过少({group_gold})，无法交易。"
     float_gold = company.float_gold
     SI = company.issuance
     value = 0.0
     inner_buy = 0
@@ -210,15 +229,15 @@
 
     if my_stock < settle:
         return f"你没有足够的股份...你的 {company_name} 还有 {my_stock} 个"
 
     company = group_data[company_id].company
     company_name = company.company_name
 
-    group_gold = Manager.group_wealths(company_id,company.level)
+    group_gold = Manager.group_wealths(company_id,company.level) + company.bank
 
     if group_gold < 10 * max_bet_gold:
         return f"【{company_name}】金币过少({group_gold})，无法交易。"
 
     float_gold = company.float_gold
     SI = company.issuance
     value = 0.0
@@ -228,14 +247,15 @@
     value = int(value)
 
     if group_account.props.get("42001",0):
         fee = 0
         tips = f"『{props_library['42001']['name']}』免手续费"
     else:
         fee = int(value * 0.02)
+        group_data[group_account.group_id].company.bank += fee
         tips = f"扣除2%手续费：{fee}"
 
     # 结算股票
     company.stock += settle
     if group_account.stocks[company_id] == settle:
         del group_account.stocks[company_id]
         stock = 0
@@ -281,15 +301,15 @@
     user,group_account = Manager.locate_user(event)
     if not group_account:
         return "私聊未关联账户，请发送【关联账户】关联群内账户。"
 
     company = group_data[company_id].company
     company_name = company.company_name
 
-    rank = [x for x in company.exchange.items() if x[0] != user.user_id]
+    rank = [(user_id,exchange) for user_id,exchange in company.exchange.items() if user_id != user.user_id and exchange.n > 0]
     if not rank:
         return f"没有正在出售的 {company_name}"
     rank.sort(key = lambda x:x[1].quote)
 
     gold = 0
     Exlist = []
     my_gold = group_account.gold
@@ -310,26 +330,23 @@
     for user_id,n in Exlist:
         exchange = company.exchange[user_id]
         # 定位卖家
         seller_user = user_data[user_id]
         seller_group_account = seller_user.group_accounts[exchange.group_id]
         # 金币结算
         unsettled = int((exchange.quote * n) + 0.5)
-        gold += unsettled
         user.gold -=  unsettled
         group_account.gold -= unsettled
-        if seller_group_account.props.get("42001",0):
-            fee = 0
-        else:
-            fee = int(unsettled * 0.02)
-        seller_user.gold += unsettled - fee
-        seller_group_account.gold += unsettled - fee
+        seller_user.gold += unsettled
+        seller_group_account.gold += unsettled
         # 股票结算
         seller_group_account.stocks[company_id] -= n
         group_account.stocks[company_id] += n
+        # 记录信息
+        gold += unsettled
         count += n
         # 更新卖家群账户信息
         value_update(seller_group_account)
         exchange.n -= n
     # 更新买家群账户信息
     value_update(group_account)
     company.exchange = {k:v for k,v in company.exchange.items() if v.n > 0}
@@ -455,34 +472,34 @@
         info.append(linecard(msg, width = 880, endline = "路灯挂件"))
 
     # 加载公司信息
     if company_name:
         msg = (
             f"公司等级 {company.level}\n"
             f"成立时间 {datetime.datetime.fromtimestamp(company.time).strftime('%Y 年 %m 月 %d 日')}\n"
+            f"账户金额 {'{:,}'.format(company.bank)}\n"
             )
         info.append(linecard(msg + stock_profile(company), width = 880, endline = "注册信息"))
 
         p = OHLC(path, group_id)
 
         overtime = time.time() + 30
         while (returncode := p.poll()) == None:
             if time.time() > overtime:
                 returncode = 1
                 break
             await asyncio.sleep(0.5)
 
         if returncode == 0:
             info.append(Image.open(path / "candlestick" / f"{group_id}.png"))
-
-        ranklist = list(company.exchange.items())
+        ranklist = [(user_id,exchange) for user_id,exchange in company.exchange.items() if exchange.n > 0]
         ranklist.sort(key=lambda x:x[1].quote)
         msg = ""
-        for x in ranklist[:10]:
-            msg += f"{user_data[x[0]].nickname}\n[pixel][20]单价 {x[1].quote}[nowrap]\n[pixel][400]数量 {x[1].n}\n"
+        for user_id,exchange in ranklist[:10]:
+            msg += f"{user_data[user_id].nickname}\n[pixel][20]单价 {exchange.quote}[nowrap]\n[pixel][400]数量 {exchange.n}\n"
         if msg:
             info.append(linecard(msg, width = 880, font_size = 40,endline = "市场详情"))
         msg = company.intro
         if msg:
             info.append(linecard(msg + '\n', width = 880, font_size = 40,endline = "公司介绍"))
 
     return MessageSegment.image(info_splicing(info, Manager.BG_path(event.user_id)))
@@ -495,15 +512,15 @@
     float_gold = company.float_gold
     issuance = company.issuance
     msg = (
         f"固定资产 {'{:,}'.format(round(company.gold,2))}\n"
         f"市场流动 {'{:,}'.format(round(group_gold))}\n"
         f"发行价格 {'{:,}'.format(round(max(group_gold,float_gold)/issuance,2))}\n"
         f"结算价格 {'{:,}'.format(round(float_gold/issuance,2))}\n"
-        f"剩余数量 {company.stock}\n"
+        f"股票数量 {company.stock}\n"
         )
     return msg
 
 def Market_info_All(event:MessageEvent):
     """
     市场信息总览
     """
@@ -577,19 +594,19 @@
 def company_update(company:Company):
     """
     刷新公司信息
         company:公司账户
     """
     company_id = company.company_id
     # 更新全群金币数
-    group_gold = Manager.group_wealths(company_id,company.level)
+    group_gold = Manager.group_wealths(company_id,company.level) + company.bank
     company.group_gold = group_gold
-    # 固定资产回归值 = 80%全群金币数 + 40%股票融资 总计：80%~120%全群金币数
+    # 固定资产回归值 = 全群金币数 + 20%股票融资比例 总计：100%~120%全群金币数
     SI = company.issuance
-    line = group_gold * (1.2 - 0.4 * (company.stock / SI))
+    line = group_gold * (1.2 - 0.2 * (company.stock / SI))
     # 公司金币数回归到固定资产回归值
     gold = company.gold
     gold += (line - gold)/96
     company.gold = gold
     if gold > 0.0:
         # 股票价格变化 = 趋势性影响（正态分布） + 随机性影响（平均分布）
         float_gold = company.float_gold
@@ -620,14 +637,16 @@
             value = int(quote*n)
             # 结算股票
             company.Buyback(group_account,n)
             # 结算金币
             user.gold += value
             group_account.gold += value
             company.gold -= value
+        # 清理无效交易信息
+        company.exchange = {user_id:exchange for user_id,exchange in company.exchange.items() if exchange.n > 0}
     else:
         float_gold = 0.0
 
     # 更新浮动价格
     company.float_gold = float_gold
 
     # 记录价格历史
@@ -656,11 +675,11 @@
 def reset():
     """
     市场重置
     """
     company_ids = set([company_index[company_id] for company_id in company_index])
     for company_id in company_ids:
         company = group_data[company_id].company
-        group_gold = Manager.group_wealths(company_id,company.level)
+        group_gold = Manager.group_wealths(company_id,company.level) + company.bank
         company.group_gold = group_gold
-        company.float_gold = group_gold * (1.2 - 0.4 * (company.stock / company.issuance))
+        company.float_gold = group_gold * (1.2 - 0.2 * (company.stock / company.issuance))
         company.gold = company.float_gold
```

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/Prop.py` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/Prop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/__init__.py` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
     msg =  Account.gold_create(event,gold)
     await gold_create.finish(msg, at_sender=True)
 
 # 获取道具
 props_create = on_command("获取道具", permission = SUPERUSER, priority = 20, block = True)
 
 @props_create.handle()
-async def _(event:MessageEvent, arg:Message = CommandArg(),):
+async def _(event:MessageEvent, arg:Message = CommandArg()):
     arg = arg.extract_plain_text().strip().split()
     test = len(arg)
     if test == 1:
         prop_name = arg[0]
         count = 1
     elif test >1:
         prop_name = arg[0]
@@ -224,14 +224,37 @@
         if count < 1:
             count = 1
     else:
         return
     msg = Account.props_create(event, prop_name, count)
     await give_props.finish(msg, at_sender = True)
 
+# 银行存取
+bank = on_command("群金库",permission = SUPERUSER | GROUP_ADMIN | GROUP_OWNER,priority = 20,block = True)
+
+@bank.handle()
+async def _(event:GroupMessageEvent, arg:Message = CommandArg()):
+    arg = arg.extract_plain_text().strip()
+    sign = arg[0]
+    if sign == "取":
+        sign = 1
+    elif sign == "存":
+        sign = -1
+    elif arg.startswith("查看"):
+        await bank.finish(f"本群金库还有{data.group[event.group_id].company.bank}枚金币。", at_sender = True)
+    else:
+        return
+    gold = arg[1:].strip()
+    if not gold.isdigit():
+        return
+    else:
+        gold = int(gold)
+    msg = Market.bank(event,sign,gold)
+    await bank.finish(msg, at_sender = True)
+
 # 金币签到
 sign = on_command("金币签到", aliases = {"轮盘签到"}, priority = 20, block = True)
 
 @sign.handle()
 async def _(event:MessageEvent):
     msg =  Account.sign(event)
     await sign.finish(msg, at_sender = True)
```

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/config.py` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/data.py` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Dict
 from pydantic import BaseModel
 from pathlib import Path
 import random
 import math
+
 try:
     import ujson as json
 except ModuleNotFoundError:
     import json
 
 from nonebot.adapters.onebot.v11 import MessageEvent,GroupMessageEvent
 
@@ -18,14 +19,15 @@
     group_id:int = None
     nickname:str = None
     is_sign:bool = False
     revolution:bool = False
     security:int = 0
     gold:int = 0
     value:float = 0.0
+    transfer:int = 0
     stocks:Dict[int,int] = {}
     props:Dict[str,int] = {}
 
     def __init__(self, event:GroupMessageEvent = None, **obj):
         """
         初始化群账户
         """
@@ -44,15 +46,14 @@
     gold:int = 0
     win:int = 0
     lose:int = 0
     Achieve_win:int = 0
     Achieve_lose:int = 0
     group_accounts:Dict[int,GroupAccount] = {}
     connect:int = 0
-    transfer_limit:int = 0
     props:Dict[str,int] = {}
     alchemy:Dict[str,int] = {}
 
     def __init__(self, event:MessageEvent = None, **obj):
         """
         初始化用户字典
         """
@@ -83,14 +84,15 @@
     level:int = 0
     time:float = 0.0
     stock:int = 0
     issuance:int = 0
     gold:float = 0.0
     float_gold:float = 0.0
     group_gold:float = 0.0
+    bank:int = 0
     intro:str = None
     exchange:Dict[int,ExchangeInfo] = {}
 
     def Buyback(self, group_account:GroupAccount, n:int = None):
         """
         让公司回收本账户的股票
         """
@@ -98,18 +100,42 @@
         count = min(n,stock) if n else stock
         stock = stock - count
         if count:
             self.stock += count
             user_id = group_account.user_id
             group_account.stocks[self.company_id] = group_account.stocks.get(self.company_id) - count
             if user_id in self.exchange and (exchange := self.exchange[user_id]).group_id == group_account.group_id:
-                if exchange.n > count:
-                    exchange.n -= count
-                else:
-                    del self.exchange[user_id]
+                exchange.n -= count
+
+    def transfer_tax(self, amount: int, transfer_today: int) -> int:
+        """
+        计算本群转账税
+            transfer_today:今日已使用额度
+        """
+        level = self.level
+        if not level:
+            return int(amount*0.1 + 0.5)
+        step = self.float_gold/(25*level)
+        levels = [[0.01, step],[0.1, step * 2],[0.2, step * 2],[0.4, float('inf')]]
+        fee = 0
+        for n,(level_tax, level_step) in enumerate(levels):
+            if transfer_today >= level_step:
+                transfer_today -= level_step
+                continue
+            levels[n][1] -= transfer_today
+            break
+
+        for level_tax, level_step in levels[n:]:
+            if amount <= level_step:
+                fee += amount * level_tax
+                break
+            fee += level_step * level_tax
+            amount -= level_step
+
+        return int(fee)
 
 class GroupDict(BaseModel):
     """
     群字典
     """
     group_id:int = None
     namelist:set = set()
@@ -225,35 +251,37 @@
                 log += (
                     f"{company.company_name} 股票库存异常。\n"
                     f"记录值：{company.stock}\n"
                     f"实测值：{stock}\n"
                     "数据已修正。\n"
                     ) if company.stock + stock_check[group_id] != company.issuance else ""
                 company.stock = stock
+                # 修正交易市场
+                company.exchange = {user_id:exchange for user_id,exchange in company.exchange.items() if exchange.n > 0}
                 # Nan检查
                 company.gold = 0.0 if math.isnan(company.gold) else company.gold
                 company.float_gold = 0.0 if math.isnan(company.float_gold) else company.float_gold
                 company.group_gold = 0.0 if math.isnan(company.group_gold) else company.group_gold
         self.save()
         return log[:-1] if log else "数据一切正常！"
 
     def Newday(self):
         """
         刷新每日
         """
         revolution_today = random.randint(1,5) != 1
         for user in self.user.values():
-            # 刷新转账限额
-            user.transfer_limit = 0
             # 全局道具有效期 - 1天
             props = user.props
             props = {k:min(v-1,30) if k[2] == '0' else v for k,v in props.items()}
             for group_account in user.group_accounts.values():
                 # 刷新今日签到
                 group_account.is_sign = False
+                # 刷新转账限额
+                group_account.transfer = 0
                 # 概率刷新重置签到
                 group_account.revolution = revolution_today
                 # 群内道具有效期 - 1天
                 props = group_account.props
                 props = {k:min(v-1,30) if k[2] == '0' else v for k,v in props.items()}
         self.save()
```

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/Stand.json` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/Stand.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/基础事件.json` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/基础事件.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/群友日常.json` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/群友日常.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/menu_data.json` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/menu_data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/props_library.json` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/props_library.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/resource/subprocess/ohlc.py` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/resource/subprocess/ohlc.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/utils/avatar.py` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/utils/chart.py` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/utils/chart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection/utils/utils.py` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/nonebot_plugin_game_collection.egg-info/SOURCES.txt` & `nonebot_plugin_game_collection-2.3.7/nonebot_plugin_game_collection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_game_collection-2.3.6/setup.py` & `nonebot_plugin_game_collection-2.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_namespace_packages
 
 setup(
 name='nonebot_plugin_game_collection',
-version='2.3.6',
+version='2.3.7',
 description='改自nonebot_plugin_russian合并了nonebot_plugin_horserace还有一些自编玩法的小游戏合集。',
 #long_description=open('README.md','r').read(),
 author='karisaya',
 author_email='1048827424@qq.com',
 license='MIT license',
 include_package_data=True,
 packages=find_namespace_packages(include=["nonebot_plugin_game_collection","nonebot_plugin_game_collection.*"]),
```

