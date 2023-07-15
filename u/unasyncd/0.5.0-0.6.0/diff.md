# Comparing `tmp/unasyncd-0.5.0.tar.gz` & `tmp/unasyncd-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unasyncd-0.5.0.tar", max compression
+gzip compressed data, was "unasyncd-0.6.0.tar", max compression
```

## Comparing `unasyncd-0.5.0.tar` & `unasyncd-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-07-12 13:56:51.676885 unasyncd-0.5.0/LICENSE
--rw-r--r--   0        0        0    17844 2023-07-12 13:56:51.676885 unasyncd-0.5.0/README.md
--rw-r--r--   0        0        0      995 2023-07-12 13:56:51.676885 unasyncd-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-12 13:56:51.676885 unasyncd-0.5.0/unasyncd/__init__.py
--rw-r--r--   0        0        0     4115 2023-07-12 13:56:51.676885 unasyncd-0.5.0/unasyncd/cli.py
--rw-r--r--   0        0        0     2553 2023-07-12 13:56:51.680885 unasyncd-0.5.0/unasyncd/config.py
--rw-r--r--   0        0        0    10349 2023-07-12 13:56:51.680885 unasyncd-0.5.0/unasyncd/main.py
--rw-r--r--   0        0        0    40332 2023-07-12 13:56:51.680885 unasyncd-0.5.0/unasyncd/transformers.py
--rw-r--r--   0        0        0    18713 1970-01-01 00:00:00.000000 unasyncd-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-15 09:18:47.816374 unasyncd-0.6.0/LICENSE
+-rw-r--r--   0        0        0    18033 2023-07-15 09:18:47.816374 unasyncd-0.6.0/README.md
+-rw-r--r--   0        0        0     1058 2023-07-15 09:18:47.816374 unasyncd-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-15 09:18:47.816374 unasyncd-0.6.0/unasyncd/__init__.py
+-rw-r--r--   0        0        0      183 2023-07-15 09:18:47.816374 unasyncd-0.6.0/unasyncd/_version.py
+-rw-r--r--   0        0        0     4089 2023-07-15 09:18:47.816374 unasyncd-0.6.0/unasyncd/cli.py
+-rw-r--r--   0        0        0     2603 2023-07-15 09:18:47.816374 unasyncd-0.6.0/unasyncd/config.py
+-rw-r--r--   0        0        0    10349 2023-07-15 09:18:47.816374 unasyncd-0.6.0/unasyncd/main.py
+-rw-r--r--   0        0        0    40366 2023-07-15 09:18:47.816374 unasyncd-0.6.0/unasyncd/transformers.py
+-rw-r--r--   0        0        0    18979 1970-01-01 00:00:00.000000 unasyncd-0.6.0/PKG-INFO
```

### Comparing `unasyncd-0.5.0/LICENSE` & `unasyncd-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unasyncd-0.5.0/README.md` & `unasyncd-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Unasync
+# Unasyncd
 
 A tool to transform asynchronous Python code to synchronous Python code.
 
 ## Why?
 
 Unasyncd is largely inspired by [unasync](https://github.com/python-trio/unasync), and
 a detailed discussion about this approach can be found
@@ -42,28 +42,29 @@
 5. Transformation of constructs like `asyncio.TaskGroup` to a thread based equivalent
 
 *A full list of supported transformations is available below.*
 
 ## Table of contents
 
 <!-- TOC -->
-* [Unasync](#unasync)
+* [Unasyncd](#unasyncd)
   * [Why?](#why)
   * [Why unasyncd?](#why-unasyncd)
   * [Table of contents](#table-of-contents)
   * [What can be transformed?](#what-can-be-transformed)
     * [Asynchronous functions](#asynchronous-functions)
     * [`await`](#await)
     * [Asynchronous iterators, iterables and generators](#asynchronous-iterators-iterables-and-generators)
     * [Asynchronous iteration](#asynchronous-iteration)
     * [Asynchronous context managers](#asynchronous-context-managers)
     * [`contextlib.AsyncExitStack`](#contextlibasyncexitstack)
     * [`asyncio.TaskGroup`](#asynciotaskgroup)
     * [`anyio.create_task_group`](#anyiocreatetaskgroup)
     * [`asyncio.sleep` / `anyio.sleep`](#asynciosleep--anyiosleep)
+    * [`anyio.Path`](#anyiopath)
     * [Type annotations](#type-annotations)
     * [Docstrings](#docstrings)
   * [Usage](#usage)
     * [Installation](#installation)
     * [CLI](#cli)
     * [As a pre-commit hook](#as-a-pre-commit-hook)
     * [Configuration](#configuration)
@@ -347,14 +348,30 @@
 
 ```python
 import asyncio
 
 await asyncio.sleep(0)
 ```
 
+### `anyio.Path`
+
+*Async*
+```python
+import anyio
+
+await anyio.Path().read_bytes()
+```
+
+*Sync*
+```python
+import pathlib
+
+pathlib.Path().read_bytes()
+```
+
 ### Type annotations
 
 |                                   |                                    |
 |-----------------------------------|------------------------------------|
 | `typing.AsyncIterable[int]`       | `typing.Iterable[int]`             |
 | `typing.AsyncIterator[int]`       | `typing.Iterator[int]`             |
 | `typing.AsyncGenerator[int, str]` | `typing.Generator[int, str, None]` |
```

### Comparing `unasyncd-0.5.0/pyproject.toml` & `unasyncd-0.6.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unasyncd"
-version = "0.5.0"
+version = "0.6.0"
 description = "A tool to transform asynchronous Python code to synchronous Python code."
 authors = ["Janek Nouvertné <j.a.nouvertne@posteo.de>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -12,14 +12,16 @@
 click = "^8.1.3"
 rich = "^13.4.1"
 anyio = "^3.7.0"
 msgspec = "^0.17.0"
 tomli-w = "^1.0.0"
 rich-click = "^1.6.1"
 ruff = {version = "*", optional = true}
+importlib-metadata = { version = "^6.8.0", python = "<3.10" }
+
 
 [tool.poetry.extras]
 ruff = ["ruff"]
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
```

### Comparing `unasyncd-0.5.0/unasyncd/cli.py` & `unasyncd-0.6.0/unasyncd/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         f"[blue]{files_unchanged}[/] {'would be ' if check_only else ''}"
         "left unchanged"
     )
 
     return files_changed > 0
 
 
-@click.command()  # type: ignore[arg-type]
+@click.command()
 @click.option(
     "--cache/--no-cache",
     is_flag=True,
     help="Cache transformation results",
     default=None,
 )
 @click.option(
```

### Comparing `unasyncd-0.5.0/unasyncd/config.py` & `unasyncd-0.6.0/unasyncd/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 import hashlib
 import itertools
 from pathlib import Path
 from typing import Any
 
 import msgspec
 
+from ._version import VERSION
+
 
 class Config(msgspec.Struct):
     add_editors_note: bool
     transform_docstrings: bool
     cache: bool
     extra_replacements: dict[str, dict[str, str]]
     exclude: dict[str, list[str]]
     files: dict[str, str]
     force_regen: bool
     check_only: bool
     infer_type_checking_imports: bool
     ruff_fix: bool
 
     def key(self) -> str:
-        return hashlib.sha1(msgspec.json.encode(self)).hexdigest()
+        return hashlib.sha1(msgspec.json.encode(self) + VERSION.encode()).hexdigest()
 
 
 def _collect_paths(file_names: dict[str, str]) -> dict[str, str]:
     files = {}
     for source_name, target_name in file_names.items():
         source_path = Path(source_name)
         target_path = Path(target_name)
```

### Comparing `unasyncd-0.5.0/unasyncd/main.py` & `unasyncd-0.6.0/unasyncd/main.py`

 * *Files identical despite different names*

### Comparing `unasyncd-0.5.0/unasyncd/transformers.py` & `unasyncd-0.6.0/unasyncd/transformers.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     "StopAsyncIteration": "StopIteration",
     "contextlib.asynccontextmanager": "contextlib.contextmanager",
     "typing.AsyncIterable": "typing.Iterable",
     "typing.AsyncIterator": "typing.Iterator",
     "typing.AsyncGenerator": "typing.Generator",
     "asyncio.sleep": "time.sleep",
     "anyio.sleep": "time.sleep",
+    "anyio.Path": "pathlib.Path",
 }
 
 
 UNASYNC_REPLACEMENTS = {
     "async def": "def",
     "async for": "for",
     "async with": "with",
```

### Comparing `unasyncd-0.5.0/PKG-INFO` & `unasyncd-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: unasyncd
-Version: 0.5.0
+Version: 0.6.0
 Summary: A tool to transform asynchronous Python code to synchronous Python code.
 License: MIT
 Author: Janek Nouvertné
 Author-email: j.a.nouvertne@posteo.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: ruff
 Requires-Dist: anyio (>=3.7.0,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: importlib-metadata (>=6.8.0,<7.0.0) ; python_version < "3.10"
 Requires-Dist: libcst (>=1.0.0,<2.0.0)
 Requires-Dist: msgspec (>=0.17.0,<0.18.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0)
 Requires-Dist: rich-click (>=1.6.1,<2.0.0)
 Requires-Dist: ruff ; extra == "ruff"
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
-# Unasync
+# Unasyncd
 
 A tool to transform asynchronous Python code to synchronous Python code.
 
 ## Why?
 
 Unasyncd is largely inspired by [unasync](https://github.com/python-trio/unasync), and
 a detailed discussion about this approach can be found
@@ -66,28 +67,29 @@
 5. Transformation of constructs like `asyncio.TaskGroup` to a thread based equivalent
 
 *A full list of supported transformations is available below.*
 
 ## Table of contents
 
 <!-- TOC -->
-* [Unasync](#unasync)
+* [Unasyncd](#unasyncd)
   * [Why?](#why)
   * [Why unasyncd?](#why-unasyncd)
   * [Table of contents](#table-of-contents)
   * [What can be transformed?](#what-can-be-transformed)
     * [Asynchronous functions](#asynchronous-functions)
     * [`await`](#await)
     * [Asynchronous iterators, iterables and generators](#asynchronous-iterators-iterables-and-generators)
     * [Asynchronous iteration](#asynchronous-iteration)
     * [Asynchronous context managers](#asynchronous-context-managers)
     * [`contextlib.AsyncExitStack`](#contextlibasyncexitstack)
     * [`asyncio.TaskGroup`](#asynciotaskgroup)
     * [`anyio.create_task_group`](#anyiocreatetaskgroup)
     * [`asyncio.sleep` / `anyio.sleep`](#asynciosleep--anyiosleep)
+    * [`anyio.Path`](#anyiopath)
     * [Type annotations](#type-annotations)
     * [Docstrings](#docstrings)
   * [Usage](#usage)
     * [Installation](#installation)
     * [CLI](#cli)
     * [As a pre-commit hook](#as-a-pre-commit-hook)
     * [Configuration](#configuration)
@@ -371,14 +373,30 @@
 
 ```python
 import asyncio
 
 await asyncio.sleep(0)
 ```
 
+### `anyio.Path`
+
+*Async*
+```python
+import anyio
+
+await anyio.Path().read_bytes()
+```
+
+*Sync*
+```python
+import pathlib
+
+pathlib.Path().read_bytes()
+```
+
 ### Type annotations
 
 |                                   |                                    |
 |-----------------------------------|------------------------------------|
 | `typing.AsyncIterable[int]`       | `typing.Iterable[int]`             |
 | `typing.AsyncIterator[int]`       | `typing.Iterator[int]`             |
 | `typing.AsyncGenerator[int, str]` | `typing.Generator[int, str, None]` |
```

