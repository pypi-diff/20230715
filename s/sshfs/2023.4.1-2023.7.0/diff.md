# Comparing `tmp/sshfs-2023.4.1.tar.gz` & `tmp/sshfs-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshfs-2023.4.1.tar", last modified: Thu Apr  6 09:48:13 2023, max compression
+gzip compressed data, was "sshfs-2023.7.0.tar", last modified: Fri Jul 14 22:12:56 2023, max compression
```

## Comparing `sshfs-2023.4.1.tar` & `sshfs-2023.7.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:48:13.901432 sshfs-2023.4.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:48:13.893432 sshfs-2023.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:48:13.897432 sshfs-2023.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-06 09:48:00.000000 sshfs-2023.4.1/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-06 09:48:00.000000 sshfs-2023.4.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-06 09:48:00.000000 sshfs-2023.4.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-06 09:48:00.000000 sshfs-2023.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-06 09:48:00.000000 sshfs-2023.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-04-06 09:48:00.000000 sshfs-2023.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-06 09:48:13.901432 sshfs-2023.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-06 09:48:00.000000 sshfs-2023.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-06 09:48:00.000000 sshfs-2023.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-06 09:48:00.000000 sshfs-2023.4.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-06 09:48:13.901432 sshfs-2023.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 09:48:00.000000 sshfs-2023.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:48:13.897432 sshfs-2023.4.1/sshfs/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-06 09:48:00.000000 sshfs-2023.4.1/sshfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-06 09:48:00.000000 sshfs-2023.4.1/sshfs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-04-06 09:48:00.000000 sshfs-2023.4.1/sshfs/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:48:13.897432 sshfs-2023.4.1/sshfs/pools/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-06 09:48:00.000000 sshfs-2023.4.1/sshfs/pools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-04-06 09:48:00.000000 sshfs-2023.4.1/sshfs/pools/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-06 09:48:00.000000 sshfs-2023.4.1/sshfs/pools/hard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-06 09:48:00.000000 sshfs-2023.4.1/sshfs/pools/soft.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-04-06 09:48:00.000000 sshfs-2023.4.1/sshfs/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-06 09:48:00.000000 sshfs-2023.4.1/sshfs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:48:13.897432 sshfs-2023.4.1/sshfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-06 09:48:13.000000 sshfs-2023.4.1/sshfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-06 09:48:13.000000 sshfs-2023.4.1/sshfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 09:48:13.000000 sshfs-2023.4.1/sshfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-06 09:48:13.000000 sshfs-2023.4.1/sshfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-06 09:48:13.000000 sshfs-2023.4.1/sshfs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:48:13.897432 sshfs-2023.4.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 09:48:13.901432 sshfs-2023.4.1/tests/static/
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-06 09:48:00.000000 sshfs-2023.4.1/tests/static/user.key
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-06 09:48:00.000000 sshfs-2023.4.1/tests/static/user.key.pub
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-06 09:48:00.000000 sshfs-2023.4.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-04-06 09:48:00.000000 sshfs-2023.4.1/tests/test_sftp_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)     8733 2023-04-06 09:48:00.000000 sshfs-2023.4.1/tests/test_sshfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:12:56.590614 sshfs-2023.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:12:56.582614 sshfs-2023.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:12:56.586614 sshfs-2023.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-14 22:12:45.000000 sshfs-2023.7.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-14 22:12:45.000000 sshfs-2023.7.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-14 22:12:45.000000 sshfs-2023.7.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-14 22:12:45.000000 sshfs-2023.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-14 22:12:45.000000 sshfs-2023.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-07-14 22:12:45.000000 sshfs-2023.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-14 22:12:56.590614 sshfs-2023.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-07-14 22:12:45.000000 sshfs-2023.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-14 22:12:45.000000 sshfs-2023.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-14 22:12:45.000000 sshfs-2023.7.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-14 22:12:56.590614 sshfs-2023.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 22:12:45.000000 sshfs-2023.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:12:56.586614 sshfs-2023.7.0/sshfs/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-14 22:12:45.000000 sshfs-2023.7.0/sshfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-14 22:12:45.000000 sshfs-2023.7.0/sshfs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-14 22:12:45.000000 sshfs-2023.7.0/sshfs/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:12:56.586614 sshfs-2023.7.0/sshfs/pools/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-14 22:12:45.000000 sshfs-2023.7.0/sshfs/pools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-14 22:12:45.000000 sshfs-2023.7.0/sshfs/pools/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-14 22:12:45.000000 sshfs-2023.7.0/sshfs/pools/hard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-07-14 22:12:45.000000 sshfs-2023.7.0/sshfs/pools/soft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-07-14 22:12:45.000000 sshfs-2023.7.0/sshfs/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-07-14 22:12:45.000000 sshfs-2023.7.0/sshfs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:12:56.586614 sshfs-2023.7.0/sshfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-14 22:12:56.000000 sshfs-2023.7.0/sshfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-14 22:12:56.000000 sshfs-2023.7.0/sshfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:12:56.000000 sshfs-2023.7.0/sshfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-14 22:12:56.000000 sshfs-2023.7.0/sshfs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-14 22:12:56.000000 sshfs-2023.7.0/sshfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 22:12:56.000000 sshfs-2023.7.0/sshfs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:12:56.590614 sshfs-2023.7.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:12:56.590614 sshfs-2023.7.0/tests/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-14 22:12:45.000000 sshfs-2023.7.0/tests/static/user.key
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-14 22:12:45.000000 sshfs-2023.7.0/tests/static/user.key.pub
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-14 22:12:45.000000 sshfs-2023.7.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-07-14 22:12:45.000000 sshfs-2023.7.0/tests/test_sftp_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-07-14 22:12:45.000000 sshfs-2023.7.0/tests/test_sshfs.py
```

### Comparing `sshfs-2023.4.1/.github/workflows/publish.yml` & `sshfs-2023.7.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `sshfs-2023.4.1/.github/workflows/test.yml` & `sshfs-2023.7.0/.github/workflows/test.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 on:
   push:
     branches:
-      - master
+      - main
   pull_request:
     branches:
       - '*'
+  schedule:
+    - cron: '5 1 * * *'
+  workflow_dispatch:
 
 name: Tests
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
```

### Comparing `sshfs-2023.4.1/.gitignore` & `sshfs-2023.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sshfs-2023.4.1/.pre-commit-config.yaml` & `sshfs-2023.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sshfs-2023.4.1/LICENSE` & `sshfs-2023.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sshfs-2023.4.1/PKG-INFO` & `sshfs-2023.7.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sshfs
-Version: 2023.4.1
+Version: 2023.7.0
 Summary: SSH Filesystem -- Async SSH/SFTP backend for fsspec
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -30,15 +30,28 @@
 - Supports features outside of the SFTP (e.g server side copy through SSH command execution)
 - Quite fast (compared to alternatives like paramiko)
 - Builtin Channel Management
 - Async! (thanks to `asyncssh`)
 
 ## Tutorial
 
-Install the `sshfs` from PyPI or the conda-forge, and import it;
+Install the `sshfs` from PyPI or the conda-forge. This will install `fsspec`
+and register `sshfs` for `ssh://` urls, so you can open files using:
+
+```py
+from fsspec import open
+
+with open('ssh://[user@]host[:port]/path/to/file', "w") as file:
+    file.write("Hello World!")
+
+with open('ssh://[user@]host[:port]/path/to/file', "r") as file:
+    print(file.read())
+```
+
+For more operations, you can use the `SSHFileSystem` class directly:
 
 ```py
 from sshfs import SSHFileSystem
 ```
 
 To connect with a password, you can simply specify `username`/`password`
 as keyword arguments and connect to the host of your choosing;
@@ -60,14 +73,16 @@
 # or with a private key
 fs = SSHFileSystem(
     'ssh.example.com',
     client_keys=['/path/to/ssh/key']
 )
 ```
 
+Note: you can also pass `client_keys` as an argument to `fsspec.open`.
+
 All operations and their descriptions are specified [here](https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem).
 Here are a few example calls you can make, starting with `info()` which allows you to retrieve the metadata about given path;
 
 ```py
 >>> details = fs.info('/tmp')
 >>> print(f'{details["name"]!r} is a {details["type"]}!')
 '/tmp/' is a directory!
@@ -78,37 +93,37 @@
 ```
 
 You can also create new files through either putting a local file with `put_file` or opening a file in write mode;
 
 ```py
 >>> with fs.open('/tmp/message.dat', 'wb') as stream:
 ...     stream.write(b'super secret messsage!')
-... 
+...
 ```
 
 And either download it through `get_file` or simply read it on the fly with opening it;
 
 ```py
 >>> with fs.open('/tmp/message.dat') as stream:
 ...     print(stream.read())
-... 
+...
 b'super secret messsage!'
 ```
 
 There are also a lot of other basic filesystem operations, such as `mkdir`, `touch` and `find`;
 
 ```py
 >>> fs.mkdir('/tmp/dir')
 >>> fs.mkdir('/tmp/dir/eggs')
 >>> fs.touch('/tmp/dir/spam')
 >>> fs.touch('/tmp/dir/eggs/quux')
->>> 
+>>>
 >>> for file in fs.find('/tmp/dir'):
 ...     print(file)
-... 
+...
 /tmp/dir/eggs/quux
 /tmp/dir/spam
 ```
 
 If you want to list a directory but not it's children, you can use `ls()`;
 
 ```py
```

### Comparing `sshfs-2023.4.1/README.md` & `sshfs-2023.7.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,28 @@
 - Supports features outside of the SFTP (e.g server side copy through SSH command execution)
 - Quite fast (compared to alternatives like paramiko)
 - Builtin Channel Management
 - Async! (thanks to `asyncssh`)
 
 ## Tutorial
 
-Install the `sshfs` from PyPI or the conda-forge, and import it;
+Install the `sshfs` from PyPI or the conda-forge. This will install `fsspec`
+and register `sshfs` for `ssh://` urls, so you can open files using:
+
+```py
+from fsspec import open
+
+with open('ssh://[user@]host[:port]/path/to/file', "w") as file:
+    file.write("Hello World!")
+
+with open('ssh://[user@]host[:port]/path/to/file', "r") as file:
+    print(file.read())
+```
+
+For more operations, you can use the `SSHFileSystem` class directly:
 
 ```py
 from sshfs import SSHFileSystem
 ```
 
 To connect with a password, you can simply specify `username`/`password`
 as keyword arguments and connect to the host of your choosing;
@@ -39,14 +52,16 @@
 # or with a private key
 fs = SSHFileSystem(
     'ssh.example.com',
     client_keys=['/path/to/ssh/key']
 )
 ```
 
+Note: you can also pass `client_keys` as an argument to `fsspec.open`.
+
 All operations and their descriptions are specified [here](https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem).
 Here are a few example calls you can make, starting with `info()` which allows you to retrieve the metadata about given path;
 
 ```py
 >>> details = fs.info('/tmp')
 >>> print(f'{details["name"]!r} is a {details["type"]}!')
 '/tmp/' is a directory!
@@ -57,37 +72,37 @@
 ```
 
 You can also create new files through either putting a local file with `put_file` or opening a file in write mode;
 
 ```py
 >>> with fs.open('/tmp/message.dat', 'wb') as stream:
 ...     stream.write(b'super secret messsage!')
-... 
+...
 ```
 
 And either download it through `get_file` or simply read it on the fly with opening it;
 
 ```py
 >>> with fs.open('/tmp/message.dat') as stream:
 ...     print(stream.read())
-... 
+...
 b'super secret messsage!'
 ```
 
 There are also a lot of other basic filesystem operations, such as `mkdir`, `touch` and `find`;
 
 ```py
 >>> fs.mkdir('/tmp/dir')
 >>> fs.mkdir('/tmp/dir/eggs')
 >>> fs.touch('/tmp/dir/spam')
 >>> fs.touch('/tmp/dir/eggs/quux')
->>> 
+>>>
 >>> for file in fs.find('/tmp/dir'):
 ...     print(file)
-... 
+...
 /tmp/dir/eggs/quux
 /tmp/dir/spam
 ```
 
 If you want to list a directory but not it's children, you can use `ls()`;
 
 ```py
```

### Comparing `sshfs-2023.4.1/setup.cfg` & `sshfs-2023.7.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -23,11 +23,15 @@
 fido2 = asyncssh[fido2]
 gssapi = asyncssh[gssapi]
 libnacl = asyncssh[libnacl]
 pkcs11 = asyncssh[python-pkcs11]
 pyopenssl = asyncssh[pyOpenSSL]
 pywin32 = asyncssh[pywin32]
 
+[options.entry_points]
+fsspec.specs = 
+	ssh = sshfs.spec:SSHFileSystem
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `sshfs-2023.4.1/sshfs/config.py` & `sshfs-2023.7.0/sshfs/config.py`

 * *Files identical despite different names*

### Comparing `sshfs-2023.4.1/sshfs/file.py` & `sshfs-2023.7.0/sshfs/file.py`

 * *Files identical despite different names*

### Comparing `sshfs-2023.4.1/sshfs/pools/base.py` & `sshfs-2023.7.0/sshfs/pools/base.py`

 * *Files identical despite different names*

### Comparing `sshfs-2023.4.1/sshfs/pools/hard.py` & `sshfs-2023.7.0/sshfs/pools/hard.py`

 * *Files identical despite different names*

### Comparing `sshfs-2023.4.1/sshfs/pools/soft.py` & `sshfs-2023.7.0/sshfs/pools/soft.py`

 * *Files identical despite different names*

### Comparing `sshfs-2023.4.1/sshfs/spec.py` & `sshfs-2023.7.0/sshfs/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import weakref
 from contextlib import AsyncExitStack, suppress
 from datetime import datetime
 
 import asyncssh
 from asyncssh.sftp import SFTPOpUnsupported
 from fsspec.asyn import AsyncFileSystem, async_methods, sync, sync_wrapper
+from fsspec.utils import infer_storage_options
 
 from sshfs.file import SSHFile
 from sshfs.pools import SFTPSoftChannelPool
 from sshfs.utils import (
     READ_BLOCK_SIZE,
     WRITE_BLOCK_SIZE,
     as_progress_handler,
@@ -69,14 +70,27 @@
             max_sftp_channels=max_sessions - _SHELL_CHANNELS,
             **_client_args,
         )
         weakref.finalize(
             self, sync, self.loop, self._finalize, self._pool, self._stack
         )
 
+    @classmethod
+    def _strip_protocol(cls, path):
+        # Remove components such as host and username from path.
+        inferred_path = infer_storage_options(path)["path"]
+        return super()._strip_protocol(inferred_path)
+
+    @staticmethod
+    def _get_kwargs_from_urls(urlpath):
+        out = infer_storage_options(urlpath)
+        out.pop("path", None)
+        out.pop("protocol", None)
+        return out
+
     @wrap_exceptions
     async def _connect(
         self, host, pool_type, max_sftp_channels, **client_args
     ):
         self._client_lock = asyncio.Semaphore(_SHELL_CHANNELS)
 
         _raw_client = asyncssh.connect(host, **client_args)
```

### Comparing `sshfs-2023.4.1/sshfs/utils.py` & `sshfs-2023.7.0/sshfs/utils.py`

 * *Files identical despite different names*

### Comparing `sshfs-2023.4.1/sshfs.egg-info/PKG-INFO` & `sshfs-2023.7.0/sshfs.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sshfs
-Version: 2023.4.1
+Version: 2023.7.0
 Summary: SSH Filesystem -- Async SSH/SFTP backend for fsspec
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -30,15 +30,28 @@
 - Supports features outside of the SFTP (e.g server side copy through SSH command execution)
 - Quite fast (compared to alternatives like paramiko)
 - Builtin Channel Management
 - Async! (thanks to `asyncssh`)
 
 ## Tutorial
 
-Install the `sshfs` from PyPI or the conda-forge, and import it;
+Install the `sshfs` from PyPI or the conda-forge. This will install `fsspec`
+and register `sshfs` for `ssh://` urls, so you can open files using:
+
+```py
+from fsspec import open
+
+with open('ssh://[user@]host[:port]/path/to/file', "w") as file:
+    file.write("Hello World!")
+
+with open('ssh://[user@]host[:port]/path/to/file', "r") as file:
+    print(file.read())
+```
+
+For more operations, you can use the `SSHFileSystem` class directly:
 
 ```py
 from sshfs import SSHFileSystem
 ```
 
 To connect with a password, you can simply specify `username`/`password`
 as keyword arguments and connect to the host of your choosing;
@@ -60,14 +73,16 @@
 # or with a private key
 fs = SSHFileSystem(
     'ssh.example.com',
     client_keys=['/path/to/ssh/key']
 )
 ```
 
+Note: you can also pass `client_keys` as an argument to `fsspec.open`.
+
 All operations and their descriptions are specified [here](https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem).
 Here are a few example calls you can make, starting with `info()` which allows you to retrieve the metadata about given path;
 
 ```py
 >>> details = fs.info('/tmp')
 >>> print(f'{details["name"]!r} is a {details["type"]}!')
 '/tmp/' is a directory!
@@ -78,37 +93,37 @@
 ```
 
 You can also create new files through either putting a local file with `put_file` or opening a file in write mode;
 
 ```py
 >>> with fs.open('/tmp/message.dat', 'wb') as stream:
 ...     stream.write(b'super secret messsage!')
-... 
+...
 ```
 
 And either download it through `get_file` or simply read it on the fly with opening it;
 
 ```py
 >>> with fs.open('/tmp/message.dat') as stream:
 ...     print(stream.read())
-... 
+...
 b'super secret messsage!'
 ```
 
 There are also a lot of other basic filesystem operations, such as `mkdir`, `touch` and `find`;
 
 ```py
 >>> fs.mkdir('/tmp/dir')
 >>> fs.mkdir('/tmp/dir/eggs')
 >>> fs.touch('/tmp/dir/spam')
 >>> fs.touch('/tmp/dir/eggs/quux')
->>> 
+>>>
 >>> for file in fs.find('/tmp/dir'):
 ...     print(file)
-... 
+...
 /tmp/dir/eggs/quux
 /tmp/dir/spam
 ```
 
 If you want to list a directory but not it's children, you can use `ls()`;
 
 ```py
```

### Comparing `sshfs-2023.4.1/sshfs.egg-info/SOURCES.txt` & `sshfs-2023.7.0/sshfs.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 sshfs/config.py
 sshfs/file.py
 sshfs/spec.py
 sshfs/utils.py
 sshfs.egg-info/PKG-INFO
 sshfs.egg-info/SOURCES.txt
 sshfs.egg-info/dependency_links.txt
+sshfs.egg-info/entry_points.txt
 sshfs.egg-info/requires.txt
 sshfs.egg-info/top_level.txt
 sshfs/pools/__init__.py
 sshfs/pools/base.py
 sshfs/pools/hard.py
 sshfs/pools/soft.py
 tests/test_config.py
```

### Comparing `sshfs-2023.4.1/tests/static/user.key` & `sshfs-2023.7.0/tests/static/user.key`

 * *Files identical despite different names*

### Comparing `sshfs-2023.4.1/tests/static/user.key.pub` & `sshfs-2023.7.0/tests/static/user.key.pub`

 * *Files identical despite different names*

### Comparing `sshfs-2023.4.1/tests/test_config.py` & `sshfs-2023.7.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `sshfs-2023.4.1/tests/test_sftp_pools.py` & `sshfs-2023.7.0/tests/test_sftp_pools.py`

 * *Files identical despite different names*

### Comparing `sshfs-2023.4.1/tests/test_sshfs.py` & `sshfs-2023.7.0/tests/test_sshfs.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import secrets
 import tempfile
 import warnings
 from concurrent import futures
 from datetime import datetime, timedelta
 from pathlib import Path
 
+import fsspec
 import pytest
 from asyncssh.sftp import SFTPFailure
 
 from sshfs import SSHFileSystem
 
 _STATIC = (Path(__file__).parent / "static").resolve()
 USERS = {"user": _STATIC / "user.key"}
@@ -67,14 +68,39 @@
 
 
 def strip_keys(info):
     for key in ["name", "time", "mtime", "atime"]:
         info.pop(key, None)
 
 
+def test_fsspec_registration(ssh_server):
+    fs = fsspec.filesystem(
+        "ssh",
+        host=ssh_server.host,
+        port=ssh_server.port,
+        username="user",
+        client_keys=[USERS["user"]],
+    )
+    assert isinstance(fs, SSHFileSystem)
+
+
+def test_fsspec_url_parsing(ssh_server, remote_dir, user="user"):
+    url = f"ssh://{user}@{ssh_server.host}:{ssh_server.port}/{remote_dir}/file"
+    with fsspec.open(url, "w", client_keys=[USERS[user]]) as file:
+        # Check the underlying file system.
+        file_fs = file.buffer.fs
+        assert isinstance(file_fs, SSHFileSystem)
+        assert file_fs.storage_options == {
+            "host": ssh_server.host,
+            "port": ssh_server.port,
+            "username": user,
+            "client_keys": [USERS[user]],
+        }
+
+
 def test_info(fs, remote_dir):
     fs.touch(remote_dir + "/a.txt")
     details = fs.info(remote_dir + "/a.txt")
     assert details["type"] == "file"
     assert details["name"] == remote_dir + "/a.txt"
     assert details["size"] == 0
```

