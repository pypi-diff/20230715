# Comparing `tmp/findpython-1.0.0a2.tar.gz` & `tmp/findpython-1.0.0a3.tar.gz`

## Comparing `findpython-1.0.0a2.tar` & `findpython-1.0.0a3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 findpython-1.0.0a2/Cargo.toml
--rw-r--r--   0      501       20     3863 2023-07-12 05:46:09.000000 findpython-1.0.0a2/.github/workflows/build.yaml
--rw-r--r--   0      501       20      124 2023-07-12 05:46:09.000000 findpython-1.0.0a2/.gitignore
--rw-r--r--   0      501       20    21016 2023-07-12 05:46:09.000000 findpython-1.0.0a2/Cargo.lock
--rw-r--r--   0      501       20     1075 2023-07-12 05:46:09.000000 findpython-1.0.0a2/LICENSE
--rw-r--r--   0      501       20     4283 2023-07-12 05:46:09.000000 findpython-1.0.0a2/README.md
--rw-r--r--   0      501       20      258 2023-07-12 05:46:09.000000 findpython-1.0.0a2/pdm.lock
--rw-r--r--   0      501       20      717 2023-07-12 05:46:09.000000 findpython-1.0.0a2/pyproject.toml
--rw-r--r--   0      501       20      297 2023-07-12 05:46:09.000000 findpython-1.0.0a2/python/findpython/__init__.py
--rw-r--r--   0      501       20     3479 2023-07-12 05:46:09.000000 findpython-1.0.0a2/python/findpython/__init__.pyi
--rw-r--r--   0      501       20     2822 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/cli.rs
--rw-r--r--   0      501       20     9097 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/finder.rs
--rw-r--r--   0      501       20     2326 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/helpers.rs
--rw-r--r--   0      501       20     1934 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/lib.rs
--rw-r--r--   0      501       20      130 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/main.rs
--rw-r--r--   0      501       20     1690 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/providers/asdf.rs
--rw-r--r--   0      501       20     2222 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/providers/mod.rs
--rw-r--r--   0      501       20     1112 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/providers/path.rs
--rw-r--r--   0      501       20     1664 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/providers/pyenv.rs
--rw-r--r--   0      501       20      628 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/providers/pyobject.rs
--rw-r--r--   0      501       20     1293 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/providers/rye.rs
--rw-r--r--   0      501       20     3729 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/providers/winreg.rs
--rw-r--r--   0      501       20    14430 2023-07-12 05:46:09.000000 findpython-1.0.0a2/src/python.rs
--rw-r--r--   0        0        0     4676 1970-01-01 00:00:00.000000 findpython-1.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 findpython-1.0.0a3/Cargo.toml
+-rw-r--r--   0      501       20     3863 2023-07-12 08:26:48.000000 findpython-1.0.0a3/.github/workflows/build.yaml
+-rw-r--r--   0      501       20      124 2023-07-12 08:26:48.000000 findpython-1.0.0a3/.gitignore
+-rw-r--r--   0      501       20    21016 2023-07-12 08:26:48.000000 findpython-1.0.0a3/Cargo.lock
+-rw-r--r--   0      501       20     1075 2023-07-12 08:26:48.000000 findpython-1.0.0a3/LICENSE
+-rw-r--r--   0      501       20     4283 2023-07-12 08:26:48.000000 findpython-1.0.0a3/README.md
+-rw-r--r--   0      501       20      258 2023-07-12 08:26:48.000000 findpython-1.0.0a3/pdm.lock
+-rw-r--r--   0      501       20      717 2023-07-12 08:26:48.000000 findpython-1.0.0a3/pyproject.toml
+-rw-r--r--   0      501       20      297 2023-07-12 08:26:48.000000 findpython-1.0.0a3/python/findpython/__init__.py
+-rw-r--r--   0      501       20     3505 2023-07-12 08:26:48.000000 findpython-1.0.0a3/python/findpython/__init__.pyi
+-rw-r--r--   0      501       20     2822 2023-07-12 08:26:48.000000 findpython-1.0.0a3/src/cli.rs
+-rw-r--r--   0      501       20     9097 2023-07-12 08:26:48.000000 findpython-1.0.0a3/src/finder.rs
+-rw-r--r--   0      501       20     2326 2023-07-12 08:26:48.000000 findpython-1.0.0a3/src/helpers.rs
+-rw-r--r--   0      501       20     2000 2023-07-12 08:26:48.000000 findpython-1.0.0a3/src/lib.rs
+-rw-r--r--   0      501       20      130 2023-07-12 08:26:48.000000 findpython-1.0.0a3/src/main.rs
+-rw-r--r--   0      501       20     1690 2023-07-12 08:26:48.000000 findpython-1.0.0a3/src/providers/asdf.rs
+-rw-r--r--   0      501       20     2238 2023-07-12 08:26:48.000000 findpython-1.0.0a3/src/providers/mod.rs
+-rw-r--r--   0      501       20     1112 2023-07-12 08:26:48.000000 findpython-1.0.0a3/src/providers/path.rs
+-rw-r--r--   0      501       20     1664 2023-07-12 08:26:48.000000 findpython-1.0.0a3/src/providers/pyenv.rs
+-rw-r--r--   0      501       20      628 2023-07-12 08:26:48.000000 findpython-1.0.0a3/src/providers/pyobject.rs
+-rw-r--r--   0      501       20     1293 2023-07-12 08:26:48.000000 findpython-1.0.0a3/src/providers/rye.rs
+-rw-r--r--   0      501       20     3729 2023-07-12 08:26:48.000000 findpython-1.0.0a3/src/providers/winreg.rs
+-rw-r--r--   0      501       20    14430 2023-07-12 08:26:48.000000 findpython-1.0.0a3/src/python.rs
+-rw-r--r--   0        0        0     4676 1970-01-01 00:00:00.000000 findpython-1.0.0a3/PKG-INFO
```

### Comparing `findpython-1.0.0a2/Cargo.toml` & `findpython-1.0.0a3/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [lib]
 name = "findpython"
 crate-type = ["cdylib", "rlib"]
 
 [package]
 name = "findpython"
-version = "1.0.0-alpha.2"
+version = "1.0.0-alpha.3"
 edition = "2021"
 license = "MIT"
 authors = ["Frost Ming <me@frostming.com>"]
 readme = "README.md"
 repository = "https://github.com/frostming/findpython"
 description = "Find python executables on your system"
```

### Comparing `findpython-1.0.0a2/.github/workflows/build.yaml` & `findpython-1.0.0a3/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a2/Cargo.lock` & `findpython-1.0.0a3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -225,15 +225,15 @@
 dependencies = [
  "bit-set",
  "regex",
 ]
 
 [[package]]
 name = "findpython"
-version = "1.0.0-alpha.2"
+version = "1.0.0-alpha.3"
 dependencies = [
  "anyhow",
  "clap",
  "dirs",
  "faccess",
  "fancy-regex",
  "lazy_static",
```

### Comparing `findpython-1.0.0a2/LICENSE` & `findpython-1.0.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a2/README.md` & `findpython-1.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a2/pyproject.toml` & `findpython-1.0.0a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a2/python/findpython/__init__.pyi` & `findpython-1.0.0a3/python/findpython/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import abc
 from pathlib import Path
 from typing import Any, Sequence
 
 from _typeshed import StrPath
 
+ALL_PROVIDERS: list[str]
+
 class Version:
     dev: Any
     epoch: Any
     post: Any
     pre: Any
     release: Any
     major: Any
```

### Comparing `findpython-1.0.0a2/src/cli.rs` & `findpython-1.0.0a3/src/cli.rs`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a2/src/finder.rs` & `findpython-1.0.0a3/src/finder.rs`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a2/src/helpers.rs` & `findpython-1.0.0a3/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a2/src/lib.rs` & `findpython-1.0.0a3/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -57,19 +57,20 @@
 fn py_find_pythons_from_path(path: PathBuf, as_interpreter: bool) -> Vec<PythonVersion> {
     providers::find_pythons_from_path(&path, as_interpreter)
 }
 
 /// A Python module implemented in Rust.
 #[cfg(feature = "pyo3")]
 #[pymodule]
-fn findpython(_py: Python, m: &PyModule) -> PyResult<()> {
+fn findpython(py: Python, m: &PyModule) -> PyResult<()> {
     use pep440_rs::PyVersion;  // re-export
 
     m.add_class::<Finder>()?;
     m.add_class::<PyVersion>()?;
     m.add_class::<PythonVersion>()?;
+    m.add("ALL_PROVIDERS", providers::ALL_PROVIDERS.into_py(py))?;
     m.add_function(wrap_pyfunction!(find, m)?)?;
     m.add_function(wrap_pyfunction!(find_all, m)?)?;
     m.add_function(wrap_pyfunction!(cli_main, m)?)?;
     m.add_function(wrap_pyfunction!(py_find_pythons_from_path, m)?)?;
     Ok(())
 }
```

### Comparing `findpython-1.0.0a2/src/providers/asdf.rs` & `findpython-1.0.0a3/src/providers/asdf.rs`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a2/src/providers/mod.rs` & `findpython-1.0.0a3/src/providers/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 pub mod pyobject;
 
 #[cfg(windows)]
 mod winreg;
 
 #[cfg(windows)]
 lazy_static! {
-    pub static ref ALL_PROVIDERS: [&'static str; 4] = ["path", "pyenv", "rye", "winreg"];
+    pub static ref ALL_PROVIDERS: [&'static str; 5] = ["path", "pyenv", "rye", "asdf", "winreg"];
 }
 
 #[cfg(not(windows))]
 lazy_static! {
-    pub static ref ALL_PROVIDERS: [&'static str; 3] = ["path", "pyenv", "rye"];
+    pub static ref ALL_PROVIDERS: [&'static str; 4] = ["path", "pyenv", "rye", "asdf"];
 }
 
 pub trait Provider: Send + Sync {
     fn create() -> Option<Self>
     where
         Self: Sized;
```

### Comparing `findpython-1.0.0a2/src/providers/path.rs` & `findpython-1.0.0a3/src/providers/path.rs`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a2/src/providers/pyenv.rs` & `findpython-1.0.0a3/src/providers/pyenv.rs`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a2/src/providers/pyobject.rs` & `findpython-1.0.0a3/src/providers/pyobject.rs`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a2/src/providers/rye.rs` & `findpython-1.0.0a3/src/providers/rye.rs`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a2/src/providers/winreg.rs` & `findpython-1.0.0a3/src/providers/winreg.rs`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a2/src/python.rs` & `findpython-1.0.0a3/src/python.rs`

 * *Files identical despite different names*

### Comparing `findpython-1.0.0a2/PKG-INFO` & `findpython-1.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findpython
-Version: 1.0.0a2
+Version: 1.0.0a3
 License-File: LICENSE
 Summary: A utility to find python versions on your system
 Author: Frost Ming <me@frostming.com>
 Author-email: Frost Ming <mianghong@gmail.com>
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: findpython Version: 1.0.0a2 License-File: LICENSE
+Metadata-Version: 2.1 Name: findpython Version: 1.0.0a3 License-File: LICENSE
 Summary: A utility to find python versions on your system Author: Frost Ming
 frostming.com> Author-email: Frost Ming
 gmail.com> License: MIT Requires-Python: >=3.7 Description-Content-Type: text/
 markdown; charset=UTF-8; variant=GFM Project-URL: Source Code, https://
 github.com/frostming/findpython # FindPython _A utility to find python versions
 on your system._ [![Tests](https://github.com/frostming/findpython/actions/
 workflows/ci.yml/badge.svg)](https://github.com/frostming/findpython/actions/
```

