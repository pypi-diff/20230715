# Comparing `tmp/talkytrend-1.7.4.tar.gz` & `tmp/talkytrend-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytrend-1.7.4.tar", max compression
+gzip compressed data, was "talkytrend-1.8.0.tar", max compression
```

## Comparing `talkytrend-1.7.4.tar` & `talkytrend-1.8.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-13 20:43:38.458302 talkytrend-1.7.4/LICENSE
--rw-r--r--   0        0        0     3446 2023-07-13 20:43:38.458302 talkytrend-1.7.4/README.md
--rw-r--r--   0        0        0     2476 2023-07-13 20:43:39.286323 talkytrend-1.7.4/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-13 20:43:39.290323 talkytrend-1.7.4/talkytrend/__init__.py
--rw-r--r--   0        0        0      706 2023-07-13 20:43:38.458302 talkytrend-1.7.4/talkytrend/config.py
--rw-r--r--   0        0        0     2285 2023-07-13 20:43:38.458302 talkytrend-1.7.4/talkytrend/default_settings.toml
--rw-r--r--   0        0        0     7304 2023-07-13 20:43:38.458302 talkytrend-1.7.4/talkytrend/main.py
--rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 talkytrend-1.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-15 10:30:27.279826 talkytrend-1.8.0/LICENSE
+-rw-r--r--   0        0        0     3446 2023-07-15 10:30:27.279826 talkytrend-1.8.0/README.md
+-rw-r--r--   0        0        0     2476 2023-07-15 10:30:28.123837 talkytrend-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-15 10:30:28.123837 talkytrend-1.8.0/talkytrend/__init__.py
+-rw-r--r--   0        0        0      706 2023-07-15 10:30:27.279826 talkytrend-1.8.0/talkytrend/config.py
+-rw-r--r--   0        0        0     2285 2023-07-15 10:30:27.279826 talkytrend-1.8.0/talkytrend/default_settings.toml
+-rw-r--r--   0        0        0     7375 2023-07-15 10:30:27.279826 talkytrend-1.8.0/talkytrend/main.py
+-rw-r--r--   0        0        0     4470 1970-01-01 00:00:00.000000 talkytrend-1.8.0/PKG-INFO
```

### Comparing `talkytrend-1.7.4/LICENSE` & `talkytrend-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytrend-1.7.4/README.md` & `talkytrend-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `talkytrend-1.7.4/pyproject.toml` & `talkytrend-1.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "talkytrend"
-version = "1.7.4"
+version = "1.8.0"
 description = "A python package to retrieve  economic data such as Trend for any financial symbol."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["finance", "crypto", "bot","trend","economic"]
 packages = [
     {include = "talkytrend"}
```

### Comparing `talkytrend-1.7.4/talkytrend/config.py` & `talkytrend-1.8.0/talkytrend/config.py`

 * *Files identical despite different names*

### Comparing `talkytrend-1.7.4/talkytrend/default_settings.toml` & `talkytrend-1.8.0/talkytrend/default_settings.toml`

 * *Files identical despite different names*

### Comparing `talkytrend-1.7.4/talkytrend/main.py` & `talkytrend-1.8.0/talkytrend/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,18 @@
             elif analysis.summary["RECOMMENDATION"] == 'STRONG_SELL':
                 return "⏬"
             else:
                 return "▶️"
         except Exception as error:
             self.logger.error("event %s", error)
 
+
+    async def get_info(self):
+        return (f"ℹ️ {__class__.__name__} {__version__}\n")
+
     async def check_signal(self):
         signals = []
         table = PrettyTable()
         table.field_names = ["Asset","4h"]
         for asset in self.assets:
             current_signal = await self.fetch_analysis(
                 asset_id=asset["id"],
@@ -161,20 +165,23 @@
                     title = data['title']
                     link = data['link']
                     return f"📰 <a href='{link}'>{title}</a>"
         except aiohttp.ClientError as error:
             self.logger.error("feed %s", error)
             return None
 
-
     async def check_fomc(self):
         event_dates = settings.fomc_decision_date
         current_date = date.today().isoformat()
         return any(event.startswith(current_date) for event in event_dates)
-     
+
+    async def get_tv(self):
+        if self.live_tv:
+            return f"📺: {self.live_tv}"
+
     async def allow_scanning(self, enable=True):
         return bool(enable)
 
     async def scanner(self):
         while await self.allow_scanning():
             if settings.enable_events:
                 if await self.fetch_key_events() is not None:
@@ -187,10 +194,7 @@
                     yield await self.fetch_key_feed()
             if settings.enable_signals:
                 if await self.check_signal() is not None:
                     yield await self.check_signal()
 
             await asyncio.sleep(settings.scanner_frequency)
 
-
-    async def get_info(self):
-        return f"{__class__.__name__} {__version__}" + "\n" + f"📺: {__version__}"
```

### Comparing `talkytrend-1.7.4/PKG-INFO` & `talkytrend-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talkytrend
-Version: 1.7.4
+Version: 1.8.0
 Summary: A python package to retrieve  economic data such as Trend for any financial symbol.
 License: MIT
 Keywords: finance,crypto,bot,trend,economic
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: talkytrend Version: 1.7.4 Summary: A python package
+Metadata-Version: 2.1 Name: talkytrend Version: 1.8.0 Summary: A python package
 to retrieve economic data such as Trend for any financial symbol. License: MIT
 Keywords: finance,crypto,bot,trend,economic Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: aiohttp
 (>=3.8.4,<4.0.0) Requires-Dist: alphavantage_api_client (>=2.2.2,<3.0.0)
```

