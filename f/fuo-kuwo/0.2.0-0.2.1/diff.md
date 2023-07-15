# Comparing `tmp/fuo-kuwo-0.2.0.tar.gz` & `tmp/fuo-kuwo-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuo-kuwo-0.2.0.tar", last modified: Wed Jul 12 17:02:22 2023, max compression
+gzip compressed data, was "fuo-kuwo-0.2.1.tar", last modified: Sat Jul 15 06:48:55 2023, max compression
```

## Comparing `fuo-kuwo-0.2.0.tar` & `fuo-kuwo-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:02:22.227140 fuo-kuwo-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35123 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-12 17:02:22.227140 fuo-kuwo-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:02:22.223140 fuo-kuwo-0.2.0/fuo_kuwo/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16723 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:02:22.223140 fuo-kuwo-0.2.0/fuo_kuwo/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/assets/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    14913 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/assets/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:02:22.223140 fuo-kuwo-0.2.0/fuo_kuwo/enc/
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/enc/DES.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/enc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/enc/decrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:02:22.227140 fuo-kuwo-0.2.0/fuo_kuwo/pages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/pages/explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/fuo_kuwo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:02:22.223140 fuo-kuwo-0.2.0/fuo_kuwo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-12 17:02:22.000000 fuo-kuwo-0.2.0/fuo_kuwo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-12 17:02:22.000000 fuo-kuwo-0.2.0/fuo_kuwo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:02:22.000000 fuo-kuwo-0.2.0/fuo_kuwo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-12 17:02:22.000000 fuo-kuwo-0.2.0/fuo_kuwo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:02:22.000000 fuo-kuwo-0.2.0/fuo_kuwo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 17:02:22.000000 fuo-kuwo-0.2.0/fuo_kuwo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:02:22.227140 fuo-kuwo-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-07-12 17:02:16.000000 fuo-kuwo-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:48:55.646412 fuo-kuwo-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35123 2023-07-15 06:48:54.000000 fuo-kuwo-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-15 06:48:55.646412 fuo-kuwo-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-15 06:48:54.000000 fuo-kuwo-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:48:55.646412 fuo-kuwo-0.2.1/fuo_kuwo/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-15 06:48:54.000000 fuo-kuwo-0.2.1/fuo_kuwo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16752 2023-07-15 06:48:54.000000 fuo-kuwo-0.2.1/fuo_kuwo/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:48:55.646412 fuo-kuwo-0.2.1/fuo_kuwo/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-15 06:48:54.000000 fuo-kuwo-0.2.1/fuo_kuwo/assets/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14913 2023-07-15 06:48:54.000000 fuo-kuwo-0.2.1/fuo_kuwo/assets/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:48:55.646412 fuo-kuwo-0.2.1/fuo_kuwo/enc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-07-15 06:48:54.000000 fuo-kuwo-0.2.1/fuo_kuwo/enc/DES.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:48:54.000000 fuo-kuwo-0.2.1/fuo_kuwo/enc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-15 06:48:54.000000 fuo-kuwo-0.2.1/fuo_kuwo/enc/decrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:48:55.646412 fuo-kuwo-0.2.1/fuo_kuwo/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:48:54.000000 fuo-kuwo-0.2.1/fuo_kuwo/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-15 06:48:54.000000 fuo-kuwo-0.2.1/fuo_kuwo/pages/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9785 2023-07-15 06:48:54.000000 fuo-kuwo-0.2.1/fuo_kuwo/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-15 06:48:54.000000 fuo-kuwo-0.2.1/fuo_kuwo/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-15 06:48:54.000000 fuo-kuwo-0.2.1/fuo_kuwo/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-15 06:48:54.000000 fuo-kuwo-0.2.1/fuo_kuwo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:48:55.646412 fuo-kuwo-0.2.1/fuo_kuwo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-15 06:48:55.000000 fuo-kuwo-0.2.1/fuo_kuwo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-15 06:48:55.000000 fuo-kuwo-0.2.1/fuo_kuwo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:48:55.000000 fuo-kuwo-0.2.1/fuo_kuwo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-15 06:48:55.000000 fuo-kuwo-0.2.1/fuo_kuwo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:48:55.000000 fuo-kuwo-0.2.1/fuo_kuwo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 06:48:55.000000 fuo-kuwo-0.2.1/fuo_kuwo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-15 06:48:54.000000 fuo-kuwo-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:48:55.646412 fuo-kuwo-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-15 06:48:54.000000 fuo-kuwo-0.2.1/setup.py
```

### Comparing `fuo-kuwo-0.2.0/LICENSE` & `fuo-kuwo-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fuo-kuwo-0.2.0/PKG-INFO` & `fuo-kuwo-0.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: fuo-kuwo
-Version: 0.2.0
-Summary: Kuwo music provider for FeelUOwn music player
-Home-page: https://github.com/feeluown/feeluown-kuwo
-Author: feeluown team
-Requires-Python: >=3.8,<4.0
-License-File: LICENSE
-
 # Kuwo music provider for FeelUOwn player
 
 ## Installation
 
 ### Arch Linux
 `pacman -S feeluown-kuwo`
 
@@ -28,14 +19,17 @@
 ## Run tests
 `pytest -v`
 
 test_kuwo_api.py -- Kuwo API tests
 
 ## Changelog
 
+### v0.2.1 (2023-07-15)
+* 修复 API 不可用的问题
+
 ### v0.2.0 (2023-07-13)
 * 修复 API 不可用的问题
 * 适配 feeluown v2 model，废弃 v1 models
 
 ### v0.1.6 (2022-06-08)
 * 修复获取歌曲/mv播放链接有一定概率会失败的问题
```

### Comparing `fuo-kuwo-0.2.0/fuo_kuwo/__init__.py` & `fuo-kuwo-0.2.1/fuo_kuwo/__init__.py`

 * *Files identical despite different names*

### Comparing `fuo-kuwo-0.2.0/fuo_kuwo/api.py` & `fuo-kuwo-0.2.1/fuo_kuwo/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import time
 from pathlib import Path
-from hashlib import md5
+from hashlib import md5, sha1
 
 import requests
 from requests.cookies import RequestsCookieJar
 from fuo_kuwo.enc.DES import base64_encrypt
 from fuo_kuwo.utils import digest_encrypt
 
 logger = logging.getLogger(__name__)
@@ -65,16 +65,17 @@
             'User-Agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) '
                           'Chrome/81.0.4044.138 Safari/537.36',
             'Host': 'kuwo.cn',
         }
         self.mobi_headers = {'User-Agent': 'okhttp/3.10.0'}
         random_str = '123456789'
         self.headers['csrf'] = random_str
-        self.cookie = {'kw_token': random_str, 'Hm_token': random_str}
-        self.headers['Cross'] = md5(random_str.encode('utf-8')).hexdigest()
+        self.cookie = {'Hm_token': random_str}
+        self.headers['Cross'] = md5(bytes(
+            sha1(random_str.encode('utf-8')).hexdigest(), 'utf-8')).hexdigest()
         self._userid = ''
         self._sid = ''
         self._cookies = {}
 
     def set_cookies(self, cookies):
         if cookies:
             self._cookies = cookies
```

### Comparing `fuo-kuwo-0.2.0/fuo_kuwo/assets/icon.svg` & `fuo-kuwo-0.2.1/fuo_kuwo/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `fuo-kuwo-0.2.0/fuo_kuwo/enc/DES.py` & `fuo-kuwo-0.2.1/fuo_kuwo/enc/DES.py`

 * *Files identical despite different names*

### Comparing `fuo-kuwo-0.2.0/fuo_kuwo/enc/decrypt.py` & `fuo-kuwo-0.2.1/fuo_kuwo/enc/decrypt.py`

 * *Files identical despite different names*

### Comparing `fuo-kuwo-0.2.0/fuo_kuwo/pages/explorer.py` & `fuo-kuwo-0.2.1/fuo_kuwo/pages/explorer.py`

 * *Files identical despite different names*

### Comparing `fuo-kuwo-0.2.0/fuo_kuwo/provider.py` & `fuo-kuwo-0.2.1/fuo_kuwo/provider.py`

 * *Files identical despite different names*

### Comparing `fuo-kuwo-0.2.0/fuo_kuwo/schemas.py` & `fuo-kuwo-0.2.1/fuo_kuwo/schemas.py`

 * *Files identical despite different names*

### Comparing `fuo-kuwo-0.2.0/fuo_kuwo/ui.py` & `fuo-kuwo-0.2.1/fuo_kuwo/ui.py`

 * *Files identical despite different names*

### Comparing `fuo-kuwo-0.2.0/fuo_kuwo/utils.py` & `fuo-kuwo-0.2.1/fuo_kuwo/utils.py`

 * *Files identical despite different names*

### Comparing `fuo-kuwo-0.2.0/fuo_kuwo.egg-info/SOURCES.txt` & `fuo-kuwo-0.2.1/fuo_kuwo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuo-kuwo-0.2.0/pyproject.toml` & `fuo-kuwo-0.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fuo_kuwo"
-version = "0.2.0"
+version = "0.2.1"
 description = "Kuwo music provider for FeelUOwn music player"
 authors = ["feeluown team"]
 readme = "README.md"
 license = "GPL"
 homepage = "https://github.com/feeluown/feeluown-kuwo"
 keywords = ["feeluown", "plugin", "kuwo"]
 packages = [{ include = "fuo_kuwo" }]
```

