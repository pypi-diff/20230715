# Comparing `tmp/yunhu-0.0.5.tar.gz` & `tmp/yunhu-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunhu-0.0.5.tar", last modified: Thu Jul  6 07:28:21 2023, max compression
+gzip compressed data, was "yunhu-0.0.6.tar", last modified: Sat Jul 15 07:35:47 2023, max compression
```

## Comparing `yunhu-0.0.5.tar` & `yunhu-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 07:28:21.212881 yunhu-0.0.5/
--rw-rw-rw-   0        0        0     1094 2023-05-08 06:42:50.000000 yunhu-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      610 2023-07-06 07:28:21.212881 yunhu-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-05-08 06:42:00.000000 yunhu-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 07:28:21.203725 yunhu-0.0.5/example_yunhu/
--rw-rw-rw-   0        0        0        0 2023-04-24 04:05:16.000000 yunhu-0.0.5/example_yunhu/__init__.py
--rw-rw-rw-   0        0        0     2424 2023-05-08 08:56:14.000000 yunhu-0.0.5/example_yunhu/flask_demo.py
--rw-rw-rw-   0        0        0      316 2023-07-06 07:26:41.000000 yunhu-0.0.5/example_yunhu/set_board_demo.py
--rw-rw-rw-   0        0        0      426 2023-07-06 07:25:02.000000 yunhu-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-06 07:28:21.213802 yunhu-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      725 2023-07-06 07:24:55.000000 yunhu-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 07:28:21.207633 yunhu-0.0.5/yunhu/
--rw-rw-rw-   0        0        0        0 2023-05-08 09:46:54.000000 yunhu-0.0.5/yunhu/__init__.py
--rw-rw-rw-   0        0        0       69 2023-05-08 01:21:22.000000 yunhu-0.0.5/yunhu/main.py
--rw-rw-rw-   0        0        0     4551 2023-07-06 07:21:44.000000 yunhu-0.0.5/yunhu/openapi.py
--rw-rw-rw-   0        0        0     2460 2023-05-08 11:27:24.000000 yunhu-0.0.5/yunhu/subscription.py
-drwxrwxrwx   0        0        0        0 2023-07-06 07:28:21.211854 yunhu-0.0.5/yunhu.egg-info/
--rw-rw-rw-   0        0        0      610 2023-07-06 07:28:21.000000 yunhu-0.0.5/yunhu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-07-06 07:28:21.000000 yunhu-0.0.5/yunhu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 07:28:21.000000 yunhu-0.0.5/yunhu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-06 07:28:21.000000 yunhu-0.0.5/yunhu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 07:35:47.406282 yunhu-0.0.6/
+-rw-rw-rw-   0        0        0     1094 2023-05-08 06:42:50.000000 yunhu-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      610 2023-07-15 07:35:47.405282 yunhu-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-05-08 06:42:00.000000 yunhu-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 07:35:47.395284 yunhu-0.0.6/example_yunhu/
+-rw-rw-rw-   0        0        0        0 2023-04-24 04:05:16.000000 yunhu-0.0.6/example_yunhu/__init__.py
+-rw-rw-rw-   0        0        0     2074 2023-07-12 09:30:03.000000 yunhu-0.0.6/example_yunhu/flask_demo.py
+-rw-rw-rw-   0        0        0      210 2023-07-15 07:32:07.000000 yunhu-0.0.6/example_yunhu/set_board_demo.py
+-rw-rw-rw-   0        0        0      426 2023-07-15 07:35:27.000000 yunhu-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-15 07:35:47.406282 yunhu-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      725 2023-07-15 07:35:20.000000 yunhu-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 07:35:47.400283 yunhu-0.0.6/yunhu/
+-rw-rw-rw-   0        0        0        0 2023-05-08 09:46:54.000000 yunhu-0.0.6/yunhu/__init__.py
+-rw-rw-rw-   0        0        0       69 2023-05-08 01:21:22.000000 yunhu-0.0.6/yunhu/main.py
+-rw-rw-rw-   0        0        0     4801 2023-07-15 07:33:42.000000 yunhu-0.0.6/yunhu/openapi.py
+-rw-rw-rw-   0        0        0     2460 2023-05-08 11:27:24.000000 yunhu-0.0.6/yunhu/subscription.py
+drwxrwxrwx   0        0        0        0 2023-07-15 07:35:47.404282 yunhu-0.0.6/yunhu.egg-info/
+-rw-rw-rw-   0        0        0      610 2023-07-15 07:35:47.000000 yunhu-0.0.6/yunhu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-07-15 07:35:47.000000 yunhu-0.0.6/yunhu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 07:35:47.000000 yunhu-0.0.6/yunhu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-15 07:35:47.000000 yunhu-0.0.6/yunhu.egg-info/top_level.txt
```

### Comparing `yunhu-0.0.5/LICENSE.txt` & `yunhu-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yunhu-0.0.5/PKG-INFO` & `yunhu-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunhu
-Version: 0.0.5
+Version: 0.0.6
 Summary: 云湖官方Python SDK
 Author: yunhu
 Author-email: yunhu <1114110051@qq.com>
 Project-URL: Homepage, https://github.com/yhchat/bot-python-sdk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yunhu-0.0.5/setup.py` & `yunhu-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="yunhu", 
-    version="0.0.5", 
+    version="0.0.6", 
     author="yunhu",  
     description="云湖官方Python SDK", #包的简述
     author_email="1114110051@qq.com",    
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yunhu-0.0.5/yunhu/openapi.py` & `yunhu-0.0.6/yunhu/openapi.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,22 +49,29 @@
         """
         return self.batchSendMessage(recvIds, recvType, "markdown", content)
     
     def batchSendMessage(self, recvIds: list, recvType: str, contentType: str, content: map):
         """
         批量，批量发送消息
         """
-        params = {
-            "recvIds": recvIds, 
-            "recvType": recvType, 
-            "contentType": contentType, 
-            "content": content
-         }
-        headers = {'Content-Type': 'application/json'}
-        return requests.post(self.baseUrl + '/bot/batch_send?token=' + self.token,headers=headers, data=json.dumps(params))
+        batchCount = 200
+        recvIdss =  [recvIds[i:i+batchCount] for i in range(0, len(recvIds), batchCount)]
+        resList = []
+        for l in recvIdss:
+            params = {
+                "recvIds": l, 
+                "recvType": recvType, 
+                "contentType": contentType, 
+                "content": content
+            }
+            headers = {'Content-Type': 'application/json'}
+            res = requests.post(self.baseUrl + '/bot/batch_send?token=' + self.token,headers=headers, data=json.dumps(params))
+            resList.append(res)
+        return resList
+
     
     def editMessage(self, msgId: str, recvId: str, recvType: str, contentType: str, content: map):
         """
         单条，编辑单条消息
         """
         params = {
             "msgId": msgId,
```

### Comparing `yunhu-0.0.5/yunhu/subscription.py` & `yunhu-0.0.6/yunhu/subscription.py`

 * *Files identical despite different names*

### Comparing `yunhu-0.0.5/yunhu.egg-info/PKG-INFO` & `yunhu-0.0.6/yunhu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunhu
-Version: 0.0.5
+Version: 0.0.6
 Summary: 云湖官方Python SDK
 Author: yunhu
 Author-email: yunhu <1114110051@qq.com>
 Project-URL: Homepage, https://github.com/yhchat/bot-python-sdk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

