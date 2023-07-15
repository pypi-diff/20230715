# Comparing `tmp/hikari_core-0.9.0.tar.gz` & `tmp/hikari_core-0.9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_core-0.9.0.tar", max compression
+gzip compressed data, was "hikari_core-0.9.0.1.tar", max compression
```

## Comparing `hikari_core-0.9.0.tar` & `hikari_core-0.9.0.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     5066 2023-07-14 18:13:45.076853 hikari_core-0.9.0/hikari_core/__init__.py
--rw-r--r--   0        0        0    12101 2023-07-14 08:37:21.396563 hikari_core-0.9.0/hikari_core/analyze.py
--rw-r--r--   0        0        0     3498 2023-07-13 10:46:01.317795 hikari_core-0.9.0/hikari_core/command_select.py
--rw-r--r--   0        0        0     1506 2023-06-09 16:02:41.277675 hikari_core-0.9.0/hikari_core/config.py
--rw-r--r--   0        0        0    10720 2023-07-14 18:21:52.431027 hikari_core-0.9.0/hikari_core/data_source.py
--rw-r--r--   0        0        0        0 2023-07-07 07:41:52.433117 hikari_core-0.9.0/hikari_core/game/__init__.py
--rw-r--r--   0        0        0     2598 2023-07-07 08:04:40.589860 hikari_core-0.9.0/hikari_core/game/ban_search.py
--rw-r--r--   0        0        0     2324 2023-07-07 09:04:55.774201 hikari_core-0.9.0/hikari_core/game/box_check.py
--rw-r--r--   0        0        0     3659 2023-07-14 08:41:52.994916 hikari_core-0.9.0/hikari_core/game/help.py
--rw-r--r--   0        0        0     2122 2023-07-10 07:31:07.868469 hikari_core-0.9.0/hikari_core/game/roll.py
--rw-r--r--   0        0        0     2311 2023-07-07 08:58:39.067755 hikari_core-0.9.0/hikari_core/game/sx.py
--rw-r--r--   0        0        0      718 2023-06-09 16:15:42.096662 hikari_core-0.9.0/hikari_core/Html_Render/__init__.py
--rw-r--r--   0        0        0     2883 2023-06-09 16:15:26.391069 hikari_core-0.9.0/hikari_core/Html_Render/browser.py
--rw-r--r--   0        0        0     5512 2023-06-09 16:14:42.407633 hikari_core-0.9.0/hikari_core/Html_Render/data_source.py
--rw-r--r--   0        0        0    18237 2023-05-14 15:19:45.725399 hikari_core-0.9.0/hikari_core/Html_Render/templates/github-markdown-light.css
--rw-r--r--   0        0        0      662 2023-05-14 15:19:45.915374 hikari_core-0.9.0/hikari_core/Html_Render/templates/markdown.html
--rw-r--r--   0        0        0     4963 2023-05-14 15:19:45.917452 hikari_core-0.9.0/hikari_core/Html_Render/templates/pygments-default.css
--rw-r--r--   0        0        0      125 2023-05-14 15:19:45.917452 hikari_core-0.9.0/hikari_core/Html_Render/templates/text.css
--rw-r--r--   0        0        0      233 2023-05-14 15:19:45.918475 hikari_core-0.9.0/hikari_core/Html_Render/templates/text.html
--rw-r--r--   0        0        0     2703 2023-06-09 16:22:21.351620 hikari_core-0.9.0/hikari_core/HttpClient_Pool.py
--rw-r--r--   0        0        0     3152 2023-07-13 08:56:17.527001 hikari_core-0.9.0/hikari_core/model.py
--rw-r--r--   0        0        0        0 2023-05-14 15:19:46.163103 hikari_core-0.9.0/hikari_core/moudle/__init__.py
--rw-r--r--   0        0        0    11581 2023-07-14 08:31:13.584765 hikari_core-0.9.0/hikari_core/moudle/publicAPI.py
--rw-r--r--   0        0        0    10567 2023-07-13 09:41:24.730553 hikari_core-0.9.0/hikari_core/moudle/wws_bind.py
--rw-r--r--   0        0        0     2726 2023-07-13 06:28:59.408115 hikari_core-0.9.0/hikari_core/moudle/wws_info.py
--rw-r--r--   0        0        0     3553 2023-07-13 06:29:52.468436 hikari_core-0.9.0/hikari_core/moudle/wws_recent.py
--rw-r--r--   0        0        0     4085 2023-07-13 08:58:03.235425 hikari_core-0.9.0/hikari_core/moudle/wws_ship_info.py
--rw-r--r--   0        0        0     3998 2023-07-13 08:58:08.113156 hikari_core-0.9.0/hikari_core/moudle/wws_ship_recent.py
--rw-r--r--   0        0        0     6867 2023-07-13 08:58:13.299011 hikari_core-0.9.0/hikari_core/moudle/wws_shiprank.py
--rw-r--r--   0        0        0     4462 2023-07-14 12:03:50.576415 hikari_core-0.9.0/hikari_core/Template/bind-list.html
--rw-r--r--   0        0        0     3783 2023-07-14 12:03:51.005556 hikari_core-0.9.0/hikari_core/Template/select-ship.html
--rw-r--r--   0        0        0     5166 2023-07-14 12:03:51.031428 hikari_core-0.9.0/hikari_core/Template/ship-rank.html
--rw-r--r--   0        0        0      449 2023-07-14 12:03:51.047079 hikari_core-0.9.0/hikari_core/Template/text.html
--rw-r--r--   0        0        0     7310 2023-07-14 12:03:51.076856 hikari_core-0.9.0/hikari_core/Template/wws-ban.html
--rw-r--r--   0        0        0    16783 2023-07-14 12:03:51.120915 hikari_core-0.9.0/hikari_core/Template/wws-box-christmas.html
--rw-r--r--   0        0        0    18454 2023-07-14 12:03:51.167932 hikari_core-0.9.0/hikari_core/Template/wws-clan.html
--rw-r--r--   0        0        0    28156 2023-07-14 13:10:22.607915 hikari_core-0.9.0/hikari_core/Template/wws-info-recent.html
--rw-r--r--   0        0        0    28082 2023-07-14 13:16:23.660810 hikari_core-0.9.0/hikari_core/Template/wws-info.html
--rw-r--r--   0        0        0     2396 2023-07-14 12:03:51.349020 hikari_core-0.9.0/hikari_core/Template/wws-personalRecord.html
--rw-r--r--   0        0        0    21684 2023-07-14 12:03:51.375787 hikari_core-0.9.0/hikari_core/Template/wws-ship-recent.html
--rw-r--r--   0        0        0    21441 2023-07-14 13:18:45.676515 hikari_core-0.9.0/hikari_core/Template/wws-ship.html
--rw-r--r--   0        0        0     9472 2023-07-14 12:03:51.448109 hikari_core-0.9.0/hikari_core/Template/wws-sx.html
--rw-r--r--   0        0        0     5810 2023-07-14 12:03:51.476400 hikari_core-0.9.0/hikari_core/Template/wws-unban.html
--rw-r--r--   0        0        0     4393 2023-06-09 16:04:19.214393 hikari_core-0.9.0/hikari_core/utils.py
--rw-r--r--   0        0        0    35823 2023-05-12 02:05:38.427107 hikari_core-0.9.0/LICENSE
--rw-r--r--   0        0        0     1547 2023-07-14 18:20:28.281571 hikari_core-0.9.0/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-12 02:05:38.429109 hikari_core-0.9.0/README.md
--rw-r--r--   0        0        0     9938 1970-01-01 00:00:00.000000 hikari_core-0.9.0/setup.py
--rw-r--r--   0        0        0     1071 1970-01-01 00:00:00.000000 hikari_core-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     5066 2023-07-15 04:38:48.665919 hikari_core-0.9.0.1/hikari_core/__init__.py
+-rw-r--r--   0        0        0    12101 2023-07-14 08:37:21.396563 hikari_core-0.9.0.1/hikari_core/analyze.py
+-rw-r--r--   0        0        0     3510 2023-07-15 04:45:24.575490 hikari_core-0.9.0.1/hikari_core/command_select.py
+-rw-r--r--   0        0        0     1506 2023-06-09 16:02:41.277675 hikari_core-0.9.0.1/hikari_core/config.py
+-rw-r--r--   0        0        0    10722 2023-07-15 04:50:27.812498 hikari_core-0.9.0.1/hikari_core/data_source.py
+-rw-r--r--   0        0        0        0 2023-07-07 07:41:52.433117 hikari_core-0.9.0.1/hikari_core/game/__init__.py
+-rw-r--r--   0        0        0     2598 2023-07-07 08:04:40.589860 hikari_core-0.9.0.1/hikari_core/game/ban_search.py
+-rw-r--r--   0        0        0     2324 2023-07-07 09:04:55.774201 hikari_core-0.9.0.1/hikari_core/game/box_check.py
+-rw-r--r--   0        0        0     4664 2023-07-15 04:49:08.329262 hikari_core-0.9.0.1/hikari_core/game/help.py
+-rw-r--r--   0        0        0     2122 2023-07-10 07:31:07.868469 hikari_core-0.9.0.1/hikari_core/game/roll.py
+-rw-r--r--   0        0        0     2311 2023-07-07 08:58:39.067755 hikari_core-0.9.0.1/hikari_core/game/sx.py
+-rw-r--r--   0        0        0      718 2023-06-09 16:15:42.096662 hikari_core-0.9.0.1/hikari_core/Html_Render/__init__.py
+-rw-r--r--   0        0        0     2883 2023-06-09 16:15:26.391069 hikari_core-0.9.0.1/hikari_core/Html_Render/browser.py
+-rw-r--r--   0        0        0     5512 2023-06-09 16:14:42.407633 hikari_core-0.9.0.1/hikari_core/Html_Render/data_source.py
+-rw-r--r--   0        0        0    18237 2023-05-14 15:19:45.725399 hikari_core-0.9.0.1/hikari_core/Html_Render/templates/github-markdown-light.css
+-rw-r--r--   0        0        0      662 2023-05-14 15:19:45.915374 hikari_core-0.9.0.1/hikari_core/Html_Render/templates/markdown.html
+-rw-r--r--   0        0        0     4963 2023-05-14 15:19:45.917452 hikari_core-0.9.0.1/hikari_core/Html_Render/templates/pygments-default.css
+-rw-r--r--   0        0        0      125 2023-05-14 15:19:45.917452 hikari_core-0.9.0.1/hikari_core/Html_Render/templates/text.css
+-rw-r--r--   0        0        0      233 2023-05-14 15:19:45.918475 hikari_core-0.9.0.1/hikari_core/Html_Render/templates/text.html
+-rw-r--r--   0        0        0     2703 2023-06-09 16:22:21.351620 hikari_core-0.9.0.1/hikari_core/HttpClient_Pool.py
+-rw-r--r--   0        0        0     3152 2023-07-13 08:56:17.527001 hikari_core-0.9.0.1/hikari_core/model.py
+-rw-r--r--   0        0        0        0 2023-05-14 15:19:46.163103 hikari_core-0.9.0.1/hikari_core/moudle/__init__.py
+-rw-r--r--   0        0        0    11581 2023-07-14 08:31:13.584765 hikari_core-0.9.0.1/hikari_core/moudle/publicAPI.py
+-rw-r--r--   0        0        0    10567 2023-07-13 09:41:24.730553 hikari_core-0.9.0.1/hikari_core/moudle/wws_bind.py
+-rw-r--r--   0        0        0     2726 2023-07-13 06:28:59.408115 hikari_core-0.9.0.1/hikari_core/moudle/wws_info.py
+-rw-r--r--   0        0        0     3553 2023-07-13 06:29:52.468436 hikari_core-0.9.0.1/hikari_core/moudle/wws_recent.py
+-rw-r--r--   0        0        0     4085 2023-07-13 08:58:03.235425 hikari_core-0.9.0.1/hikari_core/moudle/wws_ship_info.py
+-rw-r--r--   0        0        0     3998 2023-07-13 08:58:08.113156 hikari_core-0.9.0.1/hikari_core/moudle/wws_ship_recent.py
+-rw-r--r--   0        0        0     6867 2023-07-13 08:58:13.299011 hikari_core-0.9.0.1/hikari_core/moudle/wws_shiprank.py
+-rw-r--r--   0        0        0     4462 2023-07-14 12:03:50.576415 hikari_core-0.9.0.1/hikari_core/Template/bind-list.html
+-rw-r--r--   0        0        0     3783 2023-07-14 12:03:51.005556 hikari_core-0.9.0.1/hikari_core/Template/select-ship.html
+-rw-r--r--   0        0        0     5166 2023-07-14 12:03:51.031428 hikari_core-0.9.0.1/hikari_core/Template/ship-rank.html
+-rw-r--r--   0        0        0      449 2023-07-14 12:03:51.047079 hikari_core-0.9.0.1/hikari_core/Template/text.html
+-rw-r--r--   0        0        0     7310 2023-07-14 12:03:51.076856 hikari_core-0.9.0.1/hikari_core/Template/wws-ban.html
+-rw-r--r--   0        0        0    16783 2023-07-14 12:03:51.120915 hikari_core-0.9.0.1/hikari_core/Template/wws-box-christmas.html
+-rw-r--r--   0        0        0    18454 2023-07-14 12:03:51.167932 hikari_core-0.9.0.1/hikari_core/Template/wws-clan.html
+-rw-r--r--   0        0        0    28156 2023-07-14 13:10:22.607915 hikari_core-0.9.0.1/hikari_core/Template/wws-info-recent.html
+-rw-r--r--   0        0        0    28082 2023-07-14 13:16:23.660810 hikari_core-0.9.0.1/hikari_core/Template/wws-info.html
+-rw-r--r--   0        0        0     2396 2023-07-14 12:03:51.349020 hikari_core-0.9.0.1/hikari_core/Template/wws-personalRecord.html
+-rw-r--r--   0        0        0    21684 2023-07-14 12:03:51.375787 hikari_core-0.9.0.1/hikari_core/Template/wws-ship-recent.html
+-rw-r--r--   0        0        0    21441 2023-07-14 13:18:45.676515 hikari_core-0.9.0.1/hikari_core/Template/wws-ship.html
+-rw-r--r--   0        0        0     9472 2023-07-14 12:03:51.448109 hikari_core-0.9.0.1/hikari_core/Template/wws-sx.html
+-rw-r--r--   0        0        0     5810 2023-07-14 12:03:51.476400 hikari_core-0.9.0.1/hikari_core/Template/wws-unban.html
+-rw-r--r--   0        0        0     4393 2023-06-09 16:04:19.214393 hikari_core-0.9.0.1/hikari_core/utils.py
+-rw-r--r--   0        0        0    35823 2023-05-12 02:05:38.427107 hikari_core-0.9.0.1/LICENSE
+-rw-r--r--   0        0        0     1549 2023-07-15 04:51:04.294442 hikari_core-0.9.0.1/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-05-12 02:05:38.429109 hikari_core-0.9.0.1/README.md
+-rw-r--r--   0        0        0     9940 1970-01-01 00:00:00.000000 hikari_core-0.9.0.1/setup.py
+-rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 hikari_core-0.9.0.1/PKG-INFO
```

### Comparing `hikari_core-0.9.0/hikari_core/__init__.py` & `hikari_core-0.9.0.1/hikari_core/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/analyze.py` & `hikari_core-0.9.0.1/hikari_core/analyze.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/command_select.py` & `hikari_core-0.9.0.1/hikari_core/command_select.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from dataclasses import dataclass
 from typing import List, Protocol, Tuple, runtime_checkable
 
 from .game.ban_search import get_BanInfo
 from .game.box_check import check_christmas_box
-from .game.help import check_version, get_help, update_template
+from .game.help import async_update_template, check_version, get_help
 
 # from .game.ocr import get_Random_Ocr_Pic
 from .game.roll import roll_ship
 from .game.sx import get_sx_info
 from .moudle.publicAPI import get_ship_name
 from .moudle.wws_bind import change_BindInfo, delete_BindInfo, get_BindInfo, set_BindInfo, set_special_BindInfo
 
@@ -49,15 +49,15 @@
     command(('roll', '随机'), roll_ship),
     command(('sx', '扫雪'), get_sx_info),
     command(('ban', '封号记录'), get_BanInfo),
     command(('box', 'sd', '圣诞船池'), check_christmas_box),
     command(('搜船名', '查船名', '船名'), get_ship_name),
     command(('help', '帮助'), get_help),
     command(('check_version', '检查更新'), check_version),
-    command(('更新样式',), update_template),
+    command(('更新样式',), async_update_template),
 ]
 
 second_command_list = [
     command(('recent', '近期'), get_ShipRecent),
     command(('ship', '单船'), get_ShipRecent),
     # command(("clan", "军团", "公会", "工会"), get_record),
     # command(("record", "历史记录"), get_record),
```

### Comparing `hikari_core-0.9.0/hikari_core/config.py` & `hikari_core-0.9.0.1/hikari_core/config.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/data_source.py` & `hikari_core-0.9.0.1/hikari_core/data_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Tuple
 
 dir_path = Path(__file__).parent
 template_path = dir_path / 'Template'
 yuyuko_url = 'https://api.wows.shinoaki.com'
-__version__ = '0.9.0'
+__version__ = '0.9.0.1'
 
 
 @dataclass
 class matching:
     keywords: Tuple[str, ...]
     match_keywords: str
```

### Comparing `hikari_core-0.9.0/hikari_core/game/ban_search.py` & `hikari_core-0.9.0.1/hikari_core/game/ban_search.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/game/box_check.py` & `hikari_core-0.9.0.1/hikari_core/game/box_check.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/game/help.py` & `hikari_core-0.9.0.1/hikari_core/game/help.py`

 * *Files 18% similar despite different names*

```diff
@@ -79,7 +79,29 @@
             logger.info('更新模板成功')
             # for each in result:
             #    for name, url in each.items():
             #        tasks.append(asyncio.ensure_future(download_template(url, name)))
         # await asyncio.gather(*tasks)
     except Exception:
         logger.error(traceback.format_exc())
+
+
+async def async_update_template(hikari: Hikari_Model = Hikari_Model()):  # noqa: B008
+    try:
+        # tasks = []
+        url = 'https://hikari-resource.oss-cn-shanghai.aliyuncs.com/hikari_core_template/template.json'
+        with httpx.Client() as client:
+            resp = client.get(url, timeout=20)
+            result = orjson.loads(resp.content)
+            for each in result:
+                for name, url in each.items():
+                    resp = client.get(url, timeout=5)
+                    with open(template_path / name, 'wb+') as file:
+                        file.write(resp.content)
+            logger.info('更新模板成功')
+            return hikari.success('更新模板成功')
+            # for each in result:
+            #    for name, url in each.items():
+            #        tasks.append(asyncio.ensure_future(download_template(url, name)))
+        # await asyncio.gather(*tasks)
+    except Exception:
+        logger.error(traceback.format_exc())
```

### Comparing `hikari_core-0.9.0/hikari_core/game/roll.py` & `hikari_core-0.9.0.1/hikari_core/game/roll.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/game/sx.py` & `hikari_core-0.9.0.1/hikari_core/game/sx.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Html_Render/__init__.py` & `hikari_core-0.9.0.1/hikari_core/Html_Render/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Html_Render/browser.py` & `hikari_core-0.9.0.1/hikari_core/Html_Render/browser.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Html_Render/data_source.py` & `hikari_core-0.9.0.1/hikari_core/Html_Render/data_source.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Html_Render/templates/github-markdown-light.css` & `hikari_core-0.9.0.1/hikari_core/Html_Render/templates/github-markdown-light.css`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Html_Render/templates/markdown.html` & `hikari_core-0.9.0.1/hikari_core/Html_Render/templates/markdown.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Html_Render/templates/pygments-default.css` & `hikari_core-0.9.0.1/hikari_core/Html_Render/templates/pygments-default.css`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/HttpClient_Pool.py` & `hikari_core-0.9.0.1/hikari_core/HttpClient_Pool.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/model.py` & `hikari_core-0.9.0.1/hikari_core/model.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/moudle/publicAPI.py` & `hikari_core-0.9.0.1/hikari_core/moudle/publicAPI.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/moudle/wws_bind.py` & `hikari_core-0.9.0.1/hikari_core/moudle/wws_bind.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/moudle/wws_info.py` & `hikari_core-0.9.0.1/hikari_core/moudle/wws_info.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/moudle/wws_recent.py` & `hikari_core-0.9.0.1/hikari_core/moudle/wws_recent.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/moudle/wws_ship_info.py` & `hikari_core-0.9.0.1/hikari_core/moudle/wws_ship_info.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/moudle/wws_ship_recent.py` & `hikari_core-0.9.0.1/hikari_core/moudle/wws_ship_recent.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/moudle/wws_shiprank.py` & `hikari_core-0.9.0.1/hikari_core/moudle/wws_shiprank.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Template/bind-list.html` & `hikari_core-0.9.0.1/hikari_core/Template/bind-list.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Template/select-ship.html` & `hikari_core-0.9.0.1/hikari_core/Template/select-ship.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Template/ship-rank.html` & `hikari_core-0.9.0.1/hikari_core/Template/ship-rank.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Template/wws-ban.html` & `hikari_core-0.9.0.1/hikari_core/Template/wws-ban.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Template/wws-box-christmas.html` & `hikari_core-0.9.0.1/hikari_core/Template/wws-box-christmas.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Template/wws-clan.html` & `hikari_core-0.9.0.1/hikari_core/Template/wws-clan.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Template/wws-info-recent.html` & `hikari_core-0.9.0.1/hikari_core/Template/wws-info-recent.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Template/wws-info.html` & `hikari_core-0.9.0.1/hikari_core/Template/wws-info.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Template/wws-personalRecord.html` & `hikari_core-0.9.0.1/hikari_core/Template/wws-personalRecord.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Template/wws-ship-recent.html` & `hikari_core-0.9.0.1/hikari_core/Template/wws-ship-recent.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Template/wws-ship.html` & `hikari_core-0.9.0.1/hikari_core/Template/wws-ship.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Template/wws-sx.html` & `hikari_core-0.9.0.1/hikari_core/Template/wws-sx.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/Template/wws-unban.html` & `hikari_core-0.9.0.1/hikari_core/Template/wws-unban.html`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/hikari_core/utils.py` & `hikari_core-0.9.0.1/hikari_core/utils.py`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/LICENSE` & `hikari_core-0.9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_core-0.9.0/pyproject.toml` & `hikari_core-0.9.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hikari-core"
-version = "0.9.0"
+version = "0.9.0.1"
 description = "SDK for yuyuko,战舰世界yuyuko平台BOT SDK"
 authors = ["benx1n <1119809439@qq.com>"]
 readme = "README.md"
 packages = [{include = "hikari_core"}]
 homepage = "https://github.com/wows-yuyuko/Hikari-core"
 repository = "https://github.com/wows-yuyuko/Hikari-core"
 keywords = ["qqbot", "wows", "wws","bot","stats"]
```

### Comparing `hikari_core-0.9.0/setup.py` & `hikari_core-0.9.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
  'loguru>=0.7.0,<0.8.0',
  'orjson>=3.8.11,<4.0.0',
  'playwright>=1.17.2',
  'pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'hikari-core',
-    'version': '0.9.0',
+    'version': '0.9.0.1',
     'description': 'SDK for yuyuko,战舰世界yuyuko平台BOT SDK',
     'long_description': '# Hikari-core\nSDK for yuyuko API\n',
     'author': 'benx1n',
     'author_email': '1119809439@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/wows-yuyuko/Hikari-core',
```

### Comparing `hikari_core-0.9.0/PKG-INFO` & `hikari_core-0.9.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-core
-Version: 0.9.0
+Version: 0.9.0.1
 Summary: SDK for yuyuko,战舰世界yuyuko平台BOT SDK
 Home-page: https://github.com/wows-yuyuko/Hikari-core
 Keywords: qqbot,wows,wws,bot,stats
 Author: benx1n
 Author-email: 1119809439@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

