# Comparing `tmp/tally-token-0.1.0.tar.gz` & `tmp/tally-token-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tally-token-0.1.0.tar", last modified: Sat Jul 15 00:19:34 2023, max compression
+gzip compressed data, was "tally-token-0.2.0.tar", last modified: Sat Jul 15 01:35:28 2023, max compression
```

## Comparing `tally-token-0.1.0.tar` & `tally-token-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:19:34.581983 tally-token-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-15 00:19:04.000000 tally-token-0.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:19:34.581983 tally-token-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-15 00:19:04.000000 tally-token-0.1.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-15 00:19:04.000000 tally-token-0.1.0/.github/renovate.json5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:19:34.581983 tally-token-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-15 00:19:04.000000 tally-token-0.1.0/.github/workflows/happy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-15 00:19:04.000000 tally-token-0.1.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-15 00:19:04.000000 tally-token-0.1.0/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-15 00:19:04.000000 tally-token-0.1.0/.github/workflows/spellcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-15 00:19:04.000000 tally-token-0.1.0/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-07-15 00:19:04.000000 tally-token-0.1.0/.gitignore.in
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-15 00:19:34.581983 tally-token-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-15 00:19:04.000000 tally-token-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    39018 2023-07-15 00:19:04.000000 tally-token-0.1.0/poetry.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-15 00:19:04.000000 tally-token-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-15 00:19:34.581983 tally-token-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:19:34.581983 tally-token-0.1.0/tally_token/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-15 00:19:04.000000 tally-token-0.1.0/tally_token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-15 00:19:34.000000 tally-token-0.1.0/tally_token/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:19:34.581983 tally-token-0.1.0/tally_token.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-15 00:19:34.000000 tally-token-0.1.0/tally_token.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-15 00:19:34.000000 tally-token-0.1.0/tally_token.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 00:19:34.000000 tally-token-0.1.0/tally_token.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 00:19:34.000000 tally-token-0.1.0/tally_token.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:19:34.581983 tally-token-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-15 00:19:04.000000 tally-token-0.1.0/tests/test_basis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:35:28.607541 tally-token-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-15 01:35:08.000000 tally-token-0.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:35:28.603541 tally-token-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-15 01:35:08.000000 tally-token-0.2.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-15 01:35:08.000000 tally-token-0.2.0/.github/renovate.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:35:28.603541 tally-token-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-15 01:35:08.000000 tally-token-0.2.0/.github/workflows/happy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-15 01:35:08.000000 tally-token-0.2.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-15 01:35:08.000000 tally-token-0.2.0/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-15 01:35:08.000000 tally-token-0.2.0/.github/workflows/spellcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-15 01:35:08.000000 tally-token-0.2.0/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (123)      253 2023-07-15 01:35:08.000000 tally-token-0.2.0/.gitignore.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-15 01:35:28.607541 tally-token-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-15 01:35:08.000000 tally-token-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    39018 2023-07-15 01:35:08.000000 tally-token-0.2.0/poetry.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-15 01:35:08.000000 tally-token-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-15 01:35:28.607541 tally-token-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:35:28.603541 tally-token-0.2.0/tally_token/
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-15 01:35:08.000000 tally-token-0.2.0/tally_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-15 01:35:28.000000 tally-token-0.2.0/tally_token/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:35:28.607541 tally-token-0.2.0/tally_token.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-15 01:35:28.000000 tally-token-0.2.0/tally_token.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-15 01:35:28.000000 tally-token-0.2.0/tally_token.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 01:35:28.000000 tally-token-0.2.0/tally_token.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 01:35:28.000000 tally-token-0.2.0/tally_token.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:35:28.607541 tally-token-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-15 01:35:08.000000 tally-token-0.2.0/tests/test_basis.py
```

### Comparing `tally-token-0.1.0/.github/workflows/pypi-publish.yml` & `tally-token-0.2.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `tally-token-0.1.0/.github/workflows/python-test.yml` & `tally-token-0.2.0/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `tally-token-0.1.0/.gitignore` & `tally-token-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tally-token-0.1.0/poetry.lock` & `tally-token-0.2.0/poetry.lock`

 * *Files identical despite different names*

### Comparing `tally-token-0.1.0/pyproject.toml` & `tally-token-0.2.0/pyproject.toml`

 * *Files identical despite different names*

