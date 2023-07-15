# Comparing `tmp/yetl-framework-1.7.5.tar.gz` & `tmp/yetl-framework-2.0.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.7.5.tar", last modified: Sat Jul 15 18:33:25 2023, max compression
+gzip compressed data, was "yetl-framework-2.0.0.dev1.tar", last modified: Sat Jul 15 18:46:26 2023, max compression
```

## Comparing `yetl-framework-1.7.5.tar` & `yetl-framework-2.0.0.dev1.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:33:25.480985 yetl-framework-1.7.5/
--rw-r--r--   0 vsts      (1001) docker     (123)     1194 2023-07-15 18:33:25.480985 yetl-framework-1.7.5/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-15 18:33:25.480985 yetl-framework-1.7.5/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1539 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:33:25.476985 yetl-framework-1.7.5/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:33:25.476985 yetl-framework-1.7.5/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     3367 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:33:25.476985 yetl-framework-1.7.5/yetl/cli/metadata_provider/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/cli/metadata_provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17152 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/cli/metadata_provider/_xlsx.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:33:25.476985 yetl-framework-1.7.5/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3362 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2195 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10168 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17641 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:33:25.476985 yetl-framework-1.7.5/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5005 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6603 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4712 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:33:25.476985 yetl-framework-1.7.5/yetl/resource/
--rw-r--r--   0 vsts      (1001) docker     (123)      564 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/resource/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      299 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/resource/logging.yaml
--rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/resource/project.yaml
--rw-r--r--   0 vsts      (1001) docker     (123)    14649 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/resource/sibytes_yetl_pipeline_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)     2654 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/resource/sibytes_yetl_project_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)    14615 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/resource/sibytes_yetl_tables_schema.json
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:33:25.480985 yetl-framework-1.7.5/yetl/validation/
--rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/validation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1426 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/validation/_validate.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:33:25.480985 yetl-framework-1.7.5/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/workflow/_dlt.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-07-15 18:32:16.000000 yetl-framework-1.7.5/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:33:25.480985 yetl-framework-1.7.5/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     1194 2023-07-15 18:33:25.000000 yetl-framework-1.7.5/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1349 2023-07-15 18:33:25.000000 yetl-framework-1.7.5/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-15 18:33:25.000000 yetl-framework-1.7.5/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-15 18:33:25.000000 yetl-framework-1.7.5/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       76 2023-07-15 18:33:25.000000 yetl-framework-1.7.5/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-07-15 18:33:25.000000 yetl-framework-1.7.5/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:46:26.936141 yetl-framework-2.0.0.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-07-15 18:46:26.932141 yetl-framework-2.0.0.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-15 18:46:26.936141 yetl-framework-2.0.0.dev1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1544 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:46:26.924141 yetl-framework-2.0.0.dev1/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:46:26.924141 yetl-framework-2.0.0.dev1/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3367 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:46:26.924141 yetl-framework-2.0.0.dev1/yetl/cli/metadata_provider/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/cli/metadata_provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17152 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/cli/metadata_provider/_xlsx.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:46:26.928141 yetl-framework-2.0.0.dev1/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3362 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2195 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10168 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17641 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:46:26.928141 yetl-framework-2.0.0.dev1/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5005 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6603 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4712 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:46:26.932141 yetl-framework-2.0.0.dev1/yetl/resource/
+-rw-r--r--   0 vsts      (1001) docker     (123)      569 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/resource/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      299 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/resource/logging.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/resource/project.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)    14649 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/resource/sibytes_yetl_pipeline_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     2654 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/resource/sibytes_yetl_project_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    14615 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/resource/sibytes_yetl_tables_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    10012 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/resource/tables.xlsx
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:46:26.932141 yetl-framework-2.0.0.dev1/yetl/validation/
+-rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/validation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1423 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/validation/_validate.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:46:26.932141 yetl-framework-2.0.0.dev1/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/workflow/_dlt.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-07-15 18:45:23.000000 yetl-framework-2.0.0.dev1/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:46:26.932141 yetl-framework-2.0.0.dev1/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-07-15 18:46:26.000000 yetl-framework-2.0.0.dev1/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1377 2023-07-15 18:46:26.000000 yetl-framework-2.0.0.dev1/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-15 18:46:26.000000 yetl-framework-2.0.0.dev1/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-15 18:46:26.000000 yetl-framework-2.0.0.dev1/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       76 2023-07-15 18:46:26.000000 yetl-framework-2.0.0.dev1/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-07-15 18:46:26.000000 yetl-framework-2.0.0.dev1/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.7.5/PKG-INFO` & `yetl-framework-2.0.0.dev1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.7.5
+Version: 2.0.0.dev1
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.7.5/README.md` & `yetl-framework-2.0.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/setup.py` & `yetl-framework-2.0.0.dev1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.7.5",
+    version="2.0.0.dev1",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
@@ -27,15 +27,15 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     include_package_data=True,
     package_dir={"": "."},
-    package_data={"yetl.resource": ["*.json", "*.yaml", "*.xslx"]},
+    package_data={"yetl.resource": ["*.json", "*.yaml", "*.xlsx"]},
     packages=[
         "yetl",
         "yetl.resource",
         "yetl.validation",
         "yetl.cli",
         "yetl.cli.metadata_provider",
         "yetl.config",
```

### Comparing `yetl-framework-1.7.5/yetl/__main__.py` & `yetl-framework-2.0.0.dev1/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/cli/_init.py` & `yetl-framework-2.0.0.dev1/yetl/cli/_init.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/cli/metadata_provider/_xlsx.py` & `yetl-framework-2.0.0.dev1/yetl/cli/metadata_provider/_xlsx.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/config/__init__.py` & `yetl-framework-2.0.0.dev1/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/config/_config.py` & `yetl-framework-2.0.0.dev1/yetl/config/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/config/_decorators.py` & `yetl-framework-2.0.0.dev1/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/config/_logging_config.py` & `yetl-framework-2.0.0.dev1/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/config/_project.py` & `yetl-framework-2.0.0.dev1/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/config/_spark_context.py` & `yetl-framework-2.0.0.dev1/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/config/_tables.py` & `yetl-framework-2.0.0.dev1/yetl/config/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/config/_timeslice.py` & `yetl-framework-2.0.0.dev1/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/config/_utils.py` & `yetl-framework-2.0.0.dev1/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/config/deltalake.py` & `yetl-framework-2.0.0.dev1/yetl/config/deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/config/table/_deltalake.py` & `yetl-framework-2.0.0.dev1/yetl/config/table/_deltalake.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/config/table/_factory.py` & `yetl-framework-2.0.0.dev1/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/config/table/_read.py` & `yetl-framework-2.0.0.dev1/yetl/config/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/config/table/_table.py` & `yetl-framework-2.0.0.dev1/yetl/config/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/resource/__init__.py` & `yetl-framework-2.0.0.dev1/yetl/resource/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 try:
-    from importlib.resources import files  # as resources
+    from importlib.resources import files as resources
 except Exception:
     from importlib import resources
 
 _PACKAGE = "yetl.resource"
 
 
 def get_resource_text(resource: str):
     try:
-        data = files(_PACKAGE).joinpath(resource).read_text()
+        data = resources(_PACKAGE).joinpath(resource).read_text()
     except Exception:
         data = resources.read_text(_PACKAGE, resource)
     return data
 
 
 def get_resource_binary(resource: str):
     try:
-        schema = files(_PACKAGE).joinpath(resource).read_bytes()
+        schema = resources(_PACKAGE).joinpath(resource).read_bytes()
     except Exception:
         schema = resources.read_binary(_PACKAGE, resource)
     return schema
```

### Comparing `yetl-framework-1.7.5/yetl/resource/sibytes_yetl_pipeline_schema.json` & `yetl-framework-2.0.0.dev1/yetl/resource/sibytes_yetl_pipeline_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/resource/sibytes_yetl_project_schema.json` & `yetl-framework-2.0.0.dev1/yetl/resource/sibytes_yetl_project_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/resource/sibytes_yetl_tables_schema.json` & `yetl-framework-2.0.0.dev1/yetl/resource/sibytes_yetl_tables_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/validation/_validate.py` & `yetl-framework-2.0.0.dev1/yetl/validation/_validate.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 class SchemaFiles(Enum):
     tables_schema = "sibytes_yetl_tables_schema.json"
     pipeline_schema = "sibytes_yetl_pipeline_schema.json"
     project_schema = "sibytes_yetl_project_schema.json"
 
 
 def get_table_schema():
-    """Get the tables json schema from the package resources"""
+    """Get the tables json schema from the package resource"""
     schema = get_resource_text(SchemaFiles.tables_schema.value)
     json_schema = json.loads(schema)
 
     return json_schema
 
 
 def get_pipeline_schema():
-    """Get the pipeline json schema from the package resources"""
+    """Get the pipeline json schema from the package resource"""
     schema = get_resource_text(SchemaFiles.pipeline_schema.value)
     json_schema = json.loads(schema)
 
     return json_schema
 
 
 def get_project_schema():
-    """Get the project json schema from the package resources"""
+    """Get the project json schema from the package resource"""
     schema = get_resource_text(SchemaFiles.project_schema.value)
     json_schema = json.loads(schema)
 
     return json_schema
 
 
 def get_schema(schema_file: SchemaFiles):
```

### Comparing `yetl-framework-1.7.5/yetl/workflow/_dlt.py` & `yetl-framework-2.0.0.dev1/yetl/workflow/_dlt.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl/workflow/_multi_threaded.py` & `yetl-framework-2.0.0.dev1/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.5/yetl_framework.egg-info/PKG-INFO` & `yetl-framework-2.0.0.dev1/yetl_framework.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yetl-framework
-Version: 1.7.5
+Version: 2.0.0.dev1
 Summary: yet (another spark) etl framework
 Home-page: https://www.yetl.io/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/sibytes/yetl
 Project-URL: Documentation, https://www.yetl.io/
```

### Comparing `yetl-framework-1.7.5/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-2.0.0.dev1/yetl_framework.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 ./yetl/config/table/_write.py
 ./yetl/resource/__init__.py
 ./yetl/resource/logging.yaml
 ./yetl/resource/project.yaml
 ./yetl/resource/sibytes_yetl_pipeline_schema.json
 ./yetl/resource/sibytes_yetl_project_schema.json
 ./yetl/resource/sibytes_yetl_tables_schema.json
+./yetl/resource/tables.xlsx
 ./yetl/validation/__init__.py
 ./yetl/validation/_validate.py
 ./yetl/workflow/__init__.py
 ./yetl/workflow/_dlt.py
 ./yetl/workflow/_multi_threaded.py
 ./yetl/workflow/_notebook.py
 yetl_framework.egg-info/PKG-INFO
```

