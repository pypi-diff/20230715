# Comparing `tmp/bcamp-dl-1.0.0.tar.gz` & `tmp/bcamp-dl-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcamp-dl-1.0.0.tar", last modified: Thu Jul 13 22:25:49 2023, max compression
+gzip compressed data, was "bcamp-dl-1.0.1.tar", last modified: Sat Jul 15 02:43:48 2023, max compression
```

## Comparing `bcamp-dl-1.0.0.tar` & `bcamp-dl-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 22:25:49.267732 bcamp-dl-1.0.0/
--rw-rw-rw-   0        0        0     1062 2023-07-13 19:59:05.000000 bcamp-dl-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3852 2023-07-13 22:25:49.266735 bcamp-dl-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1400 2023-07-13 22:18:45.000000 bcamp-dl-1.0.0/README.md
--rw-rw-rw-   0        0        0     2127 2023-07-13 20:02:15.000000 bcamp-dl-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-13 22:25:49.267732 bcamp-dl-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-13 22:25:49.237089 bcamp-dl-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-13 22:25:49.249089 bcamp-dl-1.0.0/src/bcamp_dl/
--rw-rw-rw-   0        0        0      494 2023-07-13 19:59:16.000000 bcamp-dl-1.0.0/src/bcamp_dl/__init__.py
--rw-rw-rw-   0        0        0    11309 2023-07-13 10:33:21.000000 bcamp-dl-1.0.0/src/bcamp_dl/bcamp_dl.py
--rw-rw-rw-   0        0        0     5746 2023-07-13 19:52:49.000000 bcamp-dl-1.0.0/src/bcamp_dl/cli.py
--rw-rw-rw-   0        0        0        0 2023-07-13 10:33:21.000000 bcamp-dl-1.0.0/src/bcamp_dl/py.typed
-drwxrwxrwx   0        0        0        0 2023-07-13 22:25:49.265733 bcamp-dl-1.0.0/src/bcamp_dl.egg-info/
--rw-rw-rw-   0        0        0     3852 2023-07-13 22:25:49.000000 bcamp-dl-1.0.0/src/bcamp_dl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-07-13 22:25:49.000000 bcamp-dl-1.0.0/src/bcamp_dl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 22:25:49.000000 bcamp-dl-1.0.0/src/bcamp_dl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-13 22:25:49.000000 bcamp-dl-1.0.0/src/bcamp_dl.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-13 22:20:47.000000 bcamp-dl-1.0.0/src/bcamp_dl.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      150 2023-07-13 22:25:49.000000 bcamp-dl-1.0.0/src/bcamp_dl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-13 22:25:49.000000 bcamp-dl-1.0.0/src/bcamp_dl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:48.064311 bcamp-dl-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:48.064311 bcamp-dl-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:48.064311 bcamp-dl-1.0.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:48.064311 bcamp-dl-1.0.1/.github/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.github/templates/pr-build.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:48.064311 bcamp-dl-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-07-15 02:43:48.064311 bcamp-dl-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/bcamp-dl.sublime-project
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 02:43:48.064311 bcamp-dl-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:48.060310 bcamp-dl-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:48.064311 bcamp-dl-1.0.1/src/bcamp_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/src/bcamp_dl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-15 02:43:47.000000 bcamp-dl-1.0.1/src/bcamp_dl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/src/bcamp_dl/bcamp_dl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/src/bcamp_dl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:21.000000 bcamp-dl-1.0.1/src/bcamp_dl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 02:43:48.064311 bcamp-dl-1.0.1/src/bcamp_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-07-15 02:43:48.000000 bcamp-dl-1.0.1/src/bcamp_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-15 02:43:48.000000 bcamp-dl-1.0.1/src/bcamp_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 02:43:48.000000 bcamp-dl-1.0.1/src/bcamp_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-15 02:43:48.000000 bcamp-dl-1.0.1/src/bcamp_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 02:43:31.000000 bcamp-dl-1.0.1/src/bcamp_dl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-15 02:43:48.000000 bcamp-dl-1.0.1/src/bcamp_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 02:43:48.000000 bcamp-dl-1.0.1/src/bcamp_dl.egg-info/top_level.txt
```

### Comparing `bcamp-dl-1.0.0/LICENSE` & `bcamp-dl-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bcamp-dl-1.0.0/PKG-INFO` & `bcamp-dl-1.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,83 +1,86 @@
-Metadata-Version: 2.1
-Name: bcamp-dl
-Version: 1.0.0
-Summary: Download your collection from Bandcamp.
-Author-email: ReK42 <ReK42@users.noreply.github.com>
-Maintainer-email: ReK42 <ReK42@users.noreply.github.com>
-License: MIT License
-        
-        Copyright (c) 2023 ReK42
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Repository, https://github.com/ReK42/bcamp-dl
-Project-URL: Issues, https://github.com/ReK42/bcamp-dl/issues
-Keywords: bandcamp,music
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: Topic :: System :: Archiving
-Classifier: Topic :: Utilities
-Classifier: Typing :: Typed
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-License-File: LICENSE
-
-# bcamp-dl
-
-[![License](https://img.shields.io/github/license/ReK42/bcamp-dl)](https://github.com/ReK42/bcamp-dl/blob/main/LICENSE)
-[![PyPi Version](https://img.shields.io/pypi/v/bcamp-dl.svg)](https://pypi.python.org/pypi/bcamp-dl)
-[![PyPI Status](https://img.shields.io/pypi/status/bcamp-dl.svg)](https://pypi.python.org/pypi/bcamp-dl)
-[![Python Versions](https://img.shields.io/pypi/pyversions/bcamp-dl.svg)](https://pypi.python.org/pypi/bcamp-dl)
-[![Last Commit](https://img.shields.io/github/last-commit/ReK42/bcamp-dl/main?logo=github)](https://github.com/ReK42/bcamp-dl/commits/main)
-[![Build Status](https://img.shields.io/github/actions/workflow/status/ReK42/bcamp-dl/build.yml?logo=github)](https://github.com/ReK42/bcamp-dl/actions)
-[![Linted by Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-[![Code Style by Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-Download your collection from Bandcamp.
-
-## Installation
-```sh
-pipx install bcamp-dl
-```
-
-## Usage
-```
-bcamp-dl --browser <BROWSER> --file-format <FORMAT> --directory <DIR> <USERNAME>
-```
-
-For all options, run `bcamp-dl --help`
-
-## Development Environment
-```sh
-git clone https://github.com/ReK42/bcamp-dl.git
-cd bcamp-dl
-pre-commit install
-pip install -e .[tests]
-```
+Metadata-Version: 2.1
+Name: bcamp-dl
+Version: 1.0.1
+Summary: Download your collection from Bandcamp.
+Author-email: ReK42 <ReK42@users.noreply.github.com>
+Maintainer-email: ReK42 <ReK42@users.noreply.github.com>
+License: MIT License
+        
+        Copyright (c) 2023 ReK42
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Repository, https://github.com/ReK42/bcamp-dl
+Project-URL: Issues, https://github.com/ReK42/bcamp-dl/issues
+Keywords: bandcamp,music
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: System :: Archiving
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: build
+License-File: LICENSE
+
+# bcamp-dl
+
+[![License](https://img.shields.io/github/license/ReK42/bcamp-dl)](https://github.com/ReK42/bcamp-dl/blob/main/LICENSE)
+[![PyPi Version](https://img.shields.io/pypi/v/bcamp-dl.svg)](https://pypi.python.org/pypi/bcamp-dl)
+[![PyPI Status](https://img.shields.io/pypi/status/bcamp-dl.svg)](https://pypi.python.org/pypi/bcamp-dl)
+[![Python Versions](https://img.shields.io/pypi/pyversions/bcamp-dl.svg)](https://pypi.python.org/pypi/bcamp-dl)
+[![Last Commit](https://img.shields.io/github/last-commit/ReK42/bcamp-dl/main?logo=github)](https://github.com/ReK42/bcamp-dl/commits/main)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/ReK42/bcamp-dl/build.yml?logo=github)](https://github.com/ReK42/bcamp-dl/actions)
+[![Linted by Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Code Style by Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+Download your collection from Bandcamp.
+
+## Installation
+```sh
+pipx install bcamp-dl
+```
+
+For developers: Merged pull requests will automatically create dev builds on [TestPyPI](https://test.pypi.org/project/bcamp-dl)
+
+## Usage
+```
+bcamp-dl --browser <BROWSER> --file-format <FORMAT> --directory <DIR> <USERNAME>
+```
+
+For all options, run `bcamp-dl --help`
+
+## Development Environment
+```sh
+git clone https://github.com/ReK42/bcamp-dl.git
+cd bcamp-dl
+pre-commit install
+pip install -e .[tests]
+```
```

### Comparing `bcamp-dl-1.0.0/README.md` & `bcamp-dl-1.0.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 Download your collection from Bandcamp.
 
 ## Installation
 ```sh
 pipx install bcamp-dl
 ```
 
+For developers: Merged pull requests will automatically create dev builds on [TestPyPI](https://test.pypi.org/project/bcamp-dl)
+
 ## Usage
 ```
 bcamp-dl --browser <BROWSER> --file-format <FORMAT> --directory <DIR> <USERNAME>
 ```
 
 For all options, run `bcamp-dl --help`
```

### Comparing `bcamp-dl-1.0.0/src/bcamp_dl/bcamp_dl.py` & `bcamp-dl-1.0.1/src/bcamp_dl/bcamp_dl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# -*- coding: utf-8 -*-
 """Download your collection from Bandcamp."""
 import json
 import os
 import re
 import sys
 
 from concurrent.futures import ThreadPoolExecutor
 from html import unescape
 from http.cookiejar import MozillaCookieJar
 from pathlib import Path
 from string import Template
 from threading import Event
 from time import sleep
 from types import TracebackType
-from typing import Any, Type
+from typing import Any
 from unicodedata import normalize
 from urllib.parse import unquote
 
 import browser_cookie3
 import requests
 from bs4 import BeautifulSoup, SoupStrainer
 from rich import box
@@ -78,49 +77,50 @@
         filename = filename.rstrip(". ")
     else:
         filename = re.sub(r"[/\x00-\x1f]", replace, filename)
         filename = filename.rstrip(":")
     return Path(parent, filename + extension)
 
 
-class BandcampDownloader(object):
+class BandcampDownloader:
     """Download your collection from Bandcamp.
 
     To use, login to Bandcamp using one of the supported browsers. All albums in your
     collection will be downloaded to the output directory, with subfolders, based on the
     filename format selected.
     """
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         username: str = "",
         browser: str = "",
         directory: Path = Path("."),
         cookie_path: str = "",
         filename_format: str = "$artist/$artist - $title",
         file_format: str = "mp3-320",
         threads: int = 4,
         pause: float = 1.0,
         max_retries: int = 5,
         retry_wait: float = 5.0,
+        *,  # Following arguments are keyword arguments
         force: bool = False,
         verbose: bool = False,
         debug: bool = False,
-    ):
+    ) -> None:
         if not username:
             raise ValueError("username is required")
         if browser not in SUPPORTED_BROWSERS:
             raise ValueError(f"browser {browser} not supported")
         if threads < 1 or threads > MAX_THREADS:
             raise ValueError(f"threads must be between 1 and {MAX_THREADS}")
-        if pause < 0.0:
+        if pause < 0:
             raise ValueError("pause must be positive")
         if max_retries < 1:
             raise ValueError("max_retries must be greater than or equal to 1")
-        if retry_wait < 0.0:
+        if retry_wait < 0:
             raise ValueError("retry_wait must be positive")
 
         self.username = username
         self.browser = browser
         self.directory = directory
         self.filename_format = Template(filename_format)
         self.file_format = file_format
@@ -155,15 +155,15 @@
         table = Table.grid(expand=True)
         table.add_row(Panel(self.job_progress, box=box.SIMPLE))
         table.add_row(Panel(self.overall_progress, box=box.SIMPLE))
         self.view = Live(table, refresh_per_second=10)
 
         if self.force and self.verbose:
             self.view.console.print(
-                "Force flag set, existing files will be overwritten."
+                "Force flag set, existing files will be overwritten.",
             )
 
         if cookie_path:
             cookie_jar = MozillaCookieJar(cookie_path)
             cookie_jar.load()
             self.cookies = cookie_jar
         else:
@@ -172,31 +172,31 @@
 
     def __enter__(self) -> "BandcampDownloader":
         self.view.start(refresh=True)
         return self
 
     def __exit__(
         self,
-        exc_type: Type[BaseException] | None,
+        exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         self.view.stop()
 
     def run(self) -> int:
         """Primary execution thread."""
         self._get_albums()
         if not self.links:
             self.view.console.print(
-                f"ERROR: No album links found for user {self.username}."
+                f"ERROR: No album links found for user {self.username}.",
             )
             return 1
         if self.verbose:
             self.view.console.print(
-                f"Found {len(self.links)} links in {self.username}'s collection."
+                f"Found {len(self.links)} links in {self.username}'s collection.",
             )
             self.view.console.print("Starting album downloads...")
         self.view.console.print("To cancel, press CTRL+BREAK")
         self.main_task = self.overall_progress.add_task(
             "Downloading albums...",
             total=len(self.links),
         )
@@ -205,57 +205,72 @@
         if self.event_stop.is_set():
             self.view.console.print("ERROR: Process aborted by user...")
             return 1
         if self.verbose:
             self.view.console.print("Done")
         return 0
 
-    def _get_pagedata(self, url) -> dict[str, Any]:
-        with requests.get(url, cookies=self.cookies) as resp:  # type: ignore
+    def _get_pagedata(self, url: str) -> dict[str, Any]:
+        with requests.get(
+            url,
+            cookies=self.cookies,  # type: ignore[arg-type]
+            timeout=15.0,
+        ) as resp:
             resp.raise_for_status()
             soup = BeautifulSoup(
-                resp.text, "html.parser", parse_only=SoupStrainer("div", id="pagedata")
+                resp.text,
+                "html.parser",
+                parse_only=SoupStrainer("div", id="pagedata"),
             )
             div = soup.find("div")
         if not div:
-            raise IOError(f"No div#pagedata found at {url}")
-        return json.loads(unescape(div.get("data-blob")))  # type: ignore
+            raise OSError(f"No div#pagedata found at {url}")
+        return json.loads(
+            unescape(
+                div.get("data-blob"),  # type: ignore[union-attr]
+            ),  # type: ignore[arg-type,type-var]
+        )
 
     def _get_albums(self) -> None:
         data = self._get_pagedata(URL_USER + self.username)
         user_id = data["fan_data"]["fan_id"]
         collection_count = data["collection_count"]
         last_token = data["collection_data"]["last_token"]
         links = [*data["collection_data"]["redownload_urls"].values()]
         req = json.dumps(
             {
                 "fan_id": user_id,
                 "count": collection_count,
                 "older_than_token": last_token,
-            }
+            },
         )
-        with requests.post(URL_COLLECTION, data=req, cookies=self.cookies) as resp:  # type: ignore
+        with requests.post(
+            URL_COLLECTION,
+            data=req,
+            cookies=self.cookies,  # type: ignore[arg-type]
+            timeout=15.0,
+        ) as resp:
             resp.raise_for_status()
             data = json.loads(resp.text)
             links += data["redownload_urls"].values()
         self.links = links
 
     def _get_album(self, url: str) -> None:
         """Attempt to download an album."""
         if self.event_stop.is_set():
             return None
         try:
             data = self._get_pagedata(url)["download_items"][0]
             album = data["title"]
             if "downloads" not in data:
-                raise IOError(f"Album {album} has no downloads available")
+                raise OSError(f"Album {album} has no downloads available")
             if self.file_format not in data["downloads"]:
-                raise IOError(
+                raise OSError(
                     f"Album {album} does not have a download for format"
-                    f" {self.file_format}"
+                    f" {self.file_format}",
                 )
             url = data["downloads"][self.file_format]["url"]
             info = {k: data[k] for k in ALBUM_INFO_KEYS}
             task_id = self.job_progress.add_task(album)
             self._download_album(task_id, url, info)
         except Exception:
             self.view.console.print(f"ERROR: Failed to download album: {url}")
@@ -264,58 +279,67 @@
                 self.overall_progress.advance(self.main_task)
                 self.job_progress.remove_task(task_id)
             except Exception:
                 pass
             sleep(self.pause)
 
     def _download_album(
-        self, task_id: TaskID, url: str, info: dict[str, str], attempt: int = 1
+        self,
+        task_id: TaskID,
+        url: str,
+        info: dict[str, str],
+        attempt: int = 1,
     ) -> None:
         if self.event_stop.is_set():
             return None
         try:
-            with requests.get(url, cookies=self.cookies, stream=True) as resp:  # type: ignore
+            with requests.get(
+                url,
+                cookies=self.cookies,  # type: ignore[arg-type]
+                stream=True,
+                timeout=15.0,
+            ) as resp:
                 resp.raise_for_status()
                 content_length = int(resp.headers["content-length"])
                 match = re.search(
                     r"filename\*=UTF-8\'\'.*(\..*)$",
                     resp.headers["content-disposition"],
                 )
-                if match:
-                    extension = unquote(match.group(1))
-                else:
-                    extension = url.split("/")[-1]
+                extension = unquote(match.group(1)) if match else url.split("/")[-1]
                 path = sanitize_path(
                     Path(
                         self.directory,
                         self.filename_format.substitute(info) + extension,
-                    )
+                    ),
                 )
-                if path.exists():
-                    if not self.force and path.stat().st_size == content_length:
-                        if self.verbose:
-                            self.view.console.print(
-                                f"Skipping album, file already exists: {path}"
-                            )
-                        return None
+                if (
+                    path.exists()
+                    and not self.force
+                    and path.stat().st_size == content_length
+                ):
+                    if self.verbose:
+                        self.view.console.print(
+                            f"Skipping album, file already exists: {path}",
+                        )
+                    return None
                 path.parent.mkdir(parents=True, exist_ok=True)
                 with path.open(mode="wb") as f:
                     self.job_progress.reset(task_id, total=content_length)
                     self.job_progress.start_task(task_id)
                     for data in resp.iter_content(chunk_size=10):
                         if self.event_stop.is_set():
                             return None
                         f.write(data)
                         self.job_progress.advance(task_id, advance=len(data))
                 if path.stat().st_size != content_length:
-                    raise IOError("File does not match expected size")
-        except IOError as e:
+                    raise OSError("File does not match expected size")
+        except OSError as e:
             if attempt < self.max_retries:
                 if self.verbose:
                     self.view.console.print(
                         f"Download attempt {attempt} of {self.max_retries} failed:"
-                        f" {url}"
+                        f" {url}",
                     )
                 sleep(self.retry_wait)
                 self._download_album(task_id, url, info, attempt=attempt + 1)
             else:
-                raise IOError("Max retries exceeded") from e
+                raise OSError("Max retries exceeded") from e
```

### Comparing `bcamp-dl-1.0.0/src/bcamp_dl/cli.py` & `bcamp-dl-1.0.1/src/bcamp_dl/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,103 +1,105 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 """Download your collection from Bandcamp."""
 import os
 import sys
 
 from argparse import ArgumentParser, ArgumentTypeError, RawTextHelpFormatter
 from pathlib import Path
 
 from bcamp_dl import (
-    _name,
-    _version,
-    _copyright,
+    __name__,
+    __version__,
+    __copyright__,
     BandcampDownloader,
     MAX_THREADS,
     ALBUM_INFO_KEYS,
     SUPPORTED_BROWSERS,
     SUPPORTED_FILE_FORMATS,
 )
 
 
 def int_positive(arg: str) -> int:
     """Validate an integer is positive."""
     try:
         i = int(arg)
-    except ValueError:
-        raise ArgumentTypeError("Must be an integer")
+    except ValueError as e:
+        raise ArgumentTypeError("Must be an integer") from e
     if i < 0:
         raise ArgumentTypeError("Integer must be positive")
     return i
 
 
 def float_positive(arg: str) -> float:
     """Validate a float is positive."""
     try:
         f = float(arg)
-    except ValueError:
-        raise ArgumentTypeError("Must be a float")
+    except ValueError as e:
+        raise ArgumentTypeError("Must be a float") from e
     if f < 0:
         raise ArgumentTypeError("Float must be positive")
     return f
 
 
 def num_threads(arg: str) -> int:
     """Validate an given number of threads is supported."""
     try:
         i = int(arg)
-    except ValueError:
-        raise ArgumentTypeError("Must be an integer")
+    except ValueError as e:
+        raise ArgumentTypeError("Must be an integer") from e
     if i < 0:
         raise ArgumentTypeError("Integer must be positive")
     if i > MAX_THREADS:
         raise ArgumentTypeError(f"Integer must be <= {MAX_THREADS}")
     return i
 
 
 def path_is_writable_file(arg: str) -> Path:
     """Validate that a path is a writable file."""
     try:
         p = Path(arg)
-    except ValueError:
-        raise ArgumentTypeError("Must be a path")
+    except ValueError as e:
+        raise ArgumentTypeError("Must be a path") from e
     if p.exists():
         if not p.is_file():
             raise ArgumentTypeError("Path exists but is not a file")
         if os.access(p, os.W_OK):
             raise ArgumentTypeError("Path exists but it not writable")
     else:
         if not p.parent.is_dir():
             raise ArgumentTypeError(
-                "File does not exist and parent directory does not exist"
+                "File does not exist and parent directory does not exist",
             )
         if not os.access(p.parent, os.W_OK):
             raise ArgumentTypeError(
-                "File does not exist and parent directory is not writable"
+                "File does not exist and parent directory is not writable",
             )
     return p
 
 
 def main() -> None:
     """Script entry point."""
     parser = ArgumentParser(
-        prog=_name,
+        prog=__name__,
         add_help=False,
         description=(
             "Download your collection from Bandcamp.\n"
             "\n"
             "To use, login to Bandcamp using one of the supported browsers. All albums"
             " in your collection will be downloaded to the output directory, with"
             " subfolders, based on the filename format selected."
         ),
         epilog="",
         formatter_class=RawTextHelpFormatter,
     )
     parser.add_argument(
-        "username", type=str, metavar="USERNAME", help="Bandcamp username"
+        "username",
+        type=str,
+        metavar="USERNAME",
+        help="Bandcamp username",
     )
     parser.add_argument(
         "-b",
         "--browser",
         type=str,
         metavar="BROWSER",
         default="firefox",
@@ -175,28 +177,36 @@
         default="$artist/$artist - $title",
         help=(
             "Filename format to use, default: %(default)s\n"
             f"Supported variables: {', '.join([f'${k}' for k in ALBUM_INFO_KEYS])}"
         ),
     )
     parser.add_argument(
-        "--force", action="store_true", help="Re-download and overwrite existing albums"
+        "--force",
+        action="store_true",
+        help="Re-download and overwrite existing albums",
     )
     parser.add_argument(
-        "-v", "--verbose", action="store_true", help="Show verbose information"
+        "-v",
+        "--verbose",
+        action="store_true",
+        help="Show verbose information",
     )
     parser.add_argument("--debug", action="store_true", help="Show debug information")
     parser.add_argument(
-        "-h", "--help", action="help", help="Show this help message and exit"
+        "-h",
+        "--help",
+        action="help",
+        help="Show this help message and exit",
     )
     parser.add_argument(
         "--version",
         action="version",
         help="Show version information and exit",
-        version=f"{_name} v{_version}: {_copyright}",
+        version=f"{__name__} v{__version__} {__copyright__}",
     )
     args = parser.parse_args()
     with BandcampDownloader(**vars(args)) as app:
         sys.exit(app.run())
 
 
 if __name__ == "__main__":
```

### Comparing `bcamp-dl-1.0.0/src/bcamp_dl.egg-info/PKG-INFO` & `bcamp-dl-1.0.1/src/bcamp_dl.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,83 +1,86 @@
-Metadata-Version: 2.1
-Name: bcamp-dl
-Version: 1.0.0
-Summary: Download your collection from Bandcamp.
-Author-email: ReK42 <ReK42@users.noreply.github.com>
-Maintainer-email: ReK42 <ReK42@users.noreply.github.com>
-License: MIT License
-        
-        Copyright (c) 2023 ReK42
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Repository, https://github.com/ReK42/bcamp-dl
-Project-URL: Issues, https://github.com/ReK42/bcamp-dl/issues
-Keywords: bandcamp,music
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: Topic :: System :: Archiving
-Classifier: Topic :: Utilities
-Classifier: Typing :: Typed
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-License-File: LICENSE
-
-# bcamp-dl
-
-[![License](https://img.shields.io/github/license/ReK42/bcamp-dl)](https://github.com/ReK42/bcamp-dl/blob/main/LICENSE)
-[![PyPi Version](https://img.shields.io/pypi/v/bcamp-dl.svg)](https://pypi.python.org/pypi/bcamp-dl)
-[![PyPI Status](https://img.shields.io/pypi/status/bcamp-dl.svg)](https://pypi.python.org/pypi/bcamp-dl)
-[![Python Versions](https://img.shields.io/pypi/pyversions/bcamp-dl.svg)](https://pypi.python.org/pypi/bcamp-dl)
-[![Last Commit](https://img.shields.io/github/last-commit/ReK42/bcamp-dl/main?logo=github)](https://github.com/ReK42/bcamp-dl/commits/main)
-[![Build Status](https://img.shields.io/github/actions/workflow/status/ReK42/bcamp-dl/build.yml?logo=github)](https://github.com/ReK42/bcamp-dl/actions)
-[![Linted by Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-[![Code Style by Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-Download your collection from Bandcamp.
-
-## Installation
-```sh
-pipx install bcamp-dl
-```
-
-## Usage
-```
-bcamp-dl --browser <BROWSER> --file-format <FORMAT> --directory <DIR> <USERNAME>
-```
-
-For all options, run `bcamp-dl --help`
-
-## Development Environment
-```sh
-git clone https://github.com/ReK42/bcamp-dl.git
-cd bcamp-dl
-pre-commit install
-pip install -e .[tests]
-```
+Metadata-Version: 2.1
+Name: bcamp-dl
+Version: 1.0.1
+Summary: Download your collection from Bandcamp.
+Author-email: ReK42 <ReK42@users.noreply.github.com>
+Maintainer-email: ReK42 <ReK42@users.noreply.github.com>
+License: MIT License
+        
+        Copyright (c) 2023 ReK42
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Repository, https://github.com/ReK42/bcamp-dl
+Project-URL: Issues, https://github.com/ReK42/bcamp-dl/issues
+Keywords: bandcamp,music
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Multimedia :: Sound/Audio
+Classifier: Topic :: System :: Archiving
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: build
+License-File: LICENSE
+
+# bcamp-dl
+
+[![License](https://img.shields.io/github/license/ReK42/bcamp-dl)](https://github.com/ReK42/bcamp-dl/blob/main/LICENSE)
+[![PyPi Version](https://img.shields.io/pypi/v/bcamp-dl.svg)](https://pypi.python.org/pypi/bcamp-dl)
+[![PyPI Status](https://img.shields.io/pypi/status/bcamp-dl.svg)](https://pypi.python.org/pypi/bcamp-dl)
+[![Python Versions](https://img.shields.io/pypi/pyversions/bcamp-dl.svg)](https://pypi.python.org/pypi/bcamp-dl)
+[![Last Commit](https://img.shields.io/github/last-commit/ReK42/bcamp-dl/main?logo=github)](https://github.com/ReK42/bcamp-dl/commits/main)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/ReK42/bcamp-dl/build.yml?logo=github)](https://github.com/ReK42/bcamp-dl/actions)
+[![Linted by Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
+[![Code Style by Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+Download your collection from Bandcamp.
+
+## Installation
+```sh
+pipx install bcamp-dl
+```
+
+For developers: Merged pull requests will automatically create dev builds on [TestPyPI](https://test.pypi.org/project/bcamp-dl)
+
+## Usage
+```
+bcamp-dl --browser <BROWSER> --file-format <FORMAT> --directory <DIR> <USERNAME>
+```
+
+For all options, run `bcamp-dl --help`
+
+## Development Environment
+```sh
+git clone https://github.com/ReK42/bcamp-dl.git
+cd bcamp-dl
+pre-commit install
+pip install -e .[tests]
+```
```

