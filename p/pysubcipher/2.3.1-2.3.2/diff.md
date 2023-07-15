# Comparing `tmp/pysubcipher-2.3.1.tar.gz` & `tmp/pysubcipher-2.3.2.tar.gz`

## Comparing `pysubcipher-2.3.1.tar` & `pysubcipher-2.3.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pysubcipher-2.3.1/src/pysubcipher/__init__.py
--rw-r--r--   0        0        0    12651 2020-02-02 00:00:00.000000 pysubcipher-2.3.1/src/pysubcipher/pysubcipher.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pysubcipher-2.3.1/LICENSE
--rw-r--r--   0        0        0     8678 2020-02-02 00:00:00.000000 pysubcipher-2.3.1/README.md
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pysubcipher-2.3.1/pyproject.toml
--rw-r--r--   0        0        0     8929 2020-02-02 00:00:00.000000 pysubcipher-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 pysubcipher-2.3.2/src/pysubcipher/__init__.py
+-rw-r--r--   0        0        0    12715 2020-02-02 00:00:00.000000 pysubcipher-2.3.2/src/pysubcipher/pysubcipher.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pysubcipher-2.3.2/LICENSE
+-rw-r--r--   0        0        0     8542 2020-02-02 00:00:00.000000 pysubcipher-2.3.2/README.md
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 pysubcipher-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0     8796 2020-02-02 00:00:00.000000 pysubcipher-2.3.2/PKG-INFO
```

### Comparing `pysubcipher-2.3.1/src/pysubcipher/__init__.py` & `pysubcipher-2.3.2/src/pysubcipher/__init__.py`

 * *Files identical despite different names*

### Comparing `pysubcipher-2.3.1/src/pysubcipher/pysubcipher.py` & `pysubcipher-2.3.2/src/pysubcipher/pysubcipher.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 import os
 
 from .__init__ import HEXDIGITS, PRINTABLE
 
 from typing import Any
 from types import TracebackType
 
+from rich.traceback import install
+install()
+
 class InvalidCharacterError(ValueError):
     def __init__(self, character: str, /) -> None:
         """Raised if an invalid token is present within a string of text while encrypting or decrypting a value.
 
         Args:
             character (str): The invalid character.
         """
@@ -88,14 +91,15 @@
         self.__min_key_length: int = min_key_length
         self.__max_key_length: int = max_key_length
         self.__charset: str = charset
         self.__current_seed: int | float | str | bytes | bytearray | None = seed
         if not isinstance(charset, str):
             raise TypeError(f"Parameter charset cannot be of type {type(charset)}")
         super().__init__(min_key_length, max_key_length, seed = seed, charset = self.__charset)
+
     def encrypt(self, s: str, /) -> bytes:
         """Encrypts a string of text using pre-defined cipher keys.
 
         Args:
             s (str): The string to encrypt.
 
         Raises:
@@ -107,14 +111,15 @@
         __encrypted_string: io.StringIO = io.StringIO()
         for character in s:
             character = base64.b64encode(character.encode().hex().encode())
             if character not in self._encryption_keys:
                 raise InvalidCharacterError(bytearray.fromhex(base64.b64decode(character).decode()).decode()) 
             __encrypted_string.write(self._encryption_keys.get(character))
         return __encrypted_string.getvalue().encode()
+    
     def decrypt(self, s: bytes, /) -> bytes:
         """Decrypts a string of text using pre-defined cipher keys.
 
         Args:
             s (bytes): The string to decrypt.
 
         Raises:
@@ -134,60 +139,64 @@
                     __decrypted_string.write(bytearray.fromhex(base64.b64decode(self._decryption_keys[k].decode()).decode()).decode())
                     s = s[len(k):]
                     __match = True
                     break
             if not __match:
                 raise EncryptedStringInvalidError(s.decode())
         return __decrypted_string.getvalue().encode()
+    
     def set_seed(self, seed: int | float | str | bytes | bytearray | None, /) -> None:
         """Sets the random seed for cipher keys to be generated with.
 
         Args:
             seed (int | float | str | bytes | bytearray | None): The seed to override.
         """
         self.__current_seed = seed
         super().__init__(self.__min_key_length, self.__max_key_length, seed = seed, charset = self.__charset)
+
     def regenerate_keys(self, seed: int | float | str | bytes | bytearray | None = os.urandom(1024), /) -> None:
         """Regenerates encryption and decryption keys.
 
         Args:
             seed (int | float | str | bytes | bytearray | None, optional): The seed to generate cipher keys with. Defaults to os.urandom(1024).
         """
         self.set_seed(seed)
+
     def __test_keys(self, encryption_keys: Any, decryption_keys: Any) -> bool:
         """Tests and validates cipher keys.
 
         Args:
             encryption_keys (Any): The encryption keys to validate.
             decryption_keys (Any): The decryption keys to validate.
 
         Returns:
             bool: Returns True if cipher keys are valid, and False if not.
         """
-        text = string.printable
         cipher = SubstitutionCipher()
         cipher._encryption_keys = encryption_keys
         cipher._decryption_keys = decryption_keys
-        encrypted_text = cipher.encrypt(text)
+        encrypted_text = cipher.encrypt(PRINTABLE)
         decrypted_text = cipher.decrypt(encrypted_text)
-        if decrypted_text.decode() != text:
+        if decrypted_text.decode() != PRINTABLE:
             return False
         return True
+    
     def save_keys(self, file: str, /, *, truncate: bool = False) -> None:
         """Saves the current cipher keys to a file.
 
         Args:
             file (str): The filepath.
             truncate (bool, optional): If True, file will be truncated prematurely before storing the keys. Defaults to False.
         """
         self.__current_seed = None
         with open(file, "wb") as f:
             if truncate:
                 f.truncate(0)
             f.write(pickle.dumps([self._encryption_keys, self._decryption_keys]))
+
     def load_keys(self, file: str, /) -> None:
         """Loads cipher keys into the current instance.
 
         Args:
             file (str): The path to the file where the keys are stored.
 
         Raises:
@@ -234,14 +243,15 @@
             charset (str, optional): The character set that cipher keys will be generated with. Defaults to HEXDIGITS.
         """
         self.__min_key_length: int = min_key_length
         self.__max_key_length: int = max_key_length
         self.__seed: int | float | str | bytes | bytearray | None = seed
         self.__charset: str = charset
         super().__init__(self.__min_key_length, self.__max_key_length, seed = self.__seed, charset = self.__charset)
+
     def encrypt(self, filepath: str, /, *, write: bool = False) -> bytes | None:
         """Encrypts the contents of a file and returns the encrypted contents.
 
         Args:
             filepath (str): The path to the file that will be encrypted.
             write (bool, optional): Override the file's contents. Defaults to False.
 
@@ -251,14 +261,15 @@
         encrypted_contents: bytes = super().encrypt(open(filepath).read())
         if write:
             with open(filepath, "wb") as file:
                 file.truncate(0)
                 file.write(encrypted_contents)
         else:
             return encrypted_contents
+        
     def decrypt(self, filepath: str, /, *, write: bool = False) -> bytes | None:
         """Decrypts the contents of a file and returns the decrypted contents.
 
         Args:
             filepath (str): The path to the file that will be decrypted.
             write (bool, optional): Override the file's contents. Defaults to False.
```

### Comparing `pysubcipher-2.3.1/LICENSE` & `pysubcipher-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysubcipher-2.3.1/README.md` & `pysubcipher-2.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 ![PyPiVersion]
 ![SupportedVersions]
 ![License]
 
 [PyPiVersion]: https://img.shields.io/pypi/v/pysubcipher
-[SupportedVersions]: https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-orange
+[SupportedVersions]: https://img.shields.io/badge/python-3.10%20%7C%203.11-orange
 [License]: https://img.shields.io/badge/license-MIT-yellow
 
-`pysubcipher` is a python module built on `Python 3.10` which allows users to encrypt and decrypt strings of text using a substitution cipher algorithm.
-
 # Installation
-Tested on Python 3.9 and above.<br>
-No requirements apart from the standard module.
+Built and tested on Python 3.10 and above.<br>
+Requires third-party module `rich` which is installed automatically.
 ```py
 pip install pysubcipher
 ```
 ```py
 python3 -m pip install pysubcipher
 ```
 # Example Usage
```

### Comparing `pysubcipher-2.3.1/pyproject.toml` & `pysubcipher-2.3.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "rich"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pysubcipher"
-version = "2.3.1"
+version = "2.3.2"
 authors = [
   {name = "mxngo", email = ""}
 ]
 description = "pysubcipher allows for simple encryption and decryption of text using a basic substitution cipher algorithm."
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Topic :: Security :: Cryptography",
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent"
 ]
```

### Comparing `pysubcipher-2.3.1/PKG-INFO` & `pysubcipher-2.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: pysubcipher
-Version: 2.3.1
+Version: 2.3.2
 Summary: pysubcipher allows for simple encryption and decryption of text using a basic substitution cipher algorithm.
 Author: mxngo
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security :: Cryptography
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 ![PyPiVersion]
 ![SupportedVersions]
 ![License]
 
 [PyPiVersion]: https://img.shields.io/pypi/v/pysubcipher
-[SupportedVersions]: https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-orange
+[SupportedVersions]: https://img.shields.io/badge/python-3.10%20%7C%203.11-orange
 [License]: https://img.shields.io/badge/license-MIT-yellow
 
-`pysubcipher` is a python module built on `Python 3.10` which allows users to encrypt and decrypt strings of text using a substitution cipher algorithm.
-
 # Installation
-Tested on Python 3.9 and above.<br>
-No requirements apart from the standard module.
+Built and tested on Python 3.10 and above.<br>
+Requires third-party module `rich` which is installed automatically.
 ```py
 pip install pysubcipher
 ```
 ```py
 python3 -m pip install pysubcipher
 ```
 # Example Usage
```

