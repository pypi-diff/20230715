# Comparing `tmp/anarchy_bot-23.0.3.tar.gz` & `tmp/anarchy_bot-23.0.4.tar.gz`

## Comparing `anarchy_bot-23.0.3.tar` & `anarchy_bot-23.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1527 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/build.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/changlog.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/pyrightconfig.json
--rwxr-xr-x   0        0        0     2024 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/setup.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/anarchy_bot/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/anarchy_bot/__main__.py
--rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/anarchy_bot/cb.py
--rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/anarchy_bot/chats.py
--rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/anarchy_bot/common.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/anarchy_bot/config.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/anarchy_bot/inline.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/anarchy_bot/lang.py
--rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/anarchy_bot/lists.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/anarchy_bot/main.py
--rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/anarchy_bot/msg.py
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/anarchy_bot/lang/en.yml
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/.gitignore
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/pyproject.toml
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/readme.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 anarchy_bot-23.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1527 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/build.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/changlog.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/pyrightconfig.json
+-rwxr-xr-x   0        0        0     2024 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/setup.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/__main__.py
+-rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/cb.py
+-rw-r--r--   0        0        0     4833 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/chats.py
+-rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/common.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/config.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/inline.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/lang.py
+-rw-r--r--   0        0        0    11744 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/lists.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/main.py
+-rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/msg.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/anarchy_bot/lang/en.yml
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/.gitignore
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/pyproject.toml
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/readme.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 anarchy_bot-23.0.4/PKG-INFO
```

### Comparing `anarchy_bot-23.0.3/build.py` & `anarchy_bot-23.0.4/build.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.3/setup.py` & `anarchy_bot-23.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.3/anarchy_bot/cb.py` & `anarchy_bot-23.0.4/anarchy_bot/cb.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.3/anarchy_bot/chats.py` & `anarchy_bot-23.0.4/anarchy_bot/chats.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.3/anarchy_bot/common.py` & `anarchy_bot-23.0.4/anarchy_bot/common.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.3/anarchy_bot/config.py` & `anarchy_bot-23.0.4/anarchy_bot/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     import tgcrypto # type: ignore
     using_tgcrypto = True
 except Exception:
     using_tgcrypto = False
 
 
 app_name = 'anarchy_bot'
-app_version = '23.0.3'
+app_version = '23.0.4'
 c = rich.console.Console()
 c.log(f'imported [deep_sky_blue1]{__file__}')
 app_path = Path(
     __file__
 ).parent.parent.resolve()
 src_path = app_path / app_name
 data_path = app_path / f'{app_name}_data'
```

### Comparing `anarchy_bot-23.0.3/anarchy_bot/inline.py` & `anarchy_bot-23.0.4/anarchy_bot/inline.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.3/anarchy_bot/lang.py` & `anarchy_bot-23.0.4/anarchy_bot/lang.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.3/anarchy_bot/lists.py` & `anarchy_bot-23.0.4/anarchy_bot/lists.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.3/anarchy_bot/main.py` & `anarchy_bot-23.0.4/anarchy_bot/main.py`

 * *Files identical despite different names*

### Comparing `anarchy_bot-23.0.3/anarchy_bot/msg.py` & `anarchy_bot-23.0.4/anarchy_bot/msg.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,16 @@
 
 
 async def help_msg(
     client: Client,
     msg: Message,
 ):
     await msg.reply(
-        **get_main_message(msg)
+        **get_main_message(msg),
+        disable_web_page_preview = True,
     )
 
 
 async def becomeadmin(
     client: Client,
     msg: Message,
 ):
```

### Comparing `anarchy_bot-23.0.3/anarchy_bot/lang/en.yml` & `anarchy_bot-23.0.4/anarchy_bot/lang/en.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 help_msg: |
   """
-  wellcome to @gmanka's anarchy bot
+  welcome to @gmanka's anarchy bot
   
   /h | /help - get this command
   /becomeadmin {title} - makes you an admin with selected title
 
   admin commands:
   /setlogs - set this chat as logs chat
```

### Comparing `anarchy_bot-23.0.3/pyproject.toml` & `anarchy_bot-23.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "hatchling",]
 build-backend = "hatchling.build"
 
 [project]
 dependencies = [ "gmanka_yml==23.0.*", "pyrogram==2.0.*", "tgcrypto==1.2.*", "uvloop==0.17.*", "rich==13.4.*",]
 name = "anarchy_bot"
-version = "23.0.3"
+version = "23.0.4"
 description = "telegram bot that can add users to minecraft whitelist"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [ "Programming Language :: Python :: 3", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "gmanka"
 email = "gmankab@gmail.com"
```

### Comparing `anarchy_bot-23.0.3/readme.md` & `anarchy_bot-23.0.4/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ## run
 
 ```bash
 pythom -m anarchy_bot
 ```
 
-## translete to your language
+## translate to your language
 
 - fork repo
 - go to [anarchy_bot/lang](https://github.com/gmankab/saltomaru_connect_tg/tree/main/saltomaru_connect_tg/lang)
 - duplicate `en.yml` file
 - rename it to something like `ru.yml`
 - edit file
 - make pull request
```

### Comparing `anarchy_bot-23.0.3/PKG-INFO` & `anarchy_bot-23.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anarchy_bot
-Version: 23.0.3
+Version: 23.0.4
 Summary: telegram bot that can add users to minecraft whitelist
 Project-URL: Documentation, https://t.me/gmanka
 Project-URL: Bug Tracker, https://t.me/gmanka
 Project-URL: Homepage, https://t.me/gmanka
 Author-email: gmanka <gmankab@gmail.com>
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -28,15 +28,15 @@
 
 ## run
 
 ```bash
 pythom -m anarchy_bot
 ```
 
-## translete to your language
+## translate to your language
 
 - fork repo
 - go to [anarchy_bot/lang](https://github.com/gmankab/saltomaru_connect_tg/tree/main/saltomaru_connect_tg/lang)
 - duplicate `en.yml` file
 - rename it to something like `ru.yml`
 - edit file
 - make pull request
```

