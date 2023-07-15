# Comparing `tmp/python-ndev-blizzardapi-0.0.4.tar.gz` & `tmp/python-ndev-blizzardapi-0.0.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-ndev-blizzardapi-0.0.4.tar", last modified: Mon Jun 19 21:29:18 2023, max compression
+gzip compressed data, was "python-ndev-blizzardapi-0.0.5a0.tar", last modified: Sat Jul 15 13:33:02 2023, max compression
```

## Comparing `python-ndev-blizzardapi-0.0.4.tar` & `python-ndev-blizzardapi-0.0.5a0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 21:29:18.952839 python-ndev-blizzardapi-0.0.4/
--rw-rw-rw-   0        0        0      134 2023-03-10 17:55:01.000000 python-ndev-blizzardapi-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2202 2023-06-19 21:29:18.952339 python-ndev-blizzardapi-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1475 2023-03-10 20:02:35.000000 python-ndev-blizzardapi-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 21:29:18.916499 python-ndev-blizzardapi-0.0.4/blizzardAPI/
--rw-rw-rw-   0        0        0      161 2023-03-11 02:36:09.000000 python-ndev-blizzardapi-0.0.4/blizzardAPI/__init__.py
--rw-rw-rw-   0        0        0     4446 2023-06-19 02:12:09.000000 python-ndev-blizzardapi-0.0.4/blizzardAPI/api.py
-drwxrwxrwx   0        0        0        0 2023-06-19 21:29:18.933737 python-ndev-blizzardapi-0.0.4/blizzardAPI/battlenet/
--rw-rw-rw-   0        0        0       25 2023-03-10 03:36:02.000000 python-ndev-blizzardapi-0.0.4/blizzardAPI/battlenet/__init__.py
--rw-rw-rw-   0        0        0      458 2023-03-10 03:44:26.000000 python-ndev-blizzardapi-0.0.4/blizzardAPI/battlenet/battlenet_api.py
--rw-rw-rw-   0        0        0     1539 2023-03-10 03:47:42.000000 python-ndev-blizzardapi-0.0.4/blizzardAPI/battlenet/battlenet_oauth.py
--rw-rw-rw-   0        0        0      539 2023-06-19 02:10:51.000000 python-ndev-blizzardapi-0.0.4/blizzardAPI/blizzard_api.py
-drwxrwxrwx   0        0        0        0 2023-06-19 21:29:18.951366 python-ndev-blizzardapi-0.0.4/python_ndev_blizzardapi.egg-info/
--rw-rw-rw-   0        0        0     2202 2023-06-19 21:29:18.000000 python-ndev-blizzardapi-0.0.4/python_ndev_blizzardapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-06-19 21:29:18.000000 python-ndev-blizzardapi-0.0.4/python_ndev_blizzardapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 21:29:18.000000 python-ndev-blizzardapi-0.0.4/python_ndev_blizzardapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-19 21:29:18.000000 python-ndev-blizzardapi-0.0.4/python_ndev_blizzardapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-19 21:29:18.000000 python-ndev-blizzardapi-0.0.4/python_ndev_blizzardapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 21:29:18.952839 python-ndev-blizzardapi-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1004 2023-06-19 21:28:52.000000 python-ndev-blizzardapi-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 13:33:02.947970 python-ndev-blizzardapi-0.0.5a0/
+-rw-rw-rw-   0        0        0      134 2023-07-14 20:43:22.000000 python-ndev-blizzardapi-0.0.5a0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2311 2023-07-15 13:33:02.946972 python-ndev-blizzardapi-0.0.5a0/PKG-INFO
+-rw-rw-rw-   0        0        0     1582 2023-07-14 18:06:48.000000 python-ndev-blizzardapi-0.0.5a0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 13:33:02.912859 python-ndev-blizzardapi-0.0.5a0/blizzardAPI/
+-rw-rw-rw-   0        0        0      161 2023-03-11 02:36:09.000000 python-ndev-blizzardapi-0.0.5a0/blizzardAPI/__init__.py
+-rw-rw-rw-   0        0        0     4981 2023-06-24 20:44:02.000000 python-ndev-blizzardapi-0.0.5a0/blizzardAPI/api.py
+drwxrwxrwx   0        0        0        0 2023-07-15 13:33:02.927924 python-ndev-blizzardapi-0.0.5a0/blizzardAPI/battlenet/
+-rw-rw-rw-   0        0        0       25 2023-03-10 03:36:02.000000 python-ndev-blizzardapi-0.0.5a0/blizzardAPI/battlenet/__init__.py
+-rw-rw-rw-   0        0        0      458 2023-03-10 03:44:26.000000 python-ndev-blizzardapi-0.0.5a0/blizzardAPI/battlenet/battlenet_api.py
+-rw-rw-rw-   0        0        0     1539 2023-03-10 03:47:42.000000 python-ndev-blizzardapi-0.0.5a0/blizzardAPI/battlenet/battlenet_oauth.py
+-rw-rw-rw-   0        0        0      539 2023-06-21 18:46:57.000000 python-ndev-blizzardapi-0.0.5a0/blizzardAPI/blizzard_api.py
+drwxrwxrwx   0        0        0        0 2023-07-15 13:33:02.938451 python-ndev-blizzardapi-0.0.5a0/blizzardAPI/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-21 22:10:25.000000 python-ndev-blizzardapi-0.0.5a0/blizzardAPI/tests/__init__.py
+-rw-rw-rw-   0        0        0     1288 2023-06-22 00:13:18.000000 python-ndev-blizzardapi-0.0.5a0/blizzardAPI/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-07-15 13:33:02.944970 python-ndev-blizzardapi-0.0.5a0/python_ndev_blizzardapi.egg-info/
+-rw-rw-rw-   0        0        0     2311 2023-07-15 13:33:02.000000 python-ndev-blizzardapi-0.0.5a0/python_ndev_blizzardapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      509 2023-07-15 13:33:02.000000 python-ndev-blizzardapi-0.0.5a0/python_ndev_blizzardapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 13:33:02.000000 python-ndev-blizzardapi-0.0.5a0/python_ndev_blizzardapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-15 13:33:02.000000 python-ndev-blizzardapi-0.0.5a0/python_ndev_blizzardapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-15 13:33:02.000000 python-ndev-blizzardapi-0.0.5a0/python_ndev_blizzardapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 13:33:02.947970 python-ndev-blizzardapi-0.0.5a0/setup.cfg
+-rw-rw-rw-   0        0        0     1010 2023-07-15 13:27:51.000000 python-ndev-blizzardapi-0.0.5a0/setup.py
```

### Comparing `python-ndev-blizzardapi-0.0.4/PKG-INFO` & `python-ndev-blizzardapi-0.0.5a0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ndev-blizzardapi
-Version: 0.0.4
+Version: 0.0.5a0
 Summary: Python module created to integrate your Python project with the Blizzard API
 Home-page: https://github.com/natanrmaia/python-ndev-blizzardapi
 Author: natanrmaia
 Author-email: contato@natanael.dev.br
 Project-URL: Documentation, https://python-ndev-blizzardapi.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/natanrmaia/python-ndev-blizzardapi
 Project-URL: Bug Reports, https://github.com/natanrmaia/python-ndev-blizzardapi/issues
@@ -45,25 +45,30 @@
 ## Instalation
 ```python
   pip install python-ndev-blizzardapi
 ```
 
 ## Usage Example
 ```python
-
   from blizzardAPI import BlizzardAPI
   
   api = BlizzardAPI(client_id, client_secret)
   api.bnet.oauth.get_user_info("us","imagine_token_here")
 ```
 
-### Battle.Net API
+## Blizzard APIs Supported
+
+| API                     | Items           | Obs                   |
+| :---------------------- | :-------------- | :-------------------- |
+| **Battle.Net**          | OAuth API       | All Regions supported |
+| **World Of Warcraft**   | Game Data API   | _Profile Data API in development_ |
 
-| Python      | API URL    | API Name                                    |
-| :---------- | :--------- | :------------------------------------------ |
-| `api.bnet.oauth.get_user_info(region, access_token)`      | `/oauth/userinfo` | User Info (param) |
-| `api.bnet.oauth.get_token_validation(region, access_token)`      | `/oauth/check_token` | Token Validation (GET) |
 
+## Tests using PyTest
+To perform the tests using PyTest, I recommend using the dotenv module. Read more in the documentation provided below.
+```cmd
+pytest blizzardAPI
+```
 
 ## Documentation
 
 [Read the Docs](https://python-ndev-blizzardapi.readthedocs.io/)
```

### Comparing `python-ndev-blizzardapi-0.0.4/README.md` & `python-ndev-blizzardapi-0.0.5a0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -30,25 +30,30 @@
 ## Instalation
 ```python
   pip install python-ndev-blizzardapi
 ```
 
 ## Usage Example
 ```python
-
   from blizzardAPI import BlizzardAPI
   
   api = BlizzardAPI(client_id, client_secret)
   api.bnet.oauth.get_user_info("us","imagine_token_here")
 ```
 
-### Battle.Net API
+## Blizzard APIs Supported
+
+| API                     | Items           | Obs                   |
+| :---------------------- | :-------------- | :-------------------- |
+| **Battle.Net**          | OAuth API       | All Regions supported |
+| **World Of Warcraft**   | Game Data API   | _Profile Data API in development_ |
 
-| Python      | API URL    | API Name                                    |
-| :---------- | :--------- | :------------------------------------------ |
-| `api.bnet.oauth.get_user_info(region, access_token)`      | `/oauth/userinfo` | User Info (param) |
-| `api.bnet.oauth.get_token_validation(region, access_token)`      | `/oauth/check_token` | Token Validation (GET) |
 
+## Tests using PyTest
+To perform the tests using PyTest, I recommend using the dotenv module. Read more in the documentation provided below.
+```cmd
+pytest blizzardAPI
+```
 
 ## Documentation
 
 [Read the Docs](https://python-ndev-blizzardapi.readthedocs.io/)
```

### Comparing `python-ndev-blizzardapi-0.0.4/blizzardAPI/api.py` & `python-ndev-blizzardapi-0.0.5a0/blizzardAPI/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 
         elif format_url == 'oauth':
             if region == 'cn':
                 url = self.oauth_url_cn.format(api)
             else:
                 url = self.oauth_url.format(region, api)
 
+        else:
+            raise ValueError('format_url must be either api or oauth')
+
         return url
 
     def get_client_token(self, region):
         """
         It takes no parameters, and returns the access token
 
         :return: The access token is being returned.
@@ -62,14 +65,18 @@
         """
         It takes a response object, and returns the response object's json() method
 
         :param response: The response object returned by the request
         :return: The response.json() method will convert the JSON string into a Python dictionary.
         """
 
+        if response.status_code != 200:
+            msg = 'The response code was {0}. Error: {1}'.format(response.status_code, response.text)
+            raise ValueError(msg)
+
         return response.json()
 
     def request_handler(self, url, region, query_params):
 
         if self.access_token is None:
             client_token = self.get_client_token(region)
             self.access_token = client_token['access_token']
@@ -77,33 +84,40 @@
         if query_params.get('access_token') is None:
             query_params['access_token'] = self.access_token
 
         response = self.session.get(url, params=query_params)
 
         return self.response_handler(response)
 
-    def get_api(self, region, api, query_params=None):
+    def get_api(self, **kwargs):
         """
         It takes a region, an api, and query_params, and returns the response
 
         :param region: The region of the server you want to connect to
         :param api: The API you want to call
         :param query_params: The query parameters you want to pass to the API (optional)
         :return: The response is being returned.
         """
+
+        region          = kwargs.get('region')  or 'us'
+        api             = kwargs.get('api')     or None
+        query_params    = kwargs.get('query_params') or None
+
         if query_params is None:
             query_params = {}
 
         query_params['access_token'] = self.access_token
 
-        if query_params['locale'] is None:
+        if 'locale' not in query_params:
+            query_params['locale'] = ''
+        elif query_params['locale'] is None:
             query_params['locale'] = ''
 
-        if region is None:
-            region = 'us'
+        if api is None:
+            raise ValueError('api cannot be None')
 
         query_params['namespace'] = '{}-{}'.format(query_params['namespace'], region)
 
         url = self.format_url(region, api)
 
         return self.request_handler(url, region, query_params)
```

### Comparing `python-ndev-blizzardapi-0.0.4/blizzardAPI/battlenet/battlenet_oauth.py` & `python-ndev-blizzardapi-0.0.5a0/blizzardAPI/battlenet/battlenet_oauth.py`

 * *Files identical despite different names*

### Comparing `python-ndev-blizzardapi-0.0.4/blizzardAPI/blizzard_api.py` & `python-ndev-blizzardapi-0.0.5a0/blizzardAPI/blizzard_api.py`

 * *Files identical despite different names*

### Comparing `python-ndev-blizzardapi-0.0.4/python_ndev_blizzardapi.egg-info/PKG-INFO` & `python-ndev-blizzardapi-0.0.5a0/python_ndev_blizzardapi.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-ndev-blizzardapi
-Version: 0.0.4
+Version: 0.0.5a0
 Summary: Python module created to integrate your Python project with the Blizzard API
 Home-page: https://github.com/natanrmaia/python-ndev-blizzardapi
 Author: natanrmaia
 Author-email: contato@natanael.dev.br
 Project-URL: Documentation, https://python-ndev-blizzardapi.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/natanrmaia/python-ndev-blizzardapi
 Project-URL: Bug Reports, https://github.com/natanrmaia/python-ndev-blizzardapi/issues
@@ -45,25 +45,30 @@
 ## Instalation
 ```python
   pip install python-ndev-blizzardapi
 ```
 
 ## Usage Example
 ```python
-
   from blizzardAPI import BlizzardAPI
   
   api = BlizzardAPI(client_id, client_secret)
   api.bnet.oauth.get_user_info("us","imagine_token_here")
 ```
 
-### Battle.Net API
+## Blizzard APIs Supported
+
+| API                     | Items           | Obs                   |
+| :---------------------- | :-------------- | :-------------------- |
+| **Battle.Net**          | OAuth API       | All Regions supported |
+| **World Of Warcraft**   | Game Data API   | _Profile Data API in development_ |
 
-| Python      | API URL    | API Name                                    |
-| :---------- | :--------- | :------------------------------------------ |
-| `api.bnet.oauth.get_user_info(region, access_token)`      | `/oauth/userinfo` | User Info (param) |
-| `api.bnet.oauth.get_token_validation(region, access_token)`      | `/oauth/check_token` | Token Validation (GET) |
 
+## Tests using PyTest
+To perform the tests using PyTest, I recommend using the dotenv module. Read more in the documentation provided below.
+```cmd
+pytest blizzardAPI
+```
 
 ## Documentation
 
 [Read the Docs](https://python-ndev-blizzardapi.readthedocs.io/)
```

### Comparing `python-ndev-blizzardapi-0.0.4/setup.py` & `python-ndev-blizzardapi-0.0.5a0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="python-ndev-blizzardapi",
-    version="0.0.4",
+    version="0.0.5-alpha",
     packages=find_packages(),
     install_requires=[
         "requests>=2.28.2",
     ],
     author="natanrmaia",
     author_email="contato@natanael.dev.br",
     description="Python module created to integrate your Python project with the Blizzard API",
```

