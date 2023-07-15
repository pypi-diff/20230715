# Comparing `tmp/iamai-3.2.tar.gz` & `tmp/iamai-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai-3.2.tar", max compression
+gzip compressed data, was "iamai-3.2.1.tar", max compression
```

## Comparing `iamai-3.2.tar` & `iamai-3.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-07-14 12:11:24.499442 iamai-3.2/LICENSE
--rw-r--r--   0        0        0     9810 2023-07-14 12:11:24.499442 iamai-3.2/README.md
--rw-r--r--   0        0        0      543 2023-07-14 12:11:24.507443 iamai-3.2/iamai/__init__.py
--rw-r--r--   0        0        0     4432 2023-07-14 12:11:24.507443 iamai-3.2/iamai/adapter/__init__.py
--rw-r--r--   0        0        0     1211 2023-07-14 12:11:24.507443 iamai-3.2/iamai/adapter/http_server_test_adapter.py
--rw-r--r--   0        0        0     1059 2023-07-14 12:11:24.507443 iamai-3.2/iamai/adapter/test.py
--rw-r--r--   0        0        0     7955 2023-07-14 12:11:24.507443 iamai-3.2/iamai/adapter/utils.py
--rw-r--r--   0        0        0    35506 2023-07-14 12:11:24.507443 iamai-3.2/iamai/bot.py
--rw-r--r--   0        0        0     1970 2023-07-14 12:11:24.507443 iamai-3.2/iamai/config.py
--rw-r--r--   0        0        0     1907 2023-07-14 12:11:24.507443 iamai-3.2/iamai/event.py
--rw-r--r--   0        0        0     1088 2023-07-14 12:11:24.507443 iamai-3.2/iamai/exceptions.py
--rw-r--r--   0        0        0      986 2023-07-14 12:11:24.507443 iamai-3.2/iamai/log.py
--rw-r--r--   0        0        0    13843 2023-07-14 12:11:24.507443 iamai-3.2/iamai/message.py
--rw-r--r--   0        0        0     3503 2023-07-14 12:11:24.507443 iamai-3.2/iamai/plugin.py
--rw-r--r--   0        0        0     1052 2023-07-14 12:11:24.507443 iamai-3.2/iamai/typing.py
--rw-r--r--   0        0        0     5529 2023-07-14 12:11:24.507443 iamai-3.2/iamai/utils.py
--rw-r--r--   0        0        0     2446 2023-07-14 12:11:24.515443 iamai-3.2/pyproject.toml
--rw-r--r--   0        0        0    11071 1970-01-01 00:00:00.000000 iamai-3.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-15 05:23:38.785804 iamai-3.2.1/LICENSE
+-rw-r--r--   0        0        0     9810 2023-07-15 05:23:38.785804 iamai-3.2.1/README.md
+-rw-r--r--   0        0        0      543 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/__init__.py
+-rw-r--r--   0        0        0     4432 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/adapter/__init__.py
+-rw-r--r--   0        0        0     1211 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/adapter/http_server_test_adapter.py
+-rw-r--r--   0        0        0     1059 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/adapter/test.py
+-rw-r--r--   0        0        0     7955 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/adapter/utils.py
+-rw-r--r--   0        0        0    35504 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/bot.py
+-rw-r--r--   0        0        0     1970 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/config.py
+-rw-r--r--   0        0        0     1907 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/event.py
+-rw-r--r--   0        0        0     1088 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/exceptions.py
+-rw-r--r--   0        0        0      986 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/log.py
+-rw-r--r--   0        0        0    13843 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/message.py
+-rw-r--r--   0        0        0     3503 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/plugin.py
+-rw-r--r--   0        0        0     1052 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/typing.py
+-rw-r--r--   0        0        0     5529 2023-07-15 05:23:38.793804 iamai-3.2.1/iamai/utils.py
+-rw-r--r--   0        0        0     2601 2023-07-15 05:23:38.797804 iamai-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0    11101 1970-01-01 00:00:00.000000 iamai-3.2.1/PKG-INFO
```

### Comparing `iamai-3.2/LICENSE` & `iamai-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iamai-3.2/README.md` & `iamai-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `iamai-3.2/iamai/__init__.py` & `iamai-3.2.1/iamai/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2/iamai/adapter/__init__.py` & `iamai-3.2.1/iamai/adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2/iamai/adapter/http_server_test_adapter.py` & `iamai-3.2.1/iamai/adapter/http_server_test_adapter.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2/iamai/adapter/test.py` & `iamai-3.2.1/iamai/adapter/test.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2/iamai/adapter/utils.py` & `iamai-3.2.1/iamai/adapter/utils.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2/iamai/bot.py` & `iamai-3.2.1/iamai/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -498,15 +498,15 @@
                     e,
                     self.config.bot.log.verbose_exception,
                 )
 
         for _hook_func in self._event_postprocessor_hooks:
             await _hook_func(current_event)
 
-        logger.warning("Event Finished")
+        logger.debug("Event Finished")
 
     async def get(
         self,
         func: Optional[Callable[[T_Event], Union[bool, Awaitable[bool]]]] = None,
         *,
         max_try_times: Optional[int] = None,
         timeout: Optional[Union[int, float]] = None,
```

### Comparing `iamai-3.2/iamai/config.py` & `iamai-3.2.1/iamai/config.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2/iamai/event.py` & `iamai-3.2.1/iamai/event.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2/iamai/exceptions.py` & `iamai-3.2.1/iamai/exceptions.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2/iamai/log.py` & `iamai-3.2.1/iamai/log.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2/iamai/message.py` & `iamai-3.2.1/iamai/message.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2/iamai/plugin.py` & `iamai-3.2.1/iamai/plugin.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2/iamai/typing.py` & `iamai-3.2.1/iamai/typing.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2/iamai/utils.py` & `iamai-3.2.1/iamai/utils.py`

 * *Files identical despite different names*

### Comparing `iamai-3.2/pyproject.toml` & `iamai-3.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "iamai"
-version = "3.2"
+version = "3.2.1"
 description = "bot framework."
-authors = ["简律纯 <admin@jyunko.cn>"]
+authors = ["简律纯 <i@jyunko.cn>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://retrofor.space/"
 repository = "https://github.com/retrofor/iamai"
 documentation = "https://iamai.retrofor.space/"
-keywords = ["bot", "qq", "qqbot", "mirai", "coolq"]
+keywords = ["bot", "qq", "qqbot", "mirai", "coolq", "kook", "go-cqhttp", "dingtalk", "console"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Library",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3"
 ]
@@ -24,14 +24,15 @@
 aiohttp = "^3.8.0"
 loguru = ">=0.6,<0.8"
 typing-extensions = "^4.4.0"
 
 [tool.poetry.group.dev.dependencies]
 watchfiles = "^0.18.0"
 sophia-doc = "^0.1.0"
+iamai-adapter-console = { path = "./packages/iamai-adapter-console", develop = true }
 iamai-adapter-kook = { path = "./packages/iamai-adapter-kook", develop = true }
 iamai-adapter-cqhttp = { path = "./packages/iamai-adapter-cqhttp", develop = true }
 iamai-adapter-dingtalk = { path = "./packages/iamai-adapter-dingtalk", develop = true }
 iamai-adapter-apscheduler = { path = "./packages/iamai-adapter-apscheduler", develop = true }
 black = "^23.1.0"
 isort = "^5.12.0"
 pre-commit = "^3.1.0"
@@ -40,14 +41,15 @@
 [tool.poetry.extras]
 kook = ["iamai-adapter-kook"]
 cqhttp = ["iamai-adapter-cqhttp"]
 dingtalk = ["iamai-adapter-dingtalk"]
 apscheduler = ["iamai-adapter-apscheduler"]
 hot_reload = ["watchfiles"]
 all = [
+  "iamai-adapter-console",
   "iamai-adapter-kook",
   "iamai-adapter-cqhttp",
   "iamai-adapter-dingtalk",
   "iamai-adapter-apscheduler",
   "watchfiles",
 ]
```

### Comparing `iamai-3.2/PKG-INFO` & `iamai-3.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: iamai
-Version: 3.2
+Version: 3.2.1
 Summary: bot framework.
 Home-page: https://retrofor.space/
 License: MIT
-Keywords: bot,qq,qqbot,mirai,coolq
+Keywords: bot,qq,qqbot,mirai,coolq,kook,go-cqhttp,dingtalk,console
 Author: 简律纯
-Author-email: admin@jyunko.cn
+Author-email: i@jyunko.cn
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Library
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: iamai Version: 3.2 Summary: bot framework. Home-
-page: https://retrofor.space/ License: MIT Keywords: bot,qq,qqbot,mirai,coolq
-Author: ç®å¾çº¯ Author-email: admin@jyunko.cn Requires-Python: >=3.8,<4.0
-Classifier: Development Status :: 5 - Production/Stable Classifier: Framework
-:: Robot Framework Classifier: Framework :: Robot Framework :: Library
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Provides-Extra: all Provides-Extra:
-apscheduler Provides-Extra: cqhttp Provides-Extra: dingtalk Provides-Extra:
-hot-reload Provides-Extra: kook Requires-Dist: aiohttp (>=3.8.0,<4.0.0)
-Requires-Dist: loguru (>=0.6,<0.8) Requires-Dist: pydantic (>=1.10.0,<2.0.0)
-Requires-Dist: tomli (>=2.0.0,<3.0.0) ; python_version < "3.11" Requires-Dist:
-typing-extensions (>=4.4.0,<5.0.0) Project-URL: Documentation, https://
+Metadata-Version: 2.1 Name: iamai Version: 3.2.1 Summary: bot framework. Home-
+page: https://retrofor.space/ License: MIT Keywords:
+bot,qq,qqbot,mirai,coolq,kook,go-cqhttp,dingtalk,console Author: ç®å¾çº¯
+Author-email: i@jyunko.cn Requires-Python: >=3.8,<4.0 Classifier: Development
+Status :: 5 - Production/Stable Classifier: Framework :: Robot Framework
+Classifier: Framework :: Robot Framework :: Library Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Provides-Extra: all Provides-Extra: apscheduler
+Provides-Extra: cqhttp Provides-Extra: dingtalk Provides-Extra: hot-reload
+Provides-Extra: kook Requires-Dist: aiohttp (>=3.8.0,<4.0.0) Requires-Dist:
+loguru (>=0.6,<0.8) Requires-Dist: pydantic (>=1.10.0,<2.0.0) Requires-Dist:
+tomli (>=2.0.0,<3.0.0) ; python_version < "3.11" Requires-Dist: typing-
+extensions (>=4.4.0,<5.0.0) Project-URL: Documentation, https://
 iamai.retrofor.space/ Project-URL: Repository, https://github.com/retrofor/
 iamai Description-Content-Type: text/markdown
                    [https://iamai.retrofor.space/retro.png]
                               ****** iamai ******
                                [Discord] [QQç¾¤]
                       ç®ä½ä¸­æ ã«ã»ãã íêµ­ì´
             Cross-platform robot framework, mainly used for ML/DL.
```

