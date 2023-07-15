# Comparing `tmp/reprim-0.1.0.tar.gz` & `tmp/reprim-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprim-0.1.0.tar", last modified: Sat Jul 15 15:24:48 2023, max compression
+gzip compressed data, was "reprim-0.1.1.tar", last modified: Sat Jul 15 17:25:39 2023, max compression
```

## Comparing `reprim-0.1.0.tar` & `reprim-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 15:24:48.270657 reprim-0.1.0/
--rw-rw-rw-   0        0        0      683 2023-07-15 15:24:48.270657 reprim-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-07-06 00:02:04.000000 reprim-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 15:24:48.242732 reprim-0.1.0/RePrIm/
--rw-rw-rw-   0        0        0       22 2023-07-06 00:02:04.000000 reprim-0.1.0/RePrIm/__init__.py
--rw-rw-rw-   0        0        0    20268 2023-07-15 15:08:50.000000 reprim-0.1.0/RePrIm/reprim.py
-drwxrwxrwx   0        0        0        0 2023-07-15 15:24:48.250712 reprim-0.1.0/RePrIm/util/
--rw-rw-rw-   0        0        0     1959 2023-07-09 09:27:17.000000 reprim-0.1.0/RePrIm/util/hardware_monitor.py
--rw-rw-rw-   0        0        0     3125 2023-07-15 15:22:07.000000 reprim-0.1.0/RePrIm/util/process.py
--rw-rw-rw-   0        0        0     2268 2023-07-08 17:33:17.000000 reprim-0.1.0/RePrIm/util/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-15 15:24:48.269660 reprim-0.1.0/reprim.egg-info/
--rw-rw-rw-   0        0        0      683 2023-07-15 15:24:48.000000 reprim-0.1.0/reprim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-07-15 15:24:48.000000 reprim-0.1.0/reprim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 15:24:48.000000 reprim-0.1.0/reprim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-15 15:24:48.000000 reprim-0.1.0/reprim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-15 15:24:48.000000 reprim-0.1.0/reprim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 15:24:48.271655 reprim-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      709 2023-07-15 15:24:21.000000 reprim-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 17:25:39.516977 reprim-0.1.1/
+-rw-rw-rw-   0        0        0      683 2023-07-15 17:25:39.516977 reprim-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-07-06 00:02:04.000000 reprim-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 17:25:39.492043 reprim-0.1.1/RePrIm/
+-rw-rw-rw-   0        0        0       22 2023-07-06 00:02:04.000000 reprim-0.1.1/RePrIm/__init__.py
+-rw-rw-rw-   0        0        0    20390 2023-07-15 17:24:46.000000 reprim-0.1.1/RePrIm/reprim.py
+drwxrwxrwx   0        0        0        0 2023-07-15 17:25:39.495036 reprim-0.1.1/RePrIm/util/
+-rw-rw-rw-   0        0        0     1959 2023-07-09 09:27:17.000000 reprim-0.1.1/RePrIm/util/hardware_monitor.py
+-rw-rw-rw-   0        0        0     3125 2023-07-15 15:22:07.000000 reprim-0.1.1/RePrIm/util/process.py
+-rw-rw-rw-   0        0        0     2268 2023-07-08 17:33:17.000000 reprim-0.1.1/RePrIm/util/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-15 17:25:39.515980 reprim-0.1.1/reprim.egg-info/
+-rw-rw-rw-   0        0        0      683 2023-07-15 17:25:39.000000 reprim-0.1.1/reprim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-07-15 17:25:39.000000 reprim-0.1.1/reprim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 17:25:39.000000 reprim-0.1.1/reprim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-15 17:25:39.000000 reprim-0.1.1/reprim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-15 17:25:39.000000 reprim-0.1.1/reprim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 17:25:39.516977 reprim-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      709 2023-07-15 15:34:51.000000 reprim-0.1.1/setup.py
```

### Comparing `reprim-0.1.0/PKG-INFO` & `reprim-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprim
-Version: 0.1.0
+Version: 0.1.1
 Summary: for questions write me in Telegram (@IDieLast)
 Home-page: https://github.com/GGergy/RePrIm/
 Author: GGergy
 Author-email: gergy2k07@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### Comparing `reprim-0.1.0/RePrIm/reprim.py` & `reprim-0.1.1/RePrIm/reprim.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import shutil
 import time
 import telebot.apihelper
 from io import BytesIO
 from .util import tools, process
 from telebot import types
 
+print("starting RePrIm host util")
+
 tools.init()
 bot = tools.load_bot()
-print("using dev version...")
 
 
 def access(message):
     if message.chat.id != tools.data['host']:
         bot.send_message(chat_id=message.chat.id, text='you have no access to this RPC')
     else:
         return True
@@ -358,15 +359,16 @@
     bot.answer_callback_query(callback_query_id=call.id, text='building zip file...')
     path = tools.unlex(json.loads(call.data)['data'])
     chat_id = call.message.chat.id
     archive = shutil.make_archive('buff', 'zip', path)
     with open(archive, mode='rb') as rf:
         data = BytesIO(rf.read())
         data.name = f'{path.split("//")[-1]}.zip'
-        if data.name == 'zip':
+        print(data.name)
+        if data.name == '..zip':
             data.name = 'source.zip'
     os.remove('buff.zip')
     markup = types.InlineKeyboardMarkup()
     markup.row(types.InlineKeyboardButton(text='❌', callback_data='{"handler": "close"}'))
     send(blob=data, chat_id=chat_id, mk=markup)
 
 
@@ -402,11 +404,12 @@
 @bot.message_handler(content_types=['text', 'audio', 'photo', 'video', 'media', 'file', 'voice', 'video_note'])
 def deleter(message):
     bot.clear_step_handler_by_chat_id(chat_id=message.chat.id)
     bot.delete_message(message.chat.id, message.id)
 
 
 try:
+    print("successfully started RePrIm 0.1.1 by GGergy (https://github.com/GGergy/)")
     print('host created, dont shutdown your PC')
     bot.infinity_polling()
 except:
     tools.reset_token()
```

### Comparing `reprim-0.1.0/RePrIm/util/hardware_monitor.py` & `reprim-0.1.1/RePrIm/util/hardware_monitor.py`

 * *Files identical despite different names*

### Comparing `reprim-0.1.0/RePrIm/util/process.py` & `reprim-0.1.1/RePrIm/util/process.py`

 * *Files identical despite different names*

### Comparing `reprim-0.1.0/RePrIm/util/tools.py` & `reprim-0.1.1/RePrIm/util/tools.py`

 * *Files identical despite different names*

### Comparing `reprim-0.1.0/reprim.egg-info/PKG-INFO` & `reprim-0.1.1/reprim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprim
-Version: 0.1.0
+Version: 0.1.1
 Summary: for questions write me in Telegram (@IDieLast)
 Home-page: https://github.com/GGergy/RePrIm/
 Author: GGergy
 Author-email: gergy2k07@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### Comparing `reprim-0.1.0/setup.py` & `reprim-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = readme_file.read()
 
 requirements = ["pytelegrambotapi", "pythonnet"]
 
 
 setup(
     name="reprim",
-    version="0.1.0",
+    version="0.1.1",
     author="GGergy",
     author_email="gergy2k07@gmail.com",
     description="for questions write me in Telegram (@IDieLast)",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/GGergy/RePrIm/",
     packages=['RePrIm', 'RePrIm/util'],
```

