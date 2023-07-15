# Comparing `tmp/flux-burst-0.0.13.tar.gz` & `tmp/flux-burst-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-burst-0.0.13.tar", last modified: Sun Jul  9 17:00:05 2023, max compression
+gzip compressed data, was "flux-burst-0.0.14.tar", last modified: Sat Jul 15 03:30:48 2023, max compression
```

## Comparing `flux-burst-0.0.13.tar` & `flux-burst-0.0.14.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-09 17:00:05.259153 flux-burst-0.0.13/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-06-23 19:26:31.000000 flux-burst-0.0.13/COPYRIGHT
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-06-23 19:26:31.000000 flux-burst-0.0.13/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      313 2023-06-23 19:45:55.000000 flux-burst-0.0.13/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-06-23 19:26:31.000000 flux-burst-0.0.13/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4718 2023-07-09 17:00:05.259153 flux-burst-0.0.13/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3880 2023-07-03 07:21:31.000000 flux-burst-0.0.13/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-09 17:00:05.259153 flux-burst-0.0.13/flux_burst.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4718 2023-07-09 17:00:04.000000 flux-burst-0.0.13/flux_burst.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      744 2023-07-09 17:00:05.000000 flux-burst-0.0.13/flux_burst.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-09 17:00:04.000000 flux-burst-0.0.13/flux_burst.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       53 2023-07-09 17:00:04.000000 flux-burst-0.0.13/flux_burst.egg-info/entry_points.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 03:17:14.000000 flux-burst-0.0.13/flux_burst.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      177 2023-07-09 17:00:04.000000 flux-burst-0.0.13/flux_burst.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       10 2023-07-09 17:00:04.000000 flux-burst-0.0.13/flux_burst.egg-info/top_level.txt
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-09 17:00:05.259153 flux-burst-0.0.13/fluxburst/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       62 2023-06-23 19:45:55.000000 flux-burst-0.0.13/fluxburst/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8590 2023-07-04 01:36:48.000000 flux-burst-0.0.13/fluxburst/client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      746 2023-07-01 06:52:00.000000 flux-burst-0.0.13/fluxburst/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7538 2023-07-09 17:00:01.000000 flux-burst-0.0.13/fluxburst/handles.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-09 17:00:05.259153 flux-burst-0.0.13/fluxburst/kubernetes/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      209 2023-07-01 06:52:00.000000 flux-burst-0.0.13/fluxburst/kubernetes/README.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2023-07-01 06:52:00.000000 flux-burst-0.0.13/fluxburst/kubernetes/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5200 2023-07-04 01:36:48.000000 flux-burst-0.0.13/fluxburst/kubernetes/cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8953 2023-07-09 17:00:01.000000 flux-burst-0.0.13/fluxburst/kubernetes/plugins.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6127 2023-06-23 19:43:36.000000 flux-burst-0.0.13/fluxburst/logger.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2831 2023-07-04 00:51:56.000000 flux-burst-0.0.13/fluxburst/plugins.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      365 2023-07-09 16:49:50.000000 flux-burst-0.0.13/fluxburst/selectors.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      444 2023-06-24 04:45:23.000000 flux-burst-0.0.13/fluxburst/sorting.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-09 17:00:05.259153 flux-burst-0.0.13/fluxburst/utils/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      540 2023-06-23 19:26:33.000000 flux-burst-0.0.13/fluxburst/utils/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6250 2023-07-04 01:36:48.000000 flux-burst-0.0.13/fluxburst/utils/fileio.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1692 2023-06-23 19:41:30.000000 flux-burst-0.0.13/fluxburst/utils/misc.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3188 2023-06-23 19:45:55.000000 flux-burst-0.0.13/fluxburst/utils/terminal.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1263 2023-07-09 17:00:01.000000 flux-burst-0.0.13/fluxburst/version.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-06-23 19:26:31.000000 flux-burst-0.0.13/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      210 2023-07-09 17:00:05.259153 flux-burst-0.0.13/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3578 2023-07-01 06:52:00.000000 flux-burst-0.0.13/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-15 03:30:48.804137 flux-burst-0.0.14/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-06-23 19:26:31.000000 flux-burst-0.0.14/COPYRIGHT
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-06-23 19:26:31.000000 flux-burst-0.0.14/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      313 2023-06-23 19:45:55.000000 flux-burst-0.0.14/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-06-23 19:26:31.000000 flux-burst-0.0.14/NOTICE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4718 2023-07-15 03:30:48.804137 flux-burst-0.0.14/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3880 2023-07-03 07:21:31.000000 flux-burst-0.0.14/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-15 03:30:48.800137 flux-burst-0.0.14/flux_burst.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4718 2023-07-15 03:30:48.000000 flux-burst-0.0.14/flux_burst.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      744 2023-07-15 03:30:48.000000 flux-burst-0.0.14/flux_burst.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-15 03:30:48.000000 flux-burst-0.0.14/flux_burst.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       53 2023-07-15 03:30:48.000000 flux-burst-0.0.14/flux_burst.egg-info/entry_points.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 03:17:14.000000 flux-burst-0.0.14/flux_burst.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      167 2023-07-15 03:30:48.000000 flux-burst-0.0.14/flux_burst.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       10 2023-07-15 03:30:48.000000 flux-burst-0.0.14/flux_burst.egg-info/top_level.txt
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-15 03:30:48.804137 flux-burst-0.0.14/fluxburst/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       62 2023-06-23 19:45:55.000000 flux-burst-0.0.14/fluxburst/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8590 2023-07-04 01:36:48.000000 flux-burst-0.0.14/fluxburst/client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      746 2023-07-01 06:52:00.000000 flux-burst-0.0.14/fluxburst/defaults.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7850 2023-07-15 03:29:48.000000 flux-burst-0.0.14/fluxburst/handles.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-15 03:30:48.804137 flux-burst-0.0.14/fluxburst/kubernetes/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      209 2023-07-01 06:52:00.000000 flux-burst-0.0.14/fluxburst/kubernetes/README.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2023-07-01 06:52:00.000000 flux-burst-0.0.14/fluxburst/kubernetes/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5200 2023-07-04 01:36:48.000000 flux-burst-0.0.14/fluxburst/kubernetes/cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8953 2023-07-09 17:00:01.000000 flux-burst-0.0.14/fluxburst/kubernetes/plugins.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6127 2023-06-23 19:43:36.000000 flux-burst-0.0.14/fluxburst/logger.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2831 2023-07-04 00:51:56.000000 flux-burst-0.0.14/fluxburst/plugins.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      365 2023-07-09 16:49:50.000000 flux-burst-0.0.14/fluxburst/selectors.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      444 2023-06-24 04:45:23.000000 flux-burst-0.0.14/fluxburst/sorting.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-15 03:30:48.804137 flux-burst-0.0.14/fluxburst/utils/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      532 2023-07-15 03:29:48.000000 flux-burst-0.0.14/fluxburst/utils/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6250 2023-07-04 01:36:48.000000 flux-burst-0.0.14/fluxburst/utils/fileio.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1456 2023-07-15 03:29:48.000000 flux-burst-0.0.14/fluxburst/utils/misc.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3188 2023-06-23 19:45:55.000000 flux-burst-0.0.14/fluxburst/utils/terminal.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-07-15 03:30:11.000000 flux-burst-0.0.14/fluxburst/version.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-06-23 19:26:31.000000 flux-burst-0.0.14/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      210 2023-07-15 03:30:48.804137 flux-burst-0.0.14/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3578 2023-07-01 06:52:00.000000 flux-burst-0.0.14/setup.py
```

### Comparing `flux-burst-0.0.13/LICENSE` & `flux-burst-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.13/NOTICE` & `flux-burst-0.0.14/NOTICE`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.13/PKG-INFO` & `flux-burst-0.0.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst
-Version: 0.0.13
+Version: 0.0.14
 Summary: Flux module that enables burstable plugins.
 Home-page: https://github.com/converged-computing/flux-burst
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: cloud,flux-framework,flux,bursting
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flux-burst Version: 0.0.13 Summary: Flux module
+Metadata-Version: 2.1 Name: flux-burst Version: 0.0.14 Summary: Flux module
 that enables burstable plugins. Home-page: https://github.com/converged-
 computing/flux-burst Author: Vanessa Sochat Author-email:
 vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
 Keywords: cloud,flux-framework,flux,bursting Platform: UNKNOWN Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
```

### Comparing `flux-burst-0.0.13/README.md` & `flux-burst-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.13/flux_burst.egg-info/PKG-INFO` & `flux-burst-0.0.14/flux_burst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst
-Version: 0.0.13
+Version: 0.0.14
 Summary: Flux module that enables burstable plugins.
 Home-page: https://github.com/converged-computing/flux-burst
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: cloud,flux-framework,flux,bursting
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flux-burst Version: 0.0.13 Summary: Flux module
+Metadata-Version: 2.1 Name: flux-burst Version: 0.0.14 Summary: Flux module
 that enables burstable plugins. Home-page: https://github.com/converged-
 computing/flux-burst Author: Vanessa Sochat Author-email:
 vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
 Keywords: cloud,flux-framework,flux,bursting Platform: UNKNOWN Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
```

### Comparing `flux-burst-0.0.13/flux_burst.egg-info/SOURCES.txt` & `flux-burst-0.0.14/flux_burst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.13/fluxburst/client.py` & `flux-burst-0.0.14/fluxburst/client.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.13/fluxburst/defaults.py` & `flux-burst-0.0.14/fluxburst/defaults.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.13/fluxburst/handles.py` & `flux-burst-0.0.14/fluxburst/handles.py`

 * *Files 12% similar despite different names*

```diff
@@ -173,17 +173,29 @@
                 "version": 1,
             },
         }
 
 
 class FluxHandle:
     def __init__(self, handle=None):
+        self._handle = handle
+
+    @property
+    def handle(self):
+        """
+        A handle propery to "handle" connection! har har.
+
+        We import Flux here to allow instantiating the client possibly
+        after the instance is created.
+        """
         import flux
 
-        self.handle = handle or flux.Flux()
+        if not self._handle:
+            self._handle = flux.Flux()
+        return self._handle
 
     def update_jobspec(self, job):
         """
         Update a jobspec via the kvs
         """
         import flux.job
```

### Comparing `flux-burst-0.0.13/fluxburst/kubernetes/cluster.py` & `flux-burst-0.0.14/fluxburst/kubernetes/cluster.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.13/fluxburst/kubernetes/plugins.py` & `flux-burst-0.0.14/fluxburst/kubernetes/plugins.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.13/fluxburst/logger.py` & `flux-burst-0.0.14/fluxburst/logger.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.13/fluxburst/plugins.py` & `flux-burst-0.0.14/fluxburst/plugins.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.13/fluxburst/utils/__init__.py` & `flux-burst-0.0.14/fluxburst/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     recursive_find,
     remove_to_base,
     workdir,
     write_file,
     write_json,
     write_yaml,
 )
-from .misc import choose, chunks, get_hash, mb_to_bytes, print_bytes, slugify
+from .misc import chunks, get_hash, mb_to_bytes, print_bytes, slugify
 from .terminal import (
     check_install,
     confirm_action,
     confirm_uninstall,
     ensure_no_extra,
     get_installdir,
     run_command,
```

### Comparing `flux-burst-0.0.13/fluxburst/utils/fileio.py` & `flux-burst-0.0.14/fluxburst/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.13/fluxburst/utils/misc.py` & `flux-burst-0.0.14/fluxburst/utils/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
 import copy
 
-from pick import pick
-
 
 def chunks(listing, chunk_size):
     """
     Yield successive chunks from listing. Chunkify!
     """
     for i in range(0, len(listing), chunk_size):
         yield listing[i : i + chunk_size]
@@ -39,21 +37,14 @@
 def mb_to_bytes(mb):
     """
     Convert mb to bytes, usually so we can derive a better format.
     """
     return mb * (1048576)
 
 
-def choose(options, prompt, default_index=0):
-    """
-    Use pick to choose one of a few options, return the chosen option.
-    """
-    return pick(options, prompt, indicator="=>", default_index=default_index)
-
-
 def get_hash(obj):
     """
     Get a hash for a random object (set, tuple, list, dict)
 
     All nested attributes must at least be hashable!
     """
     if isinstance(obj, (set, tuple, list)):
```

### Comparing `flux-burst-0.0.13/fluxburst/utils/terminal.py` & `flux-burst-0.0.14/fluxburst/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.13/fluxburst/version.py` & `flux-burst-0.0.14/fluxburst/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
-__version__ = "0.0.13"
+__version__ = "0.0.14"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "flux-burst"
 PACKAGE_URL = "https://github.com/converged-computing/flux-burst"
 KEYWORDS = "cloud, flux-framework, flux, bursting"
 DESCRIPTION = "Flux module that enables burstable plugins."
 LICENSE = "LICENSE"
@@ -17,15 +17,14 @@
 
 INSTALL_REQUIRES = (
     ("ruamel.yaml", {"min_version": None}),
     ("jsonschema", {"min_version": None}),
     ("rich", {"min_version": None}),
     ("oras", {"min_version": None}),
     ("requests", {"min_version": None}),
-    ("pick", {"min_version": None}),
 )
 
 INSTALL_REQUIRES_KUBERNETES = (
     ("kubernetes", {"min_version": None}),
     ("fluxoperator", {"min_version": None}),
 )
```

### Comparing `flux-burst-0.0.13/setup.py` & `flux-burst-0.0.14/setup.py`

 * *Files identical despite different names*

