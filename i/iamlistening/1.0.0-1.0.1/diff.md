# Comparing `tmp/iamlistening-1.0.0.tar.gz` & `tmp/iamlistening-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-1.0.0.tar", max compression
+gzip compressed data, was "iamlistening-1.0.1.tar", max compression
```

## Comparing `iamlistening-1.0.0.tar` & `iamlistening-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-10 15:32:12.869114 iamlistening-1.0.0/LICENSE
--rw-r--r--   0        0        0     3035 2023-07-10 15:32:12.869114 iamlistening-1.0.0/README.md
--rw-r--r--   0        0        0       99 2023-07-10 15:32:13.613127 iamlistening-1.0.0/iamlistening/__init__.py
--rw-r--r--   0        0        0      661 2023-07-10 15:32:12.869114 iamlistening-1.0.0/iamlistening/config.py
--rw-r--r--   0        0        0      826 2023-07-10 15:32:12.869114 iamlistening-1.0.0/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     3957 2023-07-10 15:32:12.869114 iamlistening-1.0.0/iamlistening/main.py
--rw-r--r--   0        0        0     2414 2023-07-10 15:32:13.613127 iamlistening-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3962 1970-01-01 00:00:00.000000 iamlistening-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-15 12:59:39.980152 iamlistening-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3035 2023-07-15 12:59:39.980152 iamlistening-1.0.1/README.md
+-rw-r--r--   0        0        0       99 2023-07-15 12:59:40.976167 iamlistening-1.0.1/iamlistening/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-15 12:59:39.980152 iamlistening-1.0.1/iamlistening/config.py
+-rw-r--r--   0        0        0      826 2023-07-15 12:59:39.980152 iamlistening-1.0.1/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     3961 2023-07-15 12:59:39.980152 iamlistening-1.0.1/iamlistening/main.py
+-rw-r--r--   0        0        0     2414 2023-07-15 12:59:40.976167 iamlistening-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3962 1970-01-01 00:00:00.000000 iamlistening-1.0.1/PKG-INFO
```

### Comparing `iamlistening-1.0.0/LICENSE` & `iamlistening-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-1.0.0/README.md` & `iamlistening-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-1.0.0/iamlistening/config.py` & `iamlistening-1.0.1/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-1.0.0/iamlistening/default_settings.toml` & `iamlistening-1.0.1/iamlistening/default_settings.toml`

 * *Files identical despite different names*

### Comparing `iamlistening-1.0.0/iamlistening/main.py` & `iamlistening-1.0.1/iamlistening/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,9 +116,9 @@
     async def post_init(self):
         return "bot is online"
 
     def stop(self):
         """Stop the listener."""
         self.stopped = True
 
-    async def get_info(self):
-        return f"{__class__.__name__} {__version__}\n"
+    # async def get_info(self):
+    #     return f"{__class__.__name__} {__version__}\n"
```

### Comparing `iamlistening-1.0.0/pyproject.toml` & `iamlistening-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "1.0.0"
+version = "1.0.1"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["discord", "telegram", "bot","messaging","matrix"]
 packages = [
     {include = "iamlistening"}
```

### Comparing `iamlistening-1.0.0/PKG-INFO` & `iamlistening-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 1.0.0
+Version: 1.0.1
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: discord,telegram,bot,messaging,matrix
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

