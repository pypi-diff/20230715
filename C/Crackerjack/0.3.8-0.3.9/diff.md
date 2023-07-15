# Comparing `tmp/crackerjack-0.3.8.tar.gz` & `tmp/crackerjack-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crackerjack-0.3.8.tar", last modified: Sat Jul 15 16:39:35 2023, max compression
+gzip compressed data, was "crackerjack-0.3.9.tar", last modified: Sat Jul 15 16:53:09 2023, max compression
```

## Comparing `crackerjack-0.3.8.tar` & `crackerjack-0.3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.3.8/LICENSE
--rw-r--r--   0        0        0     5917 2023-06-18 16:33:36.904528 crackerjack-0.3.8/README.md
--rw-r--r--   0        0        0      233 2023-07-15 16:10:33.153833 crackerjack-0.3.8/crackerjack/.gitignore
--rw-r--r--   0        0        0      768 2023-07-15 16:10:33.184636 crackerjack-0.3.8/crackerjack/.libcst.codemod.yaml
--rw-r--r--   0        0        0     2697 2023-07-15 16:10:33.169512 crackerjack-0.3.8/crackerjack/.pre-commit-config.yaml
--rw-r--r--   0        0        0    15547 2023-06-18 10:35:54.994502 crackerjack-0.3.8/crackerjack/.pyanalyze-report.json
--rw-r--r--   0        0        0     8180 2023-06-18 10:35:54.997907 crackerjack-0.3.8/crackerjack/.pyanalyze-report.md
--rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.3.8/crackerjack/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.3.8/crackerjack/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.3.8/crackerjack/__init__.py
--rw-r--r--   0        0        0     1559 2023-07-07 13:10:39.683493 crackerjack-0.3.8/crackerjack/__main__.py
--rw-r--r--   0        0        0     6212 2023-07-15 16:04:48.965351 crackerjack-0.3.8/crackerjack/crackerjack.py
--rw-r--r--   0        0        0     1710 2023-07-15 16:10:33.923644 crackerjack-0.3.8/crackerjack/pyproject.toml
--rw-r--r--   0        0        0     2061 2023-07-15 16:39:35.644580 crackerjack-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     6910 1970-01-01 00:00:00.000000 crackerjack-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 crackerjack-0.3.9/LICENSE
+-rw-r--r--   0        0        0     5917 2023-06-18 16:33:36.904528 crackerjack-0.3.9/README.md
+-rw-r--r--   0        0        0      233 2023-07-15 16:52:50.492164 crackerjack-0.3.9/crackerjack/.gitignore
+-rw-r--r--   0        0        0      768 2023-07-15 16:52:50.522451 crackerjack-0.3.9/crackerjack/.libcst.codemod.yaml
+-rw-r--r--   0        0        0     2703 2023-07-15 16:52:50.508196 crackerjack-0.3.9/crackerjack/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    15547 2023-06-18 10:35:54.994502 crackerjack-0.3.9/crackerjack/.pyanalyze-report.json
+-rw-r--r--   0        0        0     8180 2023-06-18 10:35:54.997907 crackerjack-0.3.9/crackerjack/.pyanalyze-report.md
+-rw-r--r--   0        0        0        1 2023-04-26 10:06:29.859090 crackerjack-0.3.9/crackerjack/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2023-04-26 10:06:29.858981 crackerjack-0.3.9/crackerjack/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      121 2023-04-25 19:43:53.234903 crackerjack-0.3.9/crackerjack/__init__.py
+-rw-r--r--   0        0        0     1559 2023-07-07 13:10:39.683493 crackerjack-0.3.9/crackerjack/__main__.py
+-rw-r--r--   0        0        0     6212 2023-07-15 16:04:48.965351 crackerjack-0.3.9/crackerjack/crackerjack.py
+-rw-r--r--   0        0        0     1710 2023-07-15 16:52:51.249742 crackerjack-0.3.9/crackerjack/pyproject.toml
+-rw-r--r--   0        0        0     2061 2023-07-15 16:53:09.705274 crackerjack-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     6910 1970-01-01 00:00:00.000000 crackerjack-0.3.9/PKG-INFO
```

### Comparing `crackerjack-0.3.8/LICENSE` & `crackerjack-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.8/README.md` & `crackerjack-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.8/crackerjack/.libcst.codemod.yaml` & `crackerjack-0.3.9/crackerjack/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.8/crackerjack/.pre-commit-config.yaml` & `crackerjack-0.3.9/crackerjack/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
       - id: codespell
         additional_dependencies:
           - tomli
   - repo: local
     hooks:
       - id: pyanalyze
         name: pyanalyze
-        entry: python -m pyanalyze
+        entry: python -m pyanalyze -v -A
         language: python
         files: \.py$
         additional_dependencies:
           - pyanalyze>=0.10.1
   - repo: local
     hooks:
       - id: autotyping
```

### Comparing `crackerjack-0.3.8/crackerjack/.pyanalyze-report.json` & `crackerjack-0.3.9/crackerjack/.pyanalyze-report.json`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.8/crackerjack/.pyanalyze-report.md` & `crackerjack-0.3.9/crackerjack/.pyanalyze-report.md`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.8/crackerjack/__main__.py` & `crackerjack-0.3.9/crackerjack/__main__.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.8/crackerjack/crackerjack.py` & `crackerjack-0.3.9/crackerjack/crackerjack.py`

 * *Files identical despite different names*

### Comparing `crackerjack-0.3.8/crackerjack/pyproject.toml` & `crackerjack-0.3.9/crackerjack/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.3.8"
+version = "0.3.9"
 description = "Crackerjack code style"
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
```

### Comparing `crackerjack-0.3.8/pyproject.toml` & `crackerjack-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 ]
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.11"
 
 [project]
 name = "Crackerjack"
-version = "0.3.8"
+version = "0.3.9"
 description = "Crackerjack code style"
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "black",
     "ruff",
     "mypy",
```

### Comparing `crackerjack-0.3.8/PKG-INFO` & `crackerjack-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Crackerjack
-Version: 0.3.8
+Version: 0.3.9
 Summary: Crackerjack code style
 Keywords: black ruff mypy creosote refurb
 Home-page: https://github.com/lesleslie/crackerjack
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Environment :: Console
```

