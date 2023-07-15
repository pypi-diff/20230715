# Comparing `tmp/pyLegendSS-0.7.tar.gz` & `tmp/pyLegendSS-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyLegendSS-0.7.tar", last modified: Wed Jul 12 18:28:24 2023, max compression
+gzip compressed data, was "pyLegendSS-0.8.tar", last modified: Sat Jul 15 12:47:58 2023, max compression
```

## Comparing `pyLegendSS-0.7.tar` & `pyLegendSS-0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:28:24.458551 pyLegendSS-0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 18:28:11.000000 pyLegendSS-0.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:28:24.454551 pyLegendSS-0.7/LegendSS/
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-12 18:28:11.000000 pyLegendSS-0.7/LegendSS/Data.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:28:11.000000 pyLegendSS-0.7/LegendSS/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10432 2023-07-12 18:28:11.000000 pyLegendSS-0.7/LegendSS/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-12 18:28:24.458551 pyLegendSS-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 18:28:11.000000 pyLegendSS-0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 18:28:24.458551 pyLegendSS-0.7/pyLegendSS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-12 18:28:24.000000 pyLegendSS-0.7/pyLegendSS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-12 18:28:24.000000 pyLegendSS-0.7/pyLegendSS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 18:28:24.000000 pyLegendSS-0.7/pyLegendSS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-12 18:28:24.000000 pyLegendSS-0.7/pyLegendSS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 18:28:24.000000 pyLegendSS-0.7/pyLegendSS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 18:28:24.458551 pyLegendSS-0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-12 18:28:11.000000 pyLegendSS-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:47:58.715787 pyLegendSS-0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 12:47:45.000000 pyLegendSS-0.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:47:58.711787 pyLegendSS-0.8/LegendSS/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-15 12:47:45.000000 pyLegendSS-0.8/LegendSS/Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:47:45.000000 pyLegendSS-0.8/LegendSS/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10371 2023-07-15 12:47:45.000000 pyLegendSS-0.8/LegendSS/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-15 12:47:58.715787 pyLegendSS-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-15 12:47:45.000000 pyLegendSS-0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 12:47:58.715787 pyLegendSS-0.8/pyLegendSS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-15 12:47:58.000000 pyLegendSS-0.8/pyLegendSS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-15 12:47:58.000000 pyLegendSS-0.8/pyLegendSS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 12:47:58.000000 pyLegendSS-0.8/pyLegendSS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-15 12:47:58.000000 pyLegendSS-0.8/pyLegendSS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 12:47:58.000000 pyLegendSS-0.8/pyLegendSS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 12:47:58.715787 pyLegendSS-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-15 12:47:45.000000 pyLegendSS-0.8/setup.py
```

### Comparing `pyLegendSS-0.7/LICENSE` & `pyLegendSS-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyLegendSS-0.7/LegendSS/Data.py` & `pyLegendSS-0.8/LegendSS/Data.py`

 * *Files identical despite different names*

### Comparing `pyLegendSS-0.7/LegendSS/generate.py` & `pyLegendSS-0.8/LegendSS/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     PasswordHashInvalid as PasswordHashInvalid1,
     SessionPasswordNeeded as SessionPasswordNeeded1)
 
 ERROR_MESSAGE = "{}\n\nSomething Error in Session Generator Bot\nReport it To @LegendBot_Owner\n          ©@TeamLegendXD"
 
 
 async def generate_session(
-    bot: Client, msg: Message, telethon=False, hellbot=True, old_pyro: bool = False
+    bot: Client, msg: Message, telethon=False, hellbot=False, old_pyro: bool = False
 ):
     if telethon:
         ty = "Telethon"
     elif hellbot:
         ty = "HellBot"
     else:
         ty = "Pyrogram"
@@ -199,16 +199,15 @@
             )
     try:
         await client.join_chat("@LegendBot_OP")
     except BaseException:
         pass
     await client.disconnect()
     await phone_code_msg.reply(
-        "Successfully String  Session Has Been Generated {} \n\nPlease check your saved messages!".format(
-            "TELETHON" if telethon else "PYROGRAM"
+        "Successfully String  Session Has Been Generated \n\nPlease check your saved messages!"
         ),
         reply_markup=InlineKeyboardMarkup(Data.support_button),
     )
 
 
 
 def helltopi(text):
```

### Comparing `pyLegendSS-0.7/PKG-INFO` & `pyLegendSS-0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLegendSS
-Version: 0.7
+Version: 0.8
 Summary: This is a simple package which is used in String Generator Bot
 Home-page: https://github.com/LEGEND-AI/pyLegendSS
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyLegendSS,LegendSS
 Classifier: Framework :: AsyncIO
```

### Comparing `pyLegendSS-0.7/pyLegendSS.egg-info/PKG-INFO` & `pyLegendSS-0.8/pyLegendSS.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyLegendSS
-Version: 0.7
+Version: 0.8
 Summary: This is a simple package which is used in String Generator Bot
 Home-page: https://github.com/LEGEND-AI/pyLegendSS
 Author: LegendBoy
 Author-email: krishna045jaiswal@gmail.com
 License: GNU General Public License v3.0
 Keywords: pyLegendSS,LegendSS
 Classifier: Framework :: AsyncIO
```

### Comparing `pyLegendSS-0.7/setup.py` & `pyLegendSS-0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     sys.stderr.write( "Warning: Could not open README.md due %s\n" % error )
     
 
 setup(
     name="pyLegendSS",
     author="LegendBoy",
     author_email="krishna045jaiswal@gmail.com",
-    version="0.7",
+    version="0.8",
     description="This is a simple package which is used in String Generator Bot",
     long_description = readme_contents,
     long_description_content_type="text/markdown",
     url="https://github.com/LEGEND-AI/pyLegendSS",
     packages=find_packages(),
     license="GNU General Public License v3.0",
     include_package_data=True,
```

