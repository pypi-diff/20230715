# Comparing `tmp/safepull-2.0.4.tar.gz` & `tmp/safepull-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safepull-2.0.4.tar", last modified: Thu Jul 13 14:07:40 2023, max compression
+gzip compressed data, was "safepull-2.0.5.tar", max compression
```

## Comparing `safepull-2.0.4.tar` & `safepull-2.0.5.tar`

### file list

```diff
@@ -1,19 +1,8 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:07:40.820465 safepull-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-13 14:07:28.000000 safepull-2.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-13 14:07:40.816465 safepull-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-13 14:07:28.000000 safepull-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-13 14:07:28.000000 safepull-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:07:40.820465 safepull-2.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:07:40.816465 safepull-2.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:07:40.816465 safepull-2.0.4/src/safepull/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 14:07:28.000000 safepull-2.0.4/src/safepull/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-13 14:07:28.000000 safepull-2.0.4/src/safepull/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-13 14:07:28.000000 safepull-2.0.4/src/safepull/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-07-13 14:07:28.000000 safepull-2.0.4/src/safepull/safepull.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 14:07:40.816465 safepull-2.0.4/src/safepull.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-07-13 14:07:40.000000 safepull-2.0.4/src/safepull.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-13 14:07:40.000000 safepull-2.0.4/src/safepull.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 14:07:40.000000 safepull-2.0.4/src/safepull.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 14:07:40.000000 safepull-2.0.4/src/safepull.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 14:07:40.000000 safepull-2.0.4/src/safepull.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-13 14:07:40.000000 safepull-2.0.4/src/safepull.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1060 2023-07-15 16:01:22.713137 safepull-2.0.5/LICENSE
+-rw-r--r--   0        0        0     5359 2023-07-15 16:01:22.713137 safepull-2.0.5/README.md
+-rw-r--r--   0        0        0      619 2023-07-15 16:01:22.713137 safepull-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-15 16:01:22.713137 safepull-2.0.5/src/safepull/__init__.py
+-rw-r--r--   0        0        0       64 2023-07-15 16:01:22.713137 safepull-2.0.5/src/safepull/__main__.py
+-rw-r--r--   0        0        0     3058 2023-07-15 16:01:22.713137 safepull-2.0.5/src/safepull/models.py
+-rw-r--r--   0        0        0     3572 2023-07-15 16:01:22.713137 safepull-2.0.5/src/safepull/safepull.py
+-rw-r--r--   0        0        0     5966 1970-01-01 00:00:00.000000 safepull-2.0.5/PKG-INFO
```

### Comparing `safepull-2.0.4/LICENSE` & `safepull-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `safepull-2.0.4/PKG-INFO` & `safepull-2.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: safepull
-Version: 2.0.4
-Summary: A CLI tool for downloading and extracting packages from PyPI without interfacing with setup.py
-License: MIT
-Project-URL: repository, https://github.com/import-pandas-as-numpy/safepull/
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # safepull
 
 Safepull is a command line tool to interact with PyPI's package indexing to safely download and extract files. This is a targeted replacement for `pip download <package>` to prevent malware detonation within
 setup.py files.
 
 # Installation Instructions
 Safepull is available on PyPI.
```

### Comparing `safepull-2.0.4/src/safepull/models.py` & `safepull-2.0.5/src/safepull/models.py`

 * *Files identical despite different names*

### Comparing `safepull-2.0.4/src/safepull/safepull.py` & `safepull-2.0.5/src/safepull/safepull.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,16 +90,16 @@
                 byteobject, file_name = distribution_list[use_select].download_package()
                 unpack(byteobject, file_name)
                 break
         else:
             distros = user_package.get_distributions()
             print(*distros[0].get_metadata())
             if input("Download package? (Y/N):").lower() == "y":
-                file_name = distros[0].download_package()
-                unpack(file_name)
+                byteobject, file_name = distros[0].download_package()
+                unpack(byteobject, file_name)
     else:
         sdist = user_package.get_sdist()
         if sdist is None:
             print("No sdist found. Grabbing first package.")
             sdist = user_package.get_distributions()[0]
-        file_name = sdist.download_package()
-        unpack(file_name)
+        byteobject, file_name = sdist.download_package()
+        unpack(byteobject, file_name)
```

### Comparing `safepull-2.0.4/src/safepull.egg-info/PKG-INFO` & `safepull-2.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Metadata-Version: 2.1
 Name: safepull
-Version: 2.0.4
-Summary: A CLI tool for downloading and extracting packages from PyPI without interfacing with setup.py
+Version: 2.0.5
+Summary: A CLI tool for downloading and extracting packages from PyPI without interfacing with setup.py.
 License: MIT
-Project-URL: repository, https://github.com/import-pandas-as-numpy/safepull/
-Requires-Python: >=3.10
+Author: Rem
+Author-email: 128343390+import-pandas-as-numpy@users.noreply.github.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: rich (>=13.4.2,<14.0.0)
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # safepull
 
 Safepull is a command line tool to interact with PyPI's package indexing to safely download and extract files. This is a targeted replacement for `pip download <package>` to prevent malware detonation within
 setup.py files.
 
 # Installation Instructions
@@ -61,7 +67,8 @@
 │ 20    │ numpy-1.25.0-cp39-cp39-win_amd64.whl                                         │ bdist_wheel  │ 14.36     │
 │ 21    │ numpy-1.25.0-pp39-pypy39_pp73-macosx_10_9_x86_64.whl                         │ bdist_wheel  │ 18.51     │
 │ 22    │ numpy-1.25.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl │ bdist_wheel  │ 16.22     │
 │ 23    │ numpy-1.25.0-pp39-pypy39_pp73-win_amd64.whl                                  │ bdist_wheel  │ 14.23     │
 │ 24    │ numpy-1.25.0.tar.gz                                                          │ sdist        │ 9.94      │
 └───────┴──────────────────────────────────────────────────────────────────────────────┴──────────────┴───────────┘
 ```
+
```

