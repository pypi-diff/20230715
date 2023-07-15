# Comparing `tmp/daves_utilities-0.1.1.tar.gz` & `tmp/daves_utilities-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daves_utilities-0.1.1.tar", last modified: Sun Jan  1 11:42:26 2023, max compression
+gzip compressed data, was "daves_utilities-0.1.2.tar", max compression
```

## Comparing `daves_utilities-0.1.1.tar` & `daves_utilities-0.1.2.tar`

### file list

```diff
@@ -1,42 +1,9 @@
-drwxr-xr-x   0 davidkuchelmeister   (501) staff       (20)        0 2023-01-01 11:42:26.613772 daves_utilities-0.1.1/
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)     1109 2022-12-31 16:35:12.000000 daves_utilities-0.1.1/.gitignore
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)     1167 2022-12-31 15:33:20.000000 daves_utilities-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)       92 2022-12-31 15:33:20.000000 daves_utilities-0.1.1/Dockerfile
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)        0 2022-12-31 15:33:20.000000 daves_utilities-0.1.1/Jenkinsfile
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)     1087 2022-12-31 15:33:52.000000 daves_utilities-0.1.1/LICENSE
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)     1435 2022-12-31 16:34:28.000000 daves_utilities-0.1.1/Makefile
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)      250 2023-01-01 11:42:26.613250 daves_utilities-0.1.1/PKG-INFO
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)       19 2022-12-31 15:33:52.000000 daves_utilities-0.1.1/README.md
-drwxr-xr-x   0 davidkuchelmeister   (501) staff       (20)        0 2023-01-01 11:42:26.598142 daves_utilities-0.1.1/experiments/
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)        0 2022-12-31 15:33:20.000000 daves_utilities-0.1.1/experiments/.gitkeep
-drwxr-xr-x   0 davidkuchelmeister   (501) staff       (20)        0 2023-01-01 11:42:26.599722 daves_utilities-0.1.1/helm/
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)      440 2022-12-31 15:33:20.000000 daves_utilities-0.1.1/helm/.helmignore
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)       88 2022-12-31 15:33:20.000000 daves_utilities-0.1.1/helm/Chart.yaml
-drwxr-xr-x   0 davidkuchelmeister   (501) staff       (20)        0 2023-01-01 11:42:26.600938 daves_utilities-0.1.1/helm/templates/
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)      697 2022-12-31 15:33:20.000000 daves_utilities-0.1.1/helm/templates/deployment.yaml
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)      277 2022-12-31 15:33:20.000000 daves_utilities-0.1.1/helm/templates/service.yaml
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)       11 2022-12-31 15:33:20.000000 daves_utilities-0.1.1/helm/values.yaml
-drwxr-xr-x   0 davidkuchelmeister   (501) staff       (20)        0 2023-01-01 11:42:26.601619 daves_utilities-0.1.1/models/
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)        0 2022-12-31 15:33:20.000000 daves_utilities-0.1.1/models/.gitkeep
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)      791 2022-12-31 15:49:36.000000 daves_utilities-0.1.1/pyproject.toml
-drwxr-xr-x   0 davidkuchelmeister   (501) staff       (20)        0 2023-01-01 11:42:26.602069 daves_utilities-0.1.1/reports/
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)        0 2022-12-31 15:33:20.000000 daves_utilities-0.1.1/reports/.gitkeep
-drwxr-xr-x   0 davidkuchelmeister   (501) staff       (20)        0 2023-01-01 11:42:26.602430 daves_utilities-0.1.1/reports/figures/
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)        0 2022-12-31 15:33:20.000000 daves_utilities-0.1.1/reports/figures/.gitkeep
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)      207 2022-12-31 15:33:20.000000 daves_utilities-0.1.1/requirements.txt
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)       38 2023-01-01 11:42:26.613916 daves_utilities-0.1.1/setup.cfg
-drwxr-xr-x   0 davidkuchelmeister   (501) staff       (20)        0 2023-01-01 11:42:26.592153 daves_utilities-0.1.1/src/
-drwxr-xr-x   0 davidkuchelmeister   (501) staff       (20)        0 2023-01-01 11:42:26.608312 daves_utilities-0.1.1/src/daves_utilities/
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)      419 2022-12-31 15:46:05.000000 daves_utilities-0.1.1/src/daves_utilities/__init__.py
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)      160 2023-01-01 11:42:26.000000 daves_utilities-0.1.1/src/daves_utilities/_version.py
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)     5185 2022-12-31 15:47:32.000000 daves_utilities-0.1.1/src/daves_utilities/for_long.py
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)     2602 2022-12-31 15:47:42.000000 daves_utilities-0.1.1/src/daves_utilities/fun_save.py
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)     1800 2022-12-31 15:48:43.000000 daves_utilities-0.1.1/src/daves_utilities/is_equal.py
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)     3531 2023-01-01 11:41:18.000000 daves_utilities-0.1.1/src/daves_utilities/print_structure.py
-drwxr-xr-x   0 davidkuchelmeister   (501) staff       (20)        0 2023-01-01 11:42:26.612581 daves_utilities-0.1.1/src/daves_utilities.egg-info/
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)      250 2023-01-01 11:42:26.000000 daves_utilities-0.1.1/src/daves_utilities.egg-info/PKG-INFO
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)      725 2023-01-01 11:42:26.000000 daves_utilities-0.1.1/src/daves_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)        1 2023-01-01 11:42:26.000000 daves_utilities-0.1.1/src/daves_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)       54 2023-01-01 11:42:26.000000 daves_utilities-0.1.1/src/daves_utilities.egg-info/requires.txt
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)       16 2023-01-01 11:42:26.000000 daves_utilities-0.1.1/src/daves_utilities.egg-info/top_level.txt
--rw-r--r--   0 davidkuchelmeister   (501) staff       (20)      394 2022-12-31 15:33:20.000000 daves_utilities-0.1.1/tox.ini
+-rw-r--r--   0        0        0     1087 2022-12-31 15:33:52.562362 daves_utilities-0.1.2/LICENSE
+-rw-r--r--   0        0        0       19 2022-12-31 15:33:52.565062 daves_utilities-0.1.2/README.md
+-rw-r--r--   0        0        0     1346 2023-07-15 13:17:38.794106 daves_utilities-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      428 2023-07-15 11:50:47.947713 daves_utilities-0.1.2/src/daves_utilities/__init__.py
+-rw-r--r--   0        0        0     1476 2023-01-01 16:09:26.439971 daves_utilities-0.1.2/src/daves_utilities/archive/is_equal.py
+-rw-r--r--   0        0        0     3478 2023-01-01 15:53:17.727021 daves_utilities-0.1.2/src/daves_utilities/archive/print_structure.py
+-rw-r--r--   0        0        0      546 2023-07-15 12:12:31.015670 daves_utilities-0.1.2/src/daves_utilities/david_secrets.py
+-rw-r--r--   0        0        0     5185 2023-01-01 15:57:05.349696 daves_utilities-0.1.2/src/daves_utilities/iterator.py
+-rw-r--r--   0        0        0     2240 1970-01-01 00:00:00.000000 daves_utilities-0.1.2/PKG-INFO
```

### Comparing `daves_utilities-0.1.1/LICENSE` & `daves_utilities-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.1/src/daves_utilities/for_long.py` & `daves_utilities-0.1.2/src/daves_utilities/iterator.py`

 * *Files identical despite different names*

### Comparing `daves_utilities-0.1.1/src/daves_utilities/is_equal.py` & `daves_utilities-0.1.2/src/daves_utilities/archive/is_equal.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import pandas as pd
 
 
 def is_equal_recursive(elem1, elem2):  # noqa
 
     if type(elem1) != type(elem2):
         return False
     if isinstance(elem1, list):
@@ -47,19 +46,7 @@
 def is_equal(elem1, elem2, flatten=True):
     boolen_list = is_equal_recursive(elem1, elem2)
 
     if flatten:
         return all(list_flatten(boolen_list))
     else:
         return boolen_list
-
-
-if __name__ == "__main__":
-    df2 = pd.DataFrame(
-        np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]]), columns=["a", "b", "c"]
-    )
-
-    test1 = [{"a": 1, "b": 2}, 10, [1, 2, [4, 5, 6]], df2]
-    test2 = [{"a": 1, "b": 2}, 10, [1, 2, [4, 5, 6]], df2]
-
-    out = is_equal(test1, test2)
-    print(out)
```

### Comparing `daves_utilities-0.1.1/src/daves_utilities/print_structure.py` & `daves_utilities-0.1.2/src/daves_utilities/archive/print_structure.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,16 +76,14 @@
     """
     Testing the print_structure function
 
     execute test on command line with:
     > pytest test_print_structure.py
     """
 
-    from ..print_structure import print_str  # noqa
-
     # pandas data
     df2 = pd.DataFrame(
         np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]]), columns=["a", "b", "c"]
     )
     data = np.array(["a", "b", "c", "d"])
     s = pd.Series(data)
```

