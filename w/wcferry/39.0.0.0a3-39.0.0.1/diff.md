# Comparing `tmp/wcferry-39.0.0.0a3.tar.gz` & `tmp/wcferry-39.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcferry-39.0.0.0a3.tar", last modified: Wed Jul 12 15:06:01 2023, max compression
+gzip compressed data, was "wcferry-39.0.0.1.tar", last modified: Fri Jul 14 22:38:02 2023, max compression
```

## Comparing `wcferry-39.0.0.0a3.tar` & `wcferry-39.0.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 15:06:01.954843 wcferry-39.0.0.0a3/
--rw-rw-rw-   0        0        0       46 2023-03-10 16:21:28.000000 wcferry-39.0.0.0a3/MANIFEST.in
--rw-rw-rw-   0        0        0     5678 2023-07-12 15:06:01.939217 wcferry-39.0.0.0a3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-12 15:06:01.954843 wcferry-39.0.0.0a3/setup.cfg
--rw-rw-rw-   0        0        0     1290 2023-05-10 03:10:59.000000 wcferry-39.0.0.0a3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:06:01.939217 wcferry-39.0.0.0a3/wcferry/
--rw-rw-rw-   0        0        0      105 2023-05-04 13:34:55.000000 wcferry-39.0.0.0a3/wcferry/__init__.py
--rw-rw-rw-   0        0        0    19904 2023-07-12 15:05:51.000000 wcferry-39.0.0.0a3/wcferry/client.py
--rw-rw-rw-   0        0        0   634880 2023-07-12 14:59:48.000000 wcferry-39.0.0.0a3/wcferry/spy.dll
--rw-rw-rw-   0        0        0  1163776 2023-07-12 14:39:45.000000 wcferry-39.0.0.0a3/wcferry/spy_debug.dll
--rwxrwxrwx   0        0        0   162816 2023-07-12 15:00:02.000000 wcferry-39.0.0.0a3/wcferry/wcf.exe
--rw-rw-rw-   0        0        0     7362 2023-07-11 12:13:26.000000 wcferry-39.0.0.0a3/wcferry/wcf_pb2.py
--rw-rw-rw-   0        0        0     2055 2023-05-10 03:43:35.000000 wcferry-39.0.0.0a3/wcferry/wxmsg.py
-drwxrwxrwx   0        0        0        0 2023-07-12 15:06:01.939217 wcferry-39.0.0.0a3/wcferry.egg-info/
--rw-rw-rw-   0        0        0     5678 2023-07-12 15:06:01.000000 wcferry-39.0.0.0a3/wcferry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-07-12 15:06:01.000000 wcferry-39.0.0.0a3/wcferry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 15:06:01.000000 wcferry-39.0.0.0a3/wcferry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-12 15:06:01.000000 wcferry-39.0.0.0a3/wcferry.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-12 15:06:01.000000 wcferry-39.0.0.0a3/wcferry.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-14 22:38:02.023551 wcferry-39.0.0.1/
+-rw-rw-rw-   0        0        0       46 2023-03-10 16:21:28.000000 wcferry-39.0.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5473 2023-07-14 22:38:02.022549 wcferry-39.0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-14 22:38:02.023551 wcferry-39.0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1290 2023-05-10 03:10:59.000000 wcferry-39.0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-14 22:38:02.010550 wcferry-39.0.0.1/wcferry/
+-rw-rw-rw-   0        0        0      105 2023-05-04 13:34:55.000000 wcferry-39.0.0.1/wcferry/__init__.py
+-rw-rw-rw-   0        0        0    19902 2023-07-14 22:37:54.000000 wcferry-39.0.0.1/wcferry/client.py
+-rw-rw-rw-   0        0        0   634880 2023-07-14 22:29:13.000000 wcferry-39.0.0.1/wcferry/spy.dll
+-rw-rw-rw-   0        0        0  1163776 2023-07-14 22:31:26.000000 wcferry-39.0.0.1/wcferry/spy_debug.dll
+-rwxrwxrwx   0        0        0   162816 2023-07-14 22:29:27.000000 wcferry-39.0.0.1/wcferry/wcf.exe
+-rw-rw-rw-   0        0        0     7362 2023-07-11 12:13:26.000000 wcferry-39.0.0.1/wcferry/wcf_pb2.py
+-rw-rw-rw-   0        0        0     2055 2023-05-10 03:43:35.000000 wcferry-39.0.0.1/wcferry/wxmsg.py
+drwxrwxrwx   0        0        0        0 2023-07-14 22:38:02.020553 wcferry-39.0.0.1/wcferry.egg-info/
+-rw-rw-rw-   0        0        0     5473 2023-07-14 22:38:01.000000 wcferry-39.0.0.1/wcferry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-07-14 22:38:01.000000 wcferry-39.0.0.1/wcferry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-14 22:38:01.000000 wcferry-39.0.0.1/wcferry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-14 22:38:01.000000 wcferry-39.0.0.1/wcferry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-14 22:38:01.000000 wcferry-39.0.0.1/wcferry.egg-info/top_level.txt
```

### Comparing `wcferry-39.0.0.0a3/PKG-INFO` & `wcferry-39.0.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcferry
-Version: 39.0.0.0a3
+Version: 39.0.0.1
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WeChatFerry Python 客户端
 [![PyPi](https://img.shields.io/pypi/v/wcferry.svg)](https://pypi.python.org/pypi/wcferry) [![Downloads](https://static.pepy.tech/badge/wcferry)](https://pypi.python.org/pypi/wcferry) [![Documentation Status](https://readthedocs.org/projects/wechatferry/badge/?version=latest)](https://wechatferry.readthedocs.io/zh/latest/?badge=latest)
 
-|[📖 文档](https://wechatferry.readthedocs.io/)|[📺 视频教程](https://mp.weixin.qq.com/s/APdjGyZ2hllXxyG_sNCfXQ)|[🙋 FAQ](https://mp.weixin.qq.com/s/XTJ9H-FsCPCscixAts8i_A)|
+|[📖 文档](https://wechatferry.readthedocs.io/)|[📺 视频教程](https://mp.weixin.qq.com/s/APdjGyZ2hllXxyG_sNCfXQ)|[🙋 FAQ](https://mp.weixin.qq.com/s/vAGpn1C9stI8Xzt1hUJhLA)|
 |:-:|:-:|:-:|
 
 🤖示例机器人框架：[WeChatRobot](https://github.com/lich0821/WeChatRobot)。
 
 ## 快速开始
 ```sh
 pip install --upgrade wcferry
@@ -54,52 +54,60 @@
             continue
 
         LOG.info(msg)  # 简单打印
 
 
 def main():
     LOG.info("Start demo...")
-    wcf = Wcf(debug=True)             # 默认连接本地服务
+    wcf = Wcf(debug=True)
 
     sleep(5)  # 等微信加载好，以免信息显示异常
     LOG.info(f"已经登录: {True if wcf.is_login() else False}")
     LOG.info(f"wxid: {wcf.get_self_wxid()}")
 
     # 允许接收消息
     # wcf.enable_recv_msg(LOG.info) # deprecated
 
     # 允许接收消息
     wcf.enable_receiving_msg()
     Thread(target=process_msg, name="GetMessage", args=(wcf,), daemon=True).start()
 
     # wcf.disable_recv_msg() # 当需要停止接收消息时调用
-
+    sleep(5)
     ret = wcf.send_text("Hello world.", "filehelper")
     LOG.info(f"send_text: {ret}")
 
-    ret = wcf.send_image("TEQuant.jpeg", "filehelper")  # 需要确保图片路径正确
+    sleep(5)
+    ret = wcf.send_image("TEQuant.jpeg", "filehelper")  # 需要确保图片路径正确，建议使用绝对路径（使用双斜杠\\）
     LOG.info(f"send_image: {ret}")
 
-    ret = wcf.send_file("README.MD", "filehelper")  # 需要确保文件路径正确
+    sleep(5)
+    ret = wcf.send_file("README.MD", "filehelper")  # 需要确保文件路径正确，建议使用绝对路径（使用双斜杠\\）
     LOG.info(f"send_file: {ret}")
 
+    sleep(5)
     LOG.info(f"Message types:\n{wcf.get_msg_types()}")
     LOG.info(f"Contacts:\n{wcf.get_contacts()}")
 
+    sleep(5)
     LOG.info(f"DBs:\n{wcf.get_dbs()}")
-    LOG.info(f"Tables:\n{wcf.get_tables('db')}")
+    LOG.info(f"Tables:\n{wcf.get_tables('MicroMsg.db')}")
     LOG.info(f"Results:\n{wcf.query_sql('MicroMsg.db', 'SELECT * FROM Contact LIMIT 1;')}")
 
     # 需要真正的 V3、V4 信息
     # wcf.accept_new_friend("v3", "v4")
 
-    # 填写正确的群 ID 和成员 wxid
+    # 添加群成员，填写正确的群 ID 和成员 wxid
     # ret = wcf.add_chatroom_members("chatroom id", "wxid1,wxid2,wxid3,...")
     # LOG.info(f"add_chatroom_members: {ret}")
 
+    # 删除群成员，填写正确的群 ID 和成员 wxid
+    # ret = wcf.del_chatroom_members("chatroom id", "wxid1,wxid2,wxid3,...")
+    # LOG.info(f"add_chatroom_members: {ret}")
+
     # 一直运行
     wcf.keep_running()
 
 
 if __name__ == "__main__":
     main()
 
@@ -138,57 +146,31 @@
 
 其中：
 * `w` 是微信的大版本号，如 `37` (3.7.a.a), `38` (3.8.a.a), `39` (3.9.a.a)
 * `x` 是适配的微信的小版本号，从 0 开始
 * `y` 是 `WeChatFerry` 的版本，从 0 开始
 * `z` 是各客户端的版本，从 0 开始
 
-### 39.0.0.0a0 (2023.07.11)
-支持微信 `3.9.2.23`。
+### 39.0.0.1 (2023.07.15)
+修复不能 @ 问题。
 
 功能：
 
 * 检查登录状态
 * 获取登录账号的 wxid
 * 获取消息类型
 * 获取所有联系人
 * 获取所有好友
 * 获取数据库
 * 获取某数据库下的表
+* 获取用户信息
 * 发送文本消息（可 @）
 * 发送图片（Python 客户端支持网络路径）
 * 发送文件
 * 允许接收消息
 * 停止接收消息
 * 执行 SQL 查询
 * 接受好友申请
 * 添加群成员
+* 删除群成员
 * 解密图片
 * 某功能（Breaking Change）
-
-<details><summary>历史更新</summary>
-
-### 37.1.25.5 (2023.05.19)
-支持 `3.7.0.30` 的最后一个版本。
-
-功能：
-
-* 检查登录状态
-* 获取登录账号的 wxid
-* 获取消息类型
-* 获取所有联系人
-* 获取所有好友
-* 获取数据库
-* 获取某数据库下的表
-* 发送文本消息（可 @）
-* 发送图片（Python 客户端支持网络路径）
-* 发送文件
-* 发送 XML
-* 发送表情
-* 允许接收消息
-* 停止接收消息
-* 执行 SQL 查询
-* 接受好友申请
-* 添加群成员
-* 解密图片
-* 某功能
-</details>
```

### Comparing `wcferry-39.0.0.0a3/setup.py` & `wcferry-39.0.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `wcferry-39.0.0.0a3/wcferry/client.py` & `wcferry-39.0.0.1/wcferry/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 
-__version__ = "39.0.0.0a3"
+__version__ = "39.0.0.1"
 
 import atexit
 import base64
 import logging
 import os
 import re
 import sys
@@ -232,15 +232,15 @@
 
     def send_text(self, msg: str, receiver: str, aters: Optional[str] = "") -> int:
         """发送文本消息
 
         Args:
             msg (str): 要发送的消息，换行使用 `\\n`；如果 @ 人的话，需要带上跟 `aters` 里数量相同的 @
             receiver (str): 消息接收人，wxid 或者 roomid
-            aters (str): 要 @ 的 wxid，多个用逗号分隔；`@所有人` 只需要 `nofity@all`
+            aters (str): 要 @ 的 wxid，多个用逗号分隔；`@所有人` 只需要 `notify@all`
 
         Returns:
             int: 0 为成功，其他失败
         """
         req = wcf_pb2.Request()
         req.func = wcf_pb2.FUNC_SEND_TXT  # FUNC_SEND_TXT
         req.txt.msg = msg
```

### Comparing `wcferry-39.0.0.0a3/wcferry/spy.dll` & `wcferry-39.0.0.1/wcferry/spy.dll`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 000000c0: d829 8b4f 255c 8f4e d829 8a4f 1b5c 8f4e  .).O%\.N.).O.\.N
 000000d0: 0e37 8e4f 155c 8f4e 1a5c 8e4e fa5c 8f4e  .7.O.\.N.\.N.\.N
 000000e0: d829 874f 095c 8f4e d829 8f4f 1b5c 8f4e  .).O.\.N.).O.\.N
 000000f0: d829 704e 1b5c 8f4e 1a5c 184e 1b5c 8f4e  .)pN.\.N.\.N.\.N
 00000100: d829 8d4f 1b5c 8f4e 5269 6368 1a5c 8f4e  .).O.\.NRich.\.N
 00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000120: 0000 0000 0000 0000 5045 0000 4c01 0500  ........PE..L...
-00000130: e4bf ae64 0000 0000 0000 0000 e000 0221  ...d...........!
+00000130: 39cc b164 0000 0000 0000 0000 e000 0221  9..d...........!
 00000140: 0b01 0e1d 0074 0700 0052 0202 0000 0000  .....t...R......
 00000150: 6a18 0500 0010 0000 0090 0700 0000 0010  j...............
 00000160: 0010 0000 0002 0000 0600 0000 0000 0000  ................
 00000170: 0600 0000 0000 0000 0000 0a02 0004 0000  ................
 00000180: 0000 0000 0200 4001 0000 1000 0010 0000  ......@.........
 00000190: 0000 1000 0010 0000 0000 0000 1000 0000  ................
 000001a0: 2017 0900 5800 0000 7817 0900 a000 0000   ...X...x.......
@@ -35089,21 +35089,21 @@
 00089100: 0000 0000 0600 0000 0400 0000 0200 0000  ................
 00089110: 0000 0000 1200 0000 0c00 0000 0600 0000  ................
 00089120: 0000 0000 7f00 0000 1f00 0000 0f00 0000  ................
 00089130: 0000 0000 0000 0000 0000 0000 0000 f041  ...............A
 00089140: 0000 0000 0000 0080 0000 0000 0000 0080  ................
 00089150: 0000 0080 0000 0080 0000 0080 0000 0080  ................
 00089160: ffff ffff 0000 c03f 0000 0000 0000 0000  .......?........
-00089170: 0000 0000 0000 f041 0000 0000 e4bf ae64  .......A.......d
+00089170: 0000 0000 0000 f041 0000 0000 39cc b164  .......A....9..d
 00089180: 0000 0000 0200 0000 3d00 0000 6cdb 0800  ........=...l...
-00089190: 6cc3 0800 0000 0000 e4bf ae64 0000 0000  l..........d....
+00089190: 6cc3 0800 0000 0000 39cc b164 0000 0000  l.......9..d....
 000891a0: 0c00 0000 1400 0000 acdb 0800 acc3 0800  ................
-000891b0: 0000 0000 e4bf ae64 0000 0000 0d00 0000  .......d........
+000891b0: 0000 0000 39cc b164 0000 0000 0d00 0000  ....9..d........
 000891c0: 9803 0000 c0db 0800 c0c3 0800 0000 0000  ................
-000891d0: e4bf ae64 0000 0000 0e00 0000 0000 0000  ...d............
+000891d0: 39cc b164 0000 0000 0e00 0000 0000 0000  9..d............
 000891e0: 0000 0000 0000 0000 bc00 0000 0000 0000  ................
 000891f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00089200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00089210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00089220: 0000 0000 d43b 0910 74d8 0810 a400 0000  .....;..t.......
 00089230: b092 0710 0000 0000 0000 0000 0000 0000  ................
 00089240: 0001 0000 0000 0000 0000 0000 0000 0000  ................
@@ -35889,15 +35889,15 @@
 0008c300: 8d81 0700 1800 0000 0280 0280 1cdb 0800  ................
 0008c310: 4000 0000 5cdb 0800 1000 0000 b534 0300  @...\........4..
 0008c320: b934 0300 c84b 0300 cd4b 0300 284c 0300  .4...K...K..(L..
 0008c330: 2d4c 0300 b64c 0300 ba4c 0300 f84c 0300  -L...L...L...L..
 0008c340: fd4c 0300 284d 0300 2d4d 0300 704d 0300  .L..(M..-M..pM..
 0008c350: 754d 0300 c44d 0300 c84d 0300 401e 0300  uM...M...M..@...
 0008c360: 32f0 0100 607f 0700 aa01 0000 5253 4453  2...`.......RSDS
-0008c370: e2a3 2316 625f 9c40 af06 5b7d 0722 071c  ..#.b_.@..[}."..
+0008c370: a9e9 c1df 78af 3845 9475 244b 66c8 8d3c  ....x.8E.u$Kf..<
 0008c380: 0100 0000 433a 5c50 726f 6a73 5c57 6543  ....C:\Projs\WeC
 0008c390: 6861 7446 6572 7279 5c52 656c 6561 7365  hatFerry\Release
 0008c3a0: 5c73 7079 2e70 6462 0000 0000 0000 0000  \spy.pdb........
 0008c3b0: 8501 0000 8501 0000 1300 0000 3201 0000  ............2...
 0008c3c0: 4743 544c 0010 0000 f000 0000 2e74 6578  GCTL.........tex
 0008c3d0: 7424 6469 0000 0000 f010 0000 803f 0700  t$di.........?..
 0008c3e0: 2e74 6578 7424 6d6e 0000 0000 7050 0700  .text$mn....pP..
```

### Comparing `wcferry-39.0.0.0a3/wcferry/spy_debug.dll` & `wcferry-39.0.0.1/wcferry/spy_debug.dll`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 000000a0: 2d5e 9518 2135 9119 6b40 9418 6c35 9119  -^..!5..k@..l5..
 000000b0: 6b40 9518 2935 9119 6b40 9218 2335 9119  k@..)5..k@..#5..
 000000c0: 2d5e 9018 3635 9119 3935 9019 d835 9119  -^..65..95...5..
 000000d0: fb40 9518 7a35 9119 fb40 9418 2935 9119  .@..z5...@..)5..
 000000e0: fb40 9118 3835 9119 fb40 6e19 3835 9119  .@..85...@n.85..
 000000f0: 3935 0619 3835 9119 fb40 9318 3835 9119  95..85...@..85..
 00000100: 5269 6368 3935 9119 0000 0000 0000 0000  Rich95..........
-00000110: 5045 0000 4c01 0600 30bb ae64 0000 0000  PE..L...0..d....
+00000110: 5045 0000 4c01 0600 bdcc b164 0000 0000  PE..L......d....
 00000120: 0000 0000 e000 0221 0b01 0e1d 00de 0e00  .......!........
 00000130: 00fa 1202 0000 0000 db32 0c00 0010 0000  .........2......
 00000140: 00f0 0e00 0000 0010 0010 0000 0002 0000  ................
 00000150: 0600 0000 0000 0000 0600 0000 0000 0000  ................
 00000160: 0020 2202 0004 0000 0000 0000 0200 4001  . "...........@.
 00000170: 0000 1000 0010 0000 0000 1000 0010 0000  ................
 00000180: 0000 0000 1000 0000 90d4 1000 6000 0000  ............`...
@@ -65643,18 +65643,18 @@
 001006a0: 0000 0000 e01a cd3f 0000 0000 e01a cd3f  .......?.......?
 001006b0: 0000 0000 60e3 cc3f 0000 0000 60e3 cc3f  ....`..?....`..?
 001006c0: 0000 0000 f0a4 cc3f 0000 0000 f0a4 cc3f  .......?.......?
 001006d0: 0000 0000 706d cc3f 0000 0000 706d cc3f  ....pm.?....pm.?
 001006e0: 0000 0000 002f cc3f 0000 0000 002f cc3f  ...../.?...../.?
 001006f0: 0000 0000 80f7 cb3f 0000 0000 80f7 cb3f  .......?.......?
 00100700: 0000 0000 00c0 cb3f 0000 0000 00c0 cb3f  .......?.......?
-00100710: 0000 0000 30bb ae64 0000 0000 0200 0000  ....0..d........
+00100710: 0000 0000 bdcc b164 0000 0000 0200 0000  .......d........
 00100720: 4100 0000 2c65 1000 2c57 1000 0000 0000  A...,e..,W......
-00100730: 30bb ae64 0000 0000 0c00 0000 1400 0000  0..d............
-00100740: 7065 1000 7057 1000 0000 0000 30bb ae64  pe..pW......0..d
+00100730: bdcc b164 0000 0000 0c00 0000 1400 0000  ...d............
+00100740: 7065 1000 7057 1000 0000 0000 bdcc b164  pe..pW.........d
 00100750: 0000 0000 0d00 0000 ac03 0000 8465 1000  .............e..
 00100760: 8457 1000 0000 0000 bc00 0000 0000 0000  .W..............
 00100770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00100780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00100790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 001007a0: 0000 0000 7402 1110 0845 1010 ad01 0000  ....t....E......
 001007b0: b4f2 0e10 0000 0000 0000 0000 0000 0000  ................
@@ -66925,15 +66925,15 @@
 001056c0: 37e4 0e00 44e4 0e00 9ae4 0e00 a7e4 0e00  7...D...........
 001056d0: f7e4 0e00 5be5 0e00 68e5 0e00 b0e5 0e00  ....[...h.......
 001056e0: bde5 0e00 2be6 0e00 38e6 0e00 88e6 0e00  ....+...8.......
 001056f0: 1ce7 0e00 85e7 0e00 92e7 0e00 ede7 0e00  ................
 00105700: fae7 0e00 4de8 0e00 5ae8 0e00 0010 0000  ....M...Z.......
 00105710: ac01 0000 0012 0000 c211 0c00 9071 0e00  .............q..
 00105720: 8a78 0000 00eb 0e00 f501 0000 5253 4453  .x..........RSDS
-00105730: 278d dd9e 5b26 a945 a8c1 6461 f009 3cc1  '...[&.E..da..<.
+00105730: a2a0 749b 01e6 8f4b a970 4331 c5ef 0fa3  ..t....K.pC1....
 00105740: 0100 0000 433a 5c50 726f 6a73 5c57 6543  ....C:\Projs\WeC
 00105750: 6861 7446 6572 7279 5c44 6562 7567 5c73  hatFerry\Debug\s
 00105760: 7079 5f64 6562 7567 2e70 6462 0000 0000  py_debug.pdb....
 00105770: 0000 0000 8e01 0000 8e01 0000 1300 0000  ................
 00105780: 3b01 0000 0000 0000 0010 0000 0002 0000  ;...............
 00105790: 2e74 6578 7424 6469 0000 0000 0012 0000  .text$di........
 001057a0: 905f 0e00 2e74 6578 7424 6d6e 0000 0000  ._...text$mn....
```

### Comparing `wcferry-39.0.0.0a3/wcferry/wcf.exe` & `wcferry-39.0.0.1/wcferry/wcf.exe`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 000000a0: f834 8150 f45f 8551 be2a 8050 be5f 8551  .4.P._.Q.*.P._.Q
 000000b0: be2a 8150 fd5f 8551 be2a 8650 fb5f 8551  .*.P._.Q.*.P._.Q
 000000c0: 2e2a 8050 ed5f 8551 f834 8450 e75f 8551  .*.P._.Q.4.P._.Q
 000000d0: ec5f 8451 5b5f 8551 2e2a 8c50 e95f 8551  ._.Q[_.Q.*.P._.Q
 000000e0: 2e2a 7a51 ed5f 8551 2e2a 8750 ed5f 8551  .*zQ._.Q.*.P._.Q
 000000f0: 5269 6368 ec5f 8551 0000 0000 0000 0000  Rich._.Q........
 00000100: 0000 0000 0000 0000 5045 0000 4c01 0500  ........PE..L...
-00000110: f2bf ae64 0000 0000 0000 0000 e000 0201  ...d............
+00000110: 47cc b164 0000 0000 0000 0000 e000 0201  G..d............
 00000120: 0b01 0e1d 0084 0100 0004 0100 0000 0000  ................
 00000130: 653a 0000 0010 0000 00a0 0100 0000 4000  e:............@.
 00000140: 0010 0000 0002 0000 0600 0000 0000 0000  ................
 00000150: 0600 0000 0000 0000 00c0 0200 0004 0000  ................
 00000160: 0000 0000 0300 4081 0000 1000 0010 0000  ......@.........
 00000170: 0000 1000 0010 0000 0000 0000 1000 0000  ................
 00000180: 0000 0000 0000 0000 8c61 0200 6400 0000  .........a..d...
@@ -9051,21 +9051,21 @@
 000235a0: 7420 5b64 6562 7567 5d0a b9d8 b1d5 3a20  t [debug].....: 
 000235b0: 7763 662e 6578 6520 7374 6f70 0a70 6f72  wcf.exe stop.por
 000235c0: 743a 20c3 fcc1 eeb6 cbbf da2c 20cf fbcf  t: ........, ...
 000235d0: a2b6 cbbf dace aac3 fcc1 eeb6 cbbf da2b  ...............+
 000235e0: 310a 0000 7374 6172 7400 0000 7374 6f70  1...start...stop
 000235f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00023600: ffff ffff 0000 c03f 0000 0000 0000 0000  .......?........
-00023610: 0000 0000 0000 f041 0000 0000 f2bf ae64  .......A.......d
+00023610: 0000 0000 0000 f041 0000 0000 47cc b164  .......A....G..d
 00023620: 0000 0000 0200 0000 3d00 0000 1854 0200  ........=....T..
-00023630: 183c 0200 0000 0000 f2bf ae64 0000 0000  .<.........d....
+00023630: 183c 0200 0000 0000 47cc b164 0000 0000  .<......G..d....
 00023640: 0c00 0000 1400 0000 5854 0200 583c 0200  ........XT..X<..
-00023650: 0000 0000 f2bf ae64 0000 0000 0d00 0000  .......d........
+00023650: 0000 0000 47cc b164 0000 0000 0d00 0000  ....G..d........
 00023660: b003 0000 6c54 0200 6c3c 0200 0000 0000  ....lT..l<......
-00023670: f2bf ae64 0000 0000 0e00 0000 0000 0000  ...d............
+00023670: 47cc b164 0000 0000 0e00 0000 0000 0000  G..d............
 00023680: 0000 0000 0000 0000 bc00 0000 0000 0000  ................
 00023690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000236a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000236b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000236c0: 0000 0000 1470 4200 c053 4200 0e00 0000  .....pB..SB.....
 000236d0: 90a1 4100 0000 0000 0000 0000 0000 0000  ..A.............
 000236e0: 0001 0000 0000 0000 0000 0000 0000 0000  ................
@@ -9147,16 +9147,16 @@
 00023ba0: 0000 0000 4000 0000 8052 4200 0000 0000  ....@....RB.....
 00023bb0: 0000 0000 0000 0000 6c7b 4200 a452 4200  ........l{B..RB.
 00023bc0: 364a 0000 d34a 0000 c056 0000 f067 0000  6J...J...V...g..
 00023bd0: 958f 0100 cd8f 0100 fd8f 0100 3090 0100  ............0...
 00023be0: 7390 0100 9d90 0100 e390 0100 2791 0100  s...........'...
 00023bf0: 7e91 0100 a591 0100 1800 0000 0280 0280  ~...............
 00023c00: 0000 0000 0000 0000 1054 0200 0800 0000  .........T......
-00023c10: 8034 0000 1900 0000 5253 4453 ff28 1dc6  .4......RSDS.(..
-00023c20: 8d3f 1f4c b978 c1ce 991a 34e6 0100 0000  .?.L.x....4.....
+00023c10: 8034 0000 1900 0000 5253 4453 f117 608d  .4......RSDS..`.
+00023c20: a514 554f a200 806e 5cc2 b83e 0100 0000  ..UO...n\..>....
 00023c30: 433a 5c50 726f 6a73 5c57 6543 6861 7446  C:\Projs\WeChatF
 00023c40: 6572 7279 5c52 656c 6561 7365 5c77 6366  erry\Release\wcf
 00023c50: 2e70 6462 0000 0000 0000 0000 3301 0000  .pdb........3...
 00023c60: 3301 0000 0500 0000 2d01 0000 4743 544c  3.......-...GCTL
 00023c70: 0010 0000 5000 0000 2e74 6578 7424 6469  ....P....text$di
 00023c80: 0000 0000 5010 0000 307f 0100 2e74 6578  ....P...0....tex
 00023c90: 7424 6d6e 0000 0000 808f 0100 5002 0000  t$mn........P...
```

### Comparing `wcferry-39.0.0.0a3/wcferry/wcf_pb2.py` & `wcferry-39.0.0.1/wcferry/wcf_pb2.py`

 * *Files identical despite different names*

### Comparing `wcferry-39.0.0.0a3/wcferry/wxmsg.py` & `wcferry-39.0.0.1/wcferry/wxmsg.py`

 * *Files identical despite different names*

### Comparing `wcferry-39.0.0.0a3/wcferry.egg-info/PKG-INFO` & `wcferry-39.0.0.1/wcferry.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcferry
-Version: 39.0.0.0a3
+Version: 39.0.0.1
 Summary: 一个玩微信的工具
 Home-page: https://github.com/lich0821/WeChatFerry
 Author: Changhua
 Author-email: lichanghua0821@gmail.com
 License: MIT
 Project-URL: Documentation, https://wechatferry.readthedocs.io/zh/latest/index.html
 Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WeChatFerry Python 客户端
 [![PyPi](https://img.shields.io/pypi/v/wcferry.svg)](https://pypi.python.org/pypi/wcferry) [![Downloads](https://static.pepy.tech/badge/wcferry)](https://pypi.python.org/pypi/wcferry) [![Documentation Status](https://readthedocs.org/projects/wechatferry/badge/?version=latest)](https://wechatferry.readthedocs.io/zh/latest/?badge=latest)
 
-|[📖 文档](https://wechatferry.readthedocs.io/)|[📺 视频教程](https://mp.weixin.qq.com/s/APdjGyZ2hllXxyG_sNCfXQ)|[🙋 FAQ](https://mp.weixin.qq.com/s/XTJ9H-FsCPCscixAts8i_A)|
+|[📖 文档](https://wechatferry.readthedocs.io/)|[📺 视频教程](https://mp.weixin.qq.com/s/APdjGyZ2hllXxyG_sNCfXQ)|[🙋 FAQ](https://mp.weixin.qq.com/s/vAGpn1C9stI8Xzt1hUJhLA)|
 |:-:|:-:|:-:|
 
 🤖示例机器人框架：[WeChatRobot](https://github.com/lich0821/WeChatRobot)。
 
 ## 快速开始
 ```sh
 pip install --upgrade wcferry
@@ -54,52 +54,60 @@
             continue
 
         LOG.info(msg)  # 简单打印
 
 
 def main():
     LOG.info("Start demo...")
-    wcf = Wcf(debug=True)             # 默认连接本地服务
+    wcf = Wcf(debug=True)
 
     sleep(5)  # 等微信加载好，以免信息显示异常
     LOG.info(f"已经登录: {True if wcf.is_login() else False}")
     LOG.info(f"wxid: {wcf.get_self_wxid()}")
 
     # 允许接收消息
     # wcf.enable_recv_msg(LOG.info) # deprecated
 
     # 允许接收消息
     wcf.enable_receiving_msg()
     Thread(target=process_msg, name="GetMessage", args=(wcf,), daemon=True).start()
 
     # wcf.disable_recv_msg() # 当需要停止接收消息时调用
-
+    sleep(5)
     ret = wcf.send_text("Hello world.", "filehelper")
     LOG.info(f"send_text: {ret}")
 
-    ret = wcf.send_image("TEQuant.jpeg", "filehelper")  # 需要确保图片路径正确
+    sleep(5)
+    ret = wcf.send_image("TEQuant.jpeg", "filehelper")  # 需要确保图片路径正确，建议使用绝对路径（使用双斜杠\\）
     LOG.info(f"send_image: {ret}")
 
-    ret = wcf.send_file("README.MD", "filehelper")  # 需要确保文件路径正确
+    sleep(5)
+    ret = wcf.send_file("README.MD", "filehelper")  # 需要确保文件路径正确，建议使用绝对路径（使用双斜杠\\）
     LOG.info(f"send_file: {ret}")
 
+    sleep(5)
     LOG.info(f"Message types:\n{wcf.get_msg_types()}")
     LOG.info(f"Contacts:\n{wcf.get_contacts()}")
 
+    sleep(5)
     LOG.info(f"DBs:\n{wcf.get_dbs()}")
-    LOG.info(f"Tables:\n{wcf.get_tables('db')}")
+    LOG.info(f"Tables:\n{wcf.get_tables('MicroMsg.db')}")
     LOG.info(f"Results:\n{wcf.query_sql('MicroMsg.db', 'SELECT * FROM Contact LIMIT 1;')}")
 
     # 需要真正的 V3、V4 信息
     # wcf.accept_new_friend("v3", "v4")
 
-    # 填写正确的群 ID 和成员 wxid
+    # 添加群成员，填写正确的群 ID 和成员 wxid
     # ret = wcf.add_chatroom_members("chatroom id", "wxid1,wxid2,wxid3,...")
     # LOG.info(f"add_chatroom_members: {ret}")
 
+    # 删除群成员，填写正确的群 ID 和成员 wxid
+    # ret = wcf.del_chatroom_members("chatroom id", "wxid1,wxid2,wxid3,...")
+    # LOG.info(f"add_chatroom_members: {ret}")
+
     # 一直运行
     wcf.keep_running()
 
 
 if __name__ == "__main__":
     main()
 
@@ -138,57 +146,31 @@
 
 其中：
 * `w` 是微信的大版本号，如 `37` (3.7.a.a), `38` (3.8.a.a), `39` (3.9.a.a)
 * `x` 是适配的微信的小版本号，从 0 开始
 * `y` 是 `WeChatFerry` 的版本，从 0 开始
 * `z` 是各客户端的版本，从 0 开始
 
-### 39.0.0.0a0 (2023.07.11)
-支持微信 `3.9.2.23`。
+### 39.0.0.1 (2023.07.15)
+修复不能 @ 问题。
 
 功能：
 
 * 检查登录状态
 * 获取登录账号的 wxid
 * 获取消息类型
 * 获取所有联系人
 * 获取所有好友
 * 获取数据库
 * 获取某数据库下的表
+* 获取用户信息
 * 发送文本消息（可 @）
 * 发送图片（Python 客户端支持网络路径）
 * 发送文件
 * 允许接收消息
 * 停止接收消息
 * 执行 SQL 查询
 * 接受好友申请
 * 添加群成员
+* 删除群成员
 * 解密图片
 * 某功能（Breaking Change）
-
-<details><summary>历史更新</summary>
-
-### 37.1.25.5 (2023.05.19)
-支持 `3.7.0.30` 的最后一个版本。
-
-功能：
-
-* 检查登录状态
-* 获取登录账号的 wxid
-* 获取消息类型
-* 获取所有联系人
-* 获取所有好友
-* 获取数据库
-* 获取某数据库下的表
-* 发送文本消息（可 @）
-* 发送图片（Python 客户端支持网络路径）
-* 发送文件
-* 发送 XML
-* 发送表情
-* 允许接收消息
-* 停止接收消息
-* 执行 SQL 查询
-* 接受好友申请
-* 添加群成员
-* 解密图片
-* 某功能
-</details>
```

