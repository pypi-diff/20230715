# Comparing `tmp/letsbuilda-pypi-5.0.0b1.tar.gz` & `tmp/letsbuilda-pypi-5.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "letsbuilda-pypi-5.0.0b1.tar", last modified: Thu Jul 13 05:09:48 2023, max compression
+gzip compressed data, was "letsbuilda-pypi-5.0.0b2.tar", last modified: Fri Jul 14 23:49:04 2023, max compression
```

## Comparing `letsbuilda-pypi-5.0.0b1.tar` & `letsbuilda-pypi-5.0.0b2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 05:09:48.354054 letsbuilda-pypi-5.0.0b1/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1074 2023-07-12 21:27:21.000000 letsbuilda-pypi-5.0.0b1/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1145 2023-07-13 05:09:48.354054 letsbuilda-pypi-5.0.0b1/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      644 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b1/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1264 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b1/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-07-13 05:09:48.354054 letsbuilda-pypi-5.0.0b1/setup.cfg
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 05:09:48.354054 letsbuilda-pypi-5.0.0b1/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 05:09:48.344054 letsbuilda-pypi-5.0.0b1/src/letsbuilda/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 05:09:48.354054 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      232 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2435 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/async_client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      511 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/exceptions.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      880 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/files.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 05:09:48.354054 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/models/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      212 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/models/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3572 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/models/models_json.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1383 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/models/models_package.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1200 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/models/models_rss.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2121 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/sync_client.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 05:09:48.354054 letsbuilda-pypi-5.0.0b1/src/letsbuilda_pypi.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1145 2023-07-13 05:09:48.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda_pypi.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-07-13 05:09:48.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-13 05:09:48.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      146 2023-07-13 05:09:48.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda_pypi.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       11 2023-07-13 05:09:48.000000 letsbuilda-pypi-5.0.0b1/src/letsbuilda_pypi.egg-info/top_level.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 05:09:48.354054 letsbuilda-pypi-5.0.0b1/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1250 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b1/tests/test_rss_feed_parsing.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-14 23:49:04.437579 letsbuilda-pypi-5.0.0b2/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1074 2023-07-12 21:27:21.000000 letsbuilda-pypi-5.0.0b2/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1145 2023-07-14 23:49:04.437579 letsbuilda-pypi-5.0.0b2/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      644 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b2/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1264 2023-07-14 23:46:47.000000 letsbuilda-pypi-5.0.0b2/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-07-14 23:49:04.437579 letsbuilda-pypi-5.0.0b2/setup.cfg
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-14 23:49:04.417579 letsbuilda-pypi-5.0.0b2/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-14 23:49:04.417579 letsbuilda-pypi-5.0.0b2/src/letsbuilda/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-14 23:49:04.437579 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      232 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2444 2023-07-14 23:45:41.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/async_client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      511 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/exceptions.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      880 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/files.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-14 23:49:04.437579 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/models/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      212 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/models/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3572 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/models/models_json.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1383 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/models/models_package.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1200 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/models/models_rss.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2121 2023-07-13 05:09:35.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/sync_client.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-14 23:49:04.437579 letsbuilda-pypi-5.0.0b2/src/letsbuilda_pypi.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1145 2023-07-14 23:49:04.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-07-14 23:49:04.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-14 23:49:04.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      146 2023-07-14 23:49:04.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda_pypi.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       11 2023-07-14 23:49:04.000000 letsbuilda-pypi-5.0.0b2/src/letsbuilda_pypi.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-14 23:49:04.437579 letsbuilda-pypi-5.0.0b2/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1250 2023-07-13 03:45:05.000000 letsbuilda-pypi-5.0.0b2/tests/test_rss_feed_parsing.py
```

### Comparing `letsbuilda-pypi-5.0.0b1/LICENSE` & `letsbuilda-pypi-5.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-5.0.0b1/PKG-INFO` & `letsbuilda-pypi-5.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letsbuilda-pypi
-Version: 5.0.0b1
+Version: 5.0.0b2
 Summary: A wrapper for PyPI's API and RSS feed
 Author-email: Bradley Reynolds <bradley.reynolds@darbia.dev>
 License: MIT
 Project-URL: repository, https://github.com/letsbuilda/letsbuilda-pypi/
 Project-URL: documentation, https://docs.letsbuilda.dev/letsbuilda-pypi/
 Requires-Python: >=3.11.4
 Description-Content-Type: text/markdown
```

### Comparing `letsbuilda-pypi-5.0.0b1/README.md` & `letsbuilda-pypi-5.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-5.0.0b1/pyproject.toml` & `letsbuilda-pypi-5.0.0b2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "letsbuilda-pypi"
-version = "5.0.0b1"
+version = "5.0.0b2"
 description = "A wrapper for PyPI's API and RSS feed"
 authors = [
     { name = "Bradley Reynolds", email = "bradley.reynolds@darbia.dev" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
 requires-python = ">=3.11.4"
```

### Comparing `letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/async_client.py` & `letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     async def get_package_metadata(
         self: Self,
         package_title: str,
         package_version: str | None = None,
     ) -> Package:
         """Get metadata for a package."""
-        return Package.from_dict(await self.get_package_json_metadata(package_title, package_version))
+        return Package.from_json_api_data(await self.get_package_json_metadata(package_title, package_version))
 
     async def fetch_bytes(
         self: Self,
         url: str,
     ) -> BytesIO:
         """Fetch bytes from a URL."""
         buffer = BytesIO()
```

### Comparing `letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/files.py` & `letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/files.py`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/models/models_json.py` & `letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/models/models_json.py`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/models/models_package.py` & `letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/models/models_package.py`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/models/models_rss.py` & `letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/models/models_rss.py`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-5.0.0b1/src/letsbuilda/pypi/sync_client.py` & `letsbuilda-pypi-5.0.0b2/src/letsbuilda/pypi/sync_client.py`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-5.0.0b1/src/letsbuilda_pypi.egg-info/PKG-INFO` & `letsbuilda-pypi-5.0.0b2/src/letsbuilda_pypi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: letsbuilda-pypi
-Version: 5.0.0b1
+Version: 5.0.0b2
 Summary: A wrapper for PyPI's API and RSS feed
 Author-email: Bradley Reynolds <bradley.reynolds@darbia.dev>
 License: MIT
 Project-URL: repository, https://github.com/letsbuilda/letsbuilda-pypi/
 Project-URL: documentation, https://docs.letsbuilda.dev/letsbuilda-pypi/
 Requires-Python: >=3.11.4
 Description-Content-Type: text/markdown
```

### Comparing `letsbuilda-pypi-5.0.0b1/src/letsbuilda_pypi.egg-info/SOURCES.txt` & `letsbuilda-pypi-5.0.0b2/src/letsbuilda_pypi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `letsbuilda-pypi-5.0.0b1/tests/test_rss_feed_parsing.py` & `letsbuilda-pypi-5.0.0b2/tests/test_rss_feed_parsing.py`

 * *Files identical despite different names*

