# Comparing `tmp/Jedutils-0.1.4.tar.gz` & `tmp/Jedutils-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jedutils-0.1.4.tar", last modified: Fri Jul 14 22:26:50 2023, max compression
+gzip compressed data, was "Jedutils-0.1.5.tar", last modified: Sat Jul 15 20:54:06 2023, max compression
```

## Comparing `Jedutils-0.1.4.tar` & `Jedutils-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:26:50.165222 Jedutils-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:26:50.165222 Jedutils-0.1.4/Jedutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-14 22:26:50.000000 Jedutils-0.1.4/Jedutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-14 22:26:50.000000 Jedutils-0.1.4/Jedutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:26:50.000000 Jedutils-0.1.4/Jedutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-14 22:26:50.000000 Jedutils-0.1.4/Jedutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 22:26:48.000000 Jedutils-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 22:26:48.000000 Jedutils-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-14 22:26:50.165222 Jedutils-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-14 22:26:48.000000 Jedutils-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:26:50.165222 Jedutils-0.1.4/jedutils/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-14 22:26:48.000000 Jedutils-0.1.4/jedutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:26:50.165222 Jedutils-0.1.4/jedutils/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-14 22:26:48.000000 Jedutils-0.1.4/jedutils/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-14 22:26:48.000000 Jedutils-0.1.4/jedutils/asyncio/_async_redis_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-14 22:26:48.000000 Jedutils-0.1.4/jedutils/asyncio/_run_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:26:50.165222 Jedutils-0.1.4/jedutils/asyncio/network/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-14 22:26:48.000000 Jedutils-0.1.4/jedutils/asyncio/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-14 22:26:48.000000 Jedutils-0.1.4/jedutils/asyncio/network/_dl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:26:50.165222 Jedutils-0.1.4/jedutils/strings/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-14 22:26:48.000000 Jedutils-0.1.4/jedutils/strings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-14 22:26:48.000000 Jedutils-0.1.4/jedutils/strings/_random_string.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 22:26:50.165222 Jedutils-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-14 22:26:48.000000 Jedutils-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:54:06.207196 Jedutils-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:54:06.203196 Jedutils-0.1.5/Jedutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-15 20:54:06.000000 Jedutils-0.1.5/Jedutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-15 20:54:06.000000 Jedutils-0.1.5/Jedutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 20:54:06.000000 Jedutils-0.1.5/Jedutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-15 20:54:06.000000 Jedutils-0.1.5/Jedutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 20:54:06.000000 Jedutils-0.1.5/Jedutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-15 20:54:04.000000 Jedutils-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-15 20:54:04.000000 Jedutils-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-15 20:54:06.207196 Jedutils-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-15 20:54:04.000000 Jedutils-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:54:06.207196 Jedutils-0.1.5/jedutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-15 20:54:04.000000 Jedutils-0.1.5/jedutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:54:06.207196 Jedutils-0.1.5/jedutils/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-15 20:54:04.000000 Jedutils-0.1.5/jedutils/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-15 20:54:04.000000 Jedutils-0.1.5/jedutils/asyncio/_async_redis_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-15 20:54:04.000000 Jedutils-0.1.5/jedutils/asyncio/_run_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:54:06.207196 Jedutils-0.1.5/jedutils/asyncio/network/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-15 20:54:04.000000 Jedutils-0.1.5/jedutils/asyncio/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-15 20:54:04.000000 Jedutils-0.1.5/jedutils/asyncio/network/_dl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:54:06.207196 Jedutils-0.1.5/jedutils/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-15 20:54:04.000000 Jedutils-0.1.5/jedutils/strings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-15 20:54:04.000000 Jedutils-0.1.5/jedutils/strings/_random_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 20:54:06.207196 Jedutils-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-15 20:54:04.000000 Jedutils-0.1.5/setup.py
```

### Comparing `Jedutils-0.1.4/Jedutils.egg-info/PKG-INFO` & `Jedutils-0.1.5/Jedutils.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: Jedutils
-Version: 0.1.4
+Version: 0.1.5
 Summary: Jedutils is a Python utilities package that provides a collection of useful helper functions.
 Home-page: https://github.com/AYMENJD/jedutils
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AYMENJD/jedutils
 Project-URL: Tracker, https://github.com/AYMENJD/jedutils/issues
 Keywords: utilities,tools,library,helper,functions,development
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Provides-Extra: all
 License-File: LICENSE
 
 # Jedutils [![Version](https://img.shields.io/pypi/v/jedutils?style=flat&logo=pypi)](https://pypi.org/project/jedutils) [![Downloads](https://static.pepy.tech/personalized-badge/jedutils?period=month&units=none&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/jedutils)
 
 Jedutils is a Python utilities package that provides a collection of useful helper functions.
 
 ## Installation
 
 You can install Jedutils using `pip`:
 
 ```bash
 pip install jedutils
 ```
 
-To install the development version from Github, use the following command:
+To install all the dependencies for all utilities, use the following command:
 ```bash
-pip install git+https://github.com/AYMENJD/jedutils.git
+pip install jedutils[all]
 ```
 
 ## Contributing
 
 Contributions to Jedutils are welcome! If you have an idea for a new utility or an improvement to an existing one, please open an issue or submit a pull request on GitHub.
 
 ## License
```

### Comparing `Jedutils-0.1.4/LICENSE` & `Jedutils-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Jedutils-0.1.4/PKG-INFO` & `Jedutils-0.1.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: Jedutils
-Version: 0.1.4
+Version: 0.1.5
 Summary: Jedutils is a Python utilities package that provides a collection of useful helper functions.
 Home-page: https://github.com/AYMENJD/jedutils
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AYMENJD/jedutils
 Project-URL: Tracker, https://github.com/AYMENJD/jedutils/issues
 Keywords: utilities,tools,library,helper,functions,development
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Provides-Extra: all
 License-File: LICENSE
 
 # Jedutils [![Version](https://img.shields.io/pypi/v/jedutils?style=flat&logo=pypi)](https://pypi.org/project/jedutils) [![Downloads](https://static.pepy.tech/personalized-badge/jedutils?period=month&units=none&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/jedutils)
 
 Jedutils is a Python utilities package that provides a collection of useful helper functions.
 
 ## Installation
 
 You can install Jedutils using `pip`:
 
 ```bash
 pip install jedutils
 ```
 
-To install the development version from Github, use the following command:
+To install all the dependencies for all utilities, use the following command:
 ```bash
-pip install git+https://github.com/AYMENJD/jedutils.git
+pip install jedutils[all]
 ```
 
 ## Contributing
 
 Contributions to Jedutils are welcome! If you have an idea for a new utility or an improvement to an existing one, please open an issue or submit a pull request on GitHub.
 
 ## License
```

### Comparing `Jedutils-0.1.4/README.md` & `Jedutils-0.1.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 You can install Jedutils using `pip`:
 
 ```bash
 pip install jedutils
 ```
 
-To install the development version from Github, use the following command:
+To install all the dependencies for all utilities, use the following command:
 ```bash
-pip install git+https://github.com/AYMENJD/jedutils.git
+pip install jedutils[all]
 ```
 
 ## Contributing
 
 Contributions to Jedutils are welcome! If you have an idea for a new utility or an improvement to an existing one, please open an issue or submit a pull request on GitHub.
 
 ## License
```

### Comparing `Jedutils-0.1.4/jedutils/asyncio/_async_redis_pipe.py` & `Jedutils-0.1.5/jedutils/asyncio/_async_redis_pipe.py`

 * *Files identical despite different names*

### Comparing `Jedutils-0.1.4/jedutils/asyncio/network/_dl.py` & `Jedutils-0.1.5/jedutils/asyncio/network/_dl.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 import os
 
 
 async def download_file(
     url: str,
     filename: str,
     chunk_size: int = 8192,
-    headers: dict = None,
     ignore_status: bool = False,
-    timeout: float = None,
     progress_callback: callable = None,
     thread_pool=None,
+    **kwargs
 ) -> None:
     """
     Asynchronously download a file from the given URL and saves it to the specified filename using chunked downloading
 
     Example:
         Download a large file asynchronously:
 
@@ -32,37 +31,33 @@
 
         filename (``str``, *optional*):
             The filename to save the downloaded file as
 
         chunk_size (``int``, *optional*):
             The size of each chunk to download in bytes. Default is 8192 bytes (8 KB)
 
-        headers (``dict``, *optional*):
-            A dictionary of headers to send with the request. Default is ``None``
-
         ignore_status (``bool``, *optional*):
             Whether to ignore errors in the response from the server. Default is ``False``
 
-        timeout (``float``, *optional*):
-            A timeout for the request. Default is ``None``
-
         progress_callback (``callable``, *optional*):
             A callable function to be called with the download progress, in bytes
 
         thread_pool:
             A thread pool to use for blocking operations. Default is ``None``
 
+        \*\*kwargs:
+            Any additional keyword arguments to pass to the `aiohttp.get` call
     Returns:
         ``None``
 
     Raises:
         :py:class:`aiohttp.ClientResponseError`
     """
     async with aiohttp.ClientSession() as session:
-        async with session.get(url, timeout=timeout, headers=headers) as response:
+        async with session.get(url, **kwargs) as response:
             if not ignore_status:
                 response.raise_for_status()
 
             expected_size = int(response.headers.get("content-length", 0))
             downloaded_size = 0
             loop = asyncio.get_event_loop()
```

### Comparing `Jedutils-0.1.4/jedutils/strings/_random_string.py` & `Jedutils-0.1.5/jedutils/strings/_random_string.py`

 * *Files identical despite different names*

### Comparing `Jedutils-0.1.4/setup.py` & `Jedutils-0.1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     url="https://github.com/AYMENJD/jedutils",
     license="MIT",
     project_urls={
         "Source": "https://github.com/AYMENJD/jedutils",
         "Tracker": "https://github.com/AYMENJD/jedutils/issues",
     },
     packages=find_packages(),
+    extras_require={
+        "all": ["redis", "aiohttp"],
+    },
     keywords=[
         "utilities",
         "tools",
         "library",
         "helper",
         "functions",
         "development",
```

