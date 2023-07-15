# Comparing `tmp/mine-3.1.tar.gz` & `tmp/mine-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mine-3.1.tar", max compression
+gzip compressed data, was "mine-3.1.1.tar", max compression
```

## Comparing `mine-3.1.tar` & `mine-3.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1088 2019-05-21 02:49:19.000000 mine-3.1/LICENSE.md
--rw-r--r--   0        0        0     2840 2023-04-16 19:11:58.196023 mine-3.1/README.md
--rw-r--r--   0        0        0      340 2023-04-16 19:25:03.010573 mine-3.1/mine/__init__.py
--rw-r--r--   0        0        0     6624 2023-04-16 19:11:58.197283 mine-3.1/mine/cli.py
--rw-r--r--   0        0        0     2865 2023-04-16 19:11:58.197615 mine-3.1/mine/common.py
--rw-r--r--   0        0        0     6669 2023-04-16 19:18:48.322162 mine-3.1/mine/manager.py
--rw-r--r--   0        0        0      232 2019-05-21 02:49:19.000000 mine-3.1/mine/models/__init__.py
--rw-r--r--   0        0        0      424 2021-06-02 19:31:21.821486 mine-3.1/mine/models/_bases.py
--rw-r--r--   0        0        0     1803 2019-05-21 02:49:19.000000 mine-3.1/mine/models/application.py
--rw-r--r--   0        0        0     4386 2023-07-15 03:37:50.766601 mine-3.1/mine/models/computer.py
--rw-r--r--   0        0        0      501 2019-05-21 02:49:19.000000 mine-3.1/mine/models/config.py
--rw-r--r--   0        0        0     5145 2020-05-16 16:13:05.000000 mine-3.1/mine/models/data.py
--rw-r--r--   0        0        0     6544 2022-09-08 17:31:06.428139 mine-3.1/mine/models/status.py
--rw-r--r--   0        0        0     1052 2019-05-21 02:49:19.000000 mine-3.1/mine/models/timestamp.py
--rwxr-xr-x   0        0        0     2667 2023-04-16 19:11:58.198225 mine-3.1/mine/services.py
--rw-r--r--   0        0        0      573 2023-04-16 19:13:26.811463 mine-3.1/mine/settings.py
--rw-r--r--   0        0        0       34 2016-09-23 05:48:42.000000 mine-3.1/mine/tests/__init__.py
--rw-r--r--   0        0        0     1038 2023-04-16 19:11:58.198685 mine-3.1/mine/tests/conftest.py
--rw-r--r--   0        0        0        9 2016-09-23 02:41:14.000000 mine-3.1/mine/tests/files/.gitignore
--rw-r--r--   0        0        0      513 2016-09-23 02:41:14.000000 mine-3.1/mine/tests/files/mine-in.yml
--rw-r--r--   0        0        0      587 2016-09-23 02:41:14.000000 mine-3.1/mine/tests/files/mine-out.yml
--rw-r--r--   0        0        0     3996 2023-04-16 19:11:58.199066 mine-3.1/mine/tests/test_cli.py
--rw-r--r--   0        0        0     3506 2023-04-16 19:11:58.199194 mine-3.1/mine/tests/test_manager.py
--rw-r--r--   0        0        0     1489 2023-04-16 19:11:58.199324 mine-3.1/mine/tests/test_models_application.py
--rw-r--r--   0        0        0     4244 2023-07-15 03:33:38.370107 mine-3.1/mine/tests/test_models_computer.py
--rw-r--r--   0        0        0      316 2023-04-16 19:11:58.199968 mine-3.1/mine/tests/test_models_config.py
--rw-r--r--   0        0        0      682 2023-04-16 19:11:58.200223 mine-3.1/mine/tests/test_models_data.py
--rw-r--r--   0        0        0     4961 2023-04-16 19:11:58.200402 mine-3.1/mine/tests/test_models_status.py
--rw-r--r--   0        0        0     1750 2023-04-16 19:11:58.200536 mine-3.1/mine/tests/test_models_timestamp.py
--rw-r--r--   0        0        0     3211 2023-04-16 19:21:47.166045 mine-3.1/mine/tests/test_services.py
--rw-r--r--   0        0        0     2286 2023-07-15 03:33:38.371043 mine-3.1/pyproject.toml
--rw-r--r--   0        0        0     4364 1970-01-01 00:00:00.000000 mine-3.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2019-05-21 02:49:19.000000 mine-3.1.1/LICENSE.md
+-rw-r--r--   0        0        0     2840 2023-04-16 19:11:58.196023 mine-3.1.1/README.md
+-rw-r--r--   0        0        0      340 2023-04-16 19:25:03.010573 mine-3.1.1/mine/__init__.py
+-rw-r--r--   0        0        0     6624 2023-04-16 19:11:58.197283 mine-3.1.1/mine/cli.py
+-rw-r--r--   0        0        0     2865 2023-04-16 19:11:58.197615 mine-3.1.1/mine/common.py
+-rw-r--r--   0        0        0     6669 2023-04-16 19:18:48.322162 mine-3.1.1/mine/manager.py
+-rw-r--r--   0        0        0      232 2019-05-21 02:49:19.000000 mine-3.1.1/mine/models/__init__.py
+-rw-r--r--   0        0        0      424 2021-06-02 19:31:21.821486 mine-3.1.1/mine/models/_bases.py
+-rw-r--r--   0        0        0     1803 2019-05-21 02:49:19.000000 mine-3.1.1/mine/models/application.py
+-rw-r--r--   0        0        0     4801 2023-07-15 20:16:13.642291 mine-3.1.1/mine/models/computer.py
+-rw-r--r--   0        0        0      501 2019-05-21 02:49:19.000000 mine-3.1.1/mine/models/config.py
+-rw-r--r--   0        0        0     5145 2020-05-16 16:13:05.000000 mine-3.1.1/mine/models/data.py
+-rw-r--r--   0        0        0     6544 2022-09-08 17:31:06.428139 mine-3.1.1/mine/models/status.py
+-rw-r--r--   0        0        0     1052 2019-05-21 02:49:19.000000 mine-3.1.1/mine/models/timestamp.py
+-rwxr-xr-x   0        0        0     2667 2023-04-16 19:11:58.198225 mine-3.1.1/mine/services.py
+-rw-r--r--   0        0        0      573 2023-04-16 19:13:26.811463 mine-3.1.1/mine/settings.py
+-rw-r--r--   0        0        0       34 2016-09-23 05:48:42.000000 mine-3.1.1/mine/tests/__init__.py
+-rw-r--r--   0        0        0     1038 2023-04-16 19:11:58.198685 mine-3.1.1/mine/tests/conftest.py
+-rw-r--r--   0        0        0        9 2016-09-23 02:41:14.000000 mine-3.1.1/mine/tests/files/.gitignore
+-rw-r--r--   0        0        0      513 2016-09-23 02:41:14.000000 mine-3.1.1/mine/tests/files/mine-in.yml
+-rw-r--r--   0        0        0      587 2016-09-23 02:41:14.000000 mine-3.1.1/mine/tests/files/mine-out.yml
+-rw-r--r--   0        0        0     3996 2023-04-16 19:11:58.199066 mine-3.1.1/mine/tests/test_cli.py
+-rw-r--r--   0        0        0     3506 2023-04-16 19:11:58.199194 mine-3.1.1/mine/tests/test_manager.py
+-rw-r--r--   0        0        0     1489 2023-04-16 19:11:58.199324 mine-3.1.1/mine/tests/test_models_application.py
+-rw-r--r--   0        0        0     4244 2023-07-15 19:53:23.376622 mine-3.1.1/mine/tests/test_models_computer.py
+-rw-r--r--   0        0        0      316 2023-04-16 19:11:58.199968 mine-3.1.1/mine/tests/test_models_config.py
+-rw-r--r--   0        0        0      682 2023-04-16 19:11:58.200223 mine-3.1.1/mine/tests/test_models_data.py
+-rw-r--r--   0        0        0     4961 2023-04-16 19:11:58.200402 mine-3.1.1/mine/tests/test_models_status.py
+-rw-r--r--   0        0        0     1750 2023-04-16 19:11:58.200536 mine-3.1.1/mine/tests/test_models_timestamp.py
+-rw-r--r--   0        0        0     3211 2023-04-16 19:21:47.166045 mine-3.1.1/mine/tests/test_services.py
+-rw-r--r--   0        0        0     2294 2023-07-15 20:13:11.614336 mine-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4366 1970-01-01 00:00:00.000000 mine-3.1.1/PKG-INFO
```

### Comparing `mine-3.1/LICENSE.md` & `mine-3.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mine-3.1/README.md` & `mine-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/cli.py` & `mine-3.1.1/mine/cli.py`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/common.py` & `mine-3.1.1/mine/common.py`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/manager.py` & `mine-3.1.1/mine/manager.py`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/models/application.py` & `mine-3.1.1/mine/models/application.py`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/models/computer.py` & `mine-3.1.1/mine/models/computer.py`

 * *Files 9% similar despite different names*

```diff
@@ -99,31 +99,39 @@
         if matches:
             return min(matches, key=lambda computer: len(computer.name))
         return None
 
     def get_current(self):
         """Get the current computer's information."""
         this = Computer(None)
+        log.debug(f"Matching: {this.hostname=} {this.address=} {this.serial=}")
 
         # Search for a matching hostname
         for other in self:
             if this.hostname == other.hostname:
+                log.debug(f"Matched via hostname: {other}")
                 other.address = this.address
+                if this.serial:
+                    other.serial = this.serial
                 return other
 
         # Else, search for a matching serial
         for other in self:
             if this.serial and this.serial == other.serial:
+                log.debug(f"Matched via serial: {other}")
                 other.hostname = this.hostname
                 return other
 
         # Else, search for a matching address
         for other in self:
             if this.address == other.address:
+                log.debug(f"Matched via address: {other}")
                 other.hostname = this.hostname
+                if this.serial:
+                    other.serial = this.serial
                 return other
 
         # Else, this is a new computer
         this.name = self.generate_name(this)
         assert this.name != "localhost"
         log.debug("New computer: %s", this)
         self.append(this)
```

### Comparing `mine-3.1/mine/models/data.py` & `mine-3.1.1/mine/models/data.py`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/models/status.py` & `mine-3.1.1/mine/models/status.py`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/models/timestamp.py` & `mine-3.1.1/mine/models/timestamp.py`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/services.py` & `mine-3.1.1/mine/services.py`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/settings.py` & `mine-3.1.1/mine/settings.py`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/tests/conftest.py` & `mine-3.1.1/mine/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/tests/files/mine-in.yml` & `mine-3.1.1/mine/tests/files/mine-in.yml`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/tests/files/mine-out.yml` & `mine-3.1.1/mine/tests/files/mine-out.yml`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/tests/test_cli.py` & `mine-3.1.1/mine/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/tests/test_manager.py` & `mine-3.1.1/mine/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/tests/test_models_application.py` & `mine-3.1.1/mine/tests/test_models_application.py`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/tests/test_models_computer.py` & `mine-3.1.1/mine/tests/test_models_computer.py`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/tests/test_models_data.py` & `mine-3.1.1/mine/tests/test_models_data.py`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/tests/test_models_status.py` & `mine-3.1.1/mine/tests/test_models_status.py`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/tests/test_models_timestamp.py` & `mine-3.1.1/mine/tests/test_models_timestamp.py`

 * *Files identical despite different names*

### Comparing `mine-3.1/mine/tests/test_services.py` & `mine-3.1.1/mine/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `mine-3.1/pyproject.toml` & `mine-3.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "mine"
-version = "3.1"
+version = "3.1.1"
 description = "Share application state across computers using Dropbox."
 
 license = "MIT"
 
 authors = ["Jace Browning <jacebrowning@gmail.com>"]
 
 readme = "README.md"
@@ -35,15 +35,15 @@
 ]
 
 [tool.poetry.dependencies]
 
 python = "^3.8"
 
 YORM = "^1.6"
-psutil = "^4.4"
+psutil = ">=4.4,<6.0"
 crayons = "~0.1"
 minilog = "^2.1"
 universal-startfile = "^0.2"
 
 [tool.poetry.dev-dependencies]
 
 # Formatters
```

### Comparing `mine-3.1/PKG-INFO` & `mine-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mine
-Version: 3.1
+Version: 3.1.1
 Summary: Share application state across computers using Dropbox.
 Home-page: https://pypi.org/project/mine
 License: MIT
 Author: Jace Browning
 Author-email: jacebrowning@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -26,15 +26,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Utilities
 Requires-Dist: YORM (>=1.6,<2.0)
 Requires-Dist: crayons (>=0.1,<0.2)
 Requires-Dist: minilog (>=2.1,<3.0)
-Requires-Dist: psutil (>=4.4,<5.0)
+Requires-Dist: psutil (>=4.4,<6.0)
 Requires-Dist: universal-startfile (>=0.2,<0.3)
 Project-URL: Documentation, https://mine.readthedocs.io
 Project-URL: Repository, https://github.com/jacebrowning/mine
 Description-Content-Type: text/markdown
 
 # Overview
```

