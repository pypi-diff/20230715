# Comparing `tmp/unigui-1.8.1.tar.gz` & `tmp/unigui-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.8.1.tar", last modified: Thu Jul 13 23:20:16 2023, max compression
+gzip compressed data, was "dist/unigui-1.8.2.tar", last modified: Fri Jul 14 23:31:00 2023, max compression
```

## Comparing `unigui-1.8.1.tar` & `unigui-1.8.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 23:20:16.000000 unigui-1.8.1/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 23:20:16.000000 unigui-1.8.1/unigui/
--rw-rw-r--   0 george    (1000) george    (1000)     8633 2023-07-12 21:13:45.000000 unigui-1.8.1/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)     3344 2023-07-13 22:22:30.000000 unigui-1.8.1/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)       99 2023-07-11 08:13:29.000000 unigui-1.8.1/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     2449 2023-07-12 21:10:40.000000 unigui-1.8.1/unigui/utils.py
--rw-rw-r--   0 george    (1000) george    (1000)     9567 2023-07-13 22:25:57.000000 unigui-1.8.1/unigui/user.py
--rw-rw-r--   0 george    (1000) george    (1000)     4277 2023-07-13 23:09:22.000000 unigui-1.8.1/unigui/reloader.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 23:20:16.000000 unigui-1.8.1/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 23:20:16.000000 unigui-1.8.1/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/css/295.f0f63b8f.css
--rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/css/vendor.49a52e8f.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 23:20:16.000000 unigui-1.8.1/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 23:20:16.000000 unigui-1.8.1/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 23:20:16.000000 unigui-1.8.1/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/js/app.9384942b.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)    44706 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/js/295.e2b7be53.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/js/vendor.3e8714c2.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-13 23:16:36.000000 unigui-1.8.1/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.8.1/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      600 2023-07-13 23:18:48.000000 unigui-1.8.1/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    18989 2023-07-13 23:20:16.000000 unigui-1.8.1/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-13 23:20:16.000000 unigui-1.8.1/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    18684 2023-07-12 08:54:15.000000 unigui-1.8.1/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.8.1/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-13 23:20:16.000000 unigui-1.8.1/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       30 2023-07-13 23:20:15.000000 unigui-1.8.1/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-13 23:20:15.000000 unigui-1.8.1/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    18989 2023-07-13 23:20:15.000000 unigui-1.8.1/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.8.1/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1221 2023-07-13 23:20:15.000000 unigui-1.8.1/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-13 23:20:15.000000 unigui-1.8.1/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-14 23:31:00.000000 unigui-1.8.2/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui/
+-rw-rw-r--   0 george    (1000) george    (1000)     8633 2023-07-12 21:13:45.000000 unigui-1.8.2/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3362 2023-07-14 23:14:58.000000 unigui-1.8.2/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)      100 2023-07-14 22:20:13.000000 unigui-1.8.2/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     2881 2023-07-14 19:50:43.000000 unigui-1.8.2/unigui/utils.py
+-rw-rw-r--   0 george    (1000) george    (1000)     4564 2023-07-14 22:55:02.000000 unigui-1.8.2/unigui/reloader.py
+-rw-rw-r--   0 george    (1000) george    (1000)     9555 2023-07-14 22:58:25.000000 unigui-1.8.2/unigui/users.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/css/423.a6a82bd4.css
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/css/vendor.49a52e8f.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)    44594 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/js/423.0ad6769b.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/js/app.eb412190.js
+-rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/js/vendor.e1e2597e.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-14 23:29:39.000000 unigui-1.8.2/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.8.2/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      612 2023-07-14 23:07:35.000000 unigui-1.8.2/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    18989 2023-07-14 23:31:00.000000 unigui-1.8.2/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-14 23:31:00.000000 unigui-1.8.2/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    18684 2023-07-12 08:54:15.000000 unigui-1.8.2/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.8.2/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       39 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    18989 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.8.2/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1222 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-14 23:31:00.000000 unigui-1.8.2/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.8.1/unigui/guielements.py` & `unigui-1.8.2/unigui/guielements.py`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/unigui/server.py` & `unigui-1.8.2/unigui/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from aiohttp import web, WSMsgType
-from .user import *
-from config import port, pretty_print, socket_ip, socket_port, upload_dir
+from .users import *
+from config import port, pretty_print, socket_ip, upload_dir
 from pathlib import Path
 from .reloader import empty_app 
 
 async def post_handler(request):
     reader = await request.multipart()
     field = await reader.next()   
     filename = upload_path(field.filename)  
@@ -37,62 +37,61 @@
 
 async def websocket_handler(request):
     ws = web.WebSocketResponse()
     await ws.prepare(request)
     user = User.UserType()
 
     async def send(res):
-        await ws.send_str(jsonString(user.prepare_result(res)))        
-    user.send = send 
-    
-    ok = user.load()
-    
-    await ws.send_str(jsonString(user.screen if ok else empty_app)) 
+        res = jsonString(user.prepare_result(res))
+        await ws.send_str(res)   
 
-    async for msg in ws:
-        if msg.type == WSMsgType.TEXT:
-            if msg.data == 'close':
-                await ws.close()
-            else:
-                data = json.loads(msg.data)            
-                result = user.result4message(data)
-                if result:                
-                    await ws.send_str(jsonString(user.prepare_result(result)))
-        elif msg.type == WSMsgType.ERROR:
-            print('ws connection closed with exception %s' %
-                ws.exception())
+    user.send = send     
+    user.session__ = request.remote
+    ok = user.load()    
+    await ws.send_str(jsonString(user.screen if ok else empty_app)) 
 
-    print('websocket connection closed')
+    try:
+        async for msg in ws:
+            if msg.type == WSMsgType.TEXT:
+                if msg.data == 'close':
+                    await ws.close()
+                else:
+                    data = json.loads(msg.data)            
+                    result = user.result4message(data)
+                    if result:                
+                        await ws.send_str(jsonString(user.prepare_result(result)))
+            elif msg.type == WSMsgType.ERROR:
+                print('ws connection closed with exception %s' %
+                    ws.exception())
+    except:
+        type, value, traceback = sys.exc_info()
+        user.log(f'{type}: {value} \n{traceback.format_exc()}\n')
+    
     return ws       
 
-def start(appname, user_type = User, translate_path = None, http_handlers = []):
+def start(appname, user_type = User, http_handlers = []):
     
-    set_utils(appname, port, upload_dir, translate_path, socket_ip, socket_port)    
+    set_utils(appname, port, upload_dir, socket_ip)    
     
     if upload_dir and not os.path.exists(upload_dir):
         os.makedirs(upload_dir)
 
-    User.UserType = user_type
-
-    if socket_ip != 'localhost' or resource_port != 8000 or socket_port != 1234:
-        User.create_fixed_js()     
-        http_handlers.append(web.get(User.fix_file, static_serve))
-    else:
-        User.fix_file = None
+    User.UserType = user_type    
+    User.create_fixed_js()     
+    http_handlers.append(web.get(User.fix_file, static_serve))
     
     http_handlers.insert(0, web.get('/ws', websocket_handler))
         
-    for h in [web.get('/', static_serve), 
+    for h in [web.get('/', static_serve),        
         web.static('/js', f"{webpath}/js"),
         web.static('/fonts', f"{webpath}/fonts"),
         web.static('/css', f"{webpath}/css"),
-        web.static('/icons', f"{webpath}/icons"),
+        web.static('/icons', f"{webpath}/icons"), 
         web.static(f'/{upload_dir}', f"/{app_user_dir}/{upload_dir}"),
-        web.post('/', post_handler)]:
-
-        http_handlers.append(h)
+          web.post('/', post_handler)]:
+            http_handlers.append(h)
 
     print(f'Start {appname} server on {port} port..')    
     app = web.Application()
     app.add_routes(http_handlers)    
     web.run_app(app,  port=port)
```

### Comparing `unigui-1.8.1/unigui/utils.py` & `unigui-1.8.2/unigui/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,53 +6,64 @@
 appname = 'Unigui'
 app_user_dir = os.getcwd()
 upload_dir = 'upload'
 socket_ip = ''
 socket_port = 1234
 blocks_dir = 'blocks'        
 screens_dir =  'screens'        
+UpdateScreen = True
 
 libpath = os.path.dirname(os.path.realpath(__file__))
 webpath = libpath + '/web' 
 
+try:
+    import config
+except:
+    with open('config.py', 'w') as f:        
+        f.write("""port = 8000 
+#for remote server socket_ip is its ip 
+socket_ip = 'localhost' 
+upload_dir = 'web'
+pretty_print = True
+hot_reload = True
+""")
+        print("Config with default parameters is created!")
+
 def toJson(obj, indent, pretty_print):
     return json.dumps(json.loads(jsonpickle.encode(obj,unpicklable=False)), 
         indent = indent, sort_keys = pretty_print)
 
 def fn2url(fn):   
     if fn[0] == '/':
         fn = fn[len(app_user_dir):]   
-    s =  fn #f":{resource_port}/{fn}"
-    return s.replace(' ','%20')
+    return fn.replace(' ','%20')
 
 def url2fn(url):
     return url[url.find('/') + 1:].replace('%20',' ')
 
 def upload_fn(fn):
     return f'{upload_dir}/{fn}'     
+
+def upload_path(fpath):
+    return f'{os.getcwd()}/{upload_dir}/{fpath}'
     
 def translate_http_path(path):
     if '?' in path:
         path = path.split('?')[0]
     if path.startswith(f'/{upload_dir}/'):             
         return f'{app_user_dir}{path}'.replace('%20',' ')     
     return f'{webpath}{path}'.replace('%20',' ') 
 
-translate_path = translate_http_path
-
-def set_utils(appname_,port_,upload_dir_, translate_path_, socket_ip_, socket_port_):
-    global appname, resource_port, upload_dir, translate_path, socket_ip, socket_port
+def set_utils(appname_,port_,upload_dir_, socket_ip_):
+    global appname, resource_port, upload_dir, socket_ip, socket_port
     appname = appname_
     resource_port = port_
     upload_dir = upload_dir_
     socket_ip = socket_ip_
-    socket_port = socket_port_
-
-    if translate_path_:
-        translate_path = translate_path_
+    socket_port = port_    
 
 def flatten(*arr):
     for a in arr:
         if isinstance(a, list):
             yield from flatten(*a)
         else:
             yield a
@@ -65,39 +76,38 @@
     handlers__ = {}
 
 def handle(elem, event):
     def h(fn):
         handlers__[elem, event] = fn
     return h
 
-def Answer(data, param, id):
-    return {'answer': data,'param': param, 'id' : id}
+class Message:
+    def __init__(self, *gui_objects, user = None):
+        if gui_objects:
+            self.updates = [{'data': gui} for gui in gui_objects]
+            if user:
+                self.fill_paths4(user)
+
+    def fill_paths4(self, user):
+        if hasattr(self, 'updates'):
+            for update in self.updates:
+                update['path'] = user.find_path(update['data'])
+
+def TextMessage(type, text, *data, user = None):
+    message = Message(*data, user=user)
+    message.type = type
+    message.value = text    
+    return message    
 
-def Error(message, *data):
-    d = {'error':message}
-    if data:
-        d['data'] = data
-        d['update'] = None
-    return d
-
-def Info(message, *data):
-    d = {'info':message}
-    if data:
-        d['data'] = data
-        d['update'] = None
-    return d
-    
-def Warning(message, *data):
-    d = {'warning':message}
-    if data:
-        d['data'] = data
-        d['update'] = None
-    return d    
+def Warning(text, *data):
+    return TextMessage('warning', text, *data)
 
-def Update(data):
-    return {'data': data,'update': None}
+def Error(text, *data):
+    return TextMessage('error', text, *data)
+    
+def Info(text, *data):
+    return TextMessage('info', text, *data)
 
-def upload_path(fpath):
-    return f'{os.getcwd()}/{upload_dir}/{fpath}'
+def Answer(data, param, id):
+    return {'type' : 'answer', 'value': data,'param': param, 'id' : id}
 
-UpdateScreen = True
```

### Comparing `unigui-1.8.1/unigui/user.py` & `unigui-1.8.2/unigui/users.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 import importlib
 from .utils import *
 from .guielements import *
 import sys
 import asyncio
 import requests
 from threading import Thread
+import logging
 
 class User:      
     def __init__(self):          
         self.screens = []        
         self.active_dialog = None
         self.screen_module = None                
         self.tool_buttons = []
         User.last_user = self
 
-    def translate_path(self, path):        
-        return utils.translate_path(path)
+    def log(self, str, type = 'error'):        
+        scr = self.screen.name if self.screens else 'omitted'
+        str = f"session: {self.session__}, screen: {scr}, message: {self.message__} \n  {str}"
+        if type == 'error':
+            logging.error(str)
+        else:
+            logging.warning(str)
 
     @staticmethod
     def cache_name(url):    
         name = url.split('/')[-1]
         name = utils.upload_path(name)
         return name
         
@@ -34,44 +40,39 @@
             file = open(cname, "wb")
             file.write(response.content)
             file.close() 
         return cname
 
     @staticmethod
     def create_fixed_js():
-        dir = f"{utils.webpath}/js"        
-        def replace(b, what, tothat):
+        dir = f"{utils.webpath}/js"
+        b = None        
+        def replace(what, tothat):
             return b.replace(bytes(what,encoding='utf8'), bytes(str(tothat),encoding='utf8'))  
         for file in os.listdir(dir):
             fn = f'{dir}/{file}'
             if file[0].isdigit() and file.endswith(".js") and os.path.getsize(fn) > 25000:
                 User.fix_file = f'/js/{file}'
                 with open(fn, 'rb') as main:
                     b = main.read()
                     if utils.socket_ip != 'localhost':
-                        b = replace(b,'localhost', utils.socket_ip)
+                        b = replace('localhost', utils.socket_ip)
                     if utils.resource_port != 8000:
-                        b = replace(b,'8000',utils.resource_port)
-                    if utils.socket_port != 1234:
-                        b = replace(b,'1234', utils.socket_port)                
+                        b = replace('8000',utils.resource_port)                    
                     User.fixed_main = b.decode("utf-8") 
-                    print(f"Fixed {file} created on ip {utils.socket_ip}, http port {utils.resource_port}, socket port {utils.socket_port}.")
+                    print(f"Configuring for http port {utils.resource_port}, socket ip is {utils.socket_ip}.")
                     break
 
     def sync_send(self, obj):
         asyncio.run_coroutine_threadsafe(self.send(obj), self.extra_loop)            
 
     def progress(self, str, *updates):
-        """open or update progress window if str != null else close it  """     
-        d = {'progress': str}
-        if updates:
-            d['update'] = None            
-            d['data'] = updates          
-        self.sync_send(d)               
-
+        """open or update progress window if str != null else close it  """             
+        return self.sync_send(TextMessage('progress', str, *updates, user = self))
+                       
     def load_module(self, file):
         screen_vars = {
             'icon' : None,
             'prepare' : None,            
             'blocks' : [],
             'header' : utils.appname,                        
             'toolbar' : [], 
@@ -139,24 +140,24 @@
 
     def result4message(self, data):
         result = None
         dialog = self.active_dialog
         if dialog:            
             if len(data) == 2: #button pressed
                 self.active_dialog = None
-                result = dialog.callback(dialog, data[1]) #data[1] == returned value                                
+                #data[1] is returned value                                
+                result = dialog.callback(dialog, data[1]) 
             else:
                 el = self.find_element(data)
                 if el:
                     result = self.process_element(el, data)                
         elif len(data) == 2 and not data[1]: #dialog closed            
             return    
         else:
             result = self.process(data)           
-
         if result and isinstance(result, Dialog):
             self.active_dialog = result
         return result
 
     @property
     def blocks(self):
         return [self.active_dialog.content] if self.active_dialog and \
@@ -189,35 +190,32 @@
                 elif c == elem:
                     return [bl.name, c.name]
 
     def prepare_result(self, raw):
         if raw == UpdateScreen:
             raw = self.screen                        
         else:
-            if type(raw) == dict and 'update' in raw:
-                if isinstance(raw['data'], (list,tuple)):
-                    raw['multi'] = True
-                    raw['update'] = [self.find_path(e) for e in raw['data']]
-                else:
-                    raw['update'] = self.find_path(raw['data'])
+            if isinstance(raw, Message):
+                raw.fill_paths4(self)                
             elif isinstance(raw,Gui):
-                 raw = {'update': self.find_path(raw), 'data': raw}
+                raw = Message(raw, user = self)                 
             elif isinstance(raw, (list, tuple)) and all(isinstance(e,Gui) for e in raw):
-                raw = {'update': [self.find_path(e) for e in raw],'multi': True, 'data': raw}
+                raw = Message(*raw, user = self)
         return raw
 
     def process(self,arr):
+        self.message__ = arr
         if arr[0] == 'root':
             for s in self.screens:
                 if s.name == arr[1]:
                     self.screen_module = s
                     if getattr(s.screen,'prepare', False):
                         s.screen.prepare()
                     return True            
-            print(f'Unknown root command {s.name}')
+            print(f'Unknown screen name: {s.name}')
         else:
             elem = self.find_element(arr)                        
             return self.process_element(elem, arr)        
         
     def process_element(self, elem, arr):        
         id = arr.pop() if len(arr) == 5 else 0
         action = arr[-2]        
@@ -239,17 +237,23 @@
                 elem.value = val                                        
             return                        
 
         return Error(f'{elem} does not contain method for {action} event type!')
 
 #loop and thread is for progress window and sync interactions
 loop = asyncio.new_event_loop()
+User.extra_loop = loop
+
 def f(loop):
     asyncio.set_event_loop(loop)
     loop.run_forever() 
-
+    
 async_thread = Thread(target=f, args=(loop,))
 async_thread.start()  
 
-User.extra_loop = loop
+p = {'level' : logging.WARNING}
+if hasattr(config, 'logfile'):
+    p['filename'] = config.logfile
+logging.basicConfig(format='%(asctime)s - %(message)s', **p)
+
```

### Comparing `unigui-1.8.1/unigui/reloader.py` & `unigui-1.8.2/unigui/reloader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-import logging, os, traceback
-from watchdog.observers import Observer
-from watchdog.events import PatternMatchingEventHandler
-from unigui import User
-
 import config
 
-hot_reload = 'hot_reload'
-
 empty_app = {
     "blocks": [],
     "header": "No screens",
     "icon": None,
-    "menu": [["",None]
-    ],
+    "menu": [["You need to put at least 1 file in the 'screens' folder.",'exclamation']],
     "name": "",
     "order": 0,
     "toolbar": [],
     "type": "screen"
 }
 
-if hasattr(config, hot_reload) and config.hot_reload:
+if hasattr(config, 'hot_reload') and config.hot_reload:
+    import logging, os, traceback
+    from watchdog.observers import Observer
+    from watchdog.events import PatternMatchingEventHandler
+    from unigui import User
     busy = False        
 
     def free():
         global busy
         if request_file:
             reload(request_file)
         else:
@@ -48,38 +44,43 @@
                     same = user.screen_module.__file__ == module.__file__
                     user.screens[i] = module
                     if same:
                         user.set_screen(module.screen.name)            
                     break
             else:
                 user.screens.append(module)
+                if len(user.screens) == 1:
+                    user.set_screen(module.name)                    
 
             user.update_menu()
             user.set_clean() 
             user.sync_send(True)
 
             free()  
             return module  
 
     class ScreenEventHandler(PatternMatchingEventHandler):    
         def on_modified(self, event):
             if not event.is_directory and hasattr(User,'last_user'):            
                 arr = event.src_path.split('/') 
                 name = arr[-1]
                 dir = arr[-2]  
-                if name.endswith('.py') and dir in ['screens','blocks']:         
-                    super(ScreenEventHandler, self).on_modified(event)
+                if name.endswith('.py') and dir in ['screens','blocks']:                             
                     if busy:
                         global request_file            
                         request_file = f'{dir}/{name}' 
                     else:                    
                         fresh_module = reload(name) if dir == 'screens' else None                    
-                        current = User.last_user.screen_module.__file__
-                        if not fresh_module or current != fresh_module.__file__:
-                            reload(current.split('/')[-1]) 
+                        user = User.last_user
+                        module = user.screen_module
+                        if module:
+                            current = module.__file__
+                            if not fresh_module or current != fresh_module.__file__:
+                                reload(current.split('/')[-1]) 
+                                                    
         def on_deleted(self, event):            
             if not event.is_directory and hasattr(User,'last_user'):
                 user = User.last_user            
                 arr = event.src_path.split('/') 
                 name = arr[-1]
                 dir = arr[-2]  
                 if name.endswith('.py') and dir == 'screens':
```

### Comparing `unigui-1.8.1/unigui/web/favicon.ico` & `unigui-1.8.2/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/unigui/web/css/295.f0f63b8f.css` & `unigui-1.8.2/unigui/web/css/423.a6a82bd4.css`

 * *Files 22% similar despite different names*

```diff
@@ -1 +1 @@
-thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-2f472339]{display:flex;justify-content:center}.custom-caption[data-v-2f472339]{padding:5px!important}.web-camera-container[data-v-2f472339]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-2f472339]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-2f472339]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-2f472339]{opacity:1}.web-camera-container .camera-shoot[data-v-2f472339]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-2f472339]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-2f472339]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-2f472339]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-2f472339]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-2f472339]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-2f472339]{animation:preload-2f472339 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-2f472339]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-2f472339]:nth-child(3){animation-delay:.4s}@keyframes preload-2f472339{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-2f472339]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
+thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-047e5584]{display:flex;justify-content:center}.custom-caption[data-v-047e5584]{padding:5px!important}.web-camera-container[data-v-047e5584]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-047e5584]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-047e5584]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-047e5584]{opacity:1}.web-camera-container .camera-shoot[data-v-047e5584]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-047e5584]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-047e5584]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-047e5584]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-047e5584]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-047e5584]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-047e5584]{animation:preload-047e5584 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-047e5584]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-047e5584]:nth-child(3){animation-delay:.4s}@keyframes preload-047e5584{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-047e5584]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
```

### Comparing `unigui-1.8.1/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.8.2/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/unigui/web/icons/favicon-96x96.png` & `unigui-1.8.2/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/unigui/web/icons/favicon-16x16.png` & `unigui-1.8.2/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/unigui/web/icons/favicon-32x32.png` & `unigui-1.8.2/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/unigui/web/icons/favicon-128x128.png` & `unigui-1.8.2/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.8.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.8.2/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.8.2/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.8.2/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.8.2/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.8.2/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.8.2/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.8.2/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/unigui/web/js/app.9384942b.js` & `unigui-1.8.2/unigui/web/js/app.eb412190.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(295)]).then(r.bind(r, 8295)),
+                        component: () => Promise.all([r.e(736), r.e(423)]).then(r.bind(r, 6423)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -159,24 +159,24 @@
             })
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "283445be",
-            295: "e2b7be53",
+            423: "0ad6769b",
             430: "591e9a73"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            295: "f0f63b8f",
+            423: "a6a82bd4",
             736: "49a52e8f"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
@@ -260,15 +260,15 @@
                 e(n, l, o, a)
             })),
             o = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                295: 1
+                423: 1
             };
             o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
                 o[e] = 0
             }), (t => {
                 throw delete o[e], t
             })))
         }
```

### Comparing `unigui-1.8.1/unigui/web/js/430.591e9a73.js` & `unigui-1.8.2/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/unigui/web/js/295.e2b7be53.js` & `unigui-1.8.2/unigui/web/js/423.0ad6769b.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [295], {
-        8295: (e, t, a) => {
+    [423], {
+        6423: (e, t, a) => {
             a.r(t), a.d(t, {
-                default: () => Jt
+                default: () => Xt
             });
             var l = a(3673),
                 s = a(2323);
             const i = (0, l._)("div", {
                     class: "q-pa-lg"
                 }, null, -1),
                 o = (0, l._)("div", {
@@ -51,21 +51,23 @@
                                 style: {
                                     float: "center"
                                 }
                             }, {
                                 default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.menu, (t => ((0, l.wg)(), (0, l.iD)("div", null, [t.icon ? ((0, l.wg)(), (0, l.j4)(u, {
                                     key: 0,
                                     class: "justify-center text-white shadow-2",
+                                    "no-caps": "",
                                     name: t.name,
                                     icon: t.icon,
                                     label: t.name,
                                     onClick: a => e.tabclick(t.name)
                                 }, null, 8, ["name", "icon", "label", "onClick"])) : (0, l.kq)("", !0), t.icon ? (0, l.kq)("", !0) : ((0, l.wg)(), (0, l.j4)(u, {
                                     key: 1,
                                     class: "justify-center text-white shadow-2",
+                                    "no-caps": "",
                                     name: t.name,
                                     label: t.name,
                                     onClick: a => e.tabclick(t.name)
                                 }, null, 8, ["name", "label", "onClick"]))])))), 256))])),
                                 _: 1
                             }, 8, ["modelValue"])])),
                             _: 1
@@ -81,15 +83,14 @@
                             _: 1
                         })])),
                         _: 1
                     })])),
                     _: 1
                 })
             }
-            a(71);
 
             function d(e, t, a, i, o, n) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-item-section"),
                     c = (0, l.up)("q-item-label"),
                     h = (0, l.up)("q-item");
                 return (0, l.wg)(), (0, l.j4)(h, {
@@ -111,113 +112,106 @@
                             _: 1
                         })])),
                         _: 1
                     })])),
                     _: 1
                 }, 8, ["onClick"])
             }
-            var r, c = a(698),
-                h = a(8603);
-            let u = null,
-                p = {},
-                g = !0;
+            a(71);
+            var r = a(698),
+                c = a(8603);
+            let h = null,
+                u = {};
+            var p;
+            let g = !0;
             const m = 136,
                 f = 400,
                 y = `height: ${m}px; width: ${f}px`;
 
             function w(e) {
                 let t = e.minheight ? e.minheight : m,
                     a = e.minwidth ? e.minwidth : f;
                 return `height: ${t}px; width: ${a}px`
             }
             let b = {},
                 k = {};
-            const v = ["error", "progress", "warning", "info"];
 
-            function C(e) {
-                r = new WebSocket("ws://localhost:8000/ws"), r.onopen = () => e.statusConnect = !0, r.onmessage = t => {
-                    g && console.log("socket message", t.data), e.processMessage(JSON.parse(t.data))
-                }, r.onerror = t => e.error(t), r.onclose = t => {
-                    t.wasClean ? e.info("Connection closed and was clean.") : e.error("Connection suddenly closed!"), e.statusConnect = !1, g && console.info("close code : " + t.code + " reason: " + t.reason)
-                }, u = e
+            function v(e) {
+                p = new WebSocket("ws://localhost:8000/ws"), p.onopen = () => e.statusConnect = !0, p.onmessage = t => {
+                    g && console.log("incoming message", t.data), e.processMessage(JSON.parse(t.data))
+                }, p.onerror = t => e.error(t), p.onclose = t => {
+                    t.wasClean ? e.info("Connection was finished by the server.") : e.error("Connection suddenly closed!"), e.statusConnect = !1, g && console.info("close code : " + t.code + " reason: " + t.reason)
+                }, h = e
             }
 
-            function q(e) {
-                console.log("sended", e), r.send(JSON.stringify(e))
+            function C(e) {
+                console.log("sended", e), p.send(JSON.stringify(e))
             }
-            let j, S = 0;
+            let q, _ = 0;
 
-            function z() {
+            function j() {
                 for (let [e, t] of Object.entries(k)) t.styleSize = null
             }
 
-            function A(e, t, a, l = "complete") {
-                let s = ++S,
+            function S(e, t, a, l = "complete") {
+                let s = ++_,
                     i = [e.pdata.name, e.data.name, l, t, s];
-                q(i), p[s] = a
+                C(i), u[s] = a
             }
 
-            function Z() {
+            function z() {
                 b = {}, k = {}
             }
 
-            function D(e, t) {
+            function A(e, t) {
                 Object.assign(e.data, t), e.updated = t.value, e.value = t.value
             }
 
-            function M(e) {
-                if (e.multi)
-                    for (let [t, a] of e.update.entries())
-                        if (a.length > 1) {
-                            a.reverse();
-                            let l = a.join("@"),
-                                s = k[l];
-                            D(s, e.data[t])
-                        } else {
-                            let l = b[a[0]];
-                            Object.assign(l.data, e.data[t])
-                        }
-                else {
-                    let t, a = e.update;
-                    if (a.length > 1) {
-                        a.reverse();
-                        let e = a.join("@");
-                        t = k[e]
-                    } else t = b[a[0]];
-                    D(t, e.data), 1 == a.length && (0, h.delay)(O, 200, t)
+            function Z(e) {
+                for (let t of e) {
+                    let e = t.path;
+                    if (e.length > 1) {
+                        e.reverse();
+                        let a = e.join("@"),
+                            l = k[a];
+                        A(l, t.data)
+                    } else {
+                        let a = b[e[0]];
+                        Object.assign(a.data, t.data)
+                    }
                 }
             }
 
-            function $(e) {
-                typeof e.answer == String ? u.showError() : p[e.id](e.answer), delete p[e.id]
+            function D(e) {
+                "string" == typeof e.value ? h.error(e.value) : u[e.id](e.value), delete u[e.id]
             }
 
-            function V(e) {
+            function M(e) {
                 let t = [];
                 for (let l of e) l instanceof Array ? t.push(l) : t.push([l]);
                 let a = t.shift();
                 return t.reduce(((e, t) => e.flatMap((e => t.map((t => e instanceof Array ? [...e, t] : [e, t]))))), a)
             }
 
-            function E() {
+            function $() {
                 for (let [e, t] of Object.entries(k)) t.expanding && (t.styleSize = w(t.data));
                 (0, l.Y3)((() => {
                     requestAnimationFrame((() => {
                         requestAnimationFrame((() => {
-                            O()
+                            K()
                         }))
                     }))
                 }))
             }
-            let K = _.debounce(E, 200);
+            let V = (0, c.debounce)($, 200);
 
-            function O(e) {
-                Array.isArray(e) && (e = null), j && (j.disconnect(), j = null), g && console.log("------------------recalc design");
-                const t = W(e),
-                    a = Q(e);
+            function K(e) {
+                Array.isArray(e) && (e = null), q && (q.disconnect(), q = null), g && console.log("------------------recalc design");
+                const t = E(e),
+                    a = O(e);
                 for (let [l, s] of Object.entries(t)) {
                     let e = k[l];
                     const [t, i] = a[l];
                     let o, n = e.geom().el,
                         d = e.pdata ? e.pdata.name : e.name,
                         r = b[d];
                     for (let a of r.data.value.slice(1))
@@ -235,38 +229,38 @@
                     let c = r.data.width ? r.data.width - n.clientWidth - t : r.$el.getBoundingClientRect().right - (o ? o.geom().right : e.geom().right);
                     c /= i;
                     let h = l.startsWith("_scroll@") ? e.geom().inner.clientHeight : n.clientHeight;
                     e.styleSize = `height: ${h+s}px; width: ${n.clientWidth+c+t}px;`
                 }
             }
 
-            function W(e) {
-                const t = u.screen.blocks;
+            function E(e) {
+                const t = h.screen.blocks;
                 let a = window.innerHeight;
                 a -= 2;
                 let l = {},
                     s = new Map,
                     i = {};
                 for (let [d, r] of Object.entries(b)) i[r.name] = r.$el.getBoundingClientRect().height;
                 let o = [];
                 for (let d of t) {
                     const e = [];
                     let t = d instanceof Array,
-                        n = t ? V(d) : [
+                        n = t ? M(d) : [
                             [d]
                         ];
                     for (let a of n) {
                         let e = 0;
                         for (let t of a) e += i[t.name] + 8;
                         o.push([e, a])
                     }
                     o.sort(((e, t) => e[0] > t[0] ? -1 : e[0] == t[0] ? 0 : 1));
                     for (let l of o) {
                         let t = l[1];
-                        (0, c.hu)(Array.isArray(t));
+                        (0, r.hu)(Array.isArray(t));
                         const i = [];
                         for (let [e, a] of Object.entries(k))
                             if (a.expanding_height) {
                                 let [l, o] = e.split("@");
                                 if (t.find((e => e.name == o))) {
                                     let e = !0;
                                     const t = a.geom();
@@ -301,17 +295,17 @@
                 }
                 let n = Array.from(s.entries());
                 n.sort(((e, t) => e[0] in l || e[1] in l ? -1 : 1));
                 for (let [d, r] of n) r in l ? l[d] = l[r] : l[r] = l[d];
                 return l
             }
 
-            function Q(e) {
+            function O(e) {
                 e = null;
-                const t = e ? [e] : u.screen.blocks;
+                const t = e ? [e] : h.screen.blocks;
                 let a = window.innerWidth - 30,
                     l = [],
                     s = {};
                 for (let n of t)
                     if (0 == l.length)
                         if (Array.isArray(n))
                             for (let e of n) l.push(Array.isArray(e) ? e : [e]);
@@ -368,198 +362,198 @@
                             s[a.fullname] = [Math.floor(n / e), t[l]]
                         }
                     }
                 }
                 for (let [n, d] of o.entries()) d in s ? s[n] = s[d] : s[d] = s[n];
                 return s
             }
-            const H = (0, l.aZ)({
+            const W = (0, l.aZ)({
                 name: "menubar",
                 methods: {
                     send() {
-                        q(["root", this.name])
+                        C(["root", this.name])
                     }
                 },
                 props: {
                     name: {
                         type: String,
                         required: !0
                     },
                     icon: {
                         type: String,
                         default: ""
                     }
                 }
             });
-            var U = a(4260),
-                N = a(3414),
-                F = a(2035),
-                P = a(4554),
-                T = a(2350),
-                I = a(7518),
-                R = a.n(I);
-            const L = (0, U.Z)(H, [
+            var Q = a(4260),
+                H = a(3414),
+                U = a(2035),
+                N = a(4554),
+                F = a(2350),
+                T = a(7518),
+                P = a.n(T);
+            const I = (0, Q.Z)(W, [
                     ["render", d]
                 ]),
-                B = L;
-            R()(H, "components", {
-                QItem: N.Z,
-                QItemSection: F.Z,
-                QIcon: P.Z,
-                QItemLabel: T.Z
+                R = I;
+            P()(W, "components", {
+                QItem: H.Z,
+                QItemSection: U.Z,
+                QIcon: N.Z,
+                QItemLabel: F.Z
             });
-            const Y = {
+            const L = {
                     key: 0,
                     class: "row q-col-gutter-sm q-py-sm"
                 },
-                X = {
+                B = {
                     class: "q-col-gutter-sm"
                 },
-                G = {
+                Y = {
                     key: 0,
                     class: "column q-col-gutter-sm"
                 };
 
-            function J(e, t, a, s, i, o) {
+            function X(e, t, a, s, i, o) {
                 const n = (0, l.up)("zone", !0),
                     d = (0, l.up)("block");
-                return e.data instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", Y, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data, (e => ((0, l.wg)(), (0, l.iD)("div", X, [e instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", G, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e, (e => ((0, l.wg)(), (0, l.j4)(n, {
+                return e.data instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", L, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data, (e => ((0, l.wg)(), (0, l.iD)("div", B, [e instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", Y, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e, (e => ((0, l.wg)(), (0, l.j4)(n, {
                     data: e
                 }, null, 8, ["data"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                     key: 1,
                     data: e
                 }, null, 8, ["data"]))])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                     key: 1,
                     data: e.data
                 }, null, 8, ["data"]))
             }
-            const ee = {
+            const G = {
                     class: "row"
                 },
-                te = {
+                J = {
                     key: 2,
                     class: "q-ma-sm",
                     style: {
                         "font-size": "18px"
                     }
                 },
-                ae = ["data", "pdata"],
-                le = {
+                ee = ["data", "pdata"],
+                te = {
                     key: 0,
                     class: "row"
                 },
-                se = ["data", "pdata"],
-                ie = {
+                ae = ["data", "pdata"],
+                le = {
                     key: 0,
                     class: "row"
                 };
 
-            function oe(e, t, a, i, o, n) {
+            function se(e, t, a, i, o, n) {
                 const d = (0, l.up)("element"),
                     r = (0, l.up)("q-icon"),
                     c = (0, l.up)("q-scroll-area"),
                     h = (0, l.up)("q-card");
                 return (0, l.wg)(), (0, l.j4)(h, {
                     class: "my-card q-ma-xs"
                 }, {
-                    default: (0, l.w5)((() => [(0, l._)("div", ee, [e.data.logo ? ((0, l.wg)(), (0, l.j4)(d, {
+                    default: (0, l.w5)((() => [(0, l._)("div", G, [e.data.logo ? ((0, l.wg)(), (0, l.j4)(d, {
                         key: 0,
                         data: e.data.logo,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])) : e.data.icon ? ((0, l.wg)(), (0, l.j4)(r, {
                         key: 1,
                         size: "sm",
                         name: e.data.icon
-                    }, null, 8, ["name"])) : (0, l.kq)("", !0), "_" != e.name[0] ? ((0, l.wg)(), (0, l.iD)("p", te, (0, s.zw)(e.name), 1)) : (0, l.kq)("", !0), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.tops, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                    }, null, 8, ["name"])) : (0, l.kq)("", !0), "_" != e.name[0] ? ((0, l.wg)(), (0, l.iD)("p", J, (0, s.zw)(e.name), 1)) : (0, l.kq)("", !0), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.tops, (t => ((0, l.wg)(), (0, l.j4)(d, {
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])))), 256))]), e.data.scroll ? ((0, l.wg)(), (0, l.j4)(c, {
                         key: 0,
                         style: (0, s.j5)(e.styleSize),
                         "thumb-style": e.thumbStyle,
                         "bar-style": e.barStyle
                     }, {
                         default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data.value.slice(1), (t => ((0, l.wg)(), (0, l.iD)("div", {
                             class: "column",
                             data: t,
                             pdata: e.data
-                        }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", le, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                        }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", te, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
                             class: "q-ma-xs",
                             data: t,
                             pdata: e.data
                         }, null, 8, ["data", "pdata"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                             key: 1,
                             class: "q-ma-xs",
                             data: t,
                             pdata: e.data
-                        }, null, 8, ["data", "pdata"]))], 8, ae)))), 256))])),
+                        }, null, 8, ["data", "pdata"]))], 8, ee)))), 256))])),
                         _: 1
                     }, 8, ["style", "thumb-style", "bar-style"])) : ((0, l.wg)(!0), (0, l.iD)(l.HY, {
                         key: 1
                     }, (0, l.Ko)(e.data.value.slice(1), (t => ((0, l.wg)(), (0, l.iD)("div", {
                         class: "column",
                         data: t,
                         pdata: e.data
-                    }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", ie, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                    }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", le, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                         key: 1,
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
-                    }, null, 8, ["data", "pdata"]))], 8, se)))), 256))])),
+                    }, null, 8, ["data", "pdata"]))], 8, ae)))), 256))])),
                     _: 1
                 })
             }
-            var ne = a(8880);
-            const de = e => ((0, l.dD)("data-v-2f472339"), e = e(), (0, l.Cn)(), e),
-                re = {
+            var ie = a(8880);
+            const oe = e => ((0, l.dD)("data-v-047e5584"), e = e(), (0, l.Cn)(), e),
+                ne = {
                     key: 4
                 },
-                ce = ["width", "height"],
-                he = ["src"],
-                ue = {
+                de = ["width", "height"],
+                re = ["src"],
+                ce = {
                     key: 17,
                     class: "web-camera-container"
                 },
-                pe = {
+                he = {
                     class: "camera-button"
                 },
-                ge = {
+                ue = {
                     key: 0
                 },
-                me = {
+                pe = {
                     key: 1
                 },
-                fe = {
+                ge = {
                     class: "camera-loading"
                 },
-                ye = de((() => (0, l._)("ul", {
+                me = oe((() => (0, l._)("ul", {
                     class: "loader-circle"
                 }, [(0, l._)("li"), (0, l._)("li"), (0, l._)("li")], -1))),
-                we = [ye],
-                be = ["height"],
-                ke = ["height"],
-                ve = {
+                fe = [me],
+                ye = ["height"],
+                we = ["height"],
+                be = {
                     key: 1,
                     class: "camera-shoot"
                 },
-                xe = de((() => (0, l._)("img", {
+                ke = oe((() => (0, l._)("img", {
                     src: "https://img.icons8.com/material-outlined/50/000000/camera--v2.png"
                 }, null, -1))),
-                Ce = [xe],
-                qe = {
+                ve = [ke],
+                xe = {
                     key: 2,
                     class: "camera-download"
                 };
 
-            function _e(e, t, a, i, o, n) {
+            function Ce(e, t, a, i, o, n) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-img"),
                     c = (0, l.up)("q-badge"),
                     h = (0, l.up)("q-select"),
                     u = (0, l.up)("q-checkbox"),
                     p = (0, l.up)("q-toggle"),
                     g = (0, l.up)("q-btn"),
@@ -573,22 +567,22 @@
                     x = (0, l.up)("q-uploader"),
                     C = (0, l.up)("cgraph"),
                     q = (0, l.up)("q-tooltip");
                 return "image" == e.type ? ((0, l.wg)(), (0, l.j4)(r, {
                     key: 0,
                     src: e.data.name,
                     "spinner-color": "blue",
-                    onClick: (0, ne.iM)(e.switchValue, ["stop"]),
+                    onClick: (0, ie.iM)(e.switchValue, ["stop"]),
                     fit: "cover",
                     style: (0, s.j5)(e.elemSize)
                 }, {
                     default: (0, l.w5)((() => [e.data.header ? ((0, l.wg)(), (0, l.iD)("div", {
                         key: 0,
                         class: "absolute-bottom-right text-subtitle2 custom-caption",
-                        onClick: t[0] || (t[0] = (0, ne.iM)(((...t) => e.lens && e.lens(...t)), ["stop"]))
+                        onClick: t[0] || (t[0] = (0, ie.iM)(((...t) => e.lens && e.lens(...t)), ["stop"]))
                     }, (0, s.zw)(e.data.header), 1)) : (0, l.kq)("", !0), e.value ? ((0, l.wg)(), (0, l.j4)(d, {
                         key: 1,
                         class: "absolute all-pointer-events",
                         size: "32px",
                         name: "check_circle",
                         color: "gray",
                         style: {
@@ -628,24 +622,25 @@
                 }, null, 8, ["modelValue", "label"])) : "switch" == e.type ? ((0, l.wg)(), (0, l.j4)(p, {
                     key: 3,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[3] || (t[3] = t => e.value = t),
                     color: "primary",
                     label: e.nameLabel,
                     "left-label": ""
-                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, l.wg)(), (0, l.iD)("div", re, [e.showname ? ((0, l.wg)(), (0, l.j4)(g, {
+                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, l.wg)(), (0, l.iD)("div", ne, [e.showname ? ((0, l.wg)(), (0, l.j4)(g, {
                     key: 0,
                     ripple: !1,
                     color: "secondary",
                     disable: "",
                     label: e.name,
                     "no-caps": ""
                 }, null, 8, ["label"])) : (0, l.kq)("", !0), (0, l.Wm)(m, {
                     modelValue: e.value,
                     "onUpdate:modelValue": t[4] || (t[4] = t => e.value = t),
+                    "no-caps": "",
                     options: e.data.options.map((e => ({
                         label: e,
                         value: e
                     })))
                 }, null, 8, ["modelValue", "options"])])) : "table" == e.type ? ((0, l.wg)(), (0, l.j4)(f, {
                     key: 5,
                     data: e.data,
@@ -660,27 +655,27 @@
                     key: 7,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[5] || (t[5] = t => e.value = t),
                     label: e.name,
                     ref: "inputRef",
                     autogrow: e.data.autogrow,
                     dense: "",
-                    onKeyup: (0, ne.D2)(e.pressedEnter, ["enter"]),
+                    onKeyup: (0, ie.D2)(e.pressedEnter, ["enter"]),
                     readonly: !1 === e.data.edit
                 }, null, 8, ["modelValue", "label", "autogrow", "onKeyup", "readonly"])) : "number" == e.type ? ((0, l.wg)(), (0, l.j4)(w, {
                     key: 8,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[6] || (t[6] = t => e.value = t),
                     modelModifiers: {
                         number: !0
                     },
                     label: e.name,
                     ref: "inputRef",
                     dense: "",
-                    onKeyup: (0, ne.D2)(e.pressedEnter, ["enter"]),
+                    onKeyup: (0, ie.D2)(e.pressedEnter, ["enter"]),
                     type: "number",
                     readonly: !1 === e.data.edit
                 }, null, 8, ["modelValue", "label", "onKeyup", "readonly"])) : "autoedit" == e.type ? ((0, l.wg)(), (0, l.j4)(h, {
                     key: 9,
                     dense: "",
                     modelValue: e.value,
                     "onUpdate:modelValue": t[7] || (t[7] = t => e.value = t),
@@ -690,15 +685,15 @@
                     outlined: "",
                     "hide-bottom-space": "",
                     "fill-input": "",
                     "input-debounce": "0",
                     options: e.options,
                     onFilter: e.complete,
                     label: e.name,
-                    onKeyup: (0, ne.D2)(e.pressedEnter, ["enter"])
+                    onKeyup: (0, ie.D2)(e.pressedEnter, ["enter"])
                 }, null, 8, ["modelValue", "options", "onFilter", "label", "onKeyup"])) : "tree" == e.type || "list" == e.type ? ((0, l.wg)(), (0, l.j4)(k, {
                     key: 10,
                     style: (0, s.j5)(e.styleSize),
                     "thumb-style": e.thumbStyle,
                     "bar-style": e.barStyle
                 }, {
                     default: (0, l.w5)((() => [(0, l.Wm)(b, {
@@ -716,27 +711,27 @@
                     key: 11,
                     class: "textarea",
                     "onUpdate:modelValue": t[10] || (t[10] = t => e.value = t),
                     filled: "",
                     type: "textarea",
                     style: (0, s.j5)(e.elemSize)
                 }, null, 4)), [
-                    [ne.nr, e.value]
+                    [ie.nr, e.value]
                 ]) : "line" == e.type ? ((0, l.wg)(), (0, l.j4)(v, {
                     key: 12,
                     color: "green"
                 })) : "video" == e.type ? ((0, l.wg)(), (0, l.iD)("video", {
                     width: e.data.width,
                     height: e.data.height,
                     key: e.data.src,
                     controls: ""
                 }, [(0, l._)("source", {
                     src: e.data.src,
                     type: "video/mp4"
-                }, null, 8, he)], 8, ce)) : "gallery" == e.type ? ((0, l.wg)(), (0, l.j4)(x, {
+                }, null, 8, re)], 8, de)) : "gallery" == e.type ? ((0, l.wg)(), (0, l.j4)(x, {
                     key: 14,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
                     url: "http://localhost:8000",
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
@@ -754,53 +749,53 @@
                     ref: "uploaderRef",
                     flat: ""
                 }, null, 8, ["label", "onUploaded", "onAdded"])) : "graph" == e.type ? ((0, l.wg)(), (0, l.j4)(C, {
                     key: 16,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.elemSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, l.wg)(), (0, l.iD)("div", ue, [(0, l._)("div", pe, [(0, l._)("button", {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, l.wg)(), (0, l.iD)("div", ce, [(0, l._)("div", he, [(0, l._)("button", {
                     class: (0, s.C_)(["button is-rounded", {
                         "is-primary": !e.isCameraOpen,
                         "is-danger": e.isCameraOpen
                     }]),
                     type: "button",
                     onClick: t[11] || (t[11] = (...t) => e.toggleCamera && e.toggleCamera(...t))
-                }, [e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("span", me, "Close Camera")) : ((0, l.wg)(), (0, l.iD)("span", ge, "Open Camera"))], 2)]), (0, l.wy)((0, l._)("div", fe, we, 512), [
-                    [ne.F8, e.isCameraOpen && e.isLoading]
+                }, [e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("span", pe, "Close Camera")) : ((0, l.wg)(), (0, l.iD)("span", ue, "Open Camera"))], 2)]), (0, l.wy)((0, l._)("div", ge, fe, 512), [
+                    [ie.F8, e.isCameraOpen && e.isLoading]
                 ]), e.isCameraOpen ? (0, l.wy)(((0, l.wg)(), (0, l.iD)("div", {
                     key: 0,
                     class: (0, s.C_)(["camera-box", {
                         flash: e.isShotPhoto
                     }])
                 }, [(0, l._)("div", {
                     class: (0, s.C_)(["camera-shutter", {
                         flash: e.isShotPhoto
                     }])
                 }, null, 2), (0, l.wy)((0, l._)("video", {
                     ref: "camera",
                     width: 450,
                     height: 337.5,
                     autoplay: ""
-                }, null, 8, be), [
-                    [ne.F8, !e.isPhotoTaken]
+                }, null, 8, ye), [
+                    [ie.F8, !e.isPhotoTaken]
                 ]), (0, l.wy)((0, l._)("canvas", {
                     id: "photoTaken",
                     ref: "canvas",
                     width: 450,
                     height: 337.5
-                }, null, 8, ke), [
-                    [ne.F8, e.isPhotoTaken]
+                }, null, 8, we), [
+                    [ie.F8, e.isPhotoTaken]
                 ])], 2)), [
-                    [ne.F8, !e.isLoading]
-                ]) : (0, l.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, l.wg)(), (0, l.iD)("div", ve, [(0, l._)("button", {
+                    [ie.F8, !e.isLoading]
+                ]) : (0, l.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, l.wg)(), (0, l.iD)("div", be, [(0, l._)("button", {
                     class: "button",
                     type: "button",
                     onClick: t[12] || (t[12] = (...t) => e.takePhoto && e.takePhoto(...t))
-                }, Ce)])) : (0, l.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("div", qe, [(0, l.Wm)(g, {
+                }, ve)])) : (0, l.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("div", xe, [(0, l.Wm)(g, {
                     onClick: e.downloadImage,
                     label: "Send"
                 }, null, 8, ["onClick"])])) : (0, l.kq)("", !0)])) : "" != e.showname ? ((0, l.wg)(), (0, l.j4)(g, {
                     key: 18,
                     "no-caps": "",
                     label: e.name,
                     icon: e.data.icon,
@@ -827,23 +822,23 @@
                     }, {
                         default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, l.kq)("", !0)])),
                     _: 1
                 }, 8, ["icon", "onClick"]))
             }
-            const je = {
+            const qe = {
                     key: 0
                 },
-                Se = {
+                _e = {
                     class: "row"
                 },
-                ze = ["onClick"];
+                je = ["onClick"];
 
-            function Ae(e, t, a, i, o, n) {
+            function Se(e, t, a, i, o, n) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-tooltip"),
                     c = (0, l.up)("q-input"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-th"),
                     p = (0, l.up)("q-tr"),
                     g = (0, l.up)("q-checkbox"),
@@ -865,15 +860,15 @@
                     title: e.name,
                     rows: e.rows,
                     columns: e.columns,
                     selection: e.singleMode ? "single" : "multiple",
                     selected: e.selected,
                     "onUpdate:selected": t[2] || (t[2] = t => e.selected = t)
                 }, {
-                    "top-right": (0, l.w5)((() => [!1 !== e.data.tools ? ((0, l.wg)(), (0, l.iD)("div", je, [(0, l._)("div", Se, [(0, l.Wm)(c, {
+                    "top-right": (0, l.w5)((() => [!1 !== e.data.tools ? ((0, l.wg)(), (0, l.iD)("div", qe, [(0, l._)("div", _e, [(0, l.Wm)(c, {
                         modelValue: e.search,
                         "onUpdate:modelValue": t[1] || (t[1] = t => e.search = t),
                         label: "Search",
                         dense: "",
                         ref: "searchField"
                     }, (0, l.Nv)({
                         append: (0, l.w5)((() => ["" != e.search ? ((0, l.wg)(), (0, l.j4)(d, {
@@ -1054,34 +1049,34 @@
                                 "onUpdate:modelValue": [e => t.row[a.name] = e, e.change],
                                 dense: "",
                                 onKeydown: e.keyInput,
                                 autofocus: ""
                             }, null, 8, ["modelValue", "onUpdate:modelValue", "onKeydown"])) : ((0, l.wg)(), (0, l.iD)("div", {
                                 key: 3,
                                 onClick: a => e.select(t.row.iiid, i)
-                            }, (0, s.zw)(t.row[a.name]), 9, ze))])),
+                            }, (0, s.zw)(t.row[a.name]), 9, je))])),
                             _: 2
                         }, 1032, ["props"])))), 128))])),
                         _: 2
                     }, 1032, ["props", "onClick"])])),
                     _: 1
                 }, 8, ["style", "filter", "title", "rows", "columns", "selection", "selected"])
             }
-            var Ze = a(1959);
+            var ze = a(1959);
 
-            function De(e, t) {
+            function Ae(e, t) {
                 return e.length === t.length && e.every(((e, a) => e.iiid == t[a].iiid))
             }
-            const Me = (0, l.aZ)({
+            const Ze = (0, l.aZ)({
                 name: "utable",
                 setup(e) {
                     const {
                         data: t,
                         pdata: a
-                    } = (0, Ze.BK)(e);
+                    } = (0, ze.BK)(e);
                     let s = (0, l.Fl)((() => {
                             let e = [],
                                 a = t.value;
                             const l = a.headers,
                                 s = l.length,
                                 i = a.rows,
                                 o = i.length;
@@ -1095,19 +1090,19 @@
                         })),
                         i = () => {
                             let e = t.value,
                                 a = null === e.value || 0 == s.value.length ? [] : Array.isArray(e.value) ? e.value.map((e => s.value[e])) : [s.value[e.value]];
                             return a
                         },
                         o = i(),
-                        n = (0, Ze.iH)(o),
-                        d = (0, Ze.iH)(o),
-                        r = (0, Ze.iH)(!Array.isArray(t.value.value)),
+                        n = (0, ze.iH)(o),
+                        d = (0, ze.iH)(o),
+                        r = (0, ze.iH)(!Array.isArray(t.value.value)),
                         c = (e, l) => {
-                            q([a.value.name, t.value.name, e, l])
+                            C([a.value.name, t.value.name, e, l])
                         },
                         h = (0, l.Fl)((() => r.value ? d.value.length > 0 ? d.value[0].iiid : null : d.value.map((e => e.iiid)))),
                         u = (0, l.Fl)((() => t.value.value));
                     return (0, l.YP)(s, ((e, t) => {
                         d.value = i(), n.value = d.value
                     })), (0, l.YP)(t, ((e, a) => {
                         g && console.log("data update", a.name), d.value = i(), n.value = d.value, r.value = !Array.isArray(t.value.value)
@@ -1196,24 +1191,24 @@
                                         a = typeof t.rows[e][this.cedit];
                                     "string" != a && "number" != a || (t.value = e), this.selected = [this.rows[e]]
                                 }
                                 break
                         }
                     },
                     complete(e, t, a) {
-                        A(this, [e, [this.redit, this.cedit]], (e => t((() => {
+                        S(this, [e, [this.redit, this.cedit]], (e => t((() => {
                             this.options = e
                         }))))
                     },
                     append() {
                         let e = this.data.rows,
                             t = e.length,
                             a = this;
-                        A(this, [t, this.search], (function(l) {
-                            if (!Array.isArray(l)) return u.error(l);
+                        S(this, [t, this.search], (function(l) {
+                            if (!Array.isArray(l)) return h.error(l);
                             g && console.log("added row", l), a.search = "", e.push(l), setTimeout((() => {
                                 let e = a.rows;
                                 a.selected = [e[t]], a.showSelected(), a.editMode || a.switchEdit(), a.select(e[t], 0)
                             }), 100)
                         }), "append")
                     },
                     showSelected() {
@@ -1233,29 +1228,29 @@
                     switchMode() {
                         this.singleMode = !this.singleMode, this.singleMode && this.selected.length > 1 && this.selected.splice(1)
                     },
                     switchEdit() {
                         this.editMode = !this.editMode, this.editMode && !this.singleMode && this.switchMode()
                     },
                     delSelected() {
-                        if (!this.selected.length) return void u.error("Rows are not selected!");
+                        if (!this.selected.length) return void h.error("Rows are not selected!");
                         this.sendMessage("delete", this.value);
                         let e = this.data.rows;
                         if (this.singleMode) e.splice(this.selected[0].iiid, 1);
                         else {
                             this.selected.length > 1 && this.selected.sort(((e, t) => t.iiid - e.iiid));
                             for (let t of this.selected) e.splice(t.iiid, 1)
                         }
                         this.selected = []
                     }
                 },
                 watch: {
                     selected(e) {
                         const t = this.data;
-                        if (!De(this.updated, this.selected)) {
+                        if (!Ae(this.updated, this.selected)) {
                             let e = this.selected.length;
                             this.sendMessage("changed", this.singleMode ? 1 == e ? this.selected[0].iiid : null : this.selected.map((e => e.iiid))), this.updated = this.selected
                         }
                         t.show && (this.showSelected(), t.show = !1), this.editMode && this.selected.length && (t.value = this.selected[0].iiid)
                     }
                 },
                 computed: {
@@ -1280,52 +1275,52 @@
                 },
                 props: {
                     data: Object,
                     pdata: Object,
                     styleSize: String
                 }
             });
-            var $e = a(9267),
-                Ve = a(4842),
-                Ee = a(8870),
-                Ke = a(2165),
-                Oe = a(8186),
-                We = a(2414),
-                Qe = a(3884),
-                He = a(5735),
-                Ue = a(7208);
-            const Ne = (0, U.Z)(Me, [
-                    ["render", Ae]
+            var De = a(9267),
+                Me = a(4842),
+                $e = a(8870),
+                Ve = a(2165),
+                Ke = a(8186),
+                Ee = a(2414),
+                Oe = a(3884),
+                We = a(5735),
+                Qe = a(7208);
+            const He = (0, Q.Z)(Ze, [
+                    ["render", Se]
                 ]),
-                Fe = Ne;
-            R()(Me, "components", {
-                QTable: $e.Z,
-                QInput: Ve.Z,
-                QIcon: P.Z,
-                QTooltip: Ee.Z,
-                QBtn: Ke.Z,
-                QTr: Oe.Z,
-                QTh: We.Z,
-                QTd: Qe.Z,
-                QCheckbox: He.Z,
-                QSelect: Ue.Z
+                Ue = He;
+            P()(Ze, "components", {
+                QTable: De.Z,
+                QInput: Me.Z,
+                QIcon: N.Z,
+                QTooltip: $e.Z,
+                QBtn: Ve.Z,
+                QTr: Ke.Z,
+                QTh: Ee.Z,
+                QTd: Oe.Z,
+                QCheckbox: We.Z,
+                QSelect: Qe.Z
             });
-            const Pe = ["nodes", "edges"];
+            const Ne = ["nodes", "edges"];
 
-            function Te(e, t, a, i, o, n) {
+            function Fe(e, t, a, i, o, n) {
                 return (0, l.wg)(), (0, l.iD)("div", {
                     nodes: e.nodes,
                     edges: e.edges,
                     style: (0, s.j5)(e.styleSize),
                     ref: "cy"
-                }, null, 12, Pe)
+                }, null, 12, Ne)
             }
-            var Ie = a(2393),
-                Re = a.n(Ie);
-            const Le = Re().stylesheet().selector("node").css({
+            var Te = a(2393),
+                Pe = a.n(Te);
+            const Ie = Pe().stylesheet().selector("node").css({
                     content: "data(id)",
                     "background-color": "#4286f4",
                     "font-size": "14px"
                 }).selector(".selected").css({
                     "background-color": "#ff5555",
                     "border-color": "#ff5555",
                     "font-size": "14px"
@@ -1350,50 +1345,50 @@
                     label: "data(label)",
                     "text-rotation": "autorotate",
                     "text-margin-x": "-8px",
                     "text-margin-y": "-8px",
                     color: "gray",
                     "font-size": "12px"
                 }),
-                Be = {
+                Re = {
                     animate: !0,
                     randomize: !0
                 };
 
-            function Ye(e, t) {
+            function Le(e, t) {
                 if (e.length != t.length) return !0;
                 for (let a = 0; a < e.length; a++)
                     if (e[a].id != t[a].id || e[a].label != t[a].label) return !0;
                 return !1
             }
-            const Xe = (0, l.aZ)({
+            const Be = (0, l.aZ)({
                     name: "cgraph",
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
                         return {
                             cy: null,
-                            style: Le,
-                            layoutOptions: Be,
+                            style: Ie,
+                            layoutOptions: Re,
                             selectedNodes: [],
                             selectedEdges: [],
                             oldNodes: [],
                             oldEdges: [],
                             shiftKey: !1
                         }
                     },
                     beforeUnmount() {
                         window.removeEventListener("keydown", this.handleKeyDown), window.removeEventListener("keyup", this.handleKeyUp)
                     },
                     mounted() {
                         window.addEventListener("keydown", this.handleKeyDown), window.addEventListener("keyup", this.handleKeyUp);
-                        let e = Re()({
+                        let e = Pe()({
                                 container: this.$refs.cy,
                                 elements: {
                                     nodes: this.nodes,
                                     edges: this.edges
                                 },
                                 style: this.style
                             }),
@@ -1443,15 +1438,15 @@
                         },
                         value() {
                             return this.data.value
                         }
                     },
                     methods: {
                         sendMessage(e, t) {
-                            q([this.pdata["name"], this.data["name"], e, t])
+                            C([this.pdata["name"], this.data["name"], e, t])
                         },
                         handleKeyDown(e) {
                             "Shift" == e.key && (this.shiftKey = !0)
                         },
                         handleKeyUp(e) {
                             "Shift" == e.key && (this.shiftKey = !1)
                         },
@@ -1515,15 +1510,15 @@
                                 for (let t of e) a.edges("[id='" + t + "']").addClass("highlighted")
                             }
                         },
                         data: {
                             handler(e, t) {
                                 let a = e.value,
                                     l = !1;
-                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Ye(e.nodes, this.oldNodes) && (l = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Ye(e.edges, this.oldEdges) && (l = !0, this.oldEdges = e.edges), l && null != this.cy) {
+                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Le(e.nodes, this.oldNodes) && (l = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Le(e.edges, this.oldEdges) && (l = !0, this.oldEdges = e.edges), l && null != this.cy) {
                                     this.cy.json({
                                         elements: {
                                             nodes: this.nodes,
                                             edges: this.edges
                                         }
                                     });
                                     let e = this.data.method;
@@ -1540,43 +1535,43 @@
                             this.cy.style(e)
                         },
                         layoutOptions(e) {
                             this.cy.layout(e).run()
                         }
                     }
                 }),
-                Ge = (0, U.Z)(Xe, [
-                    ["render", Te]
+                Ye = (0, Q.Z)(Be, [
+                    ["render", Fe]
                 ]),
-                Je = Ge;
+                Xe = Ye;
 
-            function et(e, t, a, i, o, n) {
+            function Ge(e, t, a, i, o, n) {
                 const d = (0, l.up)("v-chart");
                 return (0, l.wg)(), (0, l.j4)(d, {
                     ref: "chart",
                     option: o.options,
                     style: (0, s.j5)(a.styleSize),
                     autoresize: !0,
                     onClick: n.clicked
                 }, null, 8, ["option", "style", "onClick"])
             }
-            var tt = a(5512),
-                at = a(4447),
-                lt = a(1006),
-                st = a(3526),
-                it = a(763),
-                ot = a(546),
-                nt = a(6902),
-                dt = a(2826),
-                rt = a(5256),
-                ct = a(3825),
-                ht = a(8825);
-            (0, it.D)([at.N, lt.N, st.N]), (0, it.D)([ot.N, nt.N, dt.N, rt.N, ct.N]);
-            let ut = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"],
-                pt = {
+            var Je = a(5512),
+                et = a(4447),
+                tt = a(1006),
+                at = a(3526),
+                lt = a(763),
+                st = a(546),
+                it = a(6902),
+                ot = a(2826),
+                nt = a(5256),
+                dt = a(3825),
+                rt = a(8825);
+            (0, lt.D)([et.N, tt.N, at.N]), (0, lt.D)([st.N, it.N, ot.N, nt.N, dt.N]);
+            let ct = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"],
+                ht = {
                     responsive: !0,
                     maintainAspectRatio: !1,
                     legend: {
                         data: [],
                         bottom: 10
                     },
                     tooltip: {
@@ -1611,26 +1606,26 @@
                         end: 10
                     }, {
                         start: 0,
                         end: 10
                     }],
                     series: []
                 };
-            const gt = {
+            const ut = {
                     name: "linechart",
                     components: {
-                        VChart: tt.ZP
+                        VChart: Je.ZP
                     },
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
-                        const e = (0, ht.Z)();
+                        const e = (0, rt.Z)();
                         return {
                             $q: e,
                             model: !1,
                             options: null
                         }
                     },
                     methods: {
@@ -1659,83 +1654,83 @@
                             let s = [];
                             for (let o = 0; o < l.length; o++) l[o] = "i" == l[o] ? -1 : parseInt(l[o]), s.push([]), o && (this.options.series.push({
                                 name: t[l[o]],
                                 type: "line",
                                 symbol: "none",
                                 sampling: "lttb",
                                 itemStyle: {
-                                    color: ut[o]
+                                    color: ct[o]
                                 },
                                 data: s[o]
                             }), this.options.legend.data.push(t[l[o]]));
                             this.options.xAxis.data = s[0];
                             let i = this.data.rows;
                             for (let o = 0; o < i.length; o++)
                                 for (let e = 0; e < l.length; e++) s[e].push(-1 == l[e] ? o : i[o][l[e]]);
                             this.$refs.chart.setOption(this.options)
                         }
                     },
                     mounted() {
-                        this.options = (0, h.cloneDeep)(pt), this.calcSeries(), this.$refs.chart.chart.on("click", this.clicked)
+                        this.options = (0, c.cloneDeep)(ht), this.calcSeries(), this.$refs.chart.chart.on("click", this.clicked)
                     },
                     watch: {}
                 },
-                mt = (0, U.Z)(gt, [
-                    ["render", et]
+                pt = (0, Q.Z)(ut, [
+                    ["render", Ge]
                 ]),
-                ft = mt;
+                gt = pt;
 
-            function yt(e) {
+            function mt(e) {
                 let t = new FormData;
                 t.append("image", e);
                 let a = new XMLHttpRequest;
                 a.open("POST", "http://localhost:8000", !0), a.onload = function() {
                     200 === this.status ? console.log(this.response) : console.error(a)
                 }, a.send(t)
             }
-            const wt = (0, l.aZ)({
+            const ft = (0, l.aZ)({
                 name: "element",
                 components: {
-                    utable: Fe,
-                    cgraph: Je,
-                    linechart: ft
+                    utable: Ue,
+                    cgraph: Xe,
+                    linechart: gt
                 },
                 methods: {
                     log(e) {
                         console.log(e)
                     },
                     onAdded(e) {
                         0 !== e.length && (0 !== this.fileArr.length ? (this.$refs.uploaderRef.removeFile(this.fileArr[0]), this.fileArr.splice(0, 1, e[0])) : this.fileArr.push(e[0]))
                     },
                     sendMessage(e, t) {
-                        q([this.pdata["name"], this.data["name"], e, t])
+                        C([this.pdata["name"], this.data["name"], e, t])
                     },
                     pressedEnter() {
                         "update" in this.data && this.sendMessage("update", this.value)
                     },
                     updateDom(e) {
                         let t = e.files.length;
-                        t && (this.sendMessage("changed", e.files[t - 1].name), K())
+                        t && (this.sendMessage("changed", e.files[t - 1].name), V())
                     },
                     sendValue() {
                         this.sendMessage("changed", this.value)
                     },
                     switchValue() {
                         this.value = !this.value
                     },
                     setValue(e) {
                         this.value = e
                     },
                     complete(e, t, a) {
-                        this.value = e, A(this, e, (e => t((() => {
+                        this.value = e, S(this, e, (e => t((() => {
                             this.options = e
                         }))))
                     },
                     lens() {
-                        u.lens(this.data)
+                        h.lens(this.data)
                     },
                     toggleCamera() {
                         this.isCameraOpen ? (this.isCameraOpen = !1, this.isPhotoTaken = !1, this.isShotPhoto = !1, this.stopCameraStream()) : (this.isCameraOpen = !0, this.createCameraElement())
                     },
                     createCameraElement() {
                         this.isLoading = !0;
                         const e = window.constraints = {
@@ -1763,15 +1758,15 @@
                             }), e)
                         }
                         this.isPhotoTaken = !this.isPhotoTaken;
                         const e = this.$refs.canvas.getContext("2d");
                         e.drawImage(this.$refs.camera, 0, 0, 450, 337.5)
                     },
                     downloadImage() {
-                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(yt, "image/jpeg")
+                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(mt, "image/jpeg")
                     },
                     geom() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
                         e || (e = this.$el.previousElementSibling, e = "clientHeight" in e ? e : e.nextElementSibling);
                         let t = this.type;
                         const a = "docviewer" == t || "graph" == t || "linechart" == t ? e : e.querySelector("table" == t ? ".scroll" : ".q-tree"),
                             l = e.getBoundingClientRect();
@@ -1906,47 +1901,47 @@
                         0 == a.length && (a = t.getElementsByTagName("input")), a[0].setSelectionRange(e[0], e[1])
                     },
                     data(e, t) {
                         this.styleSize || (this.styleSize = w(this.data)), this.value = this.data.value, this.updated = this.value, k[this.fullname] = this
                     }
                 }
             });
-            var bt = a(4027),
-                kt = a(9721),
-                vt = a(8886),
-                xt = a(8761),
-                Ct = a(1232),
-                qt = a(5551),
-                _t = a(5869),
-                jt = a(1745);
-            const St = (0, U.Z)(wt, [
-                    ["render", _e],
-                    ["__scopeId", "data-v-2f472339"]
+            var yt = a(4027),
+                wt = a(9721),
+                bt = a(8886),
+                kt = a(8761),
+                vt = a(1232),
+                xt = a(5551),
+                Ct = a(5869),
+                qt = a(1745);
+            const _t = (0, Q.Z)(ft, [
+                    ["render", Ce],
+                    ["__scopeId", "data-v-047e5584"]
                 ]),
-                zt = St;
-            R()(wt, "components", {
-                QImg: bt.Z,
-                QIcon: P.Z,
-                QSelect: Ue.Z,
-                QBadge: kt.Z,
-                QCheckbox: He.Z,
-                QToggle: vt.Z,
-                QBtn: Ke.Z,
-                QBtnToggle: xt.Z,
-                QInput: Ve.Z,
-                QScrollArea: Ct.Z,
-                QTree: qt.Z,
-                QSeparator: _t.Z,
-                QUploader: jt.Z,
-                QTooltip: Ee.Z
+                jt = _t;
+            P()(ft, "components", {
+                QImg: yt.Z,
+                QIcon: N.Z,
+                QSelect: Qe.Z,
+                QBadge: wt.Z,
+                QCheckbox: We.Z,
+                QToggle: bt.Z,
+                QBtn: Ve.Z,
+                QBtnToggle: kt.Z,
+                QInput: Me.Z,
+                QScrollArea: vt.Z,
+                QTree: xt.Z,
+                QSeparator: Ct.Z,
+                QUploader: qt.Z,
+                QTooltip: $e.Z
             });
-            const At = (0, l.aZ)({
+            const St = (0, l.aZ)({
                 name: "block",
                 components: {
-                    element: zt
+                    element: jt
                 },
                 data() {
                     return {
                         styleSize: y,
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
@@ -2017,51 +2012,51 @@
                 },
                 watch: {
                     data(e) {
                         g && console.log("data update", this.name), this.styleSize = y, b[this.name] = this, this.expanding && (k[this.fullname] = this)
                     }
                 }
             });
-            var Zt = a(151);
-            const Dt = (0, U.Z)(At, [
-                    ["render", oe]
+            var zt = a(151);
+            const At = (0, Q.Z)(St, [
+                    ["render", se]
                 ]),
-                Mt = Dt;
-            R()(At, "components", {
-                QCard: Zt.Z,
-                QIcon: P.Z,
-                QScrollArea: Ct.Z
+                Zt = At;
+            P()(St, "components", {
+                QCard: zt.Z,
+                QIcon: N.Z,
+                QScrollArea: vt.Z
             });
-            const $t = (0, l.aZ)({
+            const Dt = (0, l.aZ)({
                     name: "zone",
                     components: {
-                        block: Mt
+                        block: Zt
                     },
                     props: {
                         data: Object
                     },
                     updated(e) {
                         (0, l.Y3)((() => {
                             requestAnimationFrame((() => {
                                 requestAnimationFrame((() => {
-                                    O()
+                                    K()
                                 }))
                             }))
                         }))
                     }
                 }),
-                Vt = (0, U.Z)($t, [
-                    ["render", J]
+                Mt = (0, Q.Z)(Dt, [
+                    ["render", X]
                 ]),
-                Et = Vt,
-                Kt = {
+                $t = Mt,
+                Vt = {
                     class: "row q-gutter-sm row-md"
                 };
 
-            function Ot(e, t, a, i, o, n) {
+            function Kt(e, t, a, i, o, n) {
                 const d = (0, l.up)("block"),
                     r = (0, l.up)("q-item-label"),
                     c = (0, l.up)("q-space"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-card"),
                     p = (0, l.up)("q-dialog");
                 return (0, l.wg)(), (0, l.j4)(p, {
@@ -2077,40 +2072,40 @@
                             key: 0,
                             data: a.data
                         }, null, 8, ["data"])) : (0, l.kq)("", !0), (0, l.Wm)(r, {
                             class: "text-h6"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(a.data.text ? a.data.text : ""), 1)])),
                             _: 1
-                        }), (0, l._)("div", Kt, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
+                        }), (0, l._)("div", Vt, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
                             class: "col-md-3",
                             label: e,
                             color: a.buttons[0] == e ? "primary" : "secondary",
                             onClick: t => n.sendMessage(e)
                         }, null, 8, ["label", "color", "onClick"])))), 256))])])),
                         _: 1
                     }, 8, ["style"])])),
                     _: 1
                 }, 8, ["onHide"])
             }
-            const Wt = {
+            const Et = {
                 props: {
                     data: Object,
                     buttons: Array
                 },
                 components: {
-                    block: Mt
+                    block: Zt
                 },
                 emits: ["ok", "hide"],
                 methods: {
                     show() {
                         this.$refs.dialog.show()
                     },
                     sendMessage(e) {
-                        this.data.internal || q([this.data["name"], e]), this.hide()
+                        this.data.internal || C([this.data["name"], e]), this.hide()
                     },
                     hide() {
                         this.$refs.dialog.hide()
                     },
                     onDialogHide() {
                         this.$emit("hide")
                     },
@@ -2118,29 +2113,29 @@
                         this.$emit("ok"), this.hide()
                     },
                     onCancelClick() {
                         this.hide()
                     }
                 }
             };
-            var Qt = a(5926),
-                Ht = a(2025);
-            const Ut = (0, U.Z)(Wt, [
-                    ["render", Ot]
+            var Ot = a(5926),
+                Wt = a(2025);
+            const Qt = (0, Q.Z)(Et, [
+                    ["render", Kt]
                 ]),
-                Nt = Ut;
-            R()(Wt, "components", {
-                QDialog: Qt.Z,
-                QCard: Zt.Z,
-                QItemLabel: T.Z,
-                QSpace: Ht.Z,
-                QBtn: Ke.Z
+                Ht = Qt;
+            P()(Et, "components", {
+                QDialog: Ot.Z,
+                QCard: zt.Z,
+                QItemLabel: F.Z,
+                QSpace: Wt.Z,
+                QBtn: Ve.Z
             });
-            let Ft = null;
-            const Pt = (0, l.aZ)({
+            let Ut = null;
+            const Nt = (0, l.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
                         menu: [],
                         tab: "",
                         tooldata: {
@@ -2150,41 +2145,41 @@
                         statusConnect: !1,
                         screen: {
                             blocks: []
                         }
                     }
                 },
                 components: {
-                    menubar: B,
-                    zone: Et,
-                    element: zt
+                    menubar: R,
+                    zone: $t,
+                    element: jt
                 },
                 created() {
-                    C(this)
+                    v(this)
                 },
                 unmounted() {
                     window.removeEventListener("resize", this.onResize)
                 },
                 methods: {
                     toggleLeftDrawer() {
                         this.leftDrawerOpen = !this.leftDrawerOpen
                     },
                     tabclick(e) {
-                        q(["root", e])
+                        C(["root", e])
                     },
                     onResize(e) {
-                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), K()
+                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), V()
                     },
                     lens(e) {
                         let t = {
                                 title: "Photo lens",
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0,
-                                component: Nt
+                                component: Ht
                             },
                             {
                                 height: a,
                                 ...l
                             } = e;
                         l.width = 750;
                         let s = {
@@ -2203,81 +2198,80 @@
                         let a = t,
                             l = {
                                 message: e,
                                 type: t,
                                 position: "top",
                                 icon: a
                             };
-                        "progress" == t ? null == Ft ? (l = {
+                        "progress" == t ? null == Ut ? (l = {
                             group: !1,
                             timeout: 0,
                             spinner: !0,
                             type: "info",
                             message: e || "Progress..",
                             position: "top",
                             color: "secondary"
-                        }, Ft = this.$q.notify(l)) : null == e ? (Ft(), Ft = null) : (l = {
+                        }, Ut = this.$q.notify(l)) : null == e ? (Ut(), Ut = null) : (l = {
                             caption: e
-                        }, Ft(l)) : ("error" == t && l.type, this.$q.notify(l))
+                        }, Ut(l)) : ("error" == t && l.type, this.$q.notify(l))
                     },
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
                     processMessage(e) {
-                        if ("screen" == e.type) this.screen.name != e.name && z(), Z(), this.screen = e, console.log(e), this.menu = e.menu.map((e => ({
+                        if ("screen" == e.type) this.screen.name != e.name && j(), z(), this.screen = e, this.menu = e.menu.map((e => ({
                             name: e[0],
                             icon: e[1],
                             order: e[2]
                         }))), this.tab = this.screen.name;
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0
                             };
-                            t.component = Nt, t.componentProps = {
+                            t.component = Ht, t.componentProps = {
                                 data: e.content ? e.content : e,
                                 buttons: e.buttons
                             }, this.$q.dialog(t)
-                        } else if (e.hasOwnProperty("answer")) $(e);
+                        } else if ("answer" == e.type) D(e);
                         else {
-                            e.update && M(e);
+                            e.updates && Z(e.updates);
                             let t = !1;
-                            for (let a of v) a in e && (this.notify(e[a], a), t = !0);
-                            t || e.update || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
+                            ["error", "progress", "warning", "info"].includes(e.type) && (this.notify(e.value, e.type), t = !0), t || e.update || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
                         }
-                        Ft && !e.progress && this.notify(null, "progress")
+                        Ut && "progress" != e.type && this.notify(null, "progress")
                     }
                 },
                 mounted() {
                     window.addEventListener("resize", this.onResize)
                 }
             });
-            var Tt = a(9214),
-                It = a(3812),
-                Rt = a(9570),
-                Lt = a(7547),
-                Bt = a(3269),
-                Yt = a(2652),
-                Xt = a(4379);
-            const Gt = (0, U.Z)(Pt, [
+            var Ft = a(9214),
+                Tt = a(3812),
+                Pt = a(9570),
+                It = a(7547),
+                Rt = a(3269),
+                Lt = a(2652),
+                Bt = a(4379);
+            const Yt = (0, Q.Z)(Nt, [
                     ["render", n]
                 ]),
-                Jt = Gt;
-            R()(Pt, "components", {
-                QLayout: Tt.Z,
-                QHeader: It.Z,
-                QToolbar: Rt.Z,
-                QBtn: Ke.Z,
-                QItemLabel: T.Z,
-                QTabs: Lt.Z,
-                QTab: Bt.Z,
-                QPageContainer: Yt.Z,
-                QPage: Xt.Z
+                Xt = Yt;
+            P()(Nt, "components", {
+                QLayout: Ft.Z,
+                QHeader: Tt.Z,
+                QToolbar: Pt.Z,
+                QBtn: Ve.Z,
+                QItemLabel: F.Z,
+                QTabs: It.Z,
+                QTab: Rt.Z,
+                QPageContainer: Lt.Z,
+                QPage: Bt.Z
             })
         }
     }
 ]);
```

### Comparing `unigui-1.8.1/unigui/web/js/193.283445be.js` & `unigui-1.8.2/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/unigui/web/js/vendor.3e8714c2.js` & `unigui-1.8.2/unigui/web/js/vendor.e1e2597e.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -37958,15 +37958,15 @@
                         var t = e.getData(),
                             n = e.getModel("lineStyle").getLineStyle();
                         n && !n.stroke && (n.stroke = t.getVisual("style").fill), t.setVisual("legendLineStyle", n)
                     }
                 }), e.registerProcessor(e.PRIORITY.PROCESSOR.STATISTIC, bt("line"))
             }
         },
-        6423: (e, t, n) => {
+        9806: (e, t, n) => {
             "use strict";
             n.d(t, {
                 Z: () => A
             });
             var r = n(3223),
                 i = n(841),
                 o = n(391),
@@ -39253,15 +39253,15 @@
             });
             var r = n(3223),
                 i = n(841),
                 o = n(850),
                 a = n(5162),
                 s = n(1926),
                 l = n(5226),
-                u = n(6423),
+                u = n(9806),
                 c = n(5865);
 
             function d(e) {
                 var t, n = e.get("type"),
                     r = e.getModel(n + "Style");
                 return "line" === n ? (t = r.getLineStyle(), t.fill = null) : "shadow" === n && (t = r.getAreaStyle(), t.stroke = null), t
             }
@@ -41741,15 +41741,15 @@
                     return r - e + t
                 }
             }
             const pe = ue;
             var ve = n(841),
                 ge = n(391),
                 me = n(4740),
-                ye = n(6423),
+                ye = n(9806),
                 be = n(4956),
                 _e = (0, d.Yf)();
 
             function xe(e, t, n, r) {
                 var i = n.axis;
                 if (!i.scale.isBlank()) {
                     var o = n.getModel("splitArea"),
```

### Comparing `unigui-1.8.1/unigui/web/index.html` & `unigui-1.8.2/unigui/web/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3e8714c2.js></script><script defer src=js/app.9384942b.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.e1e2597e.js></script><script defer src=js/app.eb412190.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.8.1/LICENSE` & `unigui-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/setup.py` & `unigui-1.8.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.8.1',      
+      version='1.8.2',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal GUI Framework and protocol',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
       url="https://github.com/Claus1/unigui" ,      
       include_package_data=True,
       install_requires=[
-          'websockets','jsonpickle', 'aiohttp'
+          'websockets','jsonpickle', 'aiohttp', 'watchdog'
       ],
       zip_safe=False)
```

### Comparing `unigui-1.8.1/PKG-INFO` & `unigui-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.8.1
+Version: 1.8.2
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.8.1/README.md` & `unigui-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `unigui-1.8.1/unigui.egg-info/PKG-INFO` & `unigui-1.8.2/unigui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.8.1
+Version: 1.8.2
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.8.1/unigui.egg-info/SOURCES.txt` & `unigui-1.8.2/unigui.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 MANIFEST.in
 README.md
 setup.py
 unigui/__init__.py
 unigui/guielements.py
 unigui/reloader.py
 unigui/server.py
-unigui/user.py
+unigui/users.py
 unigui/utils.py
 unigui.egg-info/PKG-INFO
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/295.f0f63b8f.css
+unigui/web/css/423.a6a82bd4.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.49a52e8f.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -28,11 +28,11 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.283445be.js
-unigui/web/js/295.e2b7be53.js
+unigui/web/js/423.0ad6769b.js
 unigui/web/js/430.591e9a73.js
-unigui/web/js/app.9384942b.js
-unigui/web/js/vendor.3e8714c2.js
+unigui/web/js/app.eb412190.js
+unigui/web/js/vendor.e1e2597e.js
```

