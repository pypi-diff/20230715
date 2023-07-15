# Comparing `tmp/yt_idefix-2.2.1.tar.gz` & `tmp/yt_idefix-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt_idefix-2.2.1.tar", last modified: Wed Jun 21 06:41:50 2023, max compression
+gzip compressed data, was "yt_idefix-2.3.0.tar", last modified: Sat Jul 15 16:54:22 2023, max compression
```

## Comparing `yt_idefix-2.2.1.tar` & `yt_idefix-2.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:41:50.596519 yt_idefix-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-21 06:41:50.596519 yt_idefix-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 06:41:50.596519 yt_idefix-2.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:41:50.592519 yt_idefix-2.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:41:50.592519 yt_idefix-2.2.1/src/yt_idefix/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:41:50.596519 yt_idefix-2.2.1/src/yt_idefix/_io/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/_io/C_io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/_io/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/_io/dmp_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/_io/h5_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/_io/vtk_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    34740 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 06:41:39.000000 yt_idefix-2.2.1/src/yt_idefix/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:41:50.592519 yt_idefix-2.2.1/src/yt_idefix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-21 06:41:50.000000 yt_idefix-2.2.1/src/yt_idefix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-21 06:41:50.000000 yt_idefix-2.2.1/src/yt_idefix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 06:41:50.000000 yt_idefix-2.2.1/src/yt_idefix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-21 06:41:50.000000 yt_idefix-2.2.1/src/yt_idefix.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 06:41:50.000000 yt_idefix-2.2.1/src/yt_idefix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 06:41:50.000000 yt_idefix-2.2.1/src/yt_idefix.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 06:41:50.596519 yt_idefix-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-21 06:41:40.000000 yt_idefix-2.2.1/tests/test_C_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-21 06:41:40.000000 yt_idefix-2.2.1/tests/test_dmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-21 06:41:40.000000 yt_idefix-2.2.1/tests/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-06-21 06:41:40.000000 yt_idefix-2.2.1/tests/test_vtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-21 06:41:40.000000 yt_idefix-2.2.1/tests/test_xdmf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:54:22.634822 yt_idefix-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-15 16:54:22.634822 yt_idefix-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 16:54:22.634822 yt_idefix-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:54:22.630823 yt_idefix-2.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:54:22.634822 yt_idefix-2.3.0/src/yt_idefix/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:54:22.634822 yt_idefix-2.3.0/src/yt_idefix/_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/_io/C_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/_io/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/_io/dmp_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/_io/h5_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/_io/vtk_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34819 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 16:54:10.000000 yt_idefix-2.3.0/src/yt_idefix/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:54:22.634822 yt_idefix-2.3.0/src/yt_idefix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-15 16:54:22.000000 yt_idefix-2.3.0/src/yt_idefix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-15 16:54:22.000000 yt_idefix-2.3.0/src/yt_idefix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 16:54:22.000000 yt_idefix-2.3.0/src/yt_idefix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-15 16:54:22.000000 yt_idefix-2.3.0/src/yt_idefix.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-15 16:54:22.000000 yt_idefix-2.3.0/src/yt_idefix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-15 16:54:22.000000 yt_idefix-2.3.0/src/yt_idefix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:54:22.634822 yt_idefix-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-15 16:54:11.000000 yt_idefix-2.3.0/tests/test_C_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-15 16:54:11.000000 yt_idefix-2.3.0/tests/test_dmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-15 16:54:11.000000 yt_idefix-2.3.0/tests/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-07-15 16:54:11.000000 yt_idefix-2.3.0/tests/test_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-15 16:54:11.000000 yt_idefix-2.3.0/tests/test_xdmf.py
```

### Comparing `yt_idefix-2.2.1/LICENSE` & `yt_idefix-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.1/PKG-INFO` & `yt_idefix-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt_idefix
-Version: 2.2.1
+Version: 2.3.0
 Summary: An extension module for yt, adding a frontend for Idefix and Pluto
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Documentation, https://yt-project.org/docs/dev/
 Project-URL: Source, https://github.com/neutrinoceros/yt_idefix
 Project-URL: Tracker, https://github.com/neutrinoceros/yt_idefix/issues
```

### Comparing `yt_idefix-2.2.1/README.md` & `yt_idefix-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.1/pyproject.toml` & `yt_idefix-2.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     "astronomy astrophysics visualization amr adaptivemeshrefinement",
 ]
 requires-python = ">=3.8"
 dependencies = [
     "inifix>=4.1.0",
     "numpy>=1.17.3",
     "yt>=4.2.0",
+    "typing-extensions>=4.1.0 ; python_version < '3.11'"
 ]
 dynamic = ["version"]
 
 [tool.setuptools.dynamic]
 version = {attr = "yt_idefix.__version__"}
 
 [project.optional-dependencies]
@@ -82,14 +83,15 @@
     "*/api.py",
     "*/__init__.py",
 ]
 select = [
     "E",
     "F",
     "W",
+    "ARG",  # flake8-unused-arguments
     "C4",   # flake8-comprehensions
     "B",    # flake8-bugbear
     "G",    # flake8-logging-format
     "YTT",  # flake8-2020
     "UP",   # pyupgrade
     "I",    # isort
 ]
```

### Comparing `yt_idefix-2.2.1/src/yt_idefix/_backports.py` & `yt_idefix-2.3.0/src/yt_idefix/_backports.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.1/src/yt_idefix/_io/commons.py` & `yt_idefix-2.3.0/src/yt_idefix/_io/commons.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.1/src/yt_idefix/_io/dmp_io.py` & `yt_idefix-2.3.0/src/yt_idefix/_io/dmp_io.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,294 +1,413 @@
 from __future__ import annotations
 
 import re
 import struct
+import sys
+import warnings
 from enum import IntEnum
 from typing import BinaryIO, Literal, cast, overload
 
 import numpy as np
 
 from .commons import Dim, IdefixFieldProperties, IdefixMetadata, Prec
 
+if sys.version_info >= (3, 11):
+    from typing import assert_never
+else:
+    from typing_extensions import assert_never
+
+
 KNOWN_GEOMETRIES: dict[int, str] = {
     1: "cartesian",
     2: "cylindrical",
     3: "polar",
     4: "spherical",
 }
 
 
 class CharCount(IntEnum):
     # hardcoded in idefix
     HEADER = 128
     NAME = 16
 
 
+HEADER_REGEXP = re.compile(
+    r"Idefix (?P<version>[\w\.-]+) Dump Data" r"((?P<byteorder>(little|big)) endian)?"
+)
+
+ByteOrder = Literal["little", "big", "native"]
+
+
+def parse_byteorder(fh: BinaryIO) -> ByteOrder:
+    header = read_header(fh)
+    match = HEADER_REGEXP.match(header)
+    if match is None:
+        warnings.warn(
+            f"failed to parse dump header {header!r}",
+            stacklevel=2,
+            category=RuntimeWarning,
+        )
+        return "native"
+
+    if (res := match.group("byteorder")) in ("little", "big"):
+        return cast(Literal["little", "big"], res)
+    else:
+        # early versions of Idefix didn't include byteorder in dump headers,
+        # fallback to native for backward compatibility
+        return "native"
+
+
+def byteorder2alignment(byteorder: ByteOrder) -> Literal["<", ">", "="]:
+    if byteorder == "little":
+        return "<"
+    elif byteorder == "big":
+        return ">"
+    elif byteorder == "native":
+        return "="
+    else:
+        assert_never(byteorder)
+
+
 # emulating C++
 # enum DataType {DoubleType, SingleType, IntegerType};
 DTYPES: dict[int, Prec] = {0: "d", 1: "f", 2: "i", 3: "?"}
-DTYPES_2_NUMPY: dict[Prec, str] = {"d": "=f8", "f": "=f4", "i": "=i4"}
+DTYPES_2_NUMPY: dict[Prec, str] = {"d": "f8", "f": "f4", "i": "i4"}
 
 
 def read_null_terminated_string(fh: BinaryIO, maxsize: int = CharCount.NAME) -> str:
     """Read maxsize bytes, but only parse non-null characters."""
     b = fh.read(maxsize)
     s = b.decode("utf-8", errors="backslashreplace")
     s = s.split("\x00", maxsplit=1)[0]
     return s
 
 
 def read_next_field_properties(
     fh: BinaryIO,
+    *,
+    byteorder: ByteOrder,
 ) -> tuple[str, Prec, Dim, np.ndarray]:
     """Emulate Idefix's OutputDump::ReadNextFieldProperty"""
     field_name = read_null_terminated_string(fh)
 
-    fmt = "=i"
+    alignment = byteorder2alignment(byteorder)
+
+    fmt = f"{alignment}i"
     int_dtype = struct.unpack(fmt, fh.read(struct.calcsize(fmt)))[0]
     dtype = DTYPES[int_dtype]
     ndim = struct.unpack(fmt, fh.read(struct.calcsize(fmt)))[0]
     if not isinstance(ndim, int):
         raise TypeError(ndim)
     if not (1 <= ndim <= 3):
         raise ValueError(ndim)
     ndim = cast(Dim, ndim)
-    fmt = f"={ndim}i"
+    fmt = f"{alignment}{ndim}i"
     dim = np.array(struct.unpack(fmt, fh.read(struct.calcsize(fmt))))
     return field_name, dtype, ndim, dim
 
 
 @overload
 def read_chunk(
     fh: BinaryIO,
     ndim: int,
     dim: list[int],
     dtype: str,
     *,
+    byteorder: ByteOrder,
     is_scalar: bool,
     skip_data: Literal[True],
 ) -> None:
     ...
 
 
 @overload
 def read_chunk(
     fh: BinaryIO,
     ndim: int,
     dim: list[int],
     dtype: str,
     *,
+    byteorder: ByteOrder,
     is_scalar: Literal[True],
     skip_data: Literal[False],
 ) -> float:
     ...
 
 
 @overload
 def read_chunk(
     fh: BinaryIO,
     ndim: int,
     dim: list[int],
     dtype: str,
     *,
+    byteorder: ByteOrder,
     is_scalar: Literal[False],
     skip_data: Literal[False],
 ) -> np.ndarray:
     ...
 
 
 @overload
 def read_chunk(
     fh: BinaryIO,
     ndim: int,
     dim: list[int],
     dtype: str,
     *,
+    byteorder: ByteOrder,
     is_scalar: bool,
     skip_data: bool,
 ) -> float | np.ndarray | None:
     ...
 
 
 def read_chunk(
     fh,
     ndim,
     dim,
     dtype,
     *,
+    byteorder: ByteOrder,
     skip_data=False,
     is_scalar=False,
 ):
     # NOTE: ret type is only dependent on skip_data...
     # this could be better expressed in the type annotations but it would make
     # more sense to just refactor this function to avoid the boolean trap, so I'll keep wonky
     # type hints for now
     assert ndim == len(dim)
     count = np.prod(dim)
     size = count * np.dtype(dtype).itemsize
     if skip_data:
         fh.seek(size, 1)
         return None
 
+    alignment = byteorder2alignment(byteorder)
+
     # note: this reversal may not be desirable in general
     if is_scalar:
-        fmt = f"={count}{dtype}"
+        fmt = f"{alignment}{count}{dtype}"
         retv = struct.unpack(fmt, fh.read(size))[0]
         return retv
     else:
-        data = np.fromfile(fh, DTYPES_2_NUMPY[dtype], count=count)
+        data = np.fromfile(fh, alignment + DTYPES_2_NUMPY[dtype], count=count)
         data.shape = dim[::-1]
-        return data.T
+        return data.astype("=" + DTYPES_2_NUMPY[dtype], copy=False).T
 
 
 @overload
 def read_serial(
-    fh: BinaryIO, ndim: int, dim: np.ndarray, dtype: str, *, is_scalar: Literal[True]
+    fh: BinaryIO,
+    ndim: int,
+    dim: np.ndarray,
+    dtype: str,
+    *,
+    byteorder: ByteOrder,
+    is_scalar: Literal[True],
 ) -> float:
     ...
 
 
 @overload
 def read_serial(
-    fh: BinaryIO, ndim: int, dim: np.ndarray, dtype: str, *, is_scalar: Literal[False]
+    fh: BinaryIO,
+    ndim: int,
+    dim: np.ndarray,
+    dtype: str,
+    *,
+    byteorder: ByteOrder,
+    is_scalar: Literal[False],
 ) -> np.ndarray:
     ...
 
 
 @overload
 def read_serial(
-    fh: BinaryIO, ndim: int, dim: np.ndarray, dtype: str, *, is_scalar: bool = False
+    fh: BinaryIO,
+    ndim: int,
+    dim: np.ndarray,
+    dtype: str,
+    *,
+    byteorder: ByteOrder,
+    is_scalar: bool = False,
 ) -> float | np.ndarray:
     ...
 
 
-def read_serial(fh, ndim, dim, dtype, *, is_scalar=False):
+def read_serial(fh, ndim, dim, dtype, *, byteorder, is_scalar=False):
     """Emulate Idefix's OutputDump::ReadSerial"""
     assert ndim == 1  # corresponds to an error raised in IDEFIX
     return read_chunk(
-        fh, ndim=ndim, dim=dim, dtype=dtype, is_scalar=is_scalar, skip_data=False
+        fh,
+        ndim=ndim,
+        dim=dim,
+        dtype=dtype,
+        byteorder=byteorder,
+        is_scalar=is_scalar,
+        skip_data=False,
     )
 
 
 @overload
 def read_distributed(
-    fh: BinaryIO, dim: np.ndarray, *, dtype: str, skip_data: Literal[False]
+    fh: BinaryIO,
+    dim: np.ndarray,
+    *,
+    byteorder: ByteOrder,
+    dtype: str,
+    skip_data: Literal[False],
 ) -> np.ndarray:
     ...
 
 
 @overload
 def read_distributed(
-    fh: BinaryIO, dim: np.ndarray, *, dtype: str, skip_data: Literal[True]
+    fh: BinaryIO,
+    dim: np.ndarray,
+    *,
+    byteorder: ByteOrder,
+    dtype: str,
+    skip_data: Literal[True],
 ) -> None:
     ...
 
 
 @overload
 def read_distributed(
-    fh: BinaryIO, dim: np.ndarray, *, dtype: str, skip_data: bool = False
+    fh: BinaryIO,
+    dim: np.ndarray,
+    *,
+    byteorder: ByteOrder,
+    dtype: str,
+    skip_data: bool = False,
 ) -> np.ndarray | None:
     ...
 
 
-def read_distributed(fh, dim, *, dtype, skip_data):
+def read_distributed(fh, dim, *, byteorder, dtype, skip_data):
     """Emulate Idefix's OutputDump::ReadDistributed"""
     # note: OutputDump::ReadDistributed only reads doubles
     # because chunks written as integers are small enough
     # that parallelization is counter productive.
     # This a design choice on idefix's size.
-    return read_chunk(fh, ndim=len(dim), dim=dim, dtype=dtype, skip_data=skip_data)
+    return read_chunk(
+        fh,
+        ndim=len(dim),
+        dim=dim,
+        byteorder=byteorder,
+        dtype=dtype,
+        skip_data=skip_data,
+    )
 
 
 # The following functions are originally designed for yt
 
 
-def read_header(filename: str) -> str:
-    with open(filename, "rb") as fh:
-        header = read_null_terminated_string(fh, maxsize=CharCount.HEADER)
-    return header
+def read_header(source: str | BinaryIO, /) -> str:
+    if isinstance(source, str):
+        with open(source, "rb") as fh:
+            return read_header(fh)
+    else:
+        return read_null_terminated_string(source, maxsize=CharCount.HEADER)
 
 
 def get_field_offset_index(fh: BinaryIO) -> dict[str, int]:
     """
     Go over a dumpfile, parse bytes offsets associated with each field.
     Returns
     -------
     field_index: mapping (field name -> offset)
     """
     field_index = {}
 
-    # skip header
-    fh.seek(CharCount.HEADER)
+    fh.seek(0)
+    byteorder = parse_byteorder(fh)
+
     # skip grid properties
     for _ in range(9):
-        _field_name, dtype, ndim, dim = read_next_field_properties(fh)
-        read_serial(fh, ndim, dim, dtype)
+        _field_name, dtype, ndim, dim = read_next_field_properties(
+            fh, byteorder=byteorder
+        )
+        read_serial(fh, ndim, dim, dtype, byteorder=byteorder)
 
     while True:
         offset = fh.tell()
-        field_name, dtype, ndim, dim = read_next_field_properties(fh)
+        field_name, dtype, ndim, dim = read_next_field_properties(
+            fh, byteorder=byteorder
+        )
         if not re.match("^V[cs]-", field_name):
             break
         field_index[field_name] = offset
-        read_distributed(fh, dim, dtype=dtype, skip_data=True)
+        read_distributed(fh, dim, dtype=dtype, byteorder=byteorder, skip_data=True)
 
     return field_index
 
 
-def read_single_field(fh: BinaryIO, field_offset: int) -> np.ndarray:
+def read_single_field(
+    fh: BinaryIO, field_offset: int, *, byteorder: ByteOrder
+) -> np.ndarray:
     """
     Returns
     -------
     data: 3D np.ndarray with dtype float64
     """
     fh.seek(field_offset)
-    field_name, dtype, ndim, dim = read_next_field_properties(fh)
-    data = read_distributed(fh, dim, dtype=dtype, skip_data=False)
+    field_name, dtype, ndim, dim = read_next_field_properties(fh, byteorder=byteorder)
+    data = read_distributed(fh, dim, dtype=dtype, byteorder=byteorder, skip_data=False)
     return data
 
 
 def read_idefix_dmpfile(
     filename: str, skip_data: bool = False
 ) -> tuple[IdefixFieldProperties, IdefixMetadata]:
     with open(filename, "rb") as fh:
         return read_idefix_dump_from_buffer(fh, skip_data)
 
 
 def read_idefix_dump_from_buffer(
     fh: BinaryIO, skip_data: bool = False
 ) -> tuple[IdefixFieldProperties, IdefixMetadata]:
-    # skip header
-    fh.seek(CharCount.HEADER)
+    fh.seek(0)
+    byteorder = parse_byteorder(fh)
 
     data: float | np.ndarray | None
     fprops: IdefixFieldProperties = {}
     fdata: IdefixMetadata = {}
     for _ in range(9):
         # read grid properties
         # (cell centers, left and right edges in 3D -> 9 arrays)
-        field_name, dtype, ndim, dim = read_next_field_properties(fh)
-        data = read_serial(fh, ndim, dim, dtype)
+        field_name, dtype, ndim, dim = read_next_field_properties(
+            fh, byteorder=byteorder
+        )
+        data = read_serial(fh, ndim, dim, dtype, byteorder=byteorder)
         fprops[field_name] = dtype, ndim, dim
         fdata[field_name] = data
 
-    field_name, dtype, ndim, dim = read_next_field_properties(fh)
+    field_name, dtype, ndim, dim = read_next_field_properties(fh, byteorder=byteorder)
     while field_name != "eof":
         # note that this could likely be implemented using a call to
         # `iter` with a sentinel value, to the condition that read_next_field_properties
         # would be splitted into 2 parts (I don't the sentinel pattern works with tuples)
         fprops[field_name] = dtype, ndim, dim
         if field_name.startswith(("Vc-", "Vs-")):
-            data = read_distributed(fh, dim, dtype=dtype, skip_data=skip_data)
+            data = read_distributed(
+                fh, dim, dtype=dtype, byteorder=byteorder, skip_data=skip_data
+            )
         else:
             is_scalar = ndim == 1 and dim[0] == 1
             is_scalar &= field_name not in ("x1", "x2", "x3")
-            data = read_serial(fh, ndim, dim, dtype, is_scalar=is_scalar)
+            data = read_serial(
+                fh, ndim, dim, dtype, byteorder=byteorder, is_scalar=is_scalar
+            )
         fdata[field_name] = data
-        field_name, dtype, ndim, dim = read_next_field_properties(fh)
+        field_name, dtype, ndim, dim = read_next_field_properties(
+            fh, byteorder=byteorder
+        )
 
     if isinstance(fdata["geometry"], int):
         fdata["geometry"] = KNOWN_GEOMETRIES[fdata["geometry"]]
     else:
         raise RuntimeError(
             f"Got a geometry flag with unexpected type {type(fdata['geometry'])}; "
             f"got {fdata['geometry']}"
```

### Comparing `yt_idefix-2.2.1/src/yt_idefix/_io/h5_io.py` & `yt_idefix-2.3.0/src/yt_idefix/_io/h5_io.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,62 +24,58 @@
     # Return cell edges coordinates
     fh = h5py.File(filename, "r")
     if geometry not in (valid_geometries := tuple(KNOWN_GEOMETRIES.values())):
         raise ValueError(
             f"Got unknown geometry {geometry!r}, expected one of {valid_geometries}"
         )
 
-    nodesX = fh["/node_coords/X"].astype("=f8")
-    nodesY = fh["/node_coords/Y"].astype("=f8")
-    nodesZ = fh["/node_coords/Z"].astype("=f8")
-    dimensions = len(np.array(nodesX).shape)
-    shape = Shape(
-        *np.array(nodesX).shape
-    )  # this is reversed compared the vtk implementation in vtk_io.py
+    nodesX = np.array(fh["/node_coords/X"]).astype("=f8", copy=False)
+    nodesY = np.array(fh["/node_coords/Y"]).astype("=f8", copy=False)
+    nodesZ = np.array(fh["/node_coords/Z"]).astype("=f8", copy=False)
+
+    # this is reversed compared the vtk implementation in vtk_io.py
+    shape = Shape(*(nodesX.shape))
     coords: list[np.ndarray] = []
     # now assuming that fh is positioned at the end of metadata
     if geometry in ("cartesian", "cylindrical") or (
-        geometry in ("polar", "spherical") and dimensions == 1
+        geometry in ("polar", "spherical") and nodesX.ndim == 1
     ):
-        if dimensions == 1:
-            nodesX = np.array(nodesX)
+        if nodesX.ndim == 1:
             # Default is assumed and not parsed from pluto.ini/grid.out (not present in data)
             nodesY = np.array([0.0, 1.0])
             nodesZ = np.array([0.0, 1.0])
             if geometry == "spherical":
-                if np.fabs(np.max(nodesX) - np.min(nodesX)) < 1e-8:
-                    nodesX = fh["/cell_coords/X"].astype("=f8")
-                    nodesX = np.hstack(([nodesX[1] - nodesX[0]], np.array(nodesX)))
-                    nodesX = np.array(nodesX) / np.sin(0.5)
+                if np.fabs(np.ptp(nodesX)) < 1e-8:
+                    nodesX = np.hstack(([nodesX[1] - nodesX[0]], nodesX))
+                    nodesX /= np.sin(0.5)
             elif geometry == "polar":
-                if np.fabs(np.max(nodesX) - np.min(nodesX)) < 1e-8:
-                    nodesX = fh["/cell_coords/X"].astype("=f8")
-                    nodesX = np.hstack(([nodesX[1] - nodesX[0]], np.array(nodesX)))
-                    nodesX = np.array(nodesX) / np.cos(0.5)
+                if np.fabs(np.ptp(nodesX)) < 1e-8:
+                    nodesX = np.hstack(([nodesX[1] - nodesX[0]], nodesX))
+                    nodesX /= np.cos(0.5)
             array_shape = Shape(shape[0], 1, 1).to_cell_centered()
-        elif dimensions == 2:
-            nodesX = np.array(nodesX[0, :])
-            nodesY = np.array(nodesY[:, 0])
+        elif nodesX.ndim == 2:
+            nodesX = nodesX[0, :]
+            nodesY = nodesY[:, 0]
             # Default is assumed and not parsed from pluto.ini/grid.out (not present in data)
             if geometry == "cartesian":
                 nodesZ = np.array([0.0, 1.0])
             else:
                 nodesZ = np.array([0.0, 2 * np.pi])
             array_shape = Shape(*reversed(shape[:-1])).to_cell_centered()
         else:
-            nodesX = np.array(nodesX)[0, 0, :]
-            nodesY = np.array(nodesY)[0, :, 0]
-            nodesZ = np.array(nodesZ)[:, 0, 0]
+            nodesX = nodesX[0, 0, :]
+            nodesY = nodesY[0, :, 0]
+            nodesZ = nodesZ[:, 0, 0]
             array_shape = Shape(*reversed(shape)).to_cell_centered()
         coords = [nodesX, nodesY, nodesZ]
-    elif geometry in ("polar", "spherical") and dimensions > 1:
-        if dimensions == 2:
-            nodesX = np.array([nodesX])
-            nodesY = np.array([nodesY])
-            nodesZ = np.array([nodesZ])
+    elif geometry in ("polar", "spherical") and nodesX.ndim > 1:
+        if nodesX.ndim == 2:
+            nodesX = np.expand_dims(nodesX, axis=0)
+            nodesY = np.expand_dims(nodesY, axis=0)
+            nodesZ = np.expand_dims(nodesZ, axis=0)
             array_shape = Shape(*reversed(shape[:-1])).to_cell_centered()
         else:
             array_shape = Shape(*reversed(shape)).to_cell_centered()
 
         xcart = np.transpose(nodesX, axes=(2, 1, 0))
         ycart = np.transpose(nodesY, axes=(2, 1, 0))
         zcart = np.transpose(nodesZ, axes=(2, 1, 0))
```

### Comparing `yt_idefix-2.2.1/src/yt_idefix/_io/vtk_io.py` & `yt_idefix-2.3.0/src/yt_idefix/_io/vtk_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.1/src/yt_idefix/data_structures.py` & `yt_idefix-2.3.0/src/yt_idefix/data_structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,15 @@
     _default_definitions_header: str
     _version_regexp: re.Pattern
 
     def __init__(
         self,
         filename,
         *,
-        dataset_type: str | None = None,  # deleguated to child classes
+        dataset_type: str | None = None,  # deleguated to child classes # NOQA: ARG002
         units_override: dict[str, str] | None = None,
         unit_system: Literal["cgs", "mks", "code"] = "cgs",
         default_species_fields: Literal["neutral", "ionized"] | None = None,
         # from here, frontend-specific arguments
         geometry: Literal["cartesian", "spherical", "cylindrical", "polar"]
         | None = None,
         inifile: str | os.PathLike[str] | None = None,
@@ -762,15 +762,15 @@
 
 class IdefixDmpDataset(IdefixDataset):
     _dataset_type = "idefix-dmp"
     _index_class = IdefixDmpHierarchy
     _field_info_class = IdefixDmpFields
 
     @classmethod
-    def _is_valid(cls, filename: str, *args, **kwargs) -> bool:
+    def _is_valid(cls, filename: str, *args, **kwargs) -> bool:  # NOQA: ARG003
         try:
             header_string = dmp_io.read_header(filename)
             return re.match(r"Idefix .* Dump Data", header_string) is not None
         except Exception:
             return False
 
     def _get_fields_metadata(self) -> tuple[IdefixFieldProperties, IdefixMetadata]:
@@ -809,28 +809,28 @@
 
 
 class IdefixVtkDataset(VtkMixin, IdefixDataset):
     _dataset_type = "idefix-vtk"
     _field_info_class = IdefixVtkFields
 
     @classmethod
-    def _is_valid(cls, filename: str, *args, **kwargs) -> bool:
+    def _is_valid(cls, filename: str, *args, **kwargs) -> bool:  # NOQA: ARG003
         try:
             header = vtk_io.read_header(filename)
         except Exception:
             return False
         else:
             return "Idefix" in header
 
 
 class PlutoVtkDataset(VtkMixin, StaticPlutoDataset):
     _dataset_type = "pluto-vtk"
 
     @classmethod
-    def _is_valid(cls, filename: str, *args, **kwargs) -> bool:
+    def _is_valid(cls, filename: str, *args, **kwargs) -> bool:  # NOQA: ARG003
         try:
             header = vtk_io.read_header(filename)
         except Exception:
             return False
         else:
             return "PLUTO" in header
 
@@ -911,15 +911,15 @@
 
         if (res := re.match(r"(#.*\n)+", body)) is not None:
             return res.group()
         else:
             return ""
 
     @classmethod
-    def _is_valid(cls, filename: str, *args, **kwargs) -> bool:
+    def _is_valid(cls, filename: str, *args, **kwargs) -> bool:  # NOQA: ARG003
         if not (
             filename.endswith((".dbl.h5", ".flt.h5"))
             and os.path.isfile(removesuffix(filename, ".h5") + ".xmf")
             and os.path.isfile(
                 os.path.join(
                     os.path.dirname(filename), os.path.basename(filename[-6:]) + ".out"
                 )
```

### Comparing `yt_idefix-2.2.1/src/yt_idefix/definitions.py` & `yt_idefix-2.3.0/src/yt_idefix/definitions.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.1/src/yt_idefix/fields.py` & `yt_idefix-2.3.0/src/yt_idefix/fields.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.1/src/yt_idefix/io.py` & `yt_idefix-2.3.0/src/yt_idefix/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,16 +66,20 @@
         # idefix doesn't have particles (yet)
         raise NotImplementedError("Particles are not currently supported for Idefix")
 
 
 class IdefixDmpIO(SingleGridIO, BaseParticleIOHandler):
     _dataset_type = "idefix-dmp"
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._byteorder = dmp_io.parse_byteorder(self.ds.filename)
+
     def _read_single_field(self, fh: BinaryIO, offset: int) -> np.ndarray:
-        return dmp_io.read_single_field(fh, offset)
+        return dmp_io.read_single_field(fh, offset, byteorder=self._byteorder)
 
     def _read_particle_coords(self, chunks, ptf):
         # This needs to *yield* a series of tuples of (ptype, (x, y, z)).
         # chunks is a list of chunks, and ptf is a dict where the keys are
         # ptypes and the values are lists of fields.
         raise NotImplementedError("Particles are not currently supported for Idefix")
```

### Comparing `yt_idefix-2.2.1/src/yt_idefix.egg-info/PKG-INFO` & `yt_idefix-2.3.0/src/yt_idefix.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-idefix
-Version: 2.2.1
+Version: 2.3.0
 Summary: An extension module for yt, adding a frontend for Idefix and Pluto
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://yt-project.org/
 Project-URL: Documentation, https://yt-project.org/docs/dev/
 Project-URL: Source, https://github.com/neutrinoceros/yt_idefix
 Project-URL: Tracker, https://github.com/neutrinoceros/yt_idefix/issues
```

### Comparing `yt_idefix-2.2.1/src/yt_idefix.egg-info/SOURCES.txt` & `yt_idefix-2.3.0/src/yt_idefix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.1/tests/test_C_io.py` & `yt_idefix-2.3.0/tests/test_C_io.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.1/tests/test_dmp.py` & `yt_idefix-2.3.0/tests/test_dmp.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.1/tests/test_loading.py` & `yt_idefix-2.3.0/tests/test_loading.py`

 * *Files identical despite different names*

### Comparing `yt_idefix-2.2.1/tests/test_vtk.py` & `yt_idefix-2.3.0/tests/test_vtk.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
 
 def test_derived_field(vtk_file):
     file = vtk_file
     ds = yt.load(file["path"], geometry=file["geometry"])
     # this derived field is compatible for all current test data
     # it'll be replaced once a better universal field is defined internally.
 
-    def mom_den(field, data):
+    def mom_den(field, data):  # NOQA: ARG001
         return data["RHO"] * data["VX1"]
 
     ds.add_field(
         name=("gas", "momentum_density"),
         function=mom_den,
         units="g*cm**-2/s",
         sampling_type="cell",
```

### Comparing `yt_idefix-2.2.1/tests/test_xdmf.py` & `yt_idefix-2.3.0/tests/test_xdmf.py`

 * *Files identical despite different names*

