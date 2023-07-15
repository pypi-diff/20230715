# Comparing `tmp/oras-0.1.19.tar.gz` & `tmp/oras-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oras-0.1.19.tar", last modified: Mon Jul 10 16:16:20 2023, max compression
+gzip compressed data, was "oras-0.1.2.tar", last modified: Sat Jul 15 18:42:09 2023, max compression
```

## Comparing `oras-0.1.19.tar` & `oras-0.1.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 16:16:20.064996 oras-0.1.19/
--rw-r--r--   0 runner    (1001) docker     (122)    11343 2023-07-10 16:15:49.000000 oras-0.1.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-10 16:15:49.000000 oras-0.1.19/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6083 2023-07-10 16:16:20.064996 oras-0.1.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5239 2023-07-10 16:15:49.000000 oras-0.1.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 16:16:20.060995 oras-0.1.19/oras/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-10 16:15:49.000000 oras-0.1.19/oras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-07-10 16:15:49.000000 oras-0.1.19/oras/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     7530 2023-07-10 16:15:49.000000 oras-0.1.19/oras/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3812 2023-07-10 16:15:49.000000 oras-0.1.19/oras/container.py
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-07-10 16:15:49.000000 oras-0.1.19/oras/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-10 16:15:49.000000 oras-0.1.19/oras/defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)     8737 2023-07-10 16:15:49.000000 oras-0.1.19/oras/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 16:16:20.064996 oras-0.1.19/oras/main/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 16:15:49.000000 oras-0.1.19/oras/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-10 16:15:49.000000 oras-0.1.19/oras/main/login.py
--rw-r--r--   0 runner    (1001) docker     (122)     4470 2023-07-10 16:15:49.000000 oras-0.1.19/oras/oci.py
--rw-r--r--   0 runner    (1001) docker     (122)    35645 2023-07-10 16:15:49.000000 oras-0.1.19/oras/provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-07-10 16:15:49.000000 oras-0.1.19/oras/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 16:16:20.064996 oras-0.1.19/oras/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-10 16:15:49.000000 oras-0.1.19/oras/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-10 16:15:49.000000 oras-0.1.19/oras/tests/annotations.json
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-10 16:15:49.000000 oras-0.1.19/oras/tests/artifact.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      185 2023-07-10 16:15:49.000000 oras-0.1.19/oras/tests/run_registry.sh
--rw-r--r--   0 runner    (1001) docker     (122)     5066 2023-07-10 16:15:49.000000 oras-0.1.19/oras/tests/test_oras.py
--rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-07-10 16:15:49.000000 oras-0.1.19/oras/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-07-10 16:15:49.000000 oras-0.1.19/oras/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 16:16:20.064996 oras-0.1.19/oras/tests/upload_data/
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-10 16:15:49.000000 oras-0.1.19/oras/tests/upload_data/artifact.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 16:16:20.064996 oras-0.1.19/oras/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-10 16:15:49.000000 oras-0.1.19/oras/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10673 2023-07-10 16:15:49.000000 oras-0.1.19/oras/utils/fileio.py
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-07-10 16:15:49.000000 oras-0.1.19/oras/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (122)      985 2023-07-10 16:15:49.000000 oras-0.1.19/oras/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 16:16:20.060995 oras-0.1.19/oras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6083 2023-07-10 16:16:19.000000 oras-0.1.19/oras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-10 16:16:19.000000 oras-0.1.19/oras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 16:16:19.000000 oras-0.1.19/oras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 16:16:16.000000 oras-0.1.19/oras.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-07-10 16:16:19.000000 oras-0.1.19/oras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-10 16:16:19.000000 oras-0.1.19/oras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-10 16:15:49.000000 oras-0.1.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-07-10 16:16:20.064996 oras-0.1.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3370 2023-07-10 16:15:49.000000 oras-0.1.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 18:42:09.734842 oras-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    11343 2023-07-15 18:41:35.000000 oras-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-15 18:41:35.000000 oras-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6082 2023-07-15 18:42:09.734842 oras-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5239 2023-07-15 18:41:35.000000 oras-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 18:42:09.730842 oras-0.1.2/oras/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-15 18:41:35.000000 oras-0.1.2/oras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-07-15 18:41:35.000000 oras-0.1.2/oras/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7530 2023-07-15 18:41:35.000000 oras-0.1.2/oras/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3812 2023-07-15 18:41:35.000000 oras-0.1.2/oras/container.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-07-15 18:41:35.000000 oras-0.1.2/oras/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-15 18:41:35.000000 oras-0.1.2/oras/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8737 2023-07-15 18:41:35.000000 oras-0.1.2/oras/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 18:42:09.730842 oras-0.1.2/oras/main/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-15 18:41:35.000000 oras-0.1.2/oras/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-15 18:41:35.000000 oras-0.1.2/oras/main/login.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4470 2023-07-15 18:41:35.000000 oras-0.1.2/oras/oci.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35813 2023-07-15 18:41:35.000000 oras-0.1.2/oras/provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-07-15 18:41:35.000000 oras-0.1.2/oras/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 18:42:09.730842 oras-0.1.2/oras/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-15 18:41:35.000000 oras-0.1.2/oras/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-15 18:41:35.000000 oras-0.1.2/oras/tests/annotations.json
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-15 18:41:35.000000 oras-0.1.2/oras/tests/artifact.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      185 2023-07-15 18:41:35.000000 oras-0.1.2/oras/tests/run_registry.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     5066 2023-07-15 18:41:35.000000 oras-0.1.2/oras/tests/test_oras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-07-15 18:41:35.000000 oras-0.1.2/oras/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-07-15 18:41:35.000000 oras-0.1.2/oras/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 18:42:09.730842 oras-0.1.2/oras/tests/upload_data/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-15 18:41:35.000000 oras-0.1.2/oras/tests/upload_data/artifact.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 18:42:09.734842 oras-0.1.2/oras/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-15 18:41:35.000000 oras-0.1.2/oras/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10673 2023-07-15 18:41:35.000000 oras-0.1.2/oras/utils/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-07-15 18:41:35.000000 oras-0.1.2/oras/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      984 2023-07-15 18:41:35.000000 oras-0.1.2/oras/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 18:42:09.730842 oras-0.1.2/oras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6082 2023-07-15 18:42:09.000000 oras-0.1.2/oras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-15 18:42:09.000000 oras-0.1.2/oras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-15 18:42:09.000000 oras-0.1.2/oras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-15 18:42:05.000000 oras-0.1.2/oras.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-07-15 18:42:09.000000 oras-0.1.2/oras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-15 18:42:09.000000 oras-0.1.2/oras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-15 18:41:35.000000 oras-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-07-15 18:42:09.734842 oras-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3370 2023-07-15 18:41:35.000000 oras-0.1.2/setup.py
```

### Comparing `oras-0.1.19/LICENSE` & `oras-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oras-0.1.19/PKG-INFO` & `oras-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oras
-Version: 0.1.19
+Version: 0.1.2
 Summary: OCI Registry as Storage Python SDK
 Home-page: https://github.com/oras-project/oras-py
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: oci,registry,storage
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: oras Version: 0.1.19 Summary: OCI Registry as
+Metadata-Version: 2.1 Name: oras Version: 0.1.2 Summary: OCI Registry as
 Storage Python SDK Home-page: https://github.com/oras-project/oras-py Author:
 Vanessa Sochat Author-email: vsoch@users.noreply.github.com Maintainer: Vanessa
 Sochat License: LICENSE Keywords: oci,registry,storage Classifier: Intended
 Audience :: Science/Research Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
```

### Comparing `oras-0.1.19/README.md` & `oras-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `oras-0.1.19/oras/auth.py` & `oras-0.1.2/oras/auth.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.19/oras/client.py` & `oras-0.1.2/oras/client.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.19/oras/container.py` & `oras-0.1.2/oras/container.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.19/oras/decorator.py` & `oras-0.1.2/oras/decorator.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.19/oras/defaults.py` & `oras-0.1.2/oras/defaults.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.19/oras/logger.py` & `oras-0.1.2/oras/logger.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.19/oras/main/login.py` & `oras-0.1.2/oras/main/login.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.19/oras/oci.py` & `oras-0.1.2/oras/oci.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.19/oras/provider.py` & `oras-0.1.2/oras/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,18 @@
         self.hostname: Optional[str] = hostname
         self.headers: dict = {}
         self.session: requests.Session = requests.Session()
         self.prefix: str = "http" if insecure else "https"
         self.token: Optional[str] = None
         self._auths: dict = {}
         self._basic_auth = None
+        self._insecure = insecure
+
+        if insecure:
+            requests.packages.urllib3.disable_warnings()  # type: ignore
 
     def logout(self, hostname: str):
         """
         If auths are loaded, remove a hostname.
 
         :param hostname: the registry hostname to remove
         :type hostname: str
@@ -838,14 +842,15 @@
         response = self.session.request(
             method,
             url,
             data=data,
             json=json,
             headers=headers,
             stream=stream,
+            verify=not self._insecure,
         )
 
         # A 401 response is a request for authentication
         if response.status_code not in [401, 404]:
             return response
 
         # Otherwise, authenticate the request and retry
```

### Comparing `oras-0.1.19/oras/schemas.py` & `oras-0.1.2/oras/schemas.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.19/oras/tests/test_oras.py` & `oras-0.1.2/oras/tests/test_oras.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.19/oras/tests/test_provider.py` & `oras-0.1.2/oras/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.19/oras/tests/test_utils.py` & `oras-0.1.2/oras/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.19/oras/utils/fileio.py` & `oras-0.1.2/oras/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.19/oras/utils/request.py` & `oras-0.1.2/oras/utils/request.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.19/oras/version.py` & `oras-0.1.2/oras/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Vanessa Sochat"
 __copyright__ = "Copyright The ORAS Authors."
 __license__ = "Apache-2.0"
 
-__version__ = "0.1.19"
+__version__ = "0.1.2"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "oras"
 PACKAGE_URL = "https://github.com/oras-project/oras-py"
 KEYWORDS = "oci, registry, storage"
 DESCRIPTION = "OCI Registry as Storage Python SDK"
 LICENSE = "LICENSE"
```

### Comparing `oras-0.1.19/oras.egg-info/PKG-INFO` & `oras-0.1.2/oras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oras
-Version: 0.1.19
+Version: 0.1.2
 Summary: OCI Registry as Storage Python SDK
 Home-page: https://github.com/oras-project/oras-py
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: oci,registry,storage
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: oras Version: 0.1.19 Summary: OCI Registry as
+Metadata-Version: 2.1 Name: oras Version: 0.1.2 Summary: OCI Registry as
 Storage Python SDK Home-page: https://github.com/oras-project/oras-py Author:
 Vanessa Sochat Author-email: vsoch@users.noreply.github.com Maintainer: Vanessa
 Sochat License: LICENSE Keywords: oci,registry,storage Classifier: Intended
 Audience :: Science/Research Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
```

### Comparing `oras-0.1.19/oras.egg-info/SOURCES.txt` & `oras-0.1.2/oras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oras-0.1.19/setup.py` & `oras-0.1.2/setup.py`

 * *Files identical despite different names*

