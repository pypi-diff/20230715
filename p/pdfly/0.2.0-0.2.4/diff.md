# Comparing `tmp/pdfly-0.2.0.tar.gz` & `tmp/pdfly-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfly-0.2.0.tar", last modified: Sun Jun 25 07:58:30 2023, max compression
+gzip compressed data, was "pdfly-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pdfly-0.2.0.tar` & `pdfly-0.2.4.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxr-x   0 moose     (1000) moose     (1000)        0 2023-06-25 07:58:30.675734 pdfly-0.2.0/
--rw-rw-r--   0 moose     (1000) moose     (1000)     1514 2023-03-18 14:12:20.000000 pdfly-0.2.0/LICENSE
--rw-rw-r--   0 moose     (1000) moose     (1000)     4938 2023-06-25 07:58:30.675734 pdfly-0.2.0/PKG-INFO
--rw-rw-r--   0 moose     (1000) moose     (1000)     3938 2023-03-19 13:01:13.000000 pdfly-0.2.0/README.md
-drwxrwxr-x   0 moose     (1000) moose     (1000)        0 2023-06-25 07:58:30.675734 pdfly-0.2.0/pdfly/
--rw-rw-r--   0 moose     (1000) moose     (1000)      164 2023-03-19 13:01:13.000000 pdfly-0.2.0/pdfly/__init__.py
--rw-rw-r--   0 moose     (1000) moose     (1000)      114 2023-03-18 14:12:20.000000 pdfly-0.2.0/pdfly/__main__.py
--rw-rw-r--   0 moose     (1000) moose     (1000)       87 2023-03-19 13:01:13.000000 pdfly-0.2.0/pdfly/_utils.py
--rw-rw-r--   0 moose     (1000) moose     (1000)       22 2023-06-25 07:58:27.000000 pdfly-0.2.0/pdfly/_version.py
--rw-rw-r--   0 moose     (1000) moose     (1000)     2765 2023-03-19 13:01:13.000000 pdfly-0.2.0/pdfly/cat.py
--rw-rw-r--   0 moose     (1000) moose     (1000)     4409 2023-06-25 07:58:04.000000 pdfly-0.2.0/pdfly/cli.py
--rw-rw-r--   0 moose     (1000) moose     (1000)      594 2023-03-19 13:01:13.000000 pdfly-0.2.0/pdfly/compress.py
--rw-rw-r--   0 moose     (1000) moose     (1000)      846 2023-06-08 14:12:26.000000 pdfly-0.2.0/pdfly/extract_images.py
--rw-rw-r--   0 moose     (1000) moose     (1000)     6269 2023-06-08 14:12:26.000000 pdfly-0.2.0/pdfly/metadata.py
--rw-rw-r--   0 moose     (1000) moose     (1000)     2384 2023-03-19 13:01:13.000000 pdfly-0.2.0/pdfly/pagemeta.py
--rw-rw-r--   0 moose     (1000) moose     (1000)      724 2023-03-19 13:01:13.000000 pdfly-0.2.0/pdfly/up2.py
-drwxrwxr-x   0 moose     (1000) moose     (1000)        0 2023-06-25 07:58:30.675734 pdfly-0.2.0/pdfly.egg-info/
--rw-rw-r--   0 moose     (1000) moose     (1000)     4938 2023-06-25 07:58:30.000000 pdfly-0.2.0/pdfly.egg-info/PKG-INFO
--rw-rw-r--   0 moose     (1000) moose     (1000)      414 2023-06-25 07:58:30.000000 pdfly-0.2.0/pdfly.egg-info/SOURCES.txt
--rw-rw-r--   0 moose     (1000) moose     (1000)        1 2023-06-25 07:58:30.000000 pdfly-0.2.0/pdfly.egg-info/dependency_links.txt
--rw-rw-r--   0 moose     (1000) moose     (1000)       49 2023-06-25 07:58:30.000000 pdfly-0.2.0/pdfly.egg-info/entry_points.txt
--rw-rw-r--   0 moose     (1000) moose     (1000)       47 2023-06-25 07:58:30.000000 pdfly-0.2.0/pdfly.egg-info/requires.txt
--rw-rw-r--   0 moose     (1000) moose     (1000)        6 2023-06-25 07:58:30.000000 pdfly-0.2.0/pdfly.egg-info/top_level.txt
--rw-rw-r--   0 moose     (1000) moose     (1000)     3627 2023-03-19 13:01:13.000000 pdfly-0.2.0/pyproject.toml
--rw-rw-r--   0 moose     (1000) moose     (1000)     1791 2023-06-25 07:58:30.675734 pdfly-0.2.0/setup.cfg
--rw-rw-r--   0 moose     (1000) moose     (1000)      463 2023-03-19 13:01:13.000000 pdfly-0.2.0/setup.py
+-rw-r--r--   0        0        0     1111 2023-07-15 17:09:57.538659 pdfly-0.2.4/.github/workflows/github-ci.yaml
+-rw-r--r--   0        0        0     1764 2023-07-15 17:09:57.538659 pdfly-0.2.4/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1813 2023-07-15 17:09:57.538659 pdfly-0.2.4/.gitignore
+-rw-r--r--   0        0        0      168 2023-07-15 17:09:57.538659 pdfly-0.2.4/.isort.cfg
+-rw-r--r--   0        0        0     1318 2023-07-15 17:09:57.538659 pdfly-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1514 2023-07-15 17:09:57.538659 pdfly-0.2.4/LICENSE
+-rw-r--r--   0        0        0      635 2023-07-15 17:09:57.538659 pdfly-0.2.4/Makefile
+-rw-r--r--   0        0        0     3938 2023-07-15 17:09:57.538659 pdfly-0.2.4/README.md
+-rw-r--r--   0        0        0       31 2023-07-15 17:09:57.538659 pdfly-0.2.4/mypy.ini
+-rw-r--r--   0        0        0      164 2023-07-15 17:09:57.538659 pdfly-0.2.4/pdfly/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-15 17:09:57.538659 pdfly-0.2.4/pdfly/__main__.py
+-rw-r--r--   0        0        0       87 2023-07-15 17:09:57.538659 pdfly-0.2.4/pdfly/_utils.py
+-rw-r--r--   0        0        0       22 2023-07-15 17:09:57.538659 pdfly-0.2.4/pdfly/_version.py
+-rw-r--r--   0        0        0     2765 2023-07-15 17:09:57.538659 pdfly-0.2.4/pdfly/cat.py
+-rw-r--r--   0        0        0     4409 2023-07-15 17:09:57.538659 pdfly-0.2.4/pdfly/cli.py
+-rw-r--r--   0        0        0      594 2023-07-15 17:09:57.538659 pdfly-0.2.4/pdfly/compress.py
+-rw-r--r--   0        0        0      846 2023-07-15 17:09:57.538659 pdfly-0.2.4/pdfly/extract_images.py
+-rw-r--r--   0        0        0     6276 2023-07-15 17:09:57.538659 pdfly-0.2.4/pdfly/metadata.py
+-rw-r--r--   0        0        0     2384 2023-07-15 17:09:57.538659 pdfly-0.2.4/pdfly/pagemeta.py
+-rw-r--r--   0        0        0      724 2023-07-15 17:09:57.538659 pdfly-0.2.4/pdfly/up2.py
+-rw-r--r--   0        0        0     5053 2023-07-15 17:09:57.538659 pdfly-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-07-15 17:09:57.538659 pdfly-0.2.4/requirements/ci.in
+-rw-r--r--   0        0        0     1392 2023-07-15 17:09:57.538659 pdfly-0.2.4/requirements/ci.txt
+-rw-r--r--   0        0        0       50 2023-07-15 17:09:57.538659 pdfly-0.2.4/requirements/dev.in
+-rw-r--r--   0        0        0     2440 2023-07-15 17:09:57.538659 pdfly-0.2.4/requirements/dev.txt
+-rw-r--r--   0        0        0      519 2023-07-15 17:09:57.538659 pdfly-0.2.4/setup.cfg
+-rw-r--r--   0        0        0      463 2023-07-15 17:09:57.538659 pdfly-0.2.4/setup.py
+-rw-r--r--   0        0        0     4965 1970-01-01 00:00:00.000000 pdfly-0.2.4/PKG-INFO
```

### Comparing `pdfly-0.2.0/LICENSE` & `pdfly-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.0/PKG-INFO` & `pdfly-0.2.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: pdfly
-Version: 0.2.0
+Version: 0.2.4
 Summary: A pure-python CLI application to manipulate PDF files
-Home-page: https://github.com/py-pdf/pdfly
-Author: Martin Thoma
-Author-email: info@martin-thoma.de
-Maintainer: Martin Thoma
-Maintainer-email: info@martin-thoma.de
-License: BSD-3-Clause
-Keywords: pdf,pure-python
-Platform: UNKNOWN
+Author-email: Martin Thoma <info@martin-thoma.de>
+Maintainer-email: Martin Thoma <info@martin-thoma.de>
+Requires-Python: >=3.6.1
+Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6.1
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Requires-Dist: pypdf>=3.8.2
+Requires-Dist: typer>=0.9.0
+Requires-Dist: pillow
+Requires-Dist: pydantic
+Requires-Dist: rich
+Project-URL: Source, https://github.com/py-pdf/pdfly
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI version](https://badge.fury.io/py/pdfly.svg)](https://pypi.org/project/pdfly/)
 [![GitHub last commit](https://img.shields.io/github/last-commit/py-pdf/pdfly)](https://github.com/py-pdf/pdfly)
 [![Python Support](https://img.shields.io/pypi/pyversions/pdfly.svg)](https://pypi.org/project/pdfly/)
 
 # pdfly
@@ -83,8 +82,7 @@
 │ *    out      PATH  [default: None] [required]                              │
 ╰─────────────────────────────────────────────────────────────────────────────╯
 ╭─ Options ───────────────────────────────────────────────────────────────────╮
 │ --help          Show this message and exit.                                 │
 ╰─────────────────────────────────────────────────────────────────────────────╯
 ```
 
-
```

### Comparing `pdfly-0.2.0/README.md` & `pdfly-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.0/pdfly/cat.py` & `pdfly-0.2.4/pdfly/cat.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.0/pdfly/cli.py` & `pdfly-0.2.4/pdfly/cli.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.0/pdfly/compress.py` & `pdfly-0.2.4/pdfly/compress.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.0/pdfly/extract_images.py` & `pdfly-0.2.4/pdfly/extract_images.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.0/pdfly/metadata.py` & `pdfly-0.2.4/pdfly/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class EncryptionData(BaseModel):
     revision: int
     v_value: int
 
 
 class MetaInfo(BaseModel):
-    encryption: Optional[EncryptionData]
+    encryption: Optional[EncryptionData] = None
     pdf_file_version: str
     title: Optional[str] = None
     producer: Optional[str] = None
     author: Optional[str] = None
     pages: Optional[int] = None
     page_mode: Optional[str] = None
     page_layout: Optional[str] = None
```

### Comparing `pdfly-0.2.0/pdfly/pagemeta.py` & `pdfly-0.2.4/pdfly/pagemeta.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.0/pdfly/up2.py` & `pdfly-0.2.4/pdfly/up2.py`

 * *Files identical despite different names*

