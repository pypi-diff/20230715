# Comparing `tmp/ghastoolkit-0.4.7.tar.gz` & `tmp/ghastoolkit-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.4.7.tar", last modified: Fri Jul 14 12:47:52 2023, max compression
+gzip compressed data, was "ghastoolkit-0.5.0.tar", last modified: Sat Jul 15 17:25:12 2023, max compression
```

## Comparing `ghastoolkit-0.4.7.tar` & `ghastoolkit-0.5.0.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.464295 ghastoolkit-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-14 12:47:52.464295 ghastoolkit-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 12:47:52.464295 ghastoolkit-0.4.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.444294 ghastoolkit-0.4.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.448294 ghastoolkit-0.4.7/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.452294 ghastoolkit-0.4.7/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.456295 ghastoolkit-0.4.7/src/ghastoolkit/codeql/dataextensions/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/dataextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/dataextensions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/dataextensions/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/dataextensions/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/codeql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.456295 ghastoolkit-0.4.7/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/octokit/clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/octokit/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.456295 ghastoolkit-0.4.7/src/ghastoolkit/octokit/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/octokit/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.460295 ghastoolkit-0.4.7/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.460295 ghastoolkit-0.4.7/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.452294 ghastoolkit-0.4.7/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-14 12:47:52.000000 ghastoolkit-0.4.7/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-14 12:47:52.000000 ghastoolkit-0.4.7/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:47:52.000000 ghastoolkit-0.4.7/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-14 12:47:52.000000 ghastoolkit-0.4.7/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 12:47:52.000000 ghastoolkit-0.4.7/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:47:52.464295 ghastoolkit-0.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_codeql_dataext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-14 12:47:19.000000 ghastoolkit-0.4.7/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.622526 ghastoolkit-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-15 17:25:12.622526 ghastoolkit-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 17:25:12.622526 ghastoolkit-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.614526 ghastoolkit-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.618526 ghastoolkit-0.5.0/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.618526 ghastoolkit-0.5.0/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.618526 ghastoolkit-0.5.0/src/ghastoolkit/codeql/dataextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/dataextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/dataextensions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/dataextensions/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/dataextensions/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.618526 ghastoolkit-0.5.0/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/octokit/clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/octokit/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.618526 ghastoolkit-0.5.0/src/ghastoolkit/octokit/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/octokit/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.618526 ghastoolkit-0.5.0/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.622526 ghastoolkit-0.5.0/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.618526 ghastoolkit-0.5.0/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-15 17:25:12.000000 ghastoolkit-0.5.0/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-15 17:25:12.000000 ghastoolkit-0.5.0/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 17:25:12.000000 ghastoolkit-0.5.0/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-15 17:25:12.000000 ghastoolkit-0.5.0/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 17:25:12.000000 ghastoolkit-0.5.0/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.622526 ghastoolkit-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_codeql_dataext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.4.7/LICENSE` & `ghastoolkit-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/PKG-INFO` & `ghastoolkit-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.4.7
+Version: 0.5.0
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.4.7/README.md` & `ghastoolkit-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/pyproject.toml` & `ghastoolkit-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.4.7"
+version = "0.5.0"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/__init__.py` & `ghastoolkit-0.5.0/src/ghastoolkit/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.4.7"
+__version__ = "0.5.0"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
@@ -29,15 +29,15 @@
 from ghastoolkit.octokit.github import GitHub, Repository
 from ghastoolkit.octokit.octokit import Octokit, RestRequest, GraphQLRequest
 from ghastoolkit.octokit.codescanning import CodeScanning, CodeAlert
 from ghastoolkit.octokit.secretscanning import SecretScanning, SecretAlert
 from ghastoolkit.octokit.dependencygraph import DependencyGraph
 
 # Supply Chain
-from ghastoolkit.supplychain.advisories import Advisory
+from ghastoolkit.supplychain.advisories import Advisory, Advisories
 from ghastoolkit.supplychain.dependencyalert import DependencyAlert
 from ghastoolkit.supplychain.dependencies import Dependency, Dependencies
 from ghastoolkit.supplychain.licensing import Licenses
 
 # CodeQL
 from ghastoolkit.codeql.databases import CodeQLDatabases, CodeQLDatabase
 from ghastoolkit.codeql.cli import CodeQL
```

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/__main__.py` & `ghastoolkit-0.5.0/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/codeql/cli.py` & `ghastoolkit-0.5.0/src/ghastoolkit/codeql/cli.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.5.0/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/codeql/dataextensions/__main__.py` & `ghastoolkit-0.5.0/src/ghastoolkit/codeql/dataextensions/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,30 @@
+import logging
 import os
 import argparse
 from ghastoolkit.codeql.dataextensions.ext import DataExtensions
 
+logging.basicConfig(format="%(message)s")
 parser = argparse.ArgumentParser("ghastoolkit-codeql-dataextensions")
 parser.add_argument("-l", "--language", required=True)
 parser.add_argument("-i", "--input", required=True)
+
 args = parser.parse_args()
 
 de = DataExtensions(args.language)
 
 if os.path.isfile(args.input):
     de.load(args.input)
 elif os.path.isdir(args.input):
     for root, dirs, files in os.walk(args.input):
         for fl in files:
             path = os.path.join(root, fl)
             _, ext = os.path.splitext(fl)
             if ext in [".yml", ".yaml"]:
                 de.load(path)
 
-print(f" Language   :: {args.language} (loaded: {len(de.paths)})")
-print()
-print(f" Sources    :: {len(de.sources)}")
-print(f" Sinks      :: {len(de.sinks)}")
-print(f" Summaries  :: {len(de.summaries)}")
-print(f" Types      :: {len(de.types)}")
-print(f" Neutrals   :: {len(de.neutrals)}")
+logging.info(f" Language   :: {args.language} (loaded: {len(de.paths)})")
+logging.info(f" Sources    :: {len(de.sources)}")
+logging.info(f" Sinks      :: {len(de.sinks)}")
+logging.info(f" Summaries  :: {len(de.summaries)}")
+logging.info(f" Types      :: {len(de.types)}")
+logging.info(f" Neutrals   :: {len(de.neutrals)}")
```

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/codeql/dataextensions/ext.py` & `ghastoolkit-0.5.0/src/ghastoolkit/codeql/dataextensions/ext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/codeql/dataextensions/models.py` & `ghastoolkit-0.5.0/src/ghastoolkit/codeql/dataextensions/models.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/codeql/results.py` & `ghastoolkit-0.5.0/src/ghastoolkit/codeql/results.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/octokit/clearlydefined.py` & `ghastoolkit-0.5.0/src/ghastoolkit/octokit/clearlydefined.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.5.0/src/ghastoolkit/octokit/codescanning.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,47 +6,60 @@
 from ghastoolkit.octokit.octokit import OctoItem, RestRequest
 
 logger = logging.getLogger("ghastoolkit.octokit.codescanning")
 
 
 @dataclass
 class CodeAlert(OctoItem):
+    """Code Alert from Code Scanning API"""
+
     number: int
+    """Unique Identifier"""
     state: str
+    """State of the alert. States can be `open`, `closed`, `dismissed`, or `fixed`."""
 
     created_at: str
+    """Alert Creation date and time"""
 
     rule: dict
+    """Rule Data (rule_id, severity, description, etc)"""
     tool: dict
+    """Tool information (name, version, guid)"""
 
     _instances: Optional[list[dict]] = None
 
     @property
     def rule_id(self) -> str:
+        """Rule Identifier"""
         return self.rule.get("id", "NA")
 
     @property
     def description(self) -> Optional[str]:
+        """Rule Description / Title"""
         return self.rule.get("description")
 
     @property
     def tool_name(self) -> str:
+        """Tool name"""
         return self.tool.get("name", "NA")
 
     @property
     def tool_fullname(self) -> str:
+        """Full tool name with version information"""
         version = self.tool.get("version")
         return f"{self.tool_name}@{version}"
 
     @property
     def severity(self) -> str:
+        """Severity of the alert using `security_severity_level`"""
         return self.rule.get("security_severity_level", "NA")
 
     @property
     def instances(self) -> list[dict]:
+        """Get list of instances of the alert"""
         if not self._instances:
             self._instances = CodeScanning().getAlertInstances(self.number)
         return self._instances
 
     def __str__(self) -> str:
         return f"CodeAlert({self.number}, '{self.state}', '{self.tool_name}', '{self.rule_id}')"
 
@@ -72,27 +85,39 @@
         results = self.rest.get(
             "/orgs/{org}/code-scanning/alerts", {"state": state}, authenticated=True
         )
         if isinstance(results, list):
             return results
         raise Exception(f"Error getting alerts from Organization")
 
-    @RestRequest.restGet(
-        "/repos/{owner}/{repo}/code-scanning/alerts", authenticated=True
-    )
     def getAlerts(
         self,
         state: str = "open",
         tool_name: Optional[str] = None,
         ref: Optional[str] = None,
+        sort: Optional[str] = None,
+        severity: Optional[str] = None,
     ) -> list[CodeAlert]:
         """Get all code scanning alerts
         https://docs.github.com/en/rest/code-scanning#list-code-scanning-alerts-for-a-repository
         """
-        return []
+        results = self.rest.get(
+            "/repos/{owner}/{repo}/code-scanning/alerts",
+            {
+                "state": state,
+                "tool_name": tool_name,
+                "ref": ref,
+                "sort": sort,
+                "severity": severity,
+            },
+            authenticated=True,
+        )
+        if isinstance(results, list):
+            return results
+        raise Exception(f"Error getting alerts from Repository")
 
     def getAlertsInPR(self, base: str) -> list[CodeAlert]:
         """Get the open alerts in a Pull Request (delta / diff).
 
         Note this operation is slow due to it needing to lookup each alert instance
         information.
 
@@ -112,32 +137,35 @@
                 results.append(alert)
         return results
 
     @RestRequest.restGet(
         "/repos/{owner}/{repo}/code-scanning/alerts/{alert_number}", authenticated=True
     )
     def getAlert(self, alert_number: int) -> CodeAlert:
-        """Get Single Alert
+        """Get Single Alert information from Code Scanning
+
         https://docs.github.com/en/rest/code-scanning#get-a-code-scanning-alert
         """
         return {}
 
     def getAlertInstances(
         self, alert_number: int, ref: Optional[str] = None
     ) -> list[dict]:
+        """Get a list of alert instances"""
         result = self.rest.get(
             "/repos/{owner}/{repo}/code-scanning/alerts/{alert_number}/instances",
             {"alert_number": alert_number, "ref": ref},
         )
         return result
 
     def getAnalyses(
         self, reference: Optional[str] = None, tool: Optional[str] = None
     ) -> list[dict]:
-        """Get a list of analyses for a repository
+        """Get a list of all the analyses for a given repository
+
         https://docs.github.com/en/enterprise-cloud@latest/rest/code-scanning#list-code-scanning-analyses-for-a-repository
         """
         results = self.rest.get(
             "/repos/{org}/{repo}/code-scanning/analyses",
             {"tool_name": tool, "ref": reference or self.repository.reference},
         )
         if isinstance(results, list):
@@ -199,13 +227,14 @@
 
         https://docs.github.com/en/rest/code-scanning?apiVersion=2022-11-28#list-codeql-databases-for-a-repository
         """
         return self.rest.get("/repos/{owner}/{repo}/code-scanning/codeql/databases")
 
     def getCodeQLDatabase(self, language: str) -> dict:
         """Get a CodeQL database for a repository
+
         https://docs.github.com/en/rest/code-scanning?apiVersion=2022-11-28#get-a-codeql-database-for-a-repository
         """
         return self.rest.get(
             "/repos/{owner}/{repo}/code-scanning/codeql/databases/{language}",
             {"language": language},
         )
```

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.5.0/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.5.0/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.5.0/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/octokit/graphql/__init__.py` & `ghastoolkit-0.5.0/src/ghastoolkit/octokit/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.5.0/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.5.0/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.5.0/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.5.0/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.5.0/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.5.0/src/ghastoolkit/supplychain/licensing.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.5.0/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.4.7
+Version: 0.5.0
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.4.7/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.5.0/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 src/ghastoolkit/secretscanning/__init__.py
 src/ghastoolkit/secretscanning/secretalerts.py
 src/ghastoolkit/supplychain/__init__.py
 src/ghastoolkit/supplychain/advisories.py
 src/ghastoolkit/supplychain/dependencies.py
 src/ghastoolkit/supplychain/dependencyalert.py
 src/ghastoolkit/supplychain/licensing.py
+tests/test_advisories.py
 tests/test_clearlydefined.py
 tests/test_codeql_dataext.py
 tests/test_codeqldb.py
 tests/test_codescanning.py
 tests/test_default.py
 tests/test_dependencies.py
 tests/test_depgraph.py
```

### Comparing `ghastoolkit-0.4.7/tests/test_codeql_dataext.py` & `ghastoolkit-0.5.0/tests/test_codeql_dataext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/tests/test_codeqldb.py` & `ghastoolkit-0.5.0/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/tests/test_codescanning.py` & `ghastoolkit-0.5.0/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/tests/test_default.py` & `ghastoolkit-0.5.0/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/tests/test_dependencies.py` & `ghastoolkit-0.5.0/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/tests/test_depgraph.py` & `ghastoolkit-0.5.0/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/tests/test_github.py` & `ghastoolkit-0.5.0/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/tests/test_licenses.py` & `ghastoolkit-0.5.0/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/tests/test_octokit.py` & `ghastoolkit-0.5.0/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.4.7/tests/test_secretscanning.py` & `ghastoolkit-0.5.0/tests/test_secretscanning.py`

 * *Files identical despite different names*

