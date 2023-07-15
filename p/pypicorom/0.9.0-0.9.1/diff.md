# Comparing `tmp/pypicorom-0.9.0.tar.gz` & `tmp/pypicorom-0.9.1.tar.gz`

## Comparing `pypicorom-0.9.0.tar` & `pypicorom-0.9.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      246 1970-01-01 00:00:00.000000 pypicorom-0.9.0/local_dependencies/picolink/Cargo.toml
--rw-r--r--   0     1001      123    12985 2023-07-11 15:31:20.000000 pypicorom-0.9.0/local_dependencies/picolink/src/lib.rs
--rw-r--r--   0        0        0      346 1970-01-01 00:00:00.000000 pypicorom-0.9.0/Cargo.toml
--rw-r--r--   0     1001      123      325 2023-07-11 15:31:20.000000 pypicorom-0.9.0/.env/pyvenv.cfg
--rw-r--r--   0     1001      123     2807 2023-07-11 15:31:20.000000 pypicorom-0.9.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-07-11 15:31:20.000000 pypicorom-0.9.0/.gitignore
--rw-r--r--   0     1001      123      370 2023-07-11 15:31:20.000000 pypicorom-0.9.0/pyproject.toml
--rw-r--r--   0     1001      123     3923 2023-07-11 15:31:20.000000 pypicorom-0.9.0/src/lib.rs
--rw-r--r--   0     1001      123    12956 2023-07-11 15:31:25.000000 pypicorom-0.9.0/Cargo.lock
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pypicorom-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      413 1970-01-01 00:00:00.000000 pypicorom-0.9.1/local_dependencies/picolink/Cargo.toml
+-rw-r--r--   0     1001      123    12985 2023-07-15 05:39:16.000000 pypicorom-0.9.1/local_dependencies/picolink/src/lib.rs
+-rw-r--r--   0        0        0      346 1970-01-01 00:00:00.000000 pypicorom-0.9.1/Cargo.toml
+-rw-r--r--   0     1001      123      325 2023-07-15 05:39:16.000000 pypicorom-0.9.1/.env/pyvenv.cfg
+-rw-r--r--   0     1001      123     2807 2023-07-15 05:39:16.000000 pypicorom-0.9.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-07-15 05:39:16.000000 pypicorom-0.9.1/.gitignore
+-rw-r--r--   0     1001      123      370 2023-07-15 05:39:16.000000 pypicorom-0.9.1/pyproject.toml
+-rw-r--r--   0     1001      123     5066 2023-07-15 05:39:16.000000 pypicorom-0.9.1/src/lib.rs
+-rw-r--r--   0     1001      123    12290 2023-07-15 05:39:24.000000 pypicorom-0.9.1/Cargo.lock
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pypicorom-0.9.1/PKG-INFO
```

### Comparing `pypicorom-0.9.0/local_dependencies/picolink/src/lib.rs` & `pypicorom-0.9.1/local_dependencies/picolink/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pypicorom-0.9.0/.github/workflows/CI.yml` & `pypicorom-0.9.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pypicorom-0.9.0/.gitignore` & `pypicorom-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pypicorom-0.9.0/Cargo.lock` & `pypicorom-0.9.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -71,34 +71,14 @@
 [[package]]
 name = "libc"
 version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
-name = "libudev"
-version = "0.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "78b324152da65df7bb95acfcaab55e3097ceaab02fb19b228a9eb74d55f135e0"
-dependencies = [
- "libc",
- "libudev-sys",
-]
-
-[[package]]
-name = "libudev-sys"
-version = "0.1.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c8469b4a23b962c1396b9b451dda50ef5b283e8dd309d69033475fa9b334324"
-dependencies = [
- "libc",
- "pkg-config",
-]
-
-[[package]]
 name = "lock_api"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
@@ -153,15 +133,15 @@
 name = "num-derive"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e6a0fd4f737c707bd9086cc16c925f294943eb62eb71499e9fd4cf71f8b9f4e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.25",
+ "syn 2.0.26",
 ]
 
 [[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
@@ -205,20 +185,14 @@
  "anyhow",
  "num-derive",
  "num-traits",
  "serialport",
 ]
 
 [[package]]
-name = "pkg-config"
-version = "0.3.27"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
-
-[[package]]
 name = "proc-macro2"
 version = "1.0.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "78803b62cbf1f46fde80d7c0e803111524b9877184cfe7c3033659490ac7a7da"
 dependencies = [
  "unicode-ident",
 ]
@@ -282,15 +256,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pypicorom"
-version = "0.9.0"
+version = "0.9.1"
 dependencies = [
  "picolink",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
@@ -320,17 +294,17 @@
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.3.2"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "83d3daa6976cffb758ec878f108ba0e062a45b2d6ca3a2cca965338855476caf"
+checksum = "39354c10dd07468c2e73926b23bb9c2caca74c5501e38a35da70406f1d923310"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
@@ -343,23 +317,21 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serialport"
-version = "4.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "353dc2cbfc67c9a14a89a1292a9d8e819bd51066b083e08c1974ba08e3f48c62"
+version = "4.2.2-alpha.0"
+source = "git+https://github.com/wickerwaka/serialport-rs.git?rev=c14ea8611834c39390a02f0eec3efb51fc576712#c14ea8611834c39390a02f0eec3efb51fc576712"
 dependencies = [
  "CoreFoundation-sys",
  "IOKit-sys",
  "bitflags 2.0.2",
  "cfg-if",
- "libudev",
  "mach2",
  "nix",
  "regex",
  "scopeguard",
  "winapi",
 ]
 
@@ -384,17 +356,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.25"
+version = "2.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "15e3fc8c0c74267e2df136e5e5fb656a464158aa57624053375eb9c8c6e25ae2"
+checksum = "45c3457aacde3c65315de5031ec191ce46604304d2446e803d71ade03308d970"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

