# Comparing `tmp/wander-0.1.0.tar.gz` & `tmp/wander-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wander-0.1.0.tar", max compression
+gzip compressed data, was "wander-0.1.1.tar", max compression
```

## Comparing `wander-0.1.0.tar` & `wander-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rwxr-xr-x   0        0        0     1070 2023-05-17 09:47:14.232700 wander-0.1.0/LICENSE.md
--rwxr-xr-x   0        0        0     1267 2023-05-17 09:48:10.347421 wander-0.1.0/README.md
--rwxr-xr-x   0        0        0      416 2023-05-17 09:44:10.591595 wander-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0       30 2023-05-17 07:16:03.705863 wander-0.1.0/wander/__init__.py
--rwxr-xr-x   0        0        0     1229 2023-05-17 08:06:41.100964 wander-0.1.0/wander/models.py
--rwxr-xr-x   0        0        0       31 2023-05-17 08:06:40.605687 wander-0.1.0/wander/plugins/__init__.py
--rwxr-xr-x   0        0        0     1048 2023-05-17 09:48:58.985874 wander-0.1.0/wander/plugins/shell.py
--rwxr-xr-x   0        0        0     1664 2023-05-17 08:56:31.471009 wander-0.1.0/wander/render.py
--rwxr-xr-x   0        0        0      357 2023-05-17 08:06:40.611035 wander-0.1.0/wander/utils.py
--rw-r--r--   0        0        0     1710 1970-01-01 00:00:00.000000 wander-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-05-17 09:47:14.232700 wander-0.1.1/LICENSE.md
+-rwxr-xr-x   0        0        0     1268 2023-05-17 10:15:30.066940 wander-0.1.1/README.md
+-rwxr-xr-x   0        0        0      466 2023-07-15 12:51:36.103960 wander-0.1.1/pyproject.toml
+-rwxr-xr-x   0        0        0       30 2023-05-17 07:16:03.705863 wander-0.1.1/wander/__init__.py
+-rwxr-xr-x   0        0        0     1236 2023-05-17 13:39:13.163869 wander-0.1.1/wander/models.py
+-rwxr-xr-x   0        0        0       69 2023-05-17 13:44:24.798888 wander-0.1.1/wander/plugins/__init__.py
+-rwxr-xr-x   0        0        0      400 2023-05-17 13:43:59.486502 wander-0.1.1/wander/plugins/clipboard.py
+-rwxr-xr-x   0        0        0     1048 2023-05-17 09:48:58.985874 wander-0.1.1/wander/plugins/shell.py
+-rwxr-xr-x   0        0        0     1664 2023-05-17 08:56:31.471009 wander-0.1.1/wander/render.py
+-rwxr-xr-x   0        0        0      353 2023-05-17 13:52:21.411065 wander-0.1.1/wander/utils.py
+-rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 wander-0.1.1/PKG-INFO
```

### Comparing `wander-0.1.0/LICENSE.md` & `wander-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wander-0.1.0/README.md` & `wander-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,36 +6,36 @@
 
 You can install `wander` with `pip`
 
 ```python
 pip install wander
 ```
 
-You need to have Python version of 3.10 or above to use this library.
+You need to have Python version 3.10 or above to use this library.
 
 ## Usage
 
 Assuming you have an markdown text with a special block `!shell`.
 
 ````python
 text = """\
 Today is:
 ```!shell
 date
-```
+```\
 """
 ````
 
 Using `wander` to render it.
 
 ```python
 from wander import Renderer
 from wander.plugins import ShellPlugin
 
-renderer = Renderer(plugins=[ShellPlugin])
+renderer = Renderer(plugins=[ShellPlugin()])
 renderer.render(text)
 ```
 
 Output:
 ```
 Today is:
 Wed May 17 16:48:09 +08 2023
@@ -46,8 +46,8 @@
 
 To write your own plugin, simply inherit the `Plugin` class and do the following:
 
 - Specify `plugin_name` property. This will be the name of the directive used in your special block.
 - Specify `parser` property, which is an `argparse.ArgumentParser` object to define what CLI-like arguments are accepted after the directive name
 - Implement `run` async method. It must takes an `args` argument holding all the values of the command arguments defined in your parser as well as `content` argument holding all texts in the block.
 
-You can find an example in [shell.py](wander/plugins/shell.py).
+You can find an example in [shell.py](wander/plugins/shell.py).
```

### Comparing `wander-0.1.0/wander/models.py` & `wander-0.1.1/wander/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         for i in INVALID_SYMBOLS:
             if i in value:
                 raise ValueError(f"Plugin name contains invalid symbol {i}")
 
         return value
 
     @abstractmethod
-    async def run(self, args: Dict[str, Any], content: str):
+    async def run(self, args: Dict[str, Any], content: str) -> str:
         # We will always assume async run
         raise NotImplementedError
 
     def parse_args(self, tokenized: List[str]) -> Dict[str, Any]:
         args = self.parser.parse_args(tokenized)
         args = self.namespace_to_dict(args)
         return args
```

### Comparing `wander-0.1.0/wander/plugins/shell.py` & `wander-0.1.1/wander/plugins/shell.py`

 * *Files identical despite different names*

### Comparing `wander-0.1.0/wander/render.py` & `wander-0.1.1/wander/render.py`

 * *Files identical despite different names*

### Comparing `wander-0.1.0/PKG-INFO` & `wander-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 Metadata-Version: 2.1
 Name: wander
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
+Home-page: https://github.com/outday29/wander
 License: MIT
 Author: engkheng
 Author-email: ongengkheng929@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Project-URL: Repository, https://github.com/outday29/wander
 Description-Content-Type: text/markdown
 
 # Wander
 
 `wander` is a simple Python library that makes it easier to incorporate external data into LLM prompt.
 
 ## Installation
 
 You can install `wander` with `pip`
 
 ```python
 pip install wander
 ```
 
-You need to have Python version of 3.10 or above to use this library.
+You need to have Python version 3.10 or above to use this library.
 
 ## Usage
 
 Assuming you have an markdown text with a special block `!shell`.
 
 ````python
 text = """\
 Today is:
 ```!shell
 date
-```
+```\
 """
 ````
 
 Using `wander` to render it.
 
 ```python
 from wander import Renderer
 from wander.plugins import ShellPlugin
 
-renderer = Renderer(plugins=[ShellPlugin])
+renderer = Renderer(plugins=[ShellPlugin()])
 renderer.render(text)
 ```
 
 Output:
 ```
 Today is:
 Wed May 17 16:48:09 +08 2023
@@ -62,7 +64,8 @@
 To write your own plugin, simply inherit the `Plugin` class and do the following:
 
 - Specify `plugin_name` property. This will be the name of the directive used in your special block.
 - Specify `parser` property, which is an `argparse.ArgumentParser` object to define what CLI-like arguments are accepted after the directive name
 - Implement `run` async method. It must takes an `args` argument holding all the values of the command arguments defined in your parser as well as `content` argument holding all texts in the block.
 
 You can find an example in [shell.py](wander/plugins/shell.py).
+
```

