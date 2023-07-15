# Comparing `tmp/zenbitlib-0.0.2.tar.gz` & `tmp/zenbitlib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenbitlib-0.0.2.tar", last modified: Sat Jul 15 05:45:39 2023, max compression
+gzip compressed data, was "zenbitlib-0.0.3.tar", last modified: Sat Jul 15 05:55:49 2023, max compression
```

## Comparing `zenbitlib-0.0.2.tar` & `zenbitlib-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 05:45:39.409625 zenbitlib-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-07-15 04:13:46.000000 zenbitlib-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      586 2023-07-15 05:45:39.409625 zenbitlib-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       73 2023-07-15 05:22:08.000000 zenbitlib-0.0.2/README.md
--rw-rw-rw-   0        0        0      591 2023-07-15 05:45:27.000000 zenbitlib-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-15 05:45:39.409625 zenbitlib-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-15 05:45:39.389420 zenbitlib-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-15 05:45:39.396421 zenbitlib-0.0.2/src/zenbitlib/
--rw-rw-rw-   0        0        0        0 2023-07-15 04:08:39.000000 zenbitlib-0.0.2/src/zenbitlib/__init__.py
--rw-rw-rw-   0        0        0      155 2023-07-15 02:26:38.000000 zenbitlib-0.0.2/src/zenbitlib/zenproject.py
--rw-rw-rw-   0        0        0     1733 2023-07-15 05:41:06.000000 zenbitlib-0.0.2/src/zenbitlib/zenutils.py
-drwxrwxrwx   0        0        0        0 2023-07-15 05:45:39.407624 zenbitlib-0.0.2/src/zenbitlib.egg-info/
--rw-rw-rw-   0        0        0      586 2023-07-15 05:45:39.000000 zenbitlib-0.0.2/src/zenbitlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-07-15 05:45:39.000000 zenbitlib-0.0.2/src/zenbitlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 05:45:39.000000 zenbitlib-0.0.2/src/zenbitlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-15 05:45:39.000000 zenbitlib-0.0.2/src/zenbitlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 05:55:49.625589 zenbitlib-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-07-15 04:13:46.000000 zenbitlib-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      586 2023-07-15 05:55:49.625589 zenbitlib-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2023-07-15 05:22:08.000000 zenbitlib-0.0.3/README.md
+-rw-rw-rw-   0        0        0      591 2023-07-15 05:55:19.000000 zenbitlib-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-15 05:55:49.625589 zenbitlib-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-15 05:55:49.607781 zenbitlib-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-15 05:55:49.613833 zenbitlib-0.0.3/src/zenbitlib/
+-rw-rw-rw-   0        0        0        0 2023-07-15 04:08:39.000000 zenbitlib-0.0.3/src/zenbitlib/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-07-15 05:52:23.000000 zenbitlib-0.0.3/src/zenbitlib/zenproject.py
+-rw-rw-rw-   0        0        0     1981 2023-07-15 05:55:14.000000 zenbitlib-0.0.3/src/zenbitlib/zenutils.py
+drwxrwxrwx   0        0        0        0 2023-07-15 05:55:49.624577 zenbitlib-0.0.3/src/zenbitlib.egg-info/
+-rw-rw-rw-   0        0        0      586 2023-07-15 05:55:49.000000 zenbitlib-0.0.3/src/zenbitlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-07-15 05:55:49.000000 zenbitlib-0.0.3/src/zenbitlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 05:55:49.000000 zenbitlib-0.0.3/src/zenbitlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-15 05:55:49.000000 zenbitlib-0.0.3/src/zenbitlib.egg-info/top_level.txt
```

### Comparing `zenbitlib-0.0.2/LICENSE` & `zenbitlib-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zenbitlib-0.0.2/PKG-INFO` & `zenbitlib-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenbitlib
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for quick qml learning
 Author-email: zenzenwang <zenwang@outlook.com>
 Project-URL: Homepage, https://github.com/zenzen891/zenlib/
 Project-URL: Bug Tracker, https://github.com/zenzen891/zenlib/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `zenbitlib-0.0.2/pyproject.toml` & `zenbitlib-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zenbitlib"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="zenzenwang", email="zenwang@outlook.com" },
 ]
 description = "A package for quick qml learning"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `zenbitlib-0.0.2/src/zenbitlib/zenutils.py` & `zenbitlib-0.0.3/src/zenbitlib/zenutils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 from zenbitlib.zenproject import *
 
+import datetime
+import random
+import inspect
+import os
+import torch
+import numpy as np
+
 class info(zenproject):
     def __init__(self, project_name) -> None:
         super().__init__()
         # Project name
         self.proj_name = project_name
         # Time record
         self.nowTime = self.nowtime()
@@ -17,16 +24,16 @@
     def nowtime(self):
         nowTime = datetime.datetime.now().strftime('%Y-%m-%d-%H-%M-%S')
         return nowTime
     
     # find current file address for main script 
     '''NOT This lib's address!!'''
     def workingpath(self):
-        working_path = os.path.abspath(os.path.dirname(os.path.dirname(__file__)))
-        # working_path = os.path.dirname(__file__)
+        # working_path = os.path.abspath(os.path.dirname(os.path.dirname(__file__)))
+        working_path = os.path.dirname(os.path.abspath(inspect.getmodule(inspect.currentframe().f_back).__file__))
         return working_path
     
     # check project's direction. Create the direction if not existed.
     def check_proj_path(self):
         folder_path = self.workingpath()+ '/results/' + self.proj_name + '/'
         mod_path = self.workingpath()+ '/results/' + self.proj_name + '/mod/'
         os.makedirs(folder_path, exist_ok=True)
@@ -36,8 +43,12 @@
         torch.manual_seed(SEED)
         np.random.seed(SEED)
         random.seed(SEED)
         np.random.seed(SEED)
         torch.manual_seed(SEED)
         torch.cuda.manual_seed_all(SEED)
         torch.backends.cudnn.deterministic = True
-        torch.backends.cudnn.benchmark = False
+        torch.backends.cudnn.benchmark = False
+
+if __name__ == "__main__":
+    info_ = info("test")
+    print(info_.working_path)
```

### Comparing `zenbitlib-0.0.2/src/zenbitlib.egg-info/PKG-INFO` & `zenbitlib-0.0.3/src/zenbitlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zenbitlib
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package for quick qml learning
 Author-email: zenzenwang <zenwang@outlook.com>
 Project-URL: Homepage, https://github.com/zenzen891/zenlib/
 Project-URL: Bug Tracker, https://github.com/zenzen891/zenlib/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

