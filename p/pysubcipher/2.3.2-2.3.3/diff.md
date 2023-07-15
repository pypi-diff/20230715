# Comparing `tmp/pysubcipher-2.3.2.tar.gz` & `tmp/pysubcipher-2.3.3.tar.gz`

## Comparing `pysubcipher-2.3.2.tar` & `pysubcipher-2.3.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pysubcipher-2.3.2/src/pysubcipher/__init__.py
--rw-r--r--   0        0        0    12715 2020-02-02 00:00:00.000000 pysubcipher-2.3.2/src/pysubcipher/pysubcipher.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pysubcipher-2.3.2/LICENSE
--rw-r--r--   0        0        0     8542 2020-02-02 00:00:00.000000 pysubcipher-2.3.2/README.md
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 pysubcipher-2.3.2/pyproject.toml
--rw-r--r--   0        0        0     8796 2020-02-02 00:00:00.000000 pysubcipher-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pysubcipher-2.3.3/src/pysubcipher/__init__.py
+-rw-r--r--   0        0        0    12666 2020-02-02 00:00:00.000000 pysubcipher-2.3.3/src/pysubcipher/pysubcipher.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pysubcipher-2.3.3/LICENSE
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 pysubcipher-2.3.3/README.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 pysubcipher-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0     8773 2020-02-02 00:00:00.000000 pysubcipher-2.3.3/PKG-INFO
```

### Comparing `pysubcipher-2.3.2/src/pysubcipher/__init__.py` & `pysubcipher-2.3.3/src/pysubcipher/__init__.py`

 * *Files identical despite different names*

### Comparing `pysubcipher-2.3.2/src/pysubcipher/pysubcipher.py` & `pysubcipher-2.3.3/src/pysubcipher/pysubcipher.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 import os
 
 from .__init__ import HEXDIGITS, PRINTABLE
 
 from typing import Any
 from types import TracebackType
 
-from rich.traceback import install
-install()
-
 class InvalidCharacterError(ValueError):
     def __init__(self, character: str, /) -> None:
         """Raised if an invalid token is present within a string of text while encrypting or decrypting a value.
 
         Args:
             character (str): The invalid character.
         """
```

### Comparing `pysubcipher-2.3.2/LICENSE` & `pysubcipher-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysubcipher-2.3.2/README.md` & `pysubcipher-2.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [PyPiVersion]: https://img.shields.io/pypi/v/pysubcipher
 [SupportedVersions]: https://img.shields.io/badge/python-3.10%20%7C%203.11-orange
 [License]: https://img.shields.io/badge/license-MIT-yellow
 
 # Installation
 Built and tested on Python 3.10 and above.<br>
-Requires third-party module `rich` which is installed automatically.
+No requirements other than the module itself.
 ```py
 pip install pysubcipher
 ```
 ```py
 python3 -m pip install pysubcipher
 ```
 # Example Usage
```

### Comparing `pysubcipher-2.3.2/pyproject.toml` & `pysubcipher-2.3.3/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["hatchling", "rich"]
+requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pysubcipher"
-version = "2.3.2"
+version = "2.3.3"
 authors = [
   {name = "mxngo", email = ""}
 ]
 description = "pysubcipher allows for simple encryption and decryption of text using a basic substitution cipher algorithm."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pysubcipher-2.3.2/PKG-INFO` & `pysubcipher-2.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysubcipher
-Version: 2.3.2
+Version: 2.3.3
 Summary: pysubcipher allows for simple encryption and decryption of text using a basic substitution cipher algorithm.
 Author: mxngo
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -18,15 +18,15 @@
 
 [PyPiVersion]: https://img.shields.io/pypi/v/pysubcipher
 [SupportedVersions]: https://img.shields.io/badge/python-3.10%20%7C%203.11-orange
 [License]: https://img.shields.io/badge/license-MIT-yellow
 
 # Installation
 Built and tested on Python 3.10 and above.<br>
-Requires third-party module `rich` which is installed automatically.
+No requirements other than the module itself.
 ```py
 pip install pysubcipher
 ```
 ```py
 python3 -m pip install pysubcipher
 ```
 # Example Usage
```

