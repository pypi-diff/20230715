# Comparing `tmp/nonechat-0.1.1.tar.gz` & `tmp/nonechat-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonechat-0.1.1.tar", last modified: Fri Jul 14 17:45:22 2023, max compression
+gzip compressed data, was "nonechat-0.1.2.tar", last modified: Sat Jul 15 10:16:27 2023, max compression
```

## Comparing `nonechat-0.1.1.tar` & `nonechat-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      984 2023-07-14 17:44:51.204678 nonechat-0.1.1/README.md
--rw-r--r--   0        0        0      359 2023-07-14 17:44:51.204678 nonechat-0.1.1/nonechat/__init__.py
--rw-r--r--   0        0        0     3528 2023-07-14 17:44:51.204678 nonechat-0.1.1/nonechat/app.py
--rw-r--r--   0        0        0      745 2023-07-14 17:44:51.204678 nonechat-0.1.1/nonechat/backend.py
--rw-r--r--   0        0        0      912 2023-07-14 17:44:51.204678 nonechat-0.1.1/nonechat/components/chatroom/__init__.py
--rw-r--r--   0        0        0     2013 2023-07-14 17:44:51.204678 nonechat-0.1.1/nonechat/components/chatroom/history.py
--rw-r--r--   0        0        0     1439 2023-07-14 17:44:51.204678 nonechat-0.1.1/nonechat/components/chatroom/input.py
--rw-r--r--   0        0        0     4053 2023-07-14 17:44:51.204678 nonechat-0.1.1/nonechat/components/chatroom/message.py
--rw-r--r--   0        0        0     2234 2023-07-14 17:44:51.204678 nonechat-0.1.1/nonechat/components/chatroom/toolbar.py
--rw-r--r--   0        0        0       45 2023-07-14 17:44:51.204678 nonechat-0.1.1/nonechat/components/footer.py
--rw-r--r--   0        0        0      950 2023-07-14 17:44:51.208678 nonechat-0.1.1/nonechat/components/general/action.py
--rw-r--r--   0        0        0     1184 2023-07-14 17:44:51.208678 nonechat-0.1.1/nonechat/components/header.py
--rw-r--r--   0        0        0     1508 2023-07-14 17:44:51.208678 nonechat-0.1.1/nonechat/components/log/__init__.py
--rw-r--r--   0        0        0     1499 2023-07-14 17:44:51.208678 nonechat-0.1.1/nonechat/components/log/toolbar.py
--rw-r--r--   0        0        0      582 2023-07-14 17:44:51.208678 nonechat-0.1.1/nonechat/info.py
--rw-r--r--   0        0        0     1143 2023-07-14 17:44:51.208678 nonechat-0.1.1/nonechat/log_redirect.py
--rw-r--r--   0        0        0     4132 2023-07-14 17:44:51.208678 nonechat-0.1.1/nonechat/message.py
--rw-r--r--   0        0        0       92 2023-07-14 17:44:51.208678 nonechat-0.1.1/nonechat/router/__init__.py
--rw-r--r--   0        0        0     1222 2023-07-14 17:44:51.208678 nonechat-0.1.1/nonechat/router/router.py
--rw-r--r--   0        0        0      416 2023-07-14 17:44:51.208678 nonechat-0.1.1/nonechat/setting.py
--rw-r--r--   0        0        0     2131 2023-07-14 17:44:51.208678 nonechat-0.1.1/nonechat/storage/__init__.py
--rw-r--r--   0        0        0      285 2023-07-14 17:44:51.208678 nonechat-0.1.1/nonechat/utils.py
--rw-r--r--   0        0        0     1905 2023-07-14 17:44:51.208678 nonechat-0.1.1/nonechat/views/horizontal.py
--rw-r--r--   0        0        0      700 2023-07-14 17:44:51.208678 nonechat-0.1.1/nonechat/views/log_view.py
--rw-r--r--   0        0        0     1224 2023-07-14 17:45:22.038278 nonechat-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1409 1970-01-01 00:00:00.000000 nonechat-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      984 2023-07-15 10:15:48.014680 nonechat-0.1.2/README.md
+-rw-r--r--   0        0        0      359 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/__init__.py
+-rw-r--r--   0        0        0     3528 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/app.py
+-rw-r--r--   0        0        0      745 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/backend.py
+-rw-r--r--   0        0        0      912 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/components/chatroom/__init__.py
+-rw-r--r--   0        0        0     2013 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/components/chatroom/history.py
+-rw-r--r--   0        0        0     1418 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/components/chatroom/input.py
+-rw-r--r--   0        0        0     4053 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/components/chatroom/message.py
+-rw-r--r--   0        0        0     2234 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/components/chatroom/toolbar.py
+-rw-r--r--   0        0        0       45 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/components/footer.py
+-rw-r--r--   0        0        0      950 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/components/general/action.py
+-rw-r--r--   0        0        0     1184 2023-07-15 10:15:48.014680 nonechat-0.1.2/nonechat/components/header.py
+-rw-r--r--   0        0        0     1508 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/components/log/__init__.py
+-rw-r--r--   0        0        0     1499 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/components/log/toolbar.py
+-rw-r--r--   0        0        0      582 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/info.py
+-rw-r--r--   0        0        0     1143 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/log_redirect.py
+-rw-r--r--   0        0        0     4132 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/message.py
+-rw-r--r--   0        0        0       92 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/router/__init__.py
+-rw-r--r--   0        0        0     1222 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/router/router.py
+-rw-r--r--   0        0        0      416 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/setting.py
+-rw-r--r--   0        0        0     2131 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/storage/__init__.py
+-rw-r--r--   0        0        0      285 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/utils.py
+-rw-r--r--   0        0        0     1905 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/views/horizontal.py
+-rw-r--r--   0        0        0      700 2023-07-15 10:15:48.018680 nonechat-0.1.2/nonechat/views/log_view.py
+-rw-r--r--   0        0        0     1224 2023-07-15 10:16:27.093310 nonechat-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1409 1970-01-01 00:00:00.000000 nonechat-0.1.2/PKG-INFO
```

### Comparing `nonechat-0.1.1/README.md` & `nonechat-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.1/nonechat/app.py` & `nonechat-0.1.2/nonechat/app.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.1/nonechat/backend.py` & `nonechat-0.1.2/nonechat/backend.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.1/nonechat/components/chatroom/__init__.py` & `nonechat-0.1.2/nonechat/components/chatroom/__init__.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.1/nonechat/components/chatroom/history.py` & `nonechat-0.1.2/nonechat/components/chatroom/history.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.1/nonechat/components/chatroom/input.py` & `nonechat-0.1.2/nonechat/components/chatroom/input.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     }
     InputBox > Input:focus {
         border: $input-border-active !important;
     }
     """
 
     BINDINGS = [
-        Binding("escape", "reset_focus", "Reset focus", show=False),
+        Binding("escape", "blur", "Reset focus", show=False),
     ]
 
     def __init__(self):
         super().__init__()
         self.input = Input(placeholder="Send Message")
 
     @property
@@ -49,9 +49,9 @@
         yield self.input
 
     async def on_input_submitted(self, event: Input.Submitted):
         event.stop()
         self.input.value = ""
         await self.app.action_post_message(event.value)
 
-    def action_reset_focus(self):
-        self.input.reset_focus()
+    def action_blur(self):
+        self.input.blur()
```

### Comparing `nonechat-0.1.1/nonechat/components/chatroom/message.py` & `nonechat-0.1.2/nonechat/components/chatroom/message.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.1/nonechat/components/chatroom/toolbar.py` & `nonechat-0.1.2/nonechat/components/chatroom/toolbar.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.1/nonechat/components/general/action.py` & `nonechat-0.1.2/nonechat/components/general/action.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.1/nonechat/components/header.py` & `nonechat-0.1.2/nonechat/components/header.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.1/nonechat/components/log/__init__.py` & `nonechat-0.1.2/nonechat/components/log/__init__.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.1/nonechat/components/log/toolbar.py` & `nonechat-0.1.2/nonechat/components/log/toolbar.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.1/nonechat/info.py` & `nonechat-0.1.2/nonechat/info.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.1/nonechat/log_redirect.py` & `nonechat-0.1.2/nonechat/log_redirect.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.1/nonechat/message.py` & `nonechat-0.1.2/nonechat/message.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.1/nonechat/router/router.py` & `nonechat-0.1.2/nonechat/router/router.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.1/nonechat/storage/__init__.py` & `nonechat-0.1.2/nonechat/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.1/nonechat/views/horizontal.py` & `nonechat-0.1.2/nonechat/views/horizontal.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.1/nonechat/views/log_view.py` & `nonechat-0.1.2/nonechat/views/log_view.py`

 * *Files identical despite different names*

### Comparing `nonechat-0.1.1/pyproject.toml` & `nonechat-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonechat"
-version = "0.1.1"
+version = "0.1.2"
 description = "Awesome chat console using Textual"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "textual ~=0.29.0",
 ]
```

### Comparing `nonechat-0.1.1/PKG-INFO` & `nonechat-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonechat
-Version: 0.1.1
+Version: 0.1.2
 Summary: Awesome chat console using Textual
 Home-page: https://github.com/nonebot/nonechat
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonebot/nonechat
 Project-URL: Repository, https://github.com/nonebot/nonechat
 Requires-Python: <4.0,>=3.8
```

