# Comparing `tmp/yetanotherpicsearch-1.9.3.tar.gz` & `tmp/yetanotherpicsearch-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetanotherpicsearch-1.9.3.tar", max compression
+gzip compressed data, was "yetanotherpicsearch-1.9.4.tar", max compression
```

## Comparing `yetanotherpicsearch-1.9.3.tar` & `yetanotherpicsearch-1.9.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/LICENSE
--rw-r--r--   0        0        0     2041 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/README.md
--rw-r--r--   0        0        0     9390 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/__init__.py
--rw-r--r--   0        0        0     2089 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/ascii2d.py
--rw-r--r--   0        0        0      657 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/baidu.py
--rw-r--r--   0        0        0     2781 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/config.py
--rw-r--r--   0        0        0     5086 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/ehentai.py
--rw-r--r--   0        0        0     1195 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/google.py
--rw-r--r--   0        0        0     2003 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/iqdb.py
--rw-r--r--   0        0        0     3132 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/nhentai.py
--rw-r--r--   0        0        0      924 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/nhentai_model.py
--rw-r--r--   0        0        0     6047 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/saucenao.py
--rw-r--r--   0        0        0     7416 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/utils.py
--rw-r--r--   0        0        0     1827 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/whatanime.py
--rw-r--r--   0        0        0     1075 2023-06-04 16:53:46.154185 yetanotherpicsearch-1.9.3/YetAnotherPicSearch/yandex.py
--rw-r--r--   0        0        0     1427 2023-06-04 16:53:46.162186 yetanotherpicsearch-1.9.3/pyproject.toml
--rw-r--r--   0        0        0     3453 1970-01-01 00:00:00.000000 yetanotherpicsearch-1.9.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-15 02:25:31.143178 yetanotherpicsearch-1.9.4/LICENSE
+-rw-r--r--   0        0        0     2041 2023-07-15 02:25:31.143178 yetanotherpicsearch-1.9.4/README.md
+-rw-r--r--   0        0        0     9414 2023-07-15 02:25:31.143178 yetanotherpicsearch-1.9.4/YetAnotherPicSearch/__init__.py
+-rw-r--r--   0        0        0     2093 2023-07-15 02:25:31.143178 yetanotherpicsearch-1.9.4/YetAnotherPicSearch/ascii2d.py
+-rw-r--r--   0        0        0      657 2023-07-15 02:25:31.143178 yetanotherpicsearch-1.9.4/YetAnotherPicSearch/baidu.py
+-rw-r--r--   0        0        0     2781 2023-07-15 02:25:31.143178 yetanotherpicsearch-1.9.4/YetAnotherPicSearch/config.py
+-rw-r--r--   0        0        0     5086 2023-07-15 02:25:31.143178 yetanotherpicsearch-1.9.4/YetAnotherPicSearch/ehentai.py
+-rw-r--r--   0        0        0     1195 2023-07-15 02:25:31.143178 yetanotherpicsearch-1.9.4/YetAnotherPicSearch/google.py
+-rw-r--r--   0        0        0     2003 2023-07-15 02:25:31.143178 yetanotherpicsearch-1.9.4/YetAnotherPicSearch/iqdb.py
+-rw-r--r--   0        0        0     3132 2023-07-15 02:25:31.143178 yetanotherpicsearch-1.9.4/YetAnotherPicSearch/nhentai.py
+-rw-r--r--   0        0        0      924 2023-07-15 02:25:31.143178 yetanotherpicsearch-1.9.4/YetAnotherPicSearch/nhentai_model.py
+-rw-r--r--   0        0        0     6047 2023-07-15 02:25:31.143178 yetanotherpicsearch-1.9.4/YetAnotherPicSearch/saucenao.py
+-rw-r--r--   0        0        0     8012 2023-07-15 02:25:31.143178 yetanotherpicsearch-1.9.4/YetAnotherPicSearch/utils.py
+-rw-r--r--   0        0        0     1827 2023-07-15 02:25:31.143178 yetanotherpicsearch-1.9.4/YetAnotherPicSearch/whatanime.py
+-rw-r--r--   0        0        0     1075 2023-07-15 02:25:31.143178 yetanotherpicsearch-1.9.4/YetAnotherPicSearch/yandex.py
+-rw-r--r--   0        0        0     1428 2023-07-15 02:25:31.151178 yetanotherpicsearch-1.9.4/pyproject.toml
+-rw-r--r--   0        0        0     3454 1970-01-01 00:00:00.000000 yetanotherpicsearch-1.9.4/PKG-INFO
```

### Comparing `yetanotherpicsearch-1.9.3/LICENSE` & `yetanotherpicsearch-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.3/README.md` & `yetanotherpicsearch-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/__init__.py` & `yetanotherpicsearch-1.9.4/YetAnotherPicSearch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 
 
 async def send_result_message(
     bot: Bot, event: MessageEvent, msg_list: List[str], index: Optional[int] = None
 ) -> None:
     if not (
         isinstance(event, PrivateMessageEvent)
-        and event.user_id == int(list(config.superusers)[0])
+        and (config.superusers and event.user_id == int(list(config.superusers)[0]))
     ):
         msg_list = [
             msg.replace("❤️ 已收藏\n", "") if "已收藏" in msg else msg for msg in msg_list
         ]
 
     if flag := (config.forward_search_result and len(msg_list) > 1):
         try:
```

### Comparing `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/ascii2d.py` & `yetanotherpicsearch-1.9.4/YetAnotherPicSearch/ascii2d.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,18 +31,18 @@
             continue
 
         thumbnail = await handle_img(r.thumbnail)
         if not config.hide_img and thumbnail.startswith("预览图链接"):
             continue
 
         title = r.title
-        if r.url_list and title == r.url_list[0][1]:
+        if r.url_list and title == r.url_list[0].text:
             title = ""
 
-        source = r.url or (r.url_list and r.url_list[0][0])
+        source = r.url or (r.url_list and r.url_list[0].href)
         source = await shorten_url(source) if source else ""
 
         author = r.author
         if author and r.author_url:
             author_url = await shorten_url(r.author_url)
             author = f"[{author}]({author_url})"
```

### Comparing `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/baidu.py` & `yetanotherpicsearch-1.9.4/YetAnotherPicSearch/baidu.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/config.py` & `yetanotherpicsearch-1.9.4/YetAnotherPicSearch/config.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/ehentai.py` & `yetanotherpicsearch-1.9.4/YetAnotherPicSearch/ehentai.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/google.py` & `yetanotherpicsearch-1.9.4/YetAnotherPicSearch/google.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/iqdb.py` & `yetanotherpicsearch-1.9.4/YetAnotherPicSearch/iqdb.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/nhentai.py` & `yetanotherpicsearch-1.9.4/YetAnotherPicSearch/nhentai.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/nhentai_model.py` & `yetanotherpicsearch-1.9.4/YetAnotherPicSearch/nhentai_model.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/saucenao.py` & `yetanotherpicsearch-1.9.4/YetAnotherPicSearch/saucenao.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/utils.py` & `yetanotherpicsearch-1.9.4/YetAnotherPicSearch/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import re
 from base64 import b64encode
 from collections import defaultdict
 from difflib import SequenceMatcher
 from functools import wraps
+from io import BytesIO
 from typing import (
     Any,
     Callable,
     Coroutine,
     DefaultDict,
     Dict,
     List,
@@ -17,16 +18,18 @@
 )
 
 import arrow
 from cachetools import TTLCache
 from httpx import URL, AsyncClient, InvalidURL
 from nonebot.adapters.onebot.v11 import Bot
 from PicImageSearch.model.ehentai import EHentaiItem, EHentaiResponse
+from PIL import Image
 from pyquery import PyQuery
 from shelved_cache import cachedasyncmethod
+from tenacity import TryAgain, retry, stop_after_attempt, stop_after_delay
 
 from .config import config
 from .nhentai_model import NHentaiItem, NHentaiResponse
 
 T = TypeVar("T")
 SEARCH_FUNCTION_TYPE = Callable[..., Coroutine[Any, Any, List[str]]]
 
@@ -35,27 +38,41 @@
         "Mozilla/5.0 (Windows NT 10.0; Win64; x64) "
         "AppleWebKit/537.36 (KHTML, like Gecko) "
         "Chrome/99.0.4844.82 Safari/537.36"
     )
 }
 
 
+@retry(stop=(stop_after_attempt(3) | stop_after_delay(30)), reraise=True)
 async def get_image_bytes_by_url(
     url: str, cookies: Optional[str] = None
 ) -> Optional[bytes]:
+    _url = URL(url)
+    referer = f"{_url.scheme}://{_url.host}/"
+    headers = {"Referer": referer, **DEFAULT_HEADERS}
     async with AsyncClient(
-        headers=DEFAULT_HEADERS,
+        headers=headers,
         cookies=parse_cookies(cookies),
         proxies=config.proxy,
         follow_redirects=True,
     ) as session:
         resp = await session.get(url)
-        if resp.status_code < 400:
-            return resp.content
-    return None
+        if resp.status_code == 404:
+            return None
+
+        if resp.status_code >= 400 or len(resp.content) == 0:
+            raise TryAgain
+
+        im = Image.open(BytesIO(resp.content))
+        if im.format == "WEBP":
+            with BytesIO() as output:
+                im.save(output, "PNG")
+                return output.getvalue()
+
+    return resp.content
 
 
 async def handle_img(
     url: str,
     hide_img: bool = config.hide_img,
     cookies: Optional[str] = None,
 ) -> str:
```

### Comparing `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/whatanime.py` & `yetanotherpicsearch-1.9.4/YetAnotherPicSearch/whatanime.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.3/YetAnotherPicSearch/yandex.py` & `yetanotherpicsearch-1.9.4/YetAnotherPicSearch/yandex.py`

 * *Files identical despite different names*

### Comparing `yetanotherpicsearch-1.9.3/pyproject.toml` & `yetanotherpicsearch-1.9.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "YetAnotherPicSearch"
-version = "1.9.3"
+version = "1.9.4"
 description = "Yet Another Picture Search Nonebot Plugin"
 authors = ["NekoAria"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "YetAnotherPicSearch" },
 ]
@@ -13,19 +13,19 @@
 keywords = ["nonebot", "ascii2d", "baidu", "e-hentai", "google", "iqdb", "saucenao", "tracemoe", "yandex", "anime", "danbooru", "doujin", "pixiv"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 arrow = "^1.2.3"
 cachetools = "^5.3.1"
 httpx = "^0.24.1"
-lxml = "^4.9.2"
+lxml = "^4.9.3"
 nonebot-adapter-onebot = "^2.2.3"
 nonebot2 = "^2.0.0"
-PicImageSearch = "^3.9.2"
-pydantic = "^1.10.8"
+PicImageSearch = "^3.9.4"
+pydantic = "^1.10.11"
 pyquery = "^2.0.0"
 python-socks = {extras = ["asyncio"], version = "^2.3.0", optional = true}
 socksio = { version = "^1.0.0", optional = true }
 shelved-cache = "^0.3.1"
 tenacity = "^8.2.2"
 
 [tool.poetry.extras]
```

### Comparing `yetanotherpicsearch-1.9.3/PKG-INFO` & `yetanotherpicsearch-1.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: yetanotherpicsearch
-Version: 1.9.3
+Version: 1.9.4
 Summary: Yet Another Picture Search Nonebot Plugin
 Home-page: https://github.com/NekoAria/YetAnotherPicSearch
 License: GPL-3.0-only
 Keywords: nonebot,ascii2d,baidu,e-hentai,google,iqdb,saucenao,tracemoe,yandex,anime,danbooru,doujin,pixiv
 Author: NekoAria
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: socks
-Requires-Dist: PicImageSearch (>=3.9.2,<4.0.0)
+Requires-Dist: PicImageSearch (>=3.9.4,<4.0.0)
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: cachetools (>=5.3.1,<6.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
-Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
-Requires-Dist: pydantic (>=1.10.8,<2.0.0)
+Requires-Dist: pydantic (>=1.10.11,<2.0.0)
 Requires-Dist: pyquery (>=2.0.0,<3.0.0)
 Requires-Dist: python-socks[asyncio] (>=2.3.0,<3.0.0) ; extra == "socks"
 Requires-Dist: shelved-cache (>=0.3.1,<0.4.0)
 Requires-Dist: socksio (>=1.0.0,<2.0.0) ; extra == "socks"
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Project-URL: Repository, https://github.com/NekoAria/YetAnotherPicSearch
 Description-Content-Type: text/markdown
```

