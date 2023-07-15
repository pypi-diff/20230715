# Comparing `tmp/mkdocs_gitlab-1.1.0.tar.gz` & `tmp/mkdocs_gitlab-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_gitlab-1.1.0.tar", max compression
+gzip compressed data, was "mkdocs_gitlab-1.1.1.tar", max compression
```

## Comparing `mkdocs_gitlab-1.1.0.tar` & `mkdocs_gitlab-1.1.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1092 2023-07-11 08:55:32.926018 mkdocs_gitlab-1.1.0/LICENSE
--rw-r--r--   0        0        0      898 2023-07-11 08:55:32.926018 mkdocs_gitlab-1.1.0/README.md
--rw-r--r--   0        0        0       62 2023-07-11 08:55:32.926018 mkdocs_gitlab-1.1.0/mkdocs_gitlab/__init__.py
--rw-r--r--   0        0        0       22 2023-07-11 08:55:32.926018 mkdocs_gitlab-1.1.0/mkdocs_gitlab/_version.py
--rw-r--r--   0        0        0     1591 2023-07-11 08:55:32.926018 mkdocs_gitlab-1.1.0/mkdocs_gitlab/plugin.py
--rw-r--r--   0        0        0        0 2023-07-11 08:55:32.926018 mkdocs_gitlab-1.1.0/mkdocs_gitlab/py.typed
--rw-r--r--   0        0        0     2283 2023-07-11 08:55:32.930018 mkdocs_gitlab-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 mkdocs_gitlab-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-15 16:35:41.188703 mkdocs_gitlab-1.1.1/LICENSE
+-rw-r--r--   0        0        0      898 2023-07-15 16:35:41.188703 mkdocs_gitlab-1.1.1/README.md
+-rw-r--r--   0        0        0       22 2023-07-15 16:35:41.192703 mkdocs_gitlab-1.1.1/mkdocs_gitlab/__init__.py
+-rw-r--r--   0        0        0     1591 2023-07-15 16:35:41.192703 mkdocs_gitlab-1.1.1/mkdocs_gitlab/plugin.py
+-rw-r--r--   0        0        0        0 2023-07-15 16:35:41.192703 mkdocs_gitlab-1.1.1/mkdocs_gitlab/py.typed
+-rw-r--r--   0        0        0     2282 2023-07-15 16:35:41.192703 mkdocs_gitlab-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 mkdocs_gitlab-1.1.1/PKG-INFO
```

### Comparing `mkdocs_gitlab-1.1.0/LICENSE` & `mkdocs_gitlab-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_gitlab-1.1.0/README.md` & `mkdocs_gitlab-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_gitlab-1.1.0/mkdocs_gitlab/plugin.py` & `mkdocs_gitlab-1.1.1/mkdocs_gitlab/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_gitlab-1.1.0/pyproject.toml` & `mkdocs_gitlab-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.1.0"
+version = "1.1.1"
 tag_format = "$version"
 version_files = [
-    "mkdocs_gitlab/_version.py",
+    "mkdocs_gitlab/__init__.py",
     "pyproject.toml:version"
 ]
 bump_message = "chore(release): version $current_version → $new_version"
 update_changelog_on_bump = true
 
 [tool.poetry]
 name = "mkdocs-gitlab"
-version = "1.1.0"
+version = "1.1.1"
 description = "Use Gitlab CI variables for your docs"
 authors = ["Danil Akhtarov <daxartio@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/daxartio/mkdocs-gitlab"
 homepage = "https://pypi.org/project/mkdocs-gitlab"
 keywords = []
@@ -35,15 +35,15 @@
 pytest-cov = "^4.0.0"
 pytest-deadfixtures = "^2.2.1"
 pytest-mock = "^3.10.0"
 ruff = "^0.0.255"
 toml = "^0.10.2"
 
 [tool.poetry.group.git.dependencies]
-commitizen = "^2.42.1"
+commitizen = "^3.5.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 check_untyped_defs = true
```

### Comparing `mkdocs_gitlab-1.1.0/PKG-INFO` & `mkdocs_gitlab-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-gitlab
-Version: 1.1.0
+Version: 1.1.1
 Summary: Use Gitlab CI variables for your docs
 Home-page: https://pypi.org/project/mkdocs-gitlab
 License: MIT
 Author: Danil Akhtarov
 Author-email: daxartio@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

