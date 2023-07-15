# Comparing `tmp/crl_checker-1.0.8.tar.gz` & `tmp/crl_checker-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crl_checker-1.0.8.tar", max compression
+gzip compressed data, was "crl_checker-1.0.9.tar", max compression
```

## Comparing `crl_checker-1.0.8.tar` & `crl_checker-1.0.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1096 2023-06-05 20:23:06.503595 crl_checker-1.0.8/LICENSE
--rw-r--r--   0        0        0     1251 2023-06-05 20:23:06.503595 crl_checker-1.0.8/README.md
--rw-r--r--   0        0        0     1897 2023-06-05 20:23:06.503595 crl_checker-1.0.8/crl_checker/__init__.py
--rw-r--r--   0        0        0     1669 2023-06-05 20:23:13.850164 crl_checker-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     2382 1970-01-01 00:00:00.000000 crl_checker-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-07-15 09:03:33.334474 crl_checker-1.0.9/LICENSE
+-rw-r--r--   0        0        0     1251 2023-07-15 09:03:33.334474 crl_checker-1.0.9/README.md
+-rw-r--r--   0        0        0     1897 2023-07-15 09:03:33.334474 crl_checker-1.0.9/crl_checker/__init__.py
+-rw-r--r--   0        0        0     1669 2023-07-15 09:03:46.038547 crl_checker-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2382 1970-01-01 00:00:00.000000 crl_checker-1.0.9/PKG-INFO
```

### Comparing `crl_checker-1.0.8/LICENSE` & `crl_checker-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crl_checker-1.0.8/README.md` & `crl_checker-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `crl_checker-1.0.8/crl_checker/__init__.py` & `crl_checker-1.0.9/crl_checker/__init__.py`

 * *Files identical despite different names*

### Comparing `crl_checker-1.0.8/pyproject.toml` & `crl_checker-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crl-checker"
-version = "1.0.8"
+version = "1.0.9"
 description = "Check if certificate is revoked using the x509 CRL extension"
 authors = ["Michal Sadowski <misad90@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
```

### Comparing `crl_checker-1.0.8/PKG-INFO` & `crl_checker-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crl-checker
-Version: 1.0.8
+Version: 1.0.9
 Summary: Check if certificate is revoked using the x509 CRL extension
 Home-page: https://github.com/fulder/crl-checker
 License: MIT
 Author: Michal Sadowski
 Author-email: misad90@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

