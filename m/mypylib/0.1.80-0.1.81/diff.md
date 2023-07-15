# Comparing `tmp/mypylib-0.1.80.tar.gz` & `tmp/mypylib-0.1.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypylib-0.1.80.tar", last modified: Wed Jul 12 15:07:40 2023, max compression
+gzip compressed data, was "mypylib-0.1.81.tar", last modified: Sat Jul 15 09:06:35 2023, max compression
```

## Comparing `mypylib-0.1.80.tar` & `mypylib-0.1.81.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-12 15:07:40.232627 mypylib-0.1.80/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-07-12 15:07:40.232361 mypylib-0.1.80/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.80/README.md
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-12 15:07:40.229312 mypylib-0.1.80/mypylib/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.80/mypylib/MP_shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    47236 2023-07-12 15:07:00.000000 mypylib-0.1.80/mypylib/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.80/mypylib/binance_copy_bot.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.80/mypylib/binance_copy_bot_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.80/mypylib/chdbif.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5333 2023-07-12 15:06:31.000000 mypylib-0.1.80/mypylib/crawler.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.80/mypylib/crypto.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.80/mypylib/finmind.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.80/mypylib/libexcel.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    24435 2023-06-01 04:56:52.000000 mypylib-0.1.80/mypylib/mvp.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.80/mypylib/mytest.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.80/mypylib/option_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.80/mypylib/shioaji_history_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.80/mypylib/shioaji_kline.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.80/mypylib/shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7649 2023-04-18 13:50:52.000000 mypylib-0.1.80/mypylib/sjtools.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.80/mypylib/tLineNotify.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7735 2023-06-01 04:56:52.000000 mypylib-0.1.80/mypylib/ti.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-12 15:07:40.231707 mypylib-0.1.80/mypylib/tmpDevelopment/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.80/mypylib/tmpDevelopment/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.80/mypylib/tmpDevelopment/warrant_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2023-04-27 13:08:02.000000 mypylib-0.1.80/mypylib/tplaysound.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8466 2023-06-19 13:26:50.000000 mypylib-0.1.80/mypylib/tredis.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8217 2023-07-03 23:14:11.000000 mypylib-0.1.80/mypylib/warrant.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-12 15:07:40.231139 mypylib-0.1.80/mypylib.egg-info/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-07-12 15:07:39.000000 mypylib-0.1.80/mypylib.egg-info/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      673 2023-07-12 15:07:40.000000 mypylib-0.1.80/mypylib.egg-info/SOURCES.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-07-12 15:07:39.000000 mypylib-0.1.80/mypylib.egg-info/dependency_links.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-07-12 15:07:40.000000 mypylib-0.1.80/mypylib.egg-info/top_level.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-07-12 15:07:40.232718 mypylib-0.1.80/setup.cfg
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.80/setup.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-15 09:06:35.041960 mypylib-0.1.81/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-07-15 09:06:35.041717 mypylib-0.1.81/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.81/README.md
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-15 09:06:35.039149 mypylib-0.1.81/mypylib/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.81/mypylib/MP_shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    47319 2023-07-15 09:05:04.000000 mypylib-0.1.81/mypylib/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.81/mypylib/binance_copy_bot.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.81/mypylib/binance_copy_bot_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.81/mypylib/chdbif.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5368 2023-07-15 09:04:03.000000 mypylib-0.1.81/mypylib/crawler.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.81/mypylib/crypto.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.81/mypylib/finmind.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.81/mypylib/libexcel.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    24435 2023-06-01 04:56:52.000000 mypylib-0.1.81/mypylib/mvp.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.81/mypylib/mytest.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.81/mypylib/option_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.81/mypylib/shioaji_history_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.81/mypylib/shioaji_kline.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.81/mypylib/shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7649 2023-04-18 13:50:52.000000 mypylib-0.1.81/mypylib/sjtools.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.81/mypylib/tLineNotify.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7735 2023-06-01 04:56:52.000000 mypylib-0.1.81/mypylib/ti.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-15 09:06:35.041060 mypylib-0.1.81/mypylib/tmpDevelopment/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.81/mypylib/tmpDevelopment/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.81/mypylib/tmpDevelopment/warrant_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2023-04-27 13:08:02.000000 mypylib-0.1.81/mypylib/tplaysound.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8466 2023-06-19 13:26:50.000000 mypylib-0.1.81/mypylib/tredis.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8217 2023-07-03 23:14:11.000000 mypylib-0.1.81/mypylib/warrant.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-07-15 09:06:35.040573 mypylib-0.1.81/mypylib.egg-info/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-07-15 09:06:34.000000 mypylib-0.1.81/mypylib.egg-info/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      673 2023-07-15 09:06:34.000000 mypylib-0.1.81/mypylib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-07-15 09:06:34.000000 mypylib-0.1.81/mypylib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-07-15 09:06:34.000000 mypylib-0.1.81/mypylib.egg-info/top_level.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-07-15 09:06:35.042044 mypylib-0.1.81/setup.cfg
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.81/setup.py
```

### Comparing `mypylib-0.1.80/README.md` & `mypylib-0.1.81/README.md`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/MP_shioaji_ticks.py` & `mypylib-0.1.81/mypylib/MP_shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/__init__.py` & `mypylib-0.1.81/mypylib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,19 +68,20 @@
     '2023/05/17: 0.1.73 shioaji 1.0 改 Mmvp.py & ti.py',
     '2023/05/22: 0.1.74 mvp() 不繼承 base class。因為shioaji升級的關係。先可以跑再說',
     '2023/06/01: 0.1.75 Apply Carey change',
     '2023/06/15: 0.1.76 Add crawler',
     '2023/06/19: 0.1.77 Not using stupid Redis connection pool',
     '2023/07/05: 0.1.78 cynes api v1 support',
     '2023/07/06: 0.1.79 news crawler little modification',
-    '2023/07/12: 0.1.80 修改crawler'
+    '2023/07/12: 0.1.80 修改crawler',
+    '2023/07/15: 0.1.81 修改 crawler 的 user agent，以免被認為是爬蟲'
 
 }
 
-__version__ = '0.1.80'
+__version__ = '0.1.81'
 
 request_headers = {
     'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'
 }
 
 path_cronlog = 'cronlog'
```

### Comparing `mypylib-0.1.80/mypylib/binance_copy_bot.py` & `mypylib-0.1.81/mypylib/binance_copy_bot.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/binance_copy_bot_test.py` & `mypylib-0.1.81/mypylib/binance_copy_bot_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/chdbif.py` & `mypylib-0.1.81/mypylib/chdbif.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/crawler.py` & `mypylib-0.1.81/mypylib/crawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 import urllib3
 from loguru import logger
 
 headers = {
     'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.102 Safari/537.36 Edge/18.18362',
 }
 
+
+
 """
 {'isOutsource': 0,
     'content': '&lt;p&gt;佳世達 (2352-TW) 今 (5) 日公告 6 月營收 189 億元，月增 10%、年減 20%；第二季營收 521 億元，季增 3%、年減 17%；上半年營收 1026 億元，年減 17%。&lt;/p&gt;\n\n&lt;p&gt;佳世達說明，在各項事業表現方面，第二季各項事業幾乎都較第一季增長，其中高附加價值事業的醫療、智慧解決方案也較去年同期成長，醫院營運表現健康。&lt;/p&gt;\n\n&lt;p&gt;展望下半年，佳世達認為，雖然資訊產品不確性仍高，但庫存已回到正常，網通短期則受到庫存去化影響，不過，醫療、智慧解決方案成長動能仍佳，下半年可望優於上半年。&lt;/p&gt;\n\n&lt;p&gt;此外，佳世達集團上月參加的台北國際電腦展 COMPUTEX 業績持續發酵，基三豐旗下華鋒科技看準寵物高齡化趨勢，也將在 7 日登場的台北寵物用品展推出寵物居家照護產品。&lt;/p&gt;\n',
     'hasCoverPhoto': 1,
     'isCategoryHeadline': 1,
     'isIndex': 1,
     'newsId': 5240218,
@@ -83,30 +85,31 @@
 
         if self.version == 1:
             url = f'https://api.cnyes.com/media/api/v1/newslist/category/tw_stock?startAt={int(self.datetime_start.timestamp())}&endAt={int(self.datetime_end.timestamp())}&limit=100'
         else:
             url = f'https://news.cnyes.com/api/v3/news/category/tw_stock?startAt={int(self.datetime_start.timestamp())}' \
                   f'&endAt={int(self.datetime_end.timestamp())}&limit=100'
         logger.info(url)
-        res = requests.get(url, headers)
+        res = requests.get(url, headers=headers)
         ret = json.loads(res.text)
 
         list_news = []
         for x in ret['items']['data']:
             # print(x)
             # for key in x:
             #     print(key)
+            logger.info(x)
             title = x['title']
             str_dt = datetime.datetime.fromtimestamp(x['publishAt'])
             categoryName = x.get('categoryName', '')
             if categoryName != '台股新聞':
                 continue
             stock = ' '.join(x.get('stock', ''))
 
-            # logger.info(f'{str_dt} {title}')
+            logger.info(f'{str_dt} {title}')
             list_news.append(f'{str_dt} {title} [{categoryName}] {stock}')
 
         return list_news
 
     def fetch_new(self):
 
         self.version = 1
```

### Comparing `mypylib-0.1.80/mypylib/crypto.py` & `mypylib-0.1.81/mypylib/crypto.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/finmind.py` & `mypylib-0.1.81/mypylib/finmind.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/libexcel.py` & `mypylib-0.1.81/mypylib/libexcel.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/mvp.py` & `mypylib-0.1.81/mypylib/mvp.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/mytest.py` & `mypylib-0.1.81/mypylib/mytest.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/option_test.py` & `mypylib-0.1.81/mypylib/option_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/shioaji_history_ticks.py` & `mypylib-0.1.81/mypylib/shioaji_history_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/shioaji_kline.py` & `mypylib-0.1.81/mypylib/shioaji_kline.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/shioaji_ticks.py` & `mypylib-0.1.81/mypylib/shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/sjtools.py` & `mypylib-0.1.81/mypylib/sjtools.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/tLineNotify.py` & `mypylib-0.1.81/mypylib/tLineNotify.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/ti.py` & `mypylib-0.1.81/mypylib/ti.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/tmpDevelopment/warrant_test.py` & `mypylib-0.1.81/mypylib/tmpDevelopment/warrant_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/tplaysound.py` & `mypylib-0.1.81/mypylib/tplaysound.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/tredis.py` & `mypylib-0.1.81/mypylib/tredis.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib/warrant.py` & `mypylib-0.1.81/mypylib/warrant.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/mypylib.egg-info/SOURCES.txt` & `mypylib-0.1.81/mypylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.80/setup.py` & `mypylib-0.1.81/setup.py`

 * *Files identical despite different names*

