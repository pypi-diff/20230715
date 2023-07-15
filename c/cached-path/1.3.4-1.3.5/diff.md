# Comparing `tmp/cached_path-1.3.4.tar.gz` & `tmp/cached_path-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cached_path-1.3.4.tar", last modified: Thu Apr  6 21:14:01 2023, max compression
+gzip compressed data, was "cached_path-1.3.5.tar", last modified: Sat Jul 15 16:22:22 2023, max compression
```

## Comparing `cached_path-1.3.4.tar` & `cached_path-1.3.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:14:01.244251 cached_path-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-06 21:13:47.000000 cached_path-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-04-06 21:14:01.244251 cached_path-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-04-06 21:13:47.000000 cached_path-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:14:01.240251 cached_path-1.3.4/cached_path/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-06 21:13:47.000000 cached_path-1.3.4/cached_path/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-04-06 21:13:47.000000 cached_path-1.3.4/cached_path/_cached_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-06 21:13:47.000000 cached_path-1.3.4/cached_path/cache_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-06 21:13:47.000000 cached_path-1.3.4/cached_path/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-06 21:13:47.000000 cached_path-1.3.4/cached_path/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-06 21:13:47.000000 cached_path-1.3.4/cached_path/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-06 21:13:47.000000 cached_path-1.3.4/cached_path/progress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:14:01.244251 cached_path-1.3.4/cached_path/schemes/
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-04-06 21:13:47.000000 cached_path-1.3.4/cached_path/schemes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-06 21:13:47.000000 cached_path-1.3.4/cached_path/schemes/beaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-04-06 21:13:47.000000 cached_path-1.3.4/cached_path/schemes/gs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-06 21:13:47.000000 cached_path-1.3.4/cached_path/schemes/hf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-06 21:13:47.000000 cached_path-1.3.4/cached_path/schemes/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-06 21:13:47.000000 cached_path-1.3.4/cached_path/schemes/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-06 21:13:47.000000 cached_path-1.3.4/cached_path/schemes/scheme_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-06 21:13:47.000000 cached_path-1.3.4/cached_path/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-04-06 21:13:47.000000 cached_path-1.3.4/cached_path/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-06 21:13:47.000000 cached_path-1.3.4/cached_path/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:14:01.240251 cached_path-1.3.4/cached_path.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-04-06 21:14:01.000000 cached_path-1.3.4/cached_path.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-06 21:14:01.000000 cached_path-1.3.4/cached_path.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 21:14:01.000000 cached_path-1.3.4/cached_path.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-06 21:14:01.000000 cached_path-1.3.4/cached_path.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-06 21:14:01.000000 cached_path-1.3.4/cached_path.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-06 21:13:47.000000 cached_path-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 21:14:01.244251 cached_path-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-06 21:13:47.000000 cached_path-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:22:22.888085 cached_path-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-07-15 16:21:43.000000 cached_path-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-15 16:22:22.884085 cached_path-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-07-15 16:21:43.000000 cached_path-1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:22:22.884085 cached_path-1.3.5/cached_path/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14126 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/_cached_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/cache_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:22:22.884085 cached_path-1.3.5/cached_path/schemes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/schemes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/schemes/beaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/schemes/gs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/schemes/hf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/schemes/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/schemes/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/schemes/scheme_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-15 16:21:43.000000 cached_path-1.3.5/cached_path/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:22:22.884085 cached_path-1.3.5/cached_path.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-15 16:22:22.000000 cached_path-1.3.5/cached_path.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-15 16:22:22.000000 cached_path-1.3.5/cached_path.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 16:22:22.000000 cached_path-1.3.5/cached_path.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-15 16:22:22.000000 cached_path-1.3.5/cached_path.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 16:22:22.000000 cached_path-1.3.5/cached_path.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-15 16:21:43.000000 cached_path-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 16:22:22.888085 cached_path-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-15 16:21:43.000000 cached_path-1.3.5/setup.py
```

### Comparing `cached_path-1.3.4/LICENSE` & `cached_path-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.4/PKG-INFO` & `cached_path-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cached_path
-Version: 1.3.4
+Version: 1.3.5
 Home-page: https://github.com/allenai/cached_path
 Author: Allen Institute for Artificial Intelligence
 Author-email: contact@allenai.org
 License: Apache
 Keywords: allennlp cached_path file utils
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cached_path Version: 1.3.4 Home-page: https://
+Metadata-Version: 2.1 Name: cached_path Version: 1.3.5 Home-page: https://
 github.com/allenai/cached_path Author: Allen Institute for Artificial
 Intelligence Author-email: contact@allenai.org License: Apache Keywords:
 allennlp cached_path file utils Classifier: Intended Audience :: Science/
 Research Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.7 Description-Content-Type: text/
```

### Comparing `cached_path-1.3.4/README.md` & `cached_path-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.4/cached_path/__init__.py` & `cached_path-1.3.5/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.4/cached_path/_cached_path.py` & `cached_path-1.3.5/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.4/cached_path/cache_file.py` & `cached_path-1.3.5/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.4/cached_path/common.py` & `cached_path-1.3.5/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.4/cached_path/file_lock.py` & `cached_path-1.3.5/cached_path/file_lock.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import warnings
+from typing import Optional
 
 from filelock import AcquireReturnProxy
 from filelock import FileLock as _FileLock
 
 from .common import PathOrStr
 
 
@@ -18,27 +19,33 @@
     the lock already exists but the lock can't be acquired because write access is blocked.
     """
 
     def __init__(self, lock_file: PathOrStr, timeout=-1, read_only_ok: bool = False) -> None:
         super().__init__(str(lock_file), timeout=timeout)
         self._read_only_ok = read_only_ok
 
-    def acquire(self, timeout=None, poll_interval=0.05, **kwargs) -> AcquireReturnProxy:
+    def acquire(  # type: ignore[override]
+        self,
+        timeout=None,
+        poll_interval=0.05,
+        **kwargs,
+    ) -> Optional[AcquireReturnProxy]:
         try:
             return super().acquire(timeout=timeout, poll_interval=poll_interval, **kwargs)
         except OSError as err:
             # OSError could be a lot of different things, but what we're looking
             # for in particular are permission errors, such as:
             #  - errno 1  - EPERM  - "Operation not permitted"
             #  - errno 13 - EACCES - "Permission denied"
             #  - errno 30 - EROFS  - "Read-only file system"
             if err.errno not in (1, 13, 30):
                 raise
 
-            if os.path.isfile(self._lock_file) and self._read_only_ok:
+            if os.path.isfile(self.lock_file) and self._read_only_ok:
                 warnings.warn(
-                    f"Lacking permissions required to obtain lock '{self._lock_file}'. "
+                    f"Lacking permissions required to obtain lock '{self.lock_file}'. "
                     "Race conditions are possible if other processes are writing to the same resource.",
                     UserWarning,
                 )
+                return None
             else:
                 raise
```

### Comparing `cached_path-1.3.4/cached_path/meta.py` & `cached_path-1.3.5/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.4/cached_path/progress.py` & `cached_path-1.3.5/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.4/cached_path/schemes/__init__.py` & `cached_path-1.3.5/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.4/cached_path/schemes/beaker.py` & `cached_path-1.3.5/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.4/cached_path/schemes/gs.py` & `cached_path-1.3.5/cached_path/schemes/gs.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.4/cached_path/schemes/hf.py` & `cached_path-1.3.5/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.4/cached_path/schemes/http.py` & `cached_path-1.3.5/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.4/cached_path/schemes/s3.py` & `cached_path-1.3.5/cached_path/schemes/s3.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.4/cached_path/schemes/scheme_client.py` & `cached_path-1.3.5/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.4/cached_path/testing.py` & `cached_path-1.3.5/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.4/cached_path/util.py` & `cached_path-1.3.5/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.4/cached_path.egg-info/PKG-INFO` & `cached_path-1.3.5/cached_path.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cached-path
-Version: 1.3.4
+Version: 1.3.5
 Home-page: https://github.com/allenai/cached_path
 Author: Allen Institute for Artificial Intelligence
 Author-email: contact@allenai.org
 License: Apache
 Keywords: allennlp cached_path file utils
 Classifier: Intended Audience :: Science/Research
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cached-path Version: 1.3.4 Home-page: https://
+Metadata-Version: 2.1 Name: cached-path Version: 1.3.5 Home-page: https://
 github.com/allenai/cached_path Author: Allen Institute for Artificial
 Intelligence Author-email: contact@allenai.org License: Apache Keywords:
 allennlp cached_path file utils Classifier: Intended Audience :: Science/
 Research Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Requires-Python: >=3.7 Description-Content-Type: text/
```

### Comparing `cached_path-1.3.4/cached_path.egg-info/SOURCES.txt` & `cached_path-1.3.5/cached_path.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cached_path-1.3.4/setup.py` & `cached_path-1.3.5/setup.py`

 * *Files identical despite different names*

