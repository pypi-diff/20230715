# Comparing `tmp/spcache-1.0.0.tar.gz` & `tmp/spcache-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spcache-1.0.0.tar", max compression
+gzip compressed data, was "spcache-1.0.1.tar", max compression
```

## Comparing `spcache-1.0.0.tar` & `spcache-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1067 2023-06-24 09:50:01.464052 spcache-1.0.0/LICENSE
--rw-r--r--   0        0        0     3471 2023-06-24 09:50:01.464052 spcache-1.0.0/README.md
--rw-r--r--   0        0        0     3017 2023-06-24 09:50:01.468052 spcache-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       58 2023-06-24 09:50:01.468052 spcache-1.0.0/spcache/__init__.py
--rw-r--r--   0        0        0       64 2023-06-24 09:50:01.468052 spcache-1.0.0/spcache/__main__.py
--rw-r--r--   0        0        0     4991 2023-06-24 09:50:01.468052 spcache-1.0.0/spcache/cli.py
--rw-r--r--   0        0        0     2256 2023-06-24 09:50:01.468052 spcache-1.0.0/spcache/detect.py
--rw-r--r--   0        0        0     3798 2023-06-24 09:50:01.468052 spcache-1.0.0/spcache/env.py
--rw-r--r--   0        0        0     4850 1970-01-01 00:00:00.000000 spcache-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-15 13:41:26.793635 spcache-1.0.1/LICENSE
+-rw-r--r--   0        0        0     8318 2023-07-15 13:41:26.793635 spcache-1.0.1/LICENSE-THIRD-PARTY
+-rw-r--r--   0        0        0     3674 2023-07-15 13:41:26.793635 spcache-1.0.1/README.md
+-rw-r--r--   0        0        0     3008 2023-07-15 13:41:26.797635 spcache-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-07-15 13:41:26.797635 spcache-1.0.1/spcache/__init__.py
+-rw-r--r--   0        0        0       64 2023-07-15 13:41:26.797635 spcache-1.0.1/spcache/__main__.py
+-rw-r--r--   0        0        0     4991 2023-07-15 13:41:26.797635 spcache-1.0.1/spcache/cli.py
+-rw-r--r--   0        0        0     2256 2023-07-15 13:41:26.797635 spcache-1.0.1/spcache/detect.py
+-rw-r--r--   0        0        0     3560 2023-07-15 13:41:26.797635 spcache-1.0.1/spcache/env.py
+-rw-r--r--   0        0        0     5053 1970-01-01 00:00:00.000000 spcache-1.0.1/PKG-INFO
```

### Comparing `spcache-1.0.0/LICENSE` & `spcache-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spcache-1.0.0/README.md` & `spcache-1.0.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -23,24 +23,25 @@
 ### Windows
 
 > Open PowerShell. You can do this by searching for "PowerShell" in the Start menu.
 
 Paste the following and hit enter:
 
 ```powershell
-Invoke-WebRequest -UseBasicParsing https://raw.githubusercontent.com/Qwerty-133/spcache/main/bin/install_spcache.ps1 |
-  Invoke-Expression
+Invoke-WebRequest -UseBasicParsing https://qwertie.pages.dev/install_spcache.ps1 | Invoke-Expression
 ```
 
 ### MacOS/Linux
 
 ```bash
-curl -sSL https://raw.githubusercontent.com/Qwerty-133/spcache/main/bin/install_spcache.sh | bash -s -
+curl -sSL https://qwertie.pages.dev/install_spcache.sh | bash -s -
 ```
 
+> If the above script fails, please install spcache using Python. See [Installing From PyPI](#installing-from-pypi).
+
 ## Usage
 
 -   Set the cache size limit to 1GB:
 
     ```bash
     spcache set --size 1000
     ```
@@ -67,57 +68,60 @@
 
 ## How It Works
 
 spcache works by changing the value of `storage.size` in your Spotify prefs file.
 
 > :warning: Changes are applied when the Spotify app is restarted.
 
+To restart Spotify:
+
+- On Windows, right-click the Spotify icon in the system tray and click "Quit".
+- On MacOS, right-click the Spotify icon in the dock and click "Quit".
+
+Then open Spotify again.
+
 Spotify displays the current cache size inside the Storage section in the Settings page.
 
 ## Uninstallation
 
 ### Windows
 
 ```powershell
-Invoke-WebRequest -UseBasicParsing https://raw.githubusercontent.com/Qwerty-133/spcache/main/bin/uninstall_spcache.ps1 |
-  Invoke-Expression
+Invoke-WebRequest -UseBasicParsing https://qwertie.pages.dev/uninstall_spcache.ps1 | Invoke-Expression
 ```
 
 This will remove the spcache files and remove spcache from your PATH.
 
 ### MacOS/Linux
 
 spcache is installed in `~/.local/share/spcache`, unless `$XDG_DATA_HOME` is set.
 
 ```bash
-rm -r "~/.local/share/spcache" || rm -r "${XDG_DATA_HOME}/spcache"
+rm -r ~/.local/share/spcache || rm -r "${XDG_DATA_HOME}/spcache"
 ```
 
 ## Installing a Specific Version
 
 > Available versions are listed here <https://github.com/Qwerty-133/spcache/releases>.
 
 ### Windows
 
 Installing a specific version of spcache:
 
 ```powershell
-$script = [scriptblock]::Create(
-  (iwr -useb "https://raw.githubusercontent.com/Qwerty-133/spcache/main/bin/install_spcache.ps1").Content
-)
-& $script -Version 1.0.0
+$script = [scriptblock]::Create((iwr -useb "https://qwertie.pages.dev/install_spcache.ps1").Content)
+& $script -Version 1.0.1
 ```
 
 ### MacOS/Linux
 
 Installing a specific version of spcache:
 
 ```bash
-curl -sSL https://raw.githubusercontent.com/Qwerty-133/spcache/main/bin/install_spcache.sh |
-  bash -s - --version 1.0.0
+curl -sSL https://qwertie.pages.dev/install_spcache.sh | bash -s - -v 1.0.1
 ```
 
 ## Installing from PyPI
 
 spcache is also available on PyPI <https://pypi.org/project/spcache/>.
 If you have Python 3.8+ installed, you can install spcache using pip:
 
@@ -129,10 +133,12 @@
 
 -   On MacOS/Linux:
 
     1. Check your Python version with `python3 --version`
     2. Run `python3 -m pip install spcache` to install spcache.
     3. Use `python3 -m spcache` if `spcache` doesn't work.
 
+To install a specific version of spcache, use `pip install spcache==1.0.1` instead.
+
 ## Contributing
 
 See [CONTRIBUTING.md](CONTRIBUTING.md).
```

#### html2text {}

```diff
@@ -1,41 +1,42 @@
                              ****** spcache ******
            A simple CLI tool to set a limit on Spotify's cache size.
                           [License] [Release] [PyPI]
 ## Installation > See [Installing a Specific Version](#installing-a-specific-
 version) for additional options. ### Windows > Open PowerShell. You can do this
 by searching for "PowerShell" in the Start menu. Paste the following and hit
 enter: ```powershell Invoke-WebRequest -UseBasicParsing https://
-raw.githubusercontent.com/Qwerty-133/spcache/main/bin/install_spcache.ps1 |
-Invoke-Expression ``` ### MacOS/Linux ```bash curl -sSL https://
-raw.githubusercontent.com/Qwerty-133/spcache/main/bin/install_spcache.sh | bash
--s - ``` ## Usage - Set the cache size limit to 1GB: ```bash spcache set --size
-1000 ``` spcache will try to detect your Spotify prefs file and set the cache
-size to the specified value in megabytes (MB). - Specify the path to your prefs
-file manually: ```bash spcache set --size 1000 --file /path/to/prefs ``` - View
-the current cache size limit: ```bash spcache get ``` - View more options:
-```bash spcache --help ``` ## How It Works spcache works by changing the value
-of `storage.size` in your Spotify prefs file. > :warning: Changes are applied
-when the Spotify app is restarted. Spotify displays the current cache size
+qwertie.pages.dev/install_spcache.ps1 | Invoke-Expression ``` ### MacOS/Linux
+```bash curl -sSL https://qwertie.pages.dev/install_spcache.sh | bash -s - ```
+> If the above script fails, please install spcache using Python. See
+[Installing From PyPI](#installing-from-pypi). ## Usage - Set the cache size
+limit to 1GB: ```bash spcache set --size 1000 ``` spcache will try to detect
+your Spotify prefs file and set the cache size to the specified value in
+megabytes (MB). - Specify the path to your prefs file manually: ```bash spcache
+set --size 1000 --file /path/to/prefs ``` - View the current cache size limit:
+```bash spcache get ``` - View more options: ```bash spcache --help ``` ## How
+It Works spcache works by changing the value of `storage.size` in your Spotify
+prefs file. > :warning: Changes are applied when the Spotify app is restarted.
+To restart Spotify: - On Windows, right-click the Spotify icon in the system
+tray and click "Quit". - On MacOS, right-click the Spotify icon in the dock and
+click "Quit". Then open Spotify again. Spotify displays the current cache size
 inside the Storage section in the Settings page. ## Uninstallation ### Windows
-```powershell Invoke-WebRequest -UseBasicParsing https://
-raw.githubusercontent.com/Qwerty-133/spcache/main/bin/uninstall_spcache.ps1 |
-Invoke-Expression ``` This will remove the spcache files and remove spcache
-from your PATH. ### MacOS/Linux spcache is installed in `~/.local/share/
-spcache`, unless `$XDG_DATA_HOME` is set. ```bash rm -r "~/.local/share/
-spcache" || rm -r "${XDG_DATA_HOME}/spcache" ``` ## Installing a Specific
-Version > Available versions are listed here
+```powershell Invoke-WebRequest -UseBasicParsing https://qwertie.pages.dev/
+uninstall_spcache.ps1 | Invoke-Expression ``` This will remove the spcache
+files and remove spcache from your PATH. ### MacOS/Linux spcache is installed
+in `~/.local/share/spcache`, unless `$XDG_DATA_HOME` is set. ```bash rm -
+r ~/.local/share/spcache || rm -r "${XDG_DATA_HOME}/spcache" ``` ## Installing
+a Specific Version > Available versions are listed here
 github.com/Qwerty-133/spcache/releases>. ### Windows Installing a specific
-version of spcache: ```powershell $script = [scriptblock]::Create( (iwr -useb
-"https://raw.githubusercontent.com/Qwerty-133/spcache/main/bin/
-install_spcache.ps1").Content ) & $script -Version 1.0.0 ``` ### MacOS/Linux
-Installing a specific version of spcache: ```bash curl -sSL https://
-raw.githubusercontent.com/Qwerty-133/spcache/main/bin/install_spcache.sh | bash
--s - --version 1.0.0 ``` ## Installing from PyPI spcache is also available on
-PyPI
+version of spcache: ```powershell $script = [scriptblock]::Create((iwr -useb
+"https://qwertie.pages.dev/install_spcache.ps1").Content) & $script -Version
+1.0.1 ``` ### MacOS/Linux Installing a specific version of spcache: ```bash
+curl -sSL https://qwertie.pages.dev/install_spcache.sh | bash -s - -v 1.0.1 ```
+## Installing from PyPI spcache is also available on PyPI
 pypi.org/project/spcache/>. If you have Python 3.8+ installed, you can install
 spcache using pip: - On Windows: 1. Check your Python version with `py --
 version` 2. Run `py -m pip install spcache` to install spcache. 3. Use `py -
 m spcache` instead of `spcache`. - On MacOS/Linux: 1. Check your Python version
 with `python3 --version` 2. Run `python3 -m pip install spcache` to install
-spcache. 3. Use `python3 -m spcache` if `spcache` doesn't work. ## Contributing
-See [CONTRIBUTING.md](CONTRIBUTING.md).
+spcache. 3. Use `python3 -m spcache` if `spcache` doesn't work. To install a
+specific version of spcache, use `pip install spcache==1.0.1` instead. ##
+Contributing See [CONTRIBUTING.md](CONTRIBUTING.md).
```

### Comparing `spcache-1.0.0/pyproject.toml` & `spcache-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spcache"
-version = "1.0.0"
+version = "1.0.1"
 description = "Ensure Spotify's cache size doesn't exceed a specified threshold."
 authors = ["Qwerty-133 <74311372+Qwerty-133@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/Qwerty-133/spcache"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -40,14 +40,15 @@
 [tool.poetry.group.dev.dependencies]
 taskipy = "^1.11.0"
 pre-commit = "^3.3.2"
 ruff = "^0.0.272"
 black = "^23.3.0"
 isort = "^5.12.0"
 pyinstaller = "^5.12.0"
+pip-licenses = "^4.3.2"
 
 [tool.ruff]
 target-version = "py38"
 select = [
     "ANN",  # flake8-annotations
     "B",  # flake8-bugbear
     "C4",  # flake8-comprehensions
@@ -82,15 +83,14 @@
     "D413",  # Missing blank line after last section
     "D105",  # Missing docstring in magic method
 ]
 line-length = 99
 
 [tool.taskipy.tasks]
 lint = "pre-commit run --all-files"
-precommit = "pre-commit install"
 
 [tool.isort]
 order_by_type = false
 case_sensitive = true
 combine_as_imports = true
 atomic = true
```

### Comparing `spcache-1.0.0/spcache/cli.py` & `spcache-1.0.1/spcache/cli.py`

 * *Files identical despite different names*

### Comparing `spcache-1.0.0/spcache/detect.py` & `spcache-1.0.1/spcache/detect.py`

 * *Files identical despite different names*

### Comparing `spcache-1.0.0/spcache/env.py` & `spcache-1.0.1/spcache/env.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Improvements to the parsing functionality of the dotenv module."""
 
 import os
+import pathlib
 import shutil
 import tempfile
 import typing as t
 from contextlib import contextmanager
 
 import dotenv.main
 
@@ -19,41 +20,29 @@
 
 @contextmanager
 def rewrite(
     path: dotenv.main.StrPath,
     encoding: t.Optional[str],
 ) -> t.Iterator[t.Tuple[t.TextIO, t.TextIO]]:
     """Make changes to a file atomically."""
-    if not os.path.isfile(path):
-        with open(path, mode="w", encoding=encoding) as source:
-            pass
-
-    dest_file = tempfile.NamedTemporaryFile(mode="w", encoding=encoding, delete=False)
-
-    try:
-        source = open(path, encoding=encoding)  # noqa: SIM115
-    except BaseException:
-        dest_file.close()
-        os.unlink(dest_file.name)
-        raise
-
-    try:
-        yield (source, dest_file)
-    except BaseException:
-        failed = True
-        raise
+    pathlib.Path(path).touch()
+
+    with tempfile.NamedTemporaryFile(mode="w", encoding=encoding, delete=False) as dest:
+        error = None
+        try:
+            with open(path, encoding=encoding) as source:
+                yield (source, dest)
+        except BaseException as err:
+            error = err
+
+    if error is None:
+        shutil.move(dest.name, path)
     else:
-        failed = False
-    finally:
-        dest_file.close()
-        source.close()
-        if failed:
-            os.unlink(dest_file.name)
-        else:
-            shutil.move(dest_file.name, path)
+        os.unlink(dest.name)
+        raise error from None
 
 
 def set_key(
     dotenv_path: dotenv.main.StrPath,
     key_to_set: str,
     value_to_set: str,
     quote_mode: t.Literal["always", "auto", "never"] = "always",
```

### Comparing `spcache-1.0.0/PKG-INFO` & `spcache-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spcache
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ensure Spotify's cache size doesn't exceed a specified threshold.
 Home-page: https://github.com/Qwerty-133/spcache
 License: MIT
 Author: Qwerty-133
 Author-email: 74311372+Qwerty-133@users.noreply.github.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 4 - Beta
@@ -58,24 +58,25 @@
 ### Windows
 
 > Open PowerShell. You can do this by searching for "PowerShell" in the Start menu.
 
 Paste the following and hit enter:
 
 ```powershell
-Invoke-WebRequest -UseBasicParsing https://raw.githubusercontent.com/Qwerty-133/spcache/main/bin/install_spcache.ps1 |
-  Invoke-Expression
+Invoke-WebRequest -UseBasicParsing https://qwertie.pages.dev/install_spcache.ps1 | Invoke-Expression
 ```
 
 ### MacOS/Linux
 
 ```bash
-curl -sSL https://raw.githubusercontent.com/Qwerty-133/spcache/main/bin/install_spcache.sh | bash -s -
+curl -sSL https://qwertie.pages.dev/install_spcache.sh | bash -s -
 ```
 
+> If the above script fails, please install spcache using Python. See [Installing From PyPI](#installing-from-pypi).
+
 ## Usage
 
 -   Set the cache size limit to 1GB:
 
     ```bash
     spcache set --size 1000
     ```
@@ -102,57 +103,60 @@
 
 ## How It Works
 
 spcache works by changing the value of `storage.size` in your Spotify prefs file.
 
 > :warning: Changes are applied when the Spotify app is restarted.
 
+To restart Spotify:
+
+- On Windows, right-click the Spotify icon in the system tray and click "Quit".
+- On MacOS, right-click the Spotify icon in the dock and click "Quit".
+
+Then open Spotify again.
+
 Spotify displays the current cache size inside the Storage section in the Settings page.
 
 ## Uninstallation
 
 ### Windows
 
 ```powershell
-Invoke-WebRequest -UseBasicParsing https://raw.githubusercontent.com/Qwerty-133/spcache/main/bin/uninstall_spcache.ps1 |
-  Invoke-Expression
+Invoke-WebRequest -UseBasicParsing https://qwertie.pages.dev/uninstall_spcache.ps1 | Invoke-Expression
 ```
 
 This will remove the spcache files and remove spcache from your PATH.
 
 ### MacOS/Linux
 
 spcache is installed in `~/.local/share/spcache`, unless `$XDG_DATA_HOME` is set.
 
 ```bash
-rm -r "~/.local/share/spcache" || rm -r "${XDG_DATA_HOME}/spcache"
+rm -r ~/.local/share/spcache || rm -r "${XDG_DATA_HOME}/spcache"
 ```
 
 ## Installing a Specific Version
 
 > Available versions are listed here <https://github.com/Qwerty-133/spcache/releases>.
 
 ### Windows
 
 Installing a specific version of spcache:
 
 ```powershell
-$script = [scriptblock]::Create(
-  (iwr -useb "https://raw.githubusercontent.com/Qwerty-133/spcache/main/bin/install_spcache.ps1").Content
-)
-& $script -Version 1.0.0
+$script = [scriptblock]::Create((iwr -useb "https://qwertie.pages.dev/install_spcache.ps1").Content)
+& $script -Version 1.0.1
 ```
 
 ### MacOS/Linux
 
 Installing a specific version of spcache:
 
 ```bash
-curl -sSL https://raw.githubusercontent.com/Qwerty-133/spcache/main/bin/install_spcache.sh |
-  bash -s - --version 1.0.0
+curl -sSL https://qwertie.pages.dev/install_spcache.sh | bash -s - -v 1.0.1
 ```
 
 ## Installing from PyPI
 
 spcache is also available on PyPI <https://pypi.org/project/spcache/>.
 If you have Python 3.8+ installed, you can install spcache using pip:
 
@@ -164,11 +168,13 @@
 
 -   On MacOS/Linux:
 
     1. Check your Python version with `python3 --version`
     2. Run `python3 -m pip install spcache` to install spcache.
     3. Use `python3 -m spcache` if `spcache` doesn't work.
 
+To install a specific version of spcache, use `pip install spcache==1.0.1` instead.
+
 ## Contributing
 
 See [CONTRIBUTING.md](CONTRIBUTING.md).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spcache Version: 1.0.0 Summary: Ensure Spotify's
+Metadata-Version: 2.1 Name: spcache Version: 1.0.1 Summary: Ensure Spotify's
 cache size doesn't exceed a specified threshold. Home-page: https://github.com/
 Qwerty-133/spcache License: MIT Author: Qwerty-133 Author-email:
 74311372+Qwerty-133@users.noreply.github.com Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
 Classifier: Framework :: Flake8 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop Classifier: License :: OSI
 Approved :: MIT License Classifier: Natural Language :: English Classifier:
@@ -19,41 +19,42 @@
                              ****** spcache ******
            A simple CLI tool to set a limit on Spotify's cache size.
                           [License] [Release] [PyPI]
 ## Installation > See [Installing a Specific Version](#installing-a-specific-
 version) for additional options. ### Windows > Open PowerShell. You can do this
 by searching for "PowerShell" in the Start menu. Paste the following and hit
 enter: ```powershell Invoke-WebRequest -UseBasicParsing https://
-raw.githubusercontent.com/Qwerty-133/spcache/main/bin/install_spcache.ps1 |
-Invoke-Expression ``` ### MacOS/Linux ```bash curl -sSL https://
-raw.githubusercontent.com/Qwerty-133/spcache/main/bin/install_spcache.sh | bash
--s - ``` ## Usage - Set the cache size limit to 1GB: ```bash spcache set --size
-1000 ``` spcache will try to detect your Spotify prefs file and set the cache
-size to the specified value in megabytes (MB). - Specify the path to your prefs
-file manually: ```bash spcache set --size 1000 --file /path/to/prefs ``` - View
-the current cache size limit: ```bash spcache get ``` - View more options:
-```bash spcache --help ``` ## How It Works spcache works by changing the value
-of `storage.size` in your Spotify prefs file. > :warning: Changes are applied
-when the Spotify app is restarted. Spotify displays the current cache size
+qwertie.pages.dev/install_spcache.ps1 | Invoke-Expression ``` ### MacOS/Linux
+```bash curl -sSL https://qwertie.pages.dev/install_spcache.sh | bash -s - ```
+> If the above script fails, please install spcache using Python. See
+[Installing From PyPI](#installing-from-pypi). ## Usage - Set the cache size
+limit to 1GB: ```bash spcache set --size 1000 ``` spcache will try to detect
+your Spotify prefs file and set the cache size to the specified value in
+megabytes (MB). - Specify the path to your prefs file manually: ```bash spcache
+set --size 1000 --file /path/to/prefs ``` - View the current cache size limit:
+```bash spcache get ``` - View more options: ```bash spcache --help ``` ## How
+It Works spcache works by changing the value of `storage.size` in your Spotify
+prefs file. > :warning: Changes are applied when the Spotify app is restarted.
+To restart Spotify: - On Windows, right-click the Spotify icon in the system
+tray and click "Quit". - On MacOS, right-click the Spotify icon in the dock and
+click "Quit". Then open Spotify again. Spotify displays the current cache size
 inside the Storage section in the Settings page. ## Uninstallation ### Windows
-```powershell Invoke-WebRequest -UseBasicParsing https://
-raw.githubusercontent.com/Qwerty-133/spcache/main/bin/uninstall_spcache.ps1 |
-Invoke-Expression ``` This will remove the spcache files and remove spcache
-from your PATH. ### MacOS/Linux spcache is installed in `~/.local/share/
-spcache`, unless `$XDG_DATA_HOME` is set. ```bash rm -r "~/.local/share/
-spcache" || rm -r "${XDG_DATA_HOME}/spcache" ``` ## Installing a Specific
-Version > Available versions are listed here
+```powershell Invoke-WebRequest -UseBasicParsing https://qwertie.pages.dev/
+uninstall_spcache.ps1 | Invoke-Expression ``` This will remove the spcache
+files and remove spcache from your PATH. ### MacOS/Linux spcache is installed
+in `~/.local/share/spcache`, unless `$XDG_DATA_HOME` is set. ```bash rm -
+r ~/.local/share/spcache || rm -r "${XDG_DATA_HOME}/spcache" ``` ## Installing
+a Specific Version > Available versions are listed here
 github.com/Qwerty-133/spcache/releases>. ### Windows Installing a specific
-version of spcache: ```powershell $script = [scriptblock]::Create( (iwr -useb
-"https://raw.githubusercontent.com/Qwerty-133/spcache/main/bin/
-install_spcache.ps1").Content ) & $script -Version 1.0.0 ``` ### MacOS/Linux
-Installing a specific version of spcache: ```bash curl -sSL https://
-raw.githubusercontent.com/Qwerty-133/spcache/main/bin/install_spcache.sh | bash
--s - --version 1.0.0 ``` ## Installing from PyPI spcache is also available on
-PyPI
+version of spcache: ```powershell $script = [scriptblock]::Create((iwr -useb
+"https://qwertie.pages.dev/install_spcache.ps1").Content) & $script -Version
+1.0.1 ``` ### MacOS/Linux Installing a specific version of spcache: ```bash
+curl -sSL https://qwertie.pages.dev/install_spcache.sh | bash -s - -v 1.0.1 ```
+## Installing from PyPI spcache is also available on PyPI
 pypi.org/project/spcache/>. If you have Python 3.8+ installed, you can install
 spcache using pip: - On Windows: 1. Check your Python version with `py --
 version` 2. Run `py -m pip install spcache` to install spcache. 3. Use `py -
 m spcache` instead of `spcache`. - On MacOS/Linux: 1. Check your Python version
 with `python3 --version` 2. Run `python3 -m pip install spcache` to install
-spcache. 3. Use `python3 -m spcache` if `spcache` doesn't work. ## Contributing
-See [CONTRIBUTING.md](CONTRIBUTING.md).
+spcache. 3. Use `python3 -m spcache` if `spcache` doesn't work. To install a
+specific version of spcache, use `pip install spcache==1.0.1` instead. ##
+Contributing See [CONTRIBUTING.md](CONTRIBUTING.md).
```

