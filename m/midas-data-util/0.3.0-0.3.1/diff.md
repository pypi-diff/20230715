# Comparing `tmp/midas-data-util-0.3.0.tar.gz` & `tmp/midas-data-util-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas-data-util-0.3.0.tar", last modified: Sat Jul 15 03:10:52 2023, max compression
+gzip compressed data, was "midas-data-util-0.3.1.tar", last modified: Sat Jul 15 03:34:08 2023, max compression
```

## Comparing `midas-data-util-0.3.0.tar` & `midas-data-util-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 03:10:52.897663 midas-data-util-0.3.0/
--rw-rw-rw-   0        0        0    11558 2023-04-07 08:14:57.000000 midas-data-util-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      520 2023-07-15 03:10:52.896682 midas-data-util-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-04-07 08:58:48.000000 midas-data-util-0.3.0/README.md
--rw-rw-rw-   0        0        0      623 2023-07-15 03:10:33.000000 midas-data-util-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-15 03:10:52.897663 midas-data-util-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-15 03:10:52.866375 midas-data-util-0.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-15 03:10:52.876435 midas-data-util-0.3.0/src/midas/
--rw-rw-rw-   0        0        0     2762 2023-07-15 01:30:04.000000 midas-data-util-0.3.0/src/midas/__init__.py
--rw-rw-rw-   0        0        0     6354 2023-07-15 01:06:50.000000 midas-data-util-0.3.0/src/midas/data_encoder.py
--rw-rw-rw-   0        0        0    11578 2023-07-15 01:36:37.000000 midas-data-util-0.3.0/src/midas/event.py
--rw-rw-rw-   0        0        0    10877 2023-07-15 01:03:25.000000 midas-data-util-0.3.0/src/midas/playfab.py
--rw-rw-rw-   0        0        0     8593 2023-07-15 02:25:06.000000 midas-data-util-0.3.0/src/midas/session.py
--rw-rw-rw-   0        0        0     3686 2023-07-15 03:01:06.000000 midas-data-util-0.3.0/src/midas/user.py
-drwxrwxrwx   0        0        0        0 2023-07-15 03:10:52.895180 midas-data-util-0.3.0/src/midas_data_util.egg-info/
--rw-rw-rw-   0        0        0      520 2023-07-15 03:10:52.000000 midas-data-util-0.3.0/src/midas_data_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-07-15 03:10:52.000000 midas-data-util-0.3.0/src/midas_data_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 03:10:52.000000 midas-data-util-0.3.0/src/midas_data_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-07-15 03:10:52.000000 midas-data-util-0.3.0/src/midas_data_util.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-15 03:10:52.000000 midas-data-util-0.3.0/src/midas_data_util.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2578 2023-07-15 01:34:34.000000 midas-data-util-0.3.0/src/test.py
+drwxrwxrwx   0        0        0        0 2023-07-15 03:34:08.569627 midas-data-util-0.3.1/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 08:14:57.000000 midas-data-util-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      520 2023-07-15 03:34:08.568619 midas-data-util-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-04-07 08:58:48.000000 midas-data-util-0.3.1/README.md
+-rw-rw-rw-   0        0        0      623 2023-07-15 03:33:46.000000 midas-data-util-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-15 03:34:08.569627 midas-data-util-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-15 03:34:08.533161 midas-data-util-0.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-15 03:34:08.543972 midas-data-util-0.3.1/src/midas/
+-rw-rw-rw-   0        0        0     2762 2023-07-15 01:30:04.000000 midas-data-util-0.3.1/src/midas/__init__.py
+-rw-rw-rw-   0        0        0     6354 2023-07-15 01:06:50.000000 midas-data-util-0.3.1/src/midas/data_encoder.py
+-rw-rw-rw-   0        0        0    11578 2023-07-15 01:36:37.000000 midas-data-util-0.3.1/src/midas/event.py
+-rw-rw-rw-   0        0        0    10877 2023-07-15 01:03:25.000000 midas-data-util-0.3.1/src/midas/playfab.py
+-rw-rw-rw-   0        0        0     8593 2023-07-15 03:33:37.000000 midas-data-util-0.3.1/src/midas/session.py
+-rw-rw-rw-   0        0        0     3686 2023-07-15 03:01:06.000000 midas-data-util-0.3.1/src/midas/user.py
+drwxrwxrwx   0        0        0        0 2023-07-15 03:34:08.566635 midas-data-util-0.3.1/src/midas_data_util.egg-info/
+-rw-rw-rw-   0        0        0      520 2023-07-15 03:34:08.000000 midas-data-util-0.3.1/src/midas_data_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-15 03:34:08.000000 midas-data-util-0.3.1/src/midas_data_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 03:34:08.000000 midas-data-util-0.3.1/src/midas_data_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-07-15 03:34:08.000000 midas-data-util-0.3.1/src/midas_data_util.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-15 03:34:08.000000 midas-data-util-0.3.1/src/midas_data_util.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2578 2023-07-15 01:34:34.000000 midas-data-util-0.3.1/src/test.py
```

### Comparing `midas-data-util-0.3.0/LICENSE` & `midas-data-util-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.3.0/PKG-INFO` & `midas-data-util-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-data-util
-Version: 0.3.0
+Version: 0.3.1
 Summary: a package with useful functions for downloading and working with midas generated analytics data
 Author-email: nightcycle <coyer@nightcycle.us>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `midas-data-util-0.3.0/pyproject.toml` & `midas-data-util-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "midas-data-util"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"lxml~=4.9.2", 
 	"pandas~=2.0.0",
 	"adal~=1.2.7",
```

### Comparing `midas-data-util-0.3.0/src/midas/__init__.py` & `midas-data-util-0.3.1/src/midas/__init__.py`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.3.0/src/midas/data_encoder.py` & `midas-data-util-0.3.1/src/midas/data_encoder.py`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.3.0/src/midas/event.py` & `midas-data-util-0.3.1/src/midas/event.py`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.3.0/src/midas/playfab.py` & `midas-data-util-0.3.1/src/midas/playfab.py`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.3.0/src/midas/session.py` & `midas-data-util-0.3.1/src/midas/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 				if self.roblox_language == None:
 					self.roblox_language = safe_index("RobloxLanguage")
 
 				if self.system_language == None:
 					self.system_language = safe_index("SystemLanguage")
 
 				plat_data: Any = safe_index("Platform")
-				if plat_data == None:
+				if plat_data != None:
 					if self.accelerometer == None:
 						self.accelerometer = plat_data["Accelerometer"]
 					if self.gamepad_enabled == None:
 						self.gamepad_enabled = plat_data["Gamepad"]
 					if self.gyroscope_enabled == None:
 						self.gyroscope_enabled = plat_data["Gyroscope"]
 					if self.keyboard_enabled == None:
```

### Comparing `midas-data-util-0.3.0/src/midas/user.py` & `midas-data-util-0.3.1/src/midas/user.py`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.3.0/src/midas_data_util.egg-info/PKG-INFO` & `midas-data-util-0.3.1/src/midas_data_util.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-data-util
-Version: 0.3.0
+Version: 0.3.1
 Summary: a package with useful functions for downloading and working with midas generated analytics data
 Author-email: nightcycle <coyer@nightcycle.us>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `midas-data-util-0.3.0/src/test.py` & `midas-data-util-0.3.1/src/test.py`

 * *Files identical despite different names*

