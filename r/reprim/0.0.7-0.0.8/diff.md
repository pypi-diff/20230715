# Comparing `tmp/reprim-0.0.7.tar.gz` & `tmp/reprim-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprim-0.0.7.tar", last modified: Sat Jul 15 14:59:31 2023, max compression
+gzip compressed data, was "reprim-0.0.8.tar", last modified: Sat Jul 15 15:03:54 2023, max compression
```

## Comparing `reprim-0.0.7.tar` & `reprim-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 14:59:31.648020 reprim-0.0.7/
--rw-rw-rw-   0        0        0      683 2023-07-15 14:59:31.648020 reprim-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-07-06 00:02:04.000000 reprim-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 14:59:31.536319 reprim-0.0.7/RePrIm/
--rw-rw-rw-   0        0        0       22 2023-07-06 00:02:04.000000 reprim-0.0.7/RePrIm/__init__.py
--rw-rw-rw-   0        0        0    20237 2023-07-08 17:43:13.000000 reprim-0.0.7/RePrIm/reprim.py
-drwxrwxrwx   0        0        0        0 2023-07-15 14:59:31.630068 reprim-0.0.7/RePrIm/util/
--rw-rw-rw-   0        0        0     1959 2023-07-09 09:27:17.000000 reprim-0.0.7/RePrIm/util/hardware_monitor.py
--rw-rw-rw-   0        0        0   311808 2023-07-06 00:02:04.000000 reprim-0.0.7/RePrIm/util/lib.py
--rw-rw-rw-   0        0        0     2882 2023-07-15 14:59:13.000000 reprim-0.0.7/RePrIm/util/process.py
--rw-rw-rw-   0        0        0     2268 2023-07-08 17:33:17.000000 reprim-0.0.7/RePrIm/util/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-15 14:59:31.647023 reprim-0.0.7/reprim.egg-info/
--rw-rw-rw-   0        0        0      683 2023-07-15 14:59:31.000000 reprim-0.0.7/reprim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-07-15 14:59:31.000000 reprim-0.0.7/reprim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 14:59:31.000000 reprim-0.0.7/reprim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-15 14:59:31.000000 reprim-0.0.7/reprim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-15 14:59:31.000000 reprim-0.0.7/reprim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 14:59:31.648020 reprim-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      709 2023-07-15 14:59:30.000000 reprim-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 15:03:54.118405 reprim-0.0.8/
+-rw-rw-rw-   0        0        0      683 2023-07-15 15:03:54.118405 reprim-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-07-06 00:02:04.000000 reprim-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 15:03:54.103446 reprim-0.0.8/RePrIm/
+-rw-rw-rw-   0        0        0       22 2023-07-06 00:02:04.000000 reprim-0.0.8/RePrIm/__init__.py
+-rw-rw-rw-   0        0        0    20237 2023-07-08 17:43:13.000000 reprim-0.0.8/RePrIm/reprim.py
+drwxrwxrwx   0        0        0        0 2023-07-15 15:03:54.106438 reprim-0.0.8/RePrIm/util/
+-rw-rw-rw-   0        0        0     1959 2023-07-09 09:27:17.000000 reprim-0.0.8/RePrIm/util/hardware_monitor.py
+-rw-rw-rw-   0        0        0   311808 2023-07-06 00:02:04.000000 reprim-0.0.8/RePrIm/util/lib.py
+-rw-rw-rw-   0        0        0     2939 2023-07-15 15:03:12.000000 reprim-0.0.8/RePrIm/util/process.py
+-rw-rw-rw-   0        0        0     2268 2023-07-08 17:33:17.000000 reprim-0.0.8/RePrIm/util/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-15 15:03:54.117408 reprim-0.0.8/reprim.egg-info/
+-rw-rw-rw-   0        0        0      683 2023-07-15 15:03:54.000000 reprim-0.0.8/reprim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-07-15 15:03:54.000000 reprim-0.0.8/reprim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 15:03:54.000000 reprim-0.0.8/reprim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-15 15:03:54.000000 reprim-0.0.8/reprim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-15 15:03:54.000000 reprim-0.0.8/reprim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 15:03:54.118405 reprim-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      709 2023-07-15 15:03:39.000000 reprim-0.0.8/setup.py
```

### Comparing `reprim-0.0.7/PKG-INFO` & `reprim-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprim
-Version: 0.0.7
+Version: 0.0.8
 Summary: for questions write me in Telegram (@IDieLast)
 Home-page: https://github.com/GGergy/RePrIm/
 Author: GGergy
 Author-email: gergy2k07@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### Comparing `reprim-0.0.7/RePrIm/reprim.py` & `reprim-0.0.8/RePrIm/reprim.py`

 * *Files identical despite different names*

### Comparing `reprim-0.0.7/RePrIm/util/hardware_monitor.py` & `reprim-0.0.8/RePrIm/util/hardware_monitor.py`

 * *Files identical despite different names*

### Comparing `reprim-0.0.7/RePrIm/util/lib.py` & `reprim-0.0.8/RePrIm/util/lib.py`

 * *Files identical despite different names*

### Comparing `reprim-0.0.7/RePrIm/util/process.py` & `reprim-0.0.8/RePrIm/util/process.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,17 @@
 
     def daemon(self):
         try:
             mk = InlineKeyboardMarkup()
             mk.row(InlineKeyboardButton('communicate',
                                         callback_data=json.dumps({"handler": "communicate", "data": self.id})))
             mk.row(InlineKeyboardButton('❌', callback_data='{"handler": "close"}'))
-            while self.alive():
+            while True:
+                if not self.alive():
+                    break
                 out = self.process.stdout.readline().decode()
                 if out:
                     self.handler.send_message(chat_id=data['host'], text=f"out from {self.name}:\n{out}",
                                               reply_markup=mk)
             mk = InlineKeyboardMarkup()
             mk.row(InlineKeyboardButton('❌', callback_data='{"handler": "close"}'))
             err = self.process.stderr.read().decode()
```

### Comparing `reprim-0.0.7/RePrIm/util/tools.py` & `reprim-0.0.8/RePrIm/util/tools.py`

 * *Files identical despite different names*

### Comparing `reprim-0.0.7/reprim.egg-info/PKG-INFO` & `reprim-0.0.8/reprim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprim
-Version: 0.0.7
+Version: 0.0.8
 Summary: for questions write me in Telegram (@IDieLast)
 Home-page: https://github.com/GGergy/RePrIm/
 Author: GGergy
 Author-email: gergy2k07@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
```

### Comparing `reprim-0.0.7/setup.py` & `reprim-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readme = readme_file.read()
 
 requirements = ["pytelegrambotapi", "pythonnet"]
 
 
 setup(
     name="reprim",
-    version="0.0.7",
+    version="0.0.8",
     author="GGergy",
     author_email="gergy2k07@gmail.com",
     description="for questions write me in Telegram (@IDieLast)",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/GGergy/RePrIm/",
     packages=['RePrIm', 'RePrIm/util'],
```

