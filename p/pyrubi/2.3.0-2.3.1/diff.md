# Comparing `tmp/pyrubi-2.3.0.tar.gz` & `tmp/pyrubi-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrubi-2.3.0.tar", last modified: Fri Jun 30 22:22:24 2023, max compression
+gzip compressed data, was "pyrubi-2.3.1.tar", last modified: Sat Jul 15 18:42:36 2023, max compression
```

## Comparing `pyrubi-2.3.0.tar` & `pyrubi-2.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.030258 pyrubi-2.3.0/
--rw-rw-rw-   0        0        0     2255 2023-06-30 22:22:24.030258 pyrubi-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1409 2023-06-30 22:19:53.000000 pyrubi-2.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 22:22:23.997611 pyrubi-2.3.0/pyrubi/
--rw-rw-rw-   0        0        0      205 2023-06-30 20:13:28.000000 pyrubi-2.3.0/pyrubi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.014606 pyrubi-2.3.0/pyrubi/cryption/
--rw-rw-rw-   0        0        0     3932 2023-06-27 09:26:51.000000 pyrubi-2.3.0/pyrubi/cryption/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.015605 pyrubi-2.3.0/pyrubi/handler/
--rw-rw-rw-   0        0        0     1142 2023-06-27 09:30:29.000000 pyrubi-2.3.0/pyrubi/handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.016606 pyrubi-2.3.0/pyrubi/maker/
--rw-rw-rw-   0        0        0     3399 2023-06-27 13:42:47.000000 pyrubi-2.3.0/pyrubi/maker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.024256 pyrubi-2.3.0/pyrubi/message/
--rw-rw-rw-   0        0        0     3863 2023-06-30 22:04:18.000000 pyrubi-2.3.0/pyrubi/message/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.025259 pyrubi-2.3.0/pyrubi/methods/
--rw-rw-rw-   0        0        0    46199 2023-06-30 21:53:00.000000 pyrubi-2.3.0/pyrubi/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.027258 pyrubi-2.3.0/pyrubi/servers/
--rw-rw-rw-   0        0        0      357 2023-06-27 08:13:23.000000 pyrubi-2.3.0/pyrubi/servers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.028258 pyrubi-2.3.0/pyrubi/sessions/
--rw-rw-rw-   0        0        0      501 2023-06-30 20:18:21.000000 pyrubi-2.3.0/pyrubi/sessions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.029260 pyrubi-2.3.0/pyrubi/tools/
--rw-rw-rw-   0        0        0     7297 2023-06-26 11:48:21.000000 pyrubi-2.3.0/pyrubi/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 22:22:24.013605 pyrubi-2.3.0/pyrubi.egg-info/
--rw-rw-rw-   0        0        0     2255 2023-06-30 22:22:23.000000 pyrubi-2.3.0/pyrubi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-06-30 22:22:23.000000 pyrubi-2.3.0/pyrubi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 22:22:23.000000 pyrubi-2.3.0/pyrubi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-06-30 22:22:23.000000 pyrubi-2.3.0/pyrubi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-30 22:22:23.000000 pyrubi-2.3.0/pyrubi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-30 22:22:24.030258 pyrubi-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1113 2023-06-30 22:21:10.000000 pyrubi-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:42:36.967073 pyrubi-2.3.1/
+-rw-rw-rw-   0        0        0     2255 2023-07-15 18:42:36.967073 pyrubi-2.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1409 2023-07-15 18:41:12.000000 pyrubi-2.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 18:42:36.939082 pyrubi-2.3.1/pyrubi/
+-rw-rw-rw-   0        0        0      179 2023-07-15 18:41:28.000000 pyrubi-2.3.1/pyrubi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:42:36.958077 pyrubi-2.3.1/pyrubi/cryption/
+-rw-rw-rw-   0        0        0     3932 2023-06-27 09:26:51.000000 pyrubi-2.3.1/pyrubi/cryption/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:42:36.960077 pyrubi-2.3.1/pyrubi/handler/
+-rw-rw-rw-   0        0        0     1405 2023-07-15 17:28:24.000000 pyrubi-2.3.1/pyrubi/handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:42:36.961075 pyrubi-2.3.1/pyrubi/maker/
+-rw-rw-rw-   0        0        0     3399 2023-06-27 13:42:47.000000 pyrubi-2.3.1/pyrubi/maker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:42:36.962075 pyrubi-2.3.1/pyrubi/message/
+-rw-rw-rw-   0        0        0     3863 2023-06-30 22:04:18.000000 pyrubi-2.3.1/pyrubi/message/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:42:36.963075 pyrubi-2.3.1/pyrubi/methods/
+-rw-rw-rw-   0        0        0    46199 2023-06-30 21:53:00.000000 pyrubi-2.3.1/pyrubi/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:42:36.964074 pyrubi-2.3.1/pyrubi/servers/
+-rw-rw-rw-   0        0        0      357 2023-06-27 08:13:23.000000 pyrubi-2.3.1/pyrubi/servers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:42:36.965073 pyrubi-2.3.1/pyrubi/sessions/
+-rw-rw-rw-   0        0        0      501 2023-06-30 20:18:21.000000 pyrubi-2.3.1/pyrubi/sessions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:42:36.966074 pyrubi-2.3.1/pyrubi/tools/
+-rw-rw-rw-   0        0        0     7297 2023-06-26 11:48:21.000000 pyrubi-2.3.1/pyrubi/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:42:36.956076 pyrubi-2.3.1/pyrubi.egg-info/
+-rw-rw-rw-   0        0        0     2255 2023-07-15 18:42:36.000000 pyrubi-2.3.1/pyrubi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-07-15 18:42:36.000000 pyrubi-2.3.1/pyrubi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 18:42:36.000000 pyrubi-2.3.1/pyrubi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-07-15 18:42:36.000000 pyrubi-2.3.1/pyrubi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-15 18:42:36.000000 pyrubi-2.3.1/pyrubi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 18:42:36.968072 pyrubi-2.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1113 2023-07-15 18:41:18.000000 pyrubi-2.3.1/setup.py
```

### Comparing `pyrubi-2.3.0/PKG-INFO` & `pyrubi-2.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrubi
-Version: 2.3.0
+Version: 2.3.1
 Summary: This is a powerful and easy library for building self Bots in Rubika
 Home-page: https://github.com/AliGanji1/pyrubi
 Author: Ali Ganji zadeh
 Author-email: ali.ganji.za@gmail.com
 Keywords: rubika,rubika-bot,pyrubi,rubino,rubika.ir,pyrubika
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -13,20 +13,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 
-<h1>Pyrubi 2.3.0</h1>
+<h1>Pyrubi 2.3.1</h1>
 
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
 
 <p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.3.0' width='356' class="image">
+    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.3.1' width='356' class="image">
 </p>
 
 <p align='center'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
     •
     <a href='https://rubika.ir/pyrubika'>Documents</a>
 </p>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: pyrubi Version: 2.3.0 Summary: This is a powerful
+Metadata-Version: 2.1 Name: pyrubi Version: 2.3.1 Summary: This is a powerful
 and easy library for building self Bots in Rubika Home-page: https://
 github.com/AliGanji1/pyrubi Author: Ali Ganji zadeh Author-email:
 ali.ganji.za@gmail.com Keywords: rubika,rubika-
 bot,pyrubi,rubino,rubika.ir,pyrubika Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: License :: OSI Approved :: MIT License Requires-
 Python: ~=3.6 Description-Content-Type: text/markdown
-****** Pyrubi 2.3.0 ******
+****** Pyrubi 2.3.1 ******
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
-                            [Pyrubi Library 2.3.0]
+                            [Pyrubi Library 2.3.1]
                              GitHub â¢ Documents
 [![Downloads](https://static.pepy.tech/badge/pyrubi)](https://pepy.tech/
 project/pyrubi) **The Pyrubi library is compatible with version 6 of the
 Rubik's API**
 ===============================================================================
 ## Install or Update: ``` bash pip install -U pyrubi ```
 ===============================================================================
```

### Comparing `pyrubi-2.3.0/README.md` & `pyrubi-2.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-<h1>Pyrubi 2.3.0</h1>
+<h1>Pyrubi 2.3.1</h1>
 
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
 
 <p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.3.0' width='356' class="image">
+    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.3.1' width='356' class="image">
 </p>
 
 <p align='center'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
     •
     <a href='https://rubika.ir/pyrubika'>Documents</a>
 </p>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-****** Pyrubi 2.3.0 ******
+****** Pyrubi 2.3.1 ******
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
-                            [Pyrubi Library 2.3.0]
+                            [Pyrubi Library 2.3.1]
                              GitHub â¢ Documents
 [![Downloads](https://static.pepy.tech/badge/pyrubi)](https://pepy.tech/
 project/pyrubi) **The Pyrubi library is compatible with version 6 of the
 Rubik's API**
 ===============================================================================
 ## Install or Update: ``` bash pip install -U pyrubi ```
 ===============================================================================
```

### Comparing `pyrubi-2.3.0/pyrubi/cryption/__init__.py` & `pyrubi-2.3.1/pyrubi/cryption/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.3.0/pyrubi/handler/__init__.py` & `pyrubi-2.3.1/pyrubi/handler/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 from websocket import create_connection
 from json import dumps, loads
 from ..servers import get_server
 from ..cryption import cryption5
+from threading import Thread
+from time import sleep
+
 class handler:
 
     def __init__(self, auth):
         self.crypto = cryption5(auth) if auth else None
         self.auth = auth
         self.hs_data = {
             'api_version': '5',
             'auth': auth,
             'method': 'handShake'
         }
         del auth
     
     def hand_shake(self):
+        global ws
         print('connecting to the web socket...')
         ws = create_connection(get_server('socket'))
         ws.send(dumps(self.hs_data))
+        ws.recv()
+        ws.send(dumps({}))
+        Thread(target=self.keep_hand_shake_alive).start()
         print('connected !')
         while True:
             try:
                 recv = loads(ws.recv())
                 if recv != {"status":"OK", "status_det":"OK"}:
                     if recv['type'] == 'messenger':
                         yield loads(self.crypto.decrypt(recv['data_enc']))
             except:
                 ws.close()
-                del ws
-                ws = create_connection(self.server)
-                print(self.methods.get_me())
+                ws = create_connection(get_server('socket'))
                 ws.send(dumps(self.hs_data))
-                continue
+                continue
+    
+    def keep_hand_shake_alive(self):
+        while True:
+            sleep(60)
+            ws.send(dumps({}))
+            ws.recv()
```

### Comparing `pyrubi-2.3.0/pyrubi/maker/__init__.py` & `pyrubi-2.3.1/pyrubi/maker/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.3.0/pyrubi/message/__init__.py` & `pyrubi-2.3.1/pyrubi/message/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.3.0/pyrubi/methods/__init__.py` & `pyrubi-2.3.1/pyrubi/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.3.0/pyrubi/tools/__init__.py` & `pyrubi-2.3.1/pyrubi/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.3.0/pyrubi.egg-info/PKG-INFO` & `pyrubi-2.3.1/pyrubi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrubi
-Version: 2.3.0
+Version: 2.3.1
 Summary: This is a powerful and easy library for building self Bots in Rubika
 Home-page: https://github.com/AliGanji1/pyrubi
 Author: Ali Ganji zadeh
 Author-email: ali.ganji.za@gmail.com
 Keywords: rubika,rubika-bot,pyrubi,rubino,rubika.ir,pyrubika
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -13,20 +13,20 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 
-<h1>Pyrubi 2.3.0</h1>
+<h1>Pyrubi 2.3.1</h1>
 
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
 
 <p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.3.0' width='356' class="image">
+    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.3.1' width='356' class="image">
 </p>
 
 <p align='center'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
     •
     <a href='https://rubika.ir/pyrubika'>Documents</a>
 </p>
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: pyrubi Version: 2.3.0 Summary: This is a powerful
+Metadata-Version: 2.1 Name: pyrubi Version: 2.3.1 Summary: This is a powerful
 and easy library for building self Bots in Rubika Home-page: https://
 github.com/AliGanji1/pyrubi Author: Ali Ganji zadeh Author-email:
 ali.ganji.za@gmail.com Keywords: rubika,rubika-
 bot,pyrubi,rubino,rubika.ir,pyrubika Classifier: Programming Language :: Python
 :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: License :: OSI Approved :: MIT License Requires-
 Python: ~=3.6 Description-Content-Type: text/markdown
-****** Pyrubi 2.3.0 ******
+****** Pyrubi 2.3.1 ******
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
-                            [Pyrubi Library 2.3.0]
+                            [Pyrubi Library 2.3.1]
                              GitHub â¢ Documents
 [![Downloads](https://static.pepy.tech/badge/pyrubi)](https://pepy.tech/
 project/pyrubi) **The Pyrubi library is compatible with version 6 of the
 Rubik's API**
 ===============================================================================
 ## Install or Update: ``` bash pip install -U pyrubi ```
 ===============================================================================
```

### Comparing `pyrubi-2.3.0/setup.py` & `pyrubi-2.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'pyrubi',
-    version = '2.3.0',
+    version = '2.3.1',
     author='Ali Ganji zadeh',
     author_email = 'ali.ganji.za@gmail.com',
     description = 'This is a powerful and easy library for building self Bots in Rubika',
     keywords = ['rubika', 'rubika-bot', 'pyrubi', 'rubino', 'rubika.ir', 'pyrubika'],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
```

