# Comparing `tmp/RoInfo-0.0.2.tar.gz` & `tmp/RoInfo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RoInfo-0.0.2.tar", last modified: Sat May  6 07:13:22 2023, max compression
+gzip compressed data, was "RoInfo-0.0.3.tar", last modified: Sat Jul 15 06:05:42 2023, max compression
```

## Comparing `RoInfo-0.0.2.tar` & `RoInfo-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 07:13:21.999868 RoInfo-0.0.2/
--rw-rw-rw-   0        0        0      609 2023-05-06 07:13:21.998878 RoInfo-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-06 05:53:11.000000 RoInfo-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 07:13:21.981523 RoInfo-0.0.2/RoInfo/
--rw-rw-rw-   0        0        0     5188 2023-05-06 06:49:12.000000 RoInfo-0.0.2/RoInfo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:13:21.995544 RoInfo-0.0.2/RoInfo.egg-info/
--rw-rw-rw-   0        0        0      609 2023-05-06 07:13:21.000000 RoInfo-0.0.2/RoInfo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-05-06 07:13:21.000000 RoInfo-0.0.2/RoInfo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 07:13:21.000000 RoInfo-0.0.2/RoInfo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-06 07:13:21.000000 RoInfo-0.0.2/RoInfo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-06 07:13:21.000000 RoInfo-0.0.2/RoInfo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 07:13:22.000870 RoInfo-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1010 2023-05-06 06:51:55.000000 RoInfo-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 06:05:42.026582 RoInfo-0.0.3/
+-rw-rw-rw-   0        0        0      617 2023-07-15 06:05:42.018276 RoInfo-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-05-12 12:51:48.000000 RoInfo-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 06:05:41.980587 RoInfo-0.0.3/RoInfo/
+-rw-rw-rw-   0        0        0     5042 2023-05-12 13:27:41.000000 RoInfo-0.0.3/RoInfo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 06:05:42.013227 RoInfo-0.0.3/RoInfo.egg-info/
+-rw-rw-rw-   0        0        0      617 2023-07-15 06:05:41.000000 RoInfo-0.0.3/RoInfo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-07-15 06:05:41.000000 RoInfo-0.0.3/RoInfo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 06:05:41.000000 RoInfo-0.0.3/RoInfo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-15 06:05:41.000000 RoInfo-0.0.3/RoInfo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-15 06:05:41.000000 RoInfo-0.0.3/RoInfo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 06:05:42.026582 RoInfo-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      993 2023-05-12 12:54:26.000000 RoInfo-0.0.3/setup.py
```

### Comparing `RoInfo-0.0.2/PKG-INFO` & `RoInfo-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: RoInfo
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Roblox API Wrapper for roblox.com
 Home-page: 
 Author: Ryan_shamu
 Author-email: Ryanshamu418@Gmail.com
-Keywords: Roblox,RoInfo,Roblox Web Api,Roblox Python,Roblox For Python,Roblox Api,Roblox Api,Roblox Bot
+Keywords: Roblox,RoInfo,Roblox Web Api,Roblox Python,Roblox For Python,Roblox Api,Roblox Api Library,Roblox Bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `RoInfo-0.0.2/RoInfo/__init__.py` & `RoInfo-0.0.3/RoInfo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,74 +35,42 @@
             "Content-Type": "application/json"
         }
 
         session.cookies[".ROBLOSECURITY"] = self.token
 
         testt = rbx_request("get", "https://users.roblox.com/v1/users/authenticated")
         test = testt.json()
-        print(test)
         if test['name']:
             print(f"Welcome, {test['name']} you have signed in successfully!")
             self.id = test['id']
-            print(self.id)
-            print(test['id'])
             self._username = test['name']
         else:
             print("\033[91m WARNING!: Your are not signed into an existing account, please put the security cookie to an existing account or some functions may not work! \033[00m")
 
     
 
 
 
     def get_current_robux(self):
         request = json.dumps(rbx_request("get","https://economy.roblox.com/v1/user/currency").text)
 
-        returndata = request[0]
+        returndata = request['robux']
         
         return returndata
 
     def change_display_name(self, displayname):
         requestt = rbx_request("patch", f"https://users.roblox.com/v1/users/{self.id}/display-names", data={"newDisplayName": str(displayname)})
 
         request = requestt.json()
 
             
         return request
 
 
-    def userfollowers(self, userid):
-
-        responsee = rbx_request("get", f"https://friends.roblox.com/v1/users/{userid}/followers/count")
-
-        response = responsee.json()
-
-        returnresponse = response['count']
-
-        return returnresponse
-
-    def userfriends(self, userid):
-
-        responsee = rbx_request("get", f"https://friends.roblox.com/v1/users/{userid}/friends/count")
-
-        response = responsee.json()
-
-        returnresponse = response['count']
-
-        return returnresponse
-
-    def userjoindate(self, userid):
-
-        responsee = rbx_request("get", f"https://users.roblox.com/v1/users/{userid}")
-
-        response = responsee.json()
-
-        returnresponse = response['created']
-
-        return returnresponse
-
+    
     def sendmessage(self, recipientid, subject, body):
 
         responsee = rbx_request("post", "https://privatemessages.roblox.com/v1/messages/send", data={"userId": self.id, "subject": subject, "body": body, "recipientId": recipientid})
 
         response = responsee.json()
 
         return response
@@ -143,15 +111,14 @@
     def findusersinrole(self, groupid, roleid):
         
         responsee = rbx_request("get", f"https://groups.roblox.com/v1/groups/{groupid}/roles/{roleid}/users")
 
         response = responsee.json()
 
         json_data = response['data']
-        print(json_data)
         list = []
 
 
         for user in json_data:
             list.append(user)
 
         return list
@@ -164,8 +131,41 @@
                 "recipientId": userid,
                 "recipientType": "User",
                 "amount": amount
                 }   
             ]})
             response = responsee.json()
 
-            return response
+            return response
+
+
+
+
+def userfollowers(self, userid):
+
+    responsee = rbx_request("get", f"https://friends.roblox.com/v1/users/{userid}/followers/count")
+
+    response = responsee.json()
+
+    returnresponse = response['count']
+
+    return returnresponse
+
+def userfriends(self, userid):
+
+    responsee = rbx_request("get", f"https://friends.roblox.com/v1/users/{userid}/friends/count")
+
+    response = responsee.json()
+
+    returnresponse = response['count']
+
+    return returnresponse
+
+def userjoindate(self, userid):
+
+    responsee = rbx_request("get", f"https://users.roblox.com/v1/users/{userid}")
+
+    response = responsee.json()
+
+    returnresponse = response['created']
+
+    return returnresponse
```

### Comparing `RoInfo-0.0.2/RoInfo.egg-info/PKG-INFO` & `RoInfo-0.0.3/RoInfo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: RoInfo
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Roblox API Wrapper for roblox.com
 Home-page: 
 Author: Ryan_shamu
 Author-email: Ryanshamu418@Gmail.com
-Keywords: Roblox,RoInfo,Roblox Web Api,Roblox Python,Roblox For Python,Roblox Api,Roblox Api,Roblox Bot
+Keywords: Roblox,RoInfo,Roblox Web Api,Roblox Python,Roblox For Python,Roblox Api,Roblox Api Library,Roblox Bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
```

### Comparing `RoInfo-0.0.2/setup.py` & `RoInfo-0.0.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'A Roblox API Wrapper for roblox.com'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="RoInfo",
     version=VERSION,
     author="Ryan_shamu",
     author_email="Ryanshamu418@Gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=open('README.md').read(),
     packages=find_packages(),
-    install_requires=["websocket-client","numpy","requests","bs4", "re"],
-    keywords=['Roblox', 'RoInfo', 'Roblox Web Api', 'Roblox Python', 'Roblox For Python', 'Roblox Api', 'Roblox Api', 'Roblox Bot'],
+    install_requires=["requests", "re", "json"],
+    keywords=['Roblox', 'RoInfo', 'Roblox Web Api', 'Roblox Python', 'Roblox For Python', 'Roblox Api', 'Roblox Api Library', 'Roblox Bot'],
     url='',
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

