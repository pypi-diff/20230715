# Comparing `tmp/gamerinsta-0.0.4.tar.gz` & `tmp/gamerinsta-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamerinsta-0.0.4.tar", last modified: Mon Jun 19 05:00:52 2023, max compression
+gzip compressed data, was "gamerinsta-0.0.5.tar", last modified: Sat Jul 15 15:11:47 2023, max compression
```

## Comparing `gamerinsta-0.0.4.tar` & `gamerinsta-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 05:00:52.366630 gamerinsta-0.0.4/
--rw-rw-rw-   0        0        0     1062 2023-05-25 19:08:15.000000 gamerinsta-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      617 2023-06-19 05:00:52.365336 gamerinsta-0.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 05:00:52.321596 gamerinsta-0.0.4/gamerinsta/
--rw-rw-rw-   0        0        0    11037 2023-06-17 10:53:54.000000 gamerinsta-0.0.4/gamerinsta/__init__.py
--rw-rw-rw-   0        0        0     6450 2023-06-19 04:58:46.000000 gamerinsta-0.0.4/gamerinsta/tokens.py
-drwxrwxrwx   0        0        0        0 2023-06-19 05:00:52.357788 gamerinsta-0.0.4/gamerinsta.egg-info/
--rw-rw-rw-   0        0        0      617 2023-06-19 05:00:52.000000 gamerinsta-0.0.4/gamerinsta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-06-19 05:00:52.000000 gamerinsta-0.0.4/gamerinsta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 05:00:52.000000 gamerinsta-0.0.4/gamerinsta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-06-19 05:00:52.000000 gamerinsta-0.0.4/gamerinsta.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 05:00:52.000000 gamerinsta-0.0.4/gamerinsta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 05:00:52.367140 gamerinsta-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      918 2023-06-19 05:00:24.000000 gamerinsta-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 15:11:47.018608 gamerinsta-0.0.5/
+-rw-rw-rw-   0        0        0     1062 2023-05-25 19:08:15.000000 gamerinsta-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      617 2023-07-15 15:11:47.018608 gamerinsta-0.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-15 15:11:46.987222 gamerinsta-0.0.5/gamerinsta/
+-rw-rw-rw-   0        0        0    11554 2023-07-15 15:09:22.000000 gamerinsta-0.0.5/gamerinsta/__init__.py
+-rw-rw-rw-   0        0        0     6349 2023-07-15 15:08:11.000000 gamerinsta-0.0.5/gamerinsta/tokens.py
+drwxrwxrwx   0        0        0        0 2023-07-15 15:11:47.018608 gamerinsta-0.0.5/gamerinsta.egg-info/
+-rw-rw-rw-   0        0        0      617 2023-07-15 15:11:46.000000 gamerinsta-0.0.5/gamerinsta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-07-15 15:11:46.000000 gamerinsta-0.0.5/gamerinsta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 15:11:46.000000 gamerinsta-0.0.5/gamerinsta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-15 15:11:46.000000 gamerinsta-0.0.5/gamerinsta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-15 15:11:46.000000 gamerinsta-0.0.5/gamerinsta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 15:11:47.018608 gamerinsta-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      918 2023-07-15 15:10:46.000000 gamerinsta-0.0.5/setup.py
```

### Comparing `gamerinsta-0.0.4/LICENSE` & `gamerinsta-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gamerinsta-0.0.4/PKG-INFO` & `gamerinsta-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamerinsta
-Version: 0.0.4
+Version: 0.0.5
 Summary: Instagram Android Api For Login 
 Author: Gamer
 Author-email: godxgamer0192@gmail.com
 Keywords: Instagram,login
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gamerinsta-0.0.4/gamerinsta/__init__.py` & `gamerinsta-0.0.5/gamerinsta/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,20 @@
     return ''.join(random.choice(string.ascii_letters + string.digits) for _ in range(n))
 
 
 
 class Login:
     def __init__(self):
         self.Pigionid=f'UFS-{str(uuid.uuid4())}-0'
-        self.Block='a972d28f4dce85acc2d13c958e43cb12e5c549cbefdc3e89bc8863afcd3d98db'
+        self.Block='4a40c892c95e48d772a51c3e512eface26cba248924e73e874956fd781bcd1f4'
         self.Deviceid=str(uuid.uuid4())
         self.FDeviceid=str(uuid.uuid4())
         self.Androidid=f'android-{generateRandomString(8).encode().hex()}'
         rnd = str(random.randint(150, 999))
-        self.Useragent="Instagram 285.0.0.25.62 Android (" + ["23/6.0", "24/7.0", "25/7.1.1", "26/8.0", "27/8.1", "28/9.0"][random.randint(0, 5)] + "; " + str(random.randint(100, 1300)) + "dpi; " + str(random.randint(200, 2000)) + "x" + str(random.randint(200, 2000)) + "; " + ["SAMSUNG", "HUAWEI", "LGE/lge", "HTC", "ASUS", "ZTE", "ONEPLUS", "XIAOMI", "OPPO","VIVO", "SONY", "REALME"][random.randint(0,11)] + "; SM-T" + rnd + "; SM-T" + rnd + "; qcom; en_US; 479968426)"
+        self.Useragent="Instagram 291.1.0.34.111 Android (" + ["23/6.0", "24/7.0", "25/7.1.1", "26/8.0", "27/8.1", "28/9.0"][random.randint(0, 5)] + "; " + str(random.randint(100, 1300)) + "dpi; " + str(random.randint(200, 2000)) + "x" + str(random.randint(200, 2000)) + "; " + ["SAMSUNG", "HUAWEI", "LGE/lge", "HTC", "ASUS", "ZTE", "ONEPLUS", "XIAOMI", "OPPO","VIVO", "SONY", "REALME"][random.randint(0,11)] + "; SM-T" + rnd + "; SM-T" + rnd + "; qcom; en_US; 494078218)"
         self.Waterid=str(uuid.uuid4())
         self.qpl_join_id=str(uuid.uuid4())
 
 
     def Loginv1(self,Username,Password):
         Tokens.Cooki(self)
         self.Usernamee=Username
@@ -115,14 +115,19 @@
                     print(value)
 
 
             if 'Incorrect Password: The password you entered is incorrect. Please try again.' in response.text:
                 value = {
                     "Response": 'Incorrect Password: The password you entered is incorrect. Please try again.',
                 }
+            elif f"An unexpected error occurred. Please try logging in again." in response.text:
+
+                value = {
+                    "Response": f"Login Error: An unexpected error occurred. Please try logging in again.",
+                }
             elif 'Please wait a few minutes before you try again.' in response.text:
                 value = {
                     "Response": 'Please wait a few minutes before you try again.',
                 }
 
             elif f". Try another phone number or email, or if you don't have an Instagram account, you can sign up." in response.text:
 
@@ -185,17 +190,25 @@
 
 
             elif 'checkpoint_required' in response.text:
                 value = {
                     "Response": 'checkpoint_required',
                 }
 
+            elif f"An unexpected error occurred. Please try logging in again." in response.text:
+
+                value = {
+                    "Response": f"Login Error: An unexpected error occurred. Please try logging in again.",
+                }
+
+
             else:
                 value = {
                     "Response": response.json(),
                 }
+
             return value
         except Exception as e:
             print(e)
```

### Comparing `gamerinsta-0.0.4/gamerinsta/tokens.py` & `gamerinsta-0.0.5/gamerinsta/tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,17 @@
                 'https://b.i.instagram.com/api/v1/bloks/apps/com.bloks.www.bloks.caa.login.process_client_data_and_redirect/',
                 headers=self.headers,
                 data=data,
             )
             self.Elgn = response.text.split('"K":"email","!":"')[1].split('","":[{"㚱":{"9":"","2":""}}]')[0]
             self.Plgn = response.text.split('"K":"password","!":"')[1].split('","":[{"㚱":{"9":"","2":""}}]')[0]
             self.Insid = response.text.split(', (bk.action.i32.Const, 2), (bk.action.tree.Make, (bk.action.i32.Const, 13704))))), (bk.action.i32.Const, 35), (bk.action.core.FuncConst, (bk.action.core.TakeLast, (bk.action.qpl.MarkerPoint, (bk.action.i32.Const, 36707139), (bk.action.i32.Const, ')[1].split(r'), \"handle_async_action_result_start\", (bk.action.tree.Make, (bk.action.i32.Const, 13747))), (bk.action.core.TakeLast, (bk.action.core.TakeLast, (bk.action.bloks.WriteLocalState, \"')[0]
-            self.Mkrid = response.text.split(r'\")))), (bk.action.core.TakeLast, (bk.action.bloks.WriteGlobalConsistencyStore, \"CAA_LOGIN_FORM:is_login_pending:0\", (bk.action.bool.Const, true)), (bk.action.core.TakeLast, (bk.action.qpl.MarkerStartV2, (bk.action.i32.Const, ')[1].split('), (bk.action.i32.Const, ')[0]
+            self.Mkrid = response.text.split(
+                    r'(bk.action.tree.Make, (bk.action.i32.Const, 13704))), (bk.action.qpl.MarkerAnnotate, (bk.action.i32.Const, ')[
+                    1].split(')')[0]
 
             return self.Mid,self.Elgn,self.Plgn,self.Insid,self.Mkrid,self.headers
         except Exception as e:
             print(e)
             Tokens.Cooki(self)
 
     def Cooki2(self):
```

### Comparing `gamerinsta-0.0.4/gamerinsta.egg-info/PKG-INFO` & `gamerinsta-0.0.5/gamerinsta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamerinsta
-Version: 0.0.4
+Version: 0.0.5
 Summary: Instagram Android Api For Login 
 Author: Gamer
 Author-email: godxgamer0192@gmail.com
 Keywords: Instagram,login
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gamerinsta-0.0.4/setup.py` & `gamerinsta-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Instagram Android Api For Login '
 LONG_DESCRIPTION = 'A python library that helps you to login in instagram do various task and automaiton'
 
 # Setting up
 setup(
     name="gamerinsta",
     version=VERSION,
```

