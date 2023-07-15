# Comparing `tmp/platformdirs-3.9.0.tar.gz` & `tmp/platformdirs-3.9.1.tar.gz`

## Comparing `platformdirs-3.9.0.tar` & `platformdirs-3.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 platformdirs-3.9.0/tox.ini
--rw-r--r--   0        0        0    20392 2020-02-02 00:00:00.000000 platformdirs-3.9.0/src/platformdirs/__init__.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 platformdirs-3.9.0/src/platformdirs/__main__.py
--rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 platformdirs-3.9.0/src/platformdirs/android.py
--rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 platformdirs-3.9.0/src/platformdirs/api.py
--rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 platformdirs-3.9.0/src/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.9.0/src/platformdirs/py.typed
--rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 platformdirs-3.9.0/src/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.9.0/src/platformdirs/version.py
--rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 platformdirs-3.9.0/src/platformdirs/windows.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 platformdirs-3.9.0/tests/conftest.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 platformdirs-3.9.0/tests/test_android.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 platformdirs-3.9.0/tests/test_api.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 platformdirs-3.9.0/tests/test_comp_with_appdirs.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 platformdirs-3.9.0/tests/test_macos.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.9.0/tests/test_main.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 platformdirs-3.9.0/tests/test_unix.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.9.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.9.0/LICENSE
--rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 platformdirs-3.9.0/README.rst
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 platformdirs-3.9.0/pyproject.toml
--rw-r--r--   0        0        0    11490 2020-02-02 00:00:00.000000 platformdirs-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 platformdirs-3.9.1/tox.ini
+-rw-r--r--   0        0        0    20392 2020-02-02 00:00:00.000000 platformdirs-3.9.1/src/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 platformdirs-3.9.1/src/platformdirs/__main__.py
+-rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 platformdirs-3.9.1/src/platformdirs/android.py
+-rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 platformdirs-3.9.1/src/platformdirs/api.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 platformdirs-3.9.1/src/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.9.1/src/platformdirs/py.typed
+-rw-r--r--   0        0        0     9060 2020-02-02 00:00:00.000000 platformdirs-3.9.1/src/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.9.1/src/platformdirs/version.py
+-rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 platformdirs-3.9.1/src/platformdirs/windows.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 platformdirs-3.9.1/tests/conftest.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 platformdirs-3.9.1/tests/test_android.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 platformdirs-3.9.1/tests/test_api.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 platformdirs-3.9.1/tests/test_comp_with_appdirs.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 platformdirs-3.9.1/tests/test_macos.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.9.1/tests/test_main.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 platformdirs-3.9.1/tests/test_unix.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.9.1/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.9.1/LICENSE
+-rw-r--r--   0        0        0     9343 2020-02-02 00:00:00.000000 platformdirs-3.9.1/README.rst
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 platformdirs-3.9.1/pyproject.toml
+-rw-r--r--   0        0        0    11490 2020-02-02 00:00:00.000000 platformdirs-3.9.1/PKG-INFO
```

### Comparing `platformdirs-3.9.0/tox.ini` & `platformdirs-3.9.1/tox.ini`

 * *Files identical despite different names*

### Comparing `platformdirs-3.9.0/src/platformdirs/__init__.py` & `platformdirs-3.9.1/src/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.9.0/src/platformdirs/__main__.py` & `platformdirs-3.9.1/src/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.9.0/src/platformdirs/android.py` & `platformdirs-3.9.1/src/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.9.0/src/platformdirs/api.py` & `platformdirs-3.9.1/src/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.9.0/src/platformdirs/macos.py` & `platformdirs-3.9.1/src/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.9.0/src/platformdirs/unix.py` & `platformdirs-3.9.1/src/platformdirs/unix.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,15 @@
 
     @property
     def user_log_dir(self) -> str:
         """:return: log directory tied to the user, same as `user_state_dir` if not opinionated else ``log`` in it"""
         path = self.user_state_dir
         if self.opinion:
             path = os.path.join(path, "log")  # noqa: PTH118
+            self._optionally_create_directory(path)
         return path
 
     @property
     def user_documents_dir(self) -> str:
         """:return: documents directory tied to the user, e.g. ``~/Documents``"""
         return _get_user_media_dir("XDG_DOCUMENTS_DIR", "~/Documents")
```

### Comparing `platformdirs-3.9.0/src/platformdirs/windows.py` & `platformdirs-3.9.1/src/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.9.0/tests/conftest.py` & `platformdirs-3.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.9.0/tests/test_android.py` & `platformdirs-3.9.1/tests/test_android.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.9.0/tests/test_api.py` & `platformdirs-3.9.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.9.0/tests/test_comp_with_appdirs.py` & `platformdirs-3.9.1/tests/test_comp_with_appdirs.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.9.0/tests/test_macos.py` & `platformdirs-3.9.1/tests/test_macos.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.9.0/tests/test_unix.py` & `platformdirs-3.9.1/tests/test_unix.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.9.0/LICENSE` & `platformdirs-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `platformdirs-3.9.0/README.rst` & `platformdirs-3.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `platformdirs-3.9.0/pyproject.toml` & `platformdirs-3.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `platformdirs-3.9.0/PKG-INFO` & `platformdirs-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platformdirs
-Version: 3.9.0
+Version: 3.9.1
 Summary: A small Python package for determining appropriate platform-specific dirs, e.g. a "user data dir".
 Project-URL: Documentation, https://platformdirs.readthedocs.io
 Project-URL: Homepage, https://github.com/platformdirs/platformdirs
 Project-URL: Source, https://github.com/platformdirs/platformdirs
 Project-URL: Tracker, https://github.com/platformdirs/platformdirs/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Julian Berman <Julian@GrayVines.com>, Ofek Lev <oss@ofek.dev>, Ronny Pfannschmidt <opensource@ronnypfannschmidt.de>
 License-Expression: MIT
```

