# Comparing `tmp/pywinpty-2.0.8.tar.gz` & `tmp/pywinpty-2.0.9.tar.gz`

## Comparing `pywinpty-2.0.8.tar` & `pywinpty-2.0.9.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      665 1970-01-01 00:00:00.000000 pywinpty-2.0.8/Cargo.toml
--rw-r--r--   0     1001      121      409 2022-09-16 00:04:58.000000 pywinpty-2.0.8/.github/dependabot.yml
--rw-r--r--   0     1001      121      328 2022-09-16 00:04:58.000000 pywinpty-2.0.8/.github/scripts/copy_winpty.sh
--rw-r--r--   0     1001      121     1482 2022-09-16 00:04:58.000000 pywinpty-2.0.8/.github/workflows/linux_sdist.yml
--rw-r--r--   0     1001      121     3121 2022-09-16 00:04:58.000000 pywinpty-2.0.8/.github/workflows/windows_build.yml
--rw-r--r--   0     1001      121     1866 2022-09-16 00:04:58.000000 pywinpty-2.0.8/.github/workflows/windows_release.yml
--rw-r--r--   0     1001      121     1351 2022-09-16 00:04:58.000000 pywinpty-2.0.8/.gitignore
--rw-r--r--   0     1001      121    32123 2022-09-16 00:04:58.000000 pywinpty-2.0.8/CHANGELOG.md
--rw-r--r--   0     1001      121     1067 2022-09-16 00:04:58.000000 pywinpty-2.0.8/LICENSE.txt
--rw-r--r--   0     1001      121      124 2022-09-16 00:04:58.000000 pywinpty-2.0.8/MANIFEST.in
--rw-r--r--   0     1001      121     4588 2022-09-16 00:04:58.000000 pywinpty-2.0.8/README.md
--rw-r--r--   0     1001      121      818 2022-09-16 00:04:58.000000 pywinpty-2.0.8/RELEASE.md
--rw-r--r--   0     1001      121      133 2022-09-16 00:04:58.000000 pywinpty-2.0.8/pyproject.toml
--rw-r--r--   0     1001      121     1266 2022-09-16 00:04:58.000000 pywinpty-2.0.8/runtests.py
--rw-r--r--   0     1001      121    12409 2022-09-16 00:04:58.000000 pywinpty-2.0.8/src/lib.rs
--rw-r--r--   0     1001      121      379 2022-09-16 00:04:58.000000 pywinpty-2.0.8/winpty/__init__.py
--rw-r--r--   0     1001      121     1805 2022-09-16 00:04:58.000000 pywinpty-2.0.8/winpty/enums.py
--rw-r--r--   0     1001      121    11634 2022-09-16 00:04:58.000000 pywinpty-2.0.8/winpty/ptyprocess.py
--rw-r--r--   0     1001      121       51 2022-09-16 00:04:58.000000 pywinpty-2.0.8/winpty/tests/__init__.py
--rw-r--r--   0     1001      121     3566 2022-09-16 00:04:58.000000 pywinpty-2.0.8/winpty/tests/test_pty.py
--rw-r--r--   0     1001      121     5655 2022-09-16 00:04:58.000000 pywinpty-2.0.8/winpty/tests/test_ptyprocess.py
--rw-r--r--   0     1001      121     1366 2022-09-16 00:04:58.000000 pywinpty-2.0.8/winpty/winpty.pyi
--rw-r--r--   0        0        0     5063 1970-01-01 00:00:00.000000 pywinpty-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0      665 1970-01-01 00:00:00.000000 pywinpty-2.0.9/Cargo.toml
+-rw-r--r--   0     1001      121      409 2022-10-26 21:28:26.000000 pywinpty-2.0.9/.github/dependabot.yml
+-rw-r--r--   0     1001      121      328 2022-10-26 21:28:26.000000 pywinpty-2.0.9/.github/scripts/copy_winpty.sh
+-rw-r--r--   0     1001      121     1483 2022-10-26 21:28:26.000000 pywinpty-2.0.9/.github/workflows/linux_sdist.yml
+-rw-r--r--   0     1001      121     3129 2022-10-26 21:28:26.000000 pywinpty-2.0.9/.github/workflows/windows_build.yml
+-rw-r--r--   0     1001      121     1874 2022-10-26 21:28:26.000000 pywinpty-2.0.9/.github/workflows/windows_release.yml
+-rw-r--r--   0     1001      121     1351 2022-10-26 21:28:26.000000 pywinpty-2.0.9/.gitignore
+-rw-r--r--   0     1001      121    33473 2022-10-26 21:28:26.000000 pywinpty-2.0.9/CHANGELOG.md
+-rw-r--r--   0     1001      121     1067 2022-10-26 21:28:26.000000 pywinpty-2.0.9/LICENSE.txt
+-rw-r--r--   0     1001      121      124 2022-10-26 21:28:26.000000 pywinpty-2.0.9/MANIFEST.in
+-rw-r--r--   0     1001      121     4588 2022-10-26 21:28:26.000000 pywinpty-2.0.9/README.md
+-rw-r--r--   0     1001      121      818 2022-10-26 21:28:26.000000 pywinpty-2.0.9/RELEASE.md
+-rw-r--r--   0     1001      121      133 2022-10-26 21:28:26.000000 pywinpty-2.0.9/pyproject.toml
+-rw-r--r--   0     1001      121     1266 2022-10-26 21:28:26.000000 pywinpty-2.0.9/runtests.py
+-rw-r--r--   0     1001      121    12409 2022-10-26 21:28:26.000000 pywinpty-2.0.9/src/lib.rs
+-rw-r--r--   0     1001      121      379 2022-10-26 21:28:26.000000 pywinpty-2.0.9/winpty/__init__.py
+-rw-r--r--   0     1001      121     1805 2022-10-26 21:28:26.000000 pywinpty-2.0.9/winpty/enums.py
+-rw-r--r--   0     1001      121    11634 2022-10-26 21:28:26.000000 pywinpty-2.0.9/winpty/ptyprocess.py
+-rw-r--r--   0     1001      121       51 2022-10-26 21:28:26.000000 pywinpty-2.0.9/winpty/tests/__init__.py
+-rw-r--r--   0     1001      121     3566 2022-10-26 21:28:26.000000 pywinpty-2.0.9/winpty/tests/test_pty.py
+-rw-r--r--   0     1001      121     5655 2022-10-26 21:28:26.000000 pywinpty-2.0.9/winpty/tests/test_ptyprocess.py
+-rw-r--r--   0     1001      121     1366 2022-10-26 21:28:26.000000 pywinpty-2.0.9/winpty/winpty.pyi
+-rw-r--r--   0     1001      121    10040 2022-10-26 21:30:14.000000 pywinpty-2.0.9/Cargo.lock
+-rw-r--r--   0        0        0     5063 1970-01-01 00:00:00.000000 pywinpty-2.0.9/PKG-INFO
```

### Comparing `pywinpty-2.0.8/Cargo.toml` & `pywinpty-2.0.9/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [package]
 name = "pywinpty"
-version = "2.0.8"
+version = "2.0.9"
 authors = ["Edgar Andrés Margffoy Tuay <andfoy@gmail.com>"]
 description = "Pseudo terminal support for Windows from Python."
 repository = "https://github.com/spyder-ide/pywinpty"
 license = "MIT"
 keywords = ["pty", "pseudo-terminal", "conpty", "windows", "winpty"]
 readme = "README.md"
 edition = "2021"
 
 [lib]
 name = "winpty"
 crate-type = ["cdylib"]
 
 [dependencies]
-winpty-rs = "0.3.8"
+winpty-rs = "0.3.9"
 
 [dependencies.pyo3]
 version = "0.17.1"
 features = ["extension-module"]
 
 [package.metadata.docs.rs]
 default-target = "x86_64-pc-windows-msvc"
```

### Comparing `pywinpty-2.0.8/.github/workflows/linux_sdist.yml` & `pywinpty-2.0.9/.github/workflows/linux_sdist.yml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         runs-on: ubuntu-latest
         env:
             PYTHON_VERSION: ${{ matrix.PYTHON_VERSION }}
             RUNNER_OS: "linux"
         strategy:
             fail-fast: false
             matrix:
-                PYTHON_VERSION: ["3.9"]
+                PYTHON_VERSION: ["3.10"]
         steps:
           - name: Checkout branch
             uses: actions/checkout@v3
           - name: Install latest Rust stable
             uses: actions-rs/toolchain@v1
             with:
               toolchain: stable
```

### Comparing `pywinpty-2.0.8/.github/workflows/windows_build.yml` & `pywinpty-2.0.9/.github/workflows/windows_build.yml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             PYTHON_VERSION: ${{ matrix.PYTHON_VERSION }}
             RUNNER_OS: "windows"
             PYWINPTY_BLOCK: "1"
             CI_RUNNING: "1"
         strategy:
             fail-fast: false
             matrix:
-                PYTHON_VERSION: ["3.7", "3.8", "3.9", "3.10"]
+                PYTHON_VERSION: ["3.7", "3.8", "3.9", "3.10", "3.11"]
         steps:
             - name: Checkout branch
               uses: actions/checkout@v3
             - name: Install latest Rust stable
               uses: actions-rs/toolchain@v1
               with:
                 toolchain: stable
```

### Comparing `pywinpty-2.0.8/.github/workflows/windows_release.yml` & `pywinpty-2.0.9/.github/workflows/windows_release.yml`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         runs-on: windows-latest
         env:
             PYTHON_VERSION: ${{ matrix.PYTHON_VERSION }}
             RUNNER_OS: "windows"
         strategy:
             fail-fast: false
             matrix:
-                PYTHON_VERSION: ["3.7", "3.8", "3.9", "3.10"]
+                PYTHON_VERSION: ["3.7", "3.8", "3.9", "3.10", "3.11"]
         steps:
             - name: Checkout branch
               uses: actions/checkout@v3
             - name: Install latest Rust stable
               uses: actions-rs/toolchain@v1
               with:
                 toolchain: stable
```

### Comparing `pywinpty-2.0.8/.gitignore` & `pywinpty-2.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pywinpty-2.0.8/CHANGELOG.md` & `pywinpty-2.0.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+## Version 2.0.9 (2022/10/26)
+
+
+### Pull Requests Merged
+
+* [PR 296](https://github.com/andfoy/pywinpty/pull/296) - Enable Python 3.11 support, by [@andfoy](https://github.com/andfoy) ([295](https://github.com/andfoy/pywinpty/issues/295))
+* [PR 294](https://github.com/andfoy/pywinpty/pull/294) - Bump libc from 0.2.133 to 0.2.137, by [@dependabot[bot]](https://github.com/apps/dependabot)
+* [PR 292](https://github.com/andfoy/pywinpty/pull/292) - Bump proc-macro2 from 1.0.43 to 1.0.47, by [@dependabot[bot]](https://github.com/apps/dependabot)
+* [PR 288](https://github.com/andfoy/pywinpty/pull/288) - Bump syn from 1.0.100 to 1.0.101, by [@dependabot[bot]](https://github.com/apps/dependabot)
+* [PR 286](https://github.com/andfoy/pywinpty/pull/286) - Bump once_cell from 1.14.0 to 1.15.0, by [@dependabot[bot]](https://github.com/apps/dependabot)
+* [PR 285](https://github.com/andfoy/pywinpty/pull/285) - Bump winpty-rs from 0.3.8 to 0.3.9, by [@dependabot[bot]](https://github.com/apps/dependabot)
+* [PR 283](https://github.com/andfoy/pywinpty/pull/283) - Bump libc from 0.2.132 to 0.2.133, by [@dependabot[bot]](https://github.com/apps/dependabot)
+* [PR 282](https://github.com/andfoy/pywinpty/pull/282) - Bump syn from 1.0.99 to 1.0.100, by [@dependabot[bot]](https://github.com/apps/dependabot)
+
+In this release 8 pull requests were closed.
+
+
 ## Version 2.0.8 (2022/09/15)
 
 ### Issues Closed
 
 * [Issue 281](https://github.com/andfoy/pywinpty/issues/281) - Release v2.0.8
 
 In this release 1 issue was closed.
```

### Comparing `pywinpty-2.0.8/LICENSE.txt` & `pywinpty-2.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pywinpty-2.0.8/README.md` & `pywinpty-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pywinpty-2.0.8/RELEASE.md` & `pywinpty-2.0.9/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pywinpty-2.0.8/runtests.py` & `pywinpty-2.0.9/runtests.py`

 * *Files identical despite different names*

### Comparing `pywinpty-2.0.8/src/lib.rs` & `pywinpty-2.0.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pywinpty-2.0.8/winpty/enums.py` & `pywinpty-2.0.9/winpty/enums.py`

 * *Files identical despite different names*

### Comparing `pywinpty-2.0.8/winpty/ptyprocess.py` & `pywinpty-2.0.9/winpty/ptyprocess.py`

 * *Files identical despite different names*

### Comparing `pywinpty-2.0.8/winpty/tests/test_pty.py` & `pywinpty-2.0.9/winpty/tests/test_pty.py`

 * *Files identical despite different names*

### Comparing `pywinpty-2.0.8/winpty/tests/test_ptyprocess.py` & `pywinpty-2.0.9/winpty/tests/test_ptyprocess.py`

 * *Files identical despite different names*

### Comparing `pywinpty-2.0.8/winpty/winpty.pyi` & `pywinpty-2.0.9/winpty/winpty.pyi`

 * *Files identical despite different names*

### Comparing `pywinpty-2.0.8/PKG-INFO` & `pywinpty-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywinpty
-Version: 2.0.8
+Version: 2.0.9
 License-File: LICENSE.txt
 Summary: Pseudo terminal support for Windows from Python.
 Keywords: pty,pseudo-terminal,conpty,windows,winpty
 Author: Edgar Andrés Margffoy Tuay <andfoy@gmail.com>
 Author-email: Edgar Andrés Margffoy Tuay <andfoy@gmail.com>
 License: MIT
 Requires-Python: >=3.7
```

