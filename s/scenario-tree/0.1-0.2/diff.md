# Comparing `tmp/scenario_tree-0.1.tar.gz` & `tmp/scenario_tree-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenario_tree-0.1.tar", last modified: Sat Jul 15 05:00:07 2023, max compression
+gzip compressed data, was "scenario_tree-0.2.tar", last modified: Sat Jul 15 05:49:55 2023, max compression
```

## Comparing `scenario_tree-0.1.tar` & `scenario_tree-0.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxr-xr-x   0 zhenchen   (501) staff       (20)        0 2023-07-15 05:00:07.591192 scenario_tree-0.1/
--rw-r--r--   0 zhenchen   (501) staff       (20)      147 2023-07-15 05:00:07.590985 scenario_tree-0.1/PKG-INFO
-drwxr-xr-x   0 zhenchen   (501) staff       (20)        0 2023-07-15 05:00:07.590638 scenario_tree-0.1/scenario_tree.egg-info/
--rw-r--r--   0 zhenchen   (501) staff       (20)      147 2023-07-15 05:00:07.000000 scenario_tree-0.1/scenario_tree.egg-info/PKG-INFO
--rw-r--r--   0 zhenchen   (501) staff       (20)      156 2023-07-15 05:00:07.000000 scenario_tree-0.1/scenario_tree.egg-info/SOURCES.txt
--rw-r--r--   0 zhenchen   (501) staff       (20)        1 2023-07-15 05:00:07.000000 scenario_tree-0.1/scenario_tree.egg-info/dependency_links.txt
--rw-r--r--   0 zhenchen   (501) staff       (20)        8 2023-07-15 05:00:07.000000 scenario_tree-0.1/scenario_tree.egg-info/top_level.txt
--rw-r--r--   0 zhenchen   (501) staff       (20)       38 2023-07-15 05:00:07.591242 scenario_tree-0.1/setup.cfg
--rw-r--r--   0 zhenchen   (501) staff       (20)      386 2023-07-15 04:59:31.000000 scenario_tree-0.1/setup.py
+drwxr-xr-x   0 zhenchen   (501) staff       (20)        0 2023-07-15 05:49:55.717650 scenario_tree-0.2/
+-rw-r--r--   0 zhenchen   (501) staff       (20)      147 2023-07-15 05:49:55.717490 scenario_tree-0.2/PKG-INFO
+drwxr-xr-x   0 zhenchen   (501) staff       (20)        0 2023-07-15 05:49:55.717303 scenario_tree-0.2/scenario_tree.egg-info/
+-rw-r--r--   0 zhenchen   (501) staff       (20)      147 2023-07-15 05:49:55.000000 scenario_tree-0.2/scenario_tree.egg-info/PKG-INFO
+-rw-r--r--   0 zhenchen   (501) staff       (20)      164 2023-07-15 05:49:55.000000 scenario_tree-0.2/scenario_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 zhenchen   (501) staff       (20)        1 2023-07-15 05:49:55.000000 scenario_tree-0.2/scenario_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 zhenchen   (501) staff       (20)        5 2023-07-15 05:49:55.000000 scenario_tree-0.2/scenario_tree.egg-info/top_level.txt
+-rw-r--r--   0 zhenchen   (501) staff       (20)       38 2023-07-15 05:49:55.717708 scenario_tree-0.2/setup.cfg
+-rw-r--r--   0 zhenchen   (501) staff       (20)      430 2023-07-15 05:49:44.000000 scenario_tree-0.2/setup.py
+-rw-r--r--   0 zhenchen   (501) staff       (20)     2167 2023-07-15 05:39:16.000000 scenario_tree-0.2/tree.py
```

