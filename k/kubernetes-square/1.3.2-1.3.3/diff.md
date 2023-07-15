# Comparing `tmp/kubernetes-square-1.3.2.tar.gz` & `tmp/kubernetes_square-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubernetes-square-1.3.2.tar", max compression
+gzip compressed data, was "kubernetes_square-1.3.3.tar", max compression
```

## Comparing `kubernetes-square-1.3.2.tar` & `kubernetes_square-1.3.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    11357 2019-10-19 08:56:49.000000 kubernetes-square-1.3.2/LICENSE
--rw-r--r--   0        0        0      757 2023-05-06 09:05:28.381602 kubernetes-square-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     3531 2021-09-06 17:16:58.000000 kubernetes-square-1.3.2/resources/defaultconfig.yaml
--rw-r--r--   0        0        0     1382 2023-05-06 09:05:28.381602 kubernetes-square-1.3.2/square/__init__.py
--rw-r--r--   0        0        0      203 2023-05-06 04:43:58.328074 kubernetes-square-1.3.2/square/__main__.py
--rw-r--r--   0        0        0     5095 2023-03-16 06:14:23.918379 kubernetes-square-1.3.2/square/cfgfile.py
--rw-r--r--   0        0        0     1851 2021-09-06 17:16:58.000000 kubernetes-square-1.3.2/square/dotdict.py
--rw-r--r--   0        0        0     6867 2023-03-22 01:24:34.210365 kubernetes-square-1.3.2/square/dtypes.py
--rw-r--r--   0        0        0    33744 2023-03-22 01:24:34.210365 kubernetes-square-1.3.2/square/k8s.py
--rw-r--r--   0        0        0    14924 2023-03-16 06:14:23.918379 kubernetes-square-1.3.2/square/main.py
--rw-r--r--   0        0        0    39403 2023-03-16 06:14:23.918379 kubernetes-square-1.3.2/square/manio.py
--rw-r--r--   0        0        0    29840 2023-03-16 06:14:23.918379 kubernetes-square-1.3.2/square/square.py
--rw-r--r--   0        0        0      800 2023-05-06 09:08:47.845837 kubernetes-square-1.3.2/setup.py
--rw-r--r--   0        0        0      485 2023-05-06 09:08:47.846128 kubernetes-square-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2019-10-19 08:56:49.000000 kubernetes_square-1.3.3/LICENSE
+-rw-r--r--   0        0        0      756 2023-07-15 03:25:26.962133 kubernetes_square-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3531 2021-09-06 17:16:58.000000 kubernetes_square-1.3.3/resources/defaultconfig.yaml
+-rw-r--r--   0        0        0     1382 2023-07-15 03:25:26.962133 kubernetes_square-1.3.3/square/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-06 04:43:58.328074 kubernetes_square-1.3.3/square/__main__.py
+-rw-r--r--   0        0        0     5095 2023-03-16 06:14:23.918379 kubernetes_square-1.3.3/square/cfgfile.py
+-rw-r--r--   0        0        0     1851 2021-09-06 17:16:58.000000 kubernetes_square-1.3.3/square/dotdict.py
+-rw-r--r--   0        0        0     6887 2023-07-15 02:12:53.911779 kubernetes_square-1.3.3/square/dtypes.py
+-rw-r--r--   0        0        0    33744 2023-07-15 03:28:13.512977 kubernetes_square-1.3.3/square/k8s.py
+-rw-r--r--   0        0        0    14924 2023-03-16 06:14:23.918379 kubernetes_square-1.3.3/square/main.py
+-rw-r--r--   0        0        0    39403 2023-03-16 06:14:23.918379 kubernetes_square-1.3.3/square/manio.py
+-rw-r--r--   0        0        0    29840 2023-03-16 06:14:23.918379 kubernetes_square-1.3.3/square/square.py
+-rw-r--r--   0        0        0      536 1970-01-01 00:00:00.000000 kubernetes_square-1.3.3/PKG-INFO
```

### Comparing `kubernetes-square-1.3.2/LICENSE` & `kubernetes_square-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kubernetes-square-1.3.2/pyproject.toml` & `kubernetes_square-1.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kubernetes-square"
-version = "1.3.2"
+version = "1.3.3"
 description = ""
 authors = ["Oliver Nagy <olitheolix@gmail.com>"]
 packages = [
     { include = "square" },
 ]
 include = ["resources/defaultconfig.yaml"]
 
@@ -34,9 +34,9 @@
 requests-mock = "*"
 sh = "*"
 
 [tool.poetry.scripts]
 square = 'square.main:main'
 
 [build-system]
-requires = ["poetry>=0.12"]
+requires = ["poetry>=1.2"]
 build-backend = "poetry.masonry.api"
```

### Comparing `kubernetes-square-1.3.2/resources/defaultconfig.yaml` & `kubernetes_square-1.3.3/resources/defaultconfig.yaml`

 * *Files identical despite different names*

### Comparing `kubernetes-square-1.3.2/square/__init__.py` & `kubernetes_square-1.3.3/square/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 import sys
 
 from . import square
 from .cfgfile import load
 
-__version__ = '1.3.2'
+__version__ = '1.3.3'
 
 
 # ---------------------------------------------------------------------------
 # Global Runtime Constants
 # ---------------------------------------------------------------------------
 # Determine the base folder. This is usually the folder of this very file, but
 # will be different if we run inside a bundle produced by PyInstaller.
```

### Comparing `kubernetes-square-1.3.2/square/cfgfile.py` & `kubernetes_square-1.3.3/square/cfgfile.py`

 * *Files identical despite different names*

### Comparing `kubernetes-square-1.3.2/square/dotdict.py` & `kubernetes_square-1.3.3/square/dotdict.py`

 * *Files identical despite different names*

### Comparing `kubernetes-square-1.3.2/square/dtypes.py` & `kubernetes_square-1.3.3/square/dtypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,21 +185,21 @@
     # Path to Kubernetes credentials.
     kubeconfig: Filepath
 
     # Kubernetes context (use `None` to use the default).
     kubecontext: Optional[str]
 
     # Only operate on resources that match the selectors.
-    selectors: Selectors = Selectors()
+    selectors: Selectors = _factory(Selectors())
 
     # Sort the manifest in this order, or alphabetically at the end if not in the list.
     priorities: List[str] = _factory(list(DEFAULT_PRIORITIES))
 
     # How to structure the folder directory when syncing manifests.
-    groupby: GroupBy = GroupBy()
+    groupby: GroupBy = _factory(GroupBy())
 
     # Define which fields to skip for which resource.
     filters: Dict[str, List[str | dict]] = _factory({})
 
     # Callable: will be invoked for every local/server manifest that requires
     # patching before the actual patch will be computed.
     patch_callback: Optional[Callable] = None
```

### Comparing `kubernetes-square-1.3.2/square/k8s.py` & `kubernetes_square-1.3.3/square/k8s.py`

 * *Files identical despite different names*

### Comparing `kubernetes-square-1.3.2/square/main.py` & `kubernetes_square-1.3.3/square/main.py`

 * *Files identical despite different names*

### Comparing `kubernetes-square-1.3.2/square/manio.py` & `kubernetes_square-1.3.3/square/manio.py`

 * *Files identical despite different names*

### Comparing `kubernetes-square-1.3.2/square/square.py` & `kubernetes_square-1.3.3/square/square.py`

 * *Files identical despite different names*

