# Comparing `tmp/pydantic_yaml-1.0.0a1.tar.gz` & `tmp/pydantic_yaml-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_yaml-1.0.0a1.tar", last modified: Sun Apr 23 21:25:57 2023, max compression
+gzip compressed data, was "pydantic_yaml-1.0.0a2.tar", last modified: Wed Apr 26 17:32:24 2023, max compression
```

## Comparing `pydantic_yaml-1.0.0a1.tar` & `pydantic_yaml-1.0.0a2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.226184 pydantic_yaml-1.0.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.222184 pydantic_yaml-1.0.0a1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.222184 pydantic_yaml-1.0.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/.github/workflows/python-testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-23 21:25:57.226184 pydantic_yaml-1.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.222184 pydantic_yaml-1.0.0a1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/docs/installing.md
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/docs/versioned.md
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 21:25:57.226184 pydantic_yaml-1.0.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.222184 pydantic_yaml-1.0.0a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.222184 pydantic_yaml-1.0.0a1/src/pydantic_yaml/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.226184 pydantic_yaml-1.0.0a1/src/pydantic_yaml/deprecated/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/deprecated/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.226184 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.226184 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/a-1.1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/a-1.2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/b.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/has_enums.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/recursive.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/root_list_obj.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/root_list_str.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models/uses_refs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.226184 pydantic_yaml-1.0.0a1/src/pydantic_yaml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-23 21:25:57.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-23 21:25:57.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 21:25:57.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 21:25:40.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-23 21:25:57.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-23 21:25:57.000000 pydantic_yaml-1.0.0a1/src/pydantic_yaml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:25:57.226184 pydantic_yaml-1.0.0a1/src/test/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/test/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/test/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/test/test_failures.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/test/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-23 21:25:26.000000 pydantic_yaml-1.0.0a1/src/test/test_readme.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:32:24.328222 pydantic_yaml-1.0.0a2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:32:24.320222 pydantic_yaml-1.0.0a2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:32:24.320222 pydantic_yaml-1.0.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/.github/workflows/python-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-26 17:32:24.324222 pydantic_yaml-1.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:32:24.320222 pydantic_yaml-1.0.0a2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/docs/installing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/docs/versioned.md
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 17:32:24.328222 pydantic_yaml-1.0.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:32:24.320222 pydantic_yaml-1.0.0a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:32:24.320222 pydantic_yaml-1.0.0a2/src/pydantic_yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:32:24.324222 pydantic_yaml-1.0.0a2/src/pydantic_yaml/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml/deprecated/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml/dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:32:24.324222 pydantic_yaml-1.0.0a2/src/pydantic_yaml/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:32:24.324222 pydantic_yaml-1.0.0a2/src/pydantic_yaml/examples/base_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml/examples/base_models/a-1.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml/examples/base_models/a-1.2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml/examples/base_models/a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml/examples/base_models/b.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml/examples/base_models/has_enums.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml/examples/base_models/recursive.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml/examples/base_models/root_list_obj.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml/examples/base_models/root_list_str.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml/examples/base_models/uses_refs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml/examples/base_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:32:24.324222 pydantic_yaml-1.0.0a2/src/pydantic_yaml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-04-26 17:32:24.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-26 17:32:24.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:32:24.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:32:04.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-26 17:32:24.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 17:32:24.000000 pydantic_yaml-1.0.0a2/src/pydantic_yaml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:32:24.324222 pydantic_yaml-1.0.0a2/src/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/test/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/test/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/test/test_failures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/test/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-26 17:31:48.000000 pydantic_yaml-1.0.0a2/src/test/test_readme.py
```

### Comparing `pydantic_yaml-1.0.0a1/.github/dependabot.yml` & `pydantic_yaml-1.0.0a2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pydantic_yaml-1.0.0a1/.github/workflows/python-publish.yml` & `pydantic_yaml-1.0.0a2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pydantic_yaml-1.0.0a1/.github/workflows/python-testing.yml` & `pydantic_yaml-1.0.0a2/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `pydantic_yaml-1.0.0a1/.pre-commit-config.yaml` & `pydantic_yaml-1.0.0a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydantic_yaml-1.0.0a1/LICENSE` & `pydantic_yaml-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_yaml-1.0.0a1/PKG-INFO` & `pydantic_yaml-1.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic_yaml
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Adds some YAML functionality to the excellent `pydantic` library.
 Author-email: NowanIlfideme <git@nowan.dev>
 License: MIT License
         
         Copyright (c) 2020 Anatoly Makarevich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pydantic_yaml-1.0.0a1/README.md` & `pydantic_yaml-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_yaml-1.0.0a1/docs/index.md` & `pydantic_yaml-1.0.0a2/docs/index.md`

 * *Files identical despite different names*

### Comparing `pydantic_yaml-1.0.0a1/docs/installing.md` & `pydantic_yaml-1.0.0a2/docs/installing.md`

 * *Files identical despite different names*

### Comparing `pydantic_yaml-1.0.0a1/docs/versioned.md` & `pydantic_yaml-1.0.0a2/docs/versioned.md`

 * *Files identical despite different names*

### Comparing `pydantic_yaml-1.0.0a1/mkdocs.yml` & `pydantic_yaml-1.0.0a2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pydantic_yaml-1.0.0a1/pyproject.toml` & `pydantic_yaml-1.0.0a2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 urls = { github = "https://github.com/NowanIlfideme/pydantic-yaml", docs = "https://pydantic-yaml.readthedocs.io/en/latest/" }
 
 [project.optional-dependencies]
 dev = [
     "setuptools>=61.0.0",
     "setuptools-scm[toml]>=6.2",
     "pre-commit==2.21.0",
-    "ruff==0.0.262",
+    "ruff==0.0.263",
     "black==23.3.0",
     "mypy==1.2.0",
     "pytest==7.3.1",
 ]
 docs = [
     "mkdocs",
     "mkdocs-material",
```

### Comparing `pydantic_yaml-1.0.0a1/src/pydantic_yaml/__init__.py` & `pydantic_yaml-1.0.0a2/src/pydantic_yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_yaml-1.0.0a1/src/pydantic_yaml/deprecated/types.py` & `pydantic_yaml-1.0.0a2/src/pydantic_yaml/deprecated/types.py`

 * *Files identical despite different names*

### Comparing `pydantic_yaml-1.0.0a1/src/pydantic_yaml/dumper.py` & `pydantic_yaml-1.0.0a2/src/pydantic_yaml/dumper.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 def _chk_model(model: Any) -> BaseModel:
     """Ensure the model passed is a Pydantic model."""
     if isinstance(model, BaseModel):
         return model
     raise TypeError(f"We can currently only write `pydantic.BaseModel`, but recieved: {model!r}")
 
 
-def _write_yaml_model(stream: IOBase, model: BaseModel, **kwargs):
+def _write_yaml_model(stream: IOBase, model: BaseModel, **kwargs) -> None:
     """Write YAML model to the stream object.
 
     This uses JSON dumping as an intermediary.
 
     Parameters
     ----------
     stream : IOBase
@@ -84,14 +84,15 @@
     -----
     This currently uses JSON dumping as an intermediary.
     This means that you can use `json_encoders` in your model.
     """
     model = _chk_model(model)
     if isinstance(file, IOBase):
         _write_yaml_model(file, model, **kwargs)
+        return
 
     if isinstance(file, str):
         file = Path(file).resolve()
     elif isinstance(file, Path):
         file = file.resolve()
     else:
         raise TypeError(f"Expected Path, str, or stream, but got {file!r}")
```

### Comparing `pydantic_yaml-1.0.0a1/src/pydantic_yaml/examples/base_models.py` & `pydantic_yaml-1.0.0a2/src/pydantic_yaml/examples/base_models.py`

 * *Files identical despite different names*

### Comparing `pydantic_yaml-1.0.0a1/src/pydantic_yaml/loader.py` & `pydantic_yaml-1.0.0a2/src/pydantic_yaml/loader.py`

 * *Files identical despite different names*

### Comparing `pydantic_yaml-1.0.0a1/src/pydantic_yaml/version.py` & `pydantic_yaml-1.0.0a2/src/pydantic_yaml/version.py`

 * *Files identical despite different names*

### Comparing `pydantic_yaml-1.0.0a1/src/pydantic_yaml.egg-info/PKG-INFO` & `pydantic_yaml-1.0.0a2/src/pydantic_yaml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-yaml
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Adds some YAML functionality to the excellent `pydantic` library.
 Author-email: NowanIlfideme <git@nowan.dev>
 License: MIT License
         
         Copyright (c) 2020 Anatoly Makarevich
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pydantic_yaml-1.0.0a1/src/pydantic_yaml.egg-info/SOURCES.txt` & `pydantic_yaml-1.0.0a2/src/pydantic_yaml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydantic_yaml-1.0.0a1/src/test/test_basic.py` & `pydantic_yaml-1.0.0a2/src/test/test_basic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Tests for basic functionality."""
 
+from pathlib import Path
 from typing import Type
 
 import pydantic
 import pytest
 from pydantic import BaseModel
 
-from pydantic_yaml import parse_yaml_file_as, parse_yaml_raw_as, to_yaml_str
+from pydantic_yaml import parse_yaml_file_as, parse_yaml_raw_as, to_yaml_str, to_yaml_file
 from pydantic_yaml.examples.base_models import (
     A,
     B,
     CustomRootListObj,
     CustomRootListStr,
     Empty,
     HasEnums,
@@ -73,7 +74,13 @@
     assert sm.ss.get_secret_value() == "123"
     assert sm.sb.get_secret_value() == b"321"
 
     raw = to_yaml_str(sm)
     mdl = parse_yaml_raw_as(SecretTstModelDumpable, raw)
     assert mdl.ss.get_secret_value() == "123"
     assert mdl.sb.get_secret_value() == b"321"
+
+
+def test_write_open_file(tmpdir):
+    """Test writing to a pre-opened file."""
+    with (Path(tmpdir) / "test_write_open_file.yaml").open(mode="w") as f:
+        to_yaml_file(f, A(a="a"))
```

### Comparing `pydantic_yaml-1.0.0a1/src/test/test_failures.py` & `pydantic_yaml-1.0.0a2/src/test/test_failures.py`

 * *Files identical despite different names*

### Comparing `pydantic_yaml-1.0.0a1/src/test/test_readme.py` & `pydantic_yaml-1.0.0a2/src/test/test_readme.py`

 * *Files identical despite different names*

