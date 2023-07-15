# Comparing `tmp/yetl-framework-1.7.3.tar.gz` & `tmp/yetl-framework-1.7.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.7.3.tar", last modified: Fri Jul 14 10:14:36 2023, max compression
+gzip compressed data, was "yetl-framework-1.7.4.dev1.tar", last modified: Sat Jul 15 18:23:21 2023, max compression
```

## Comparing `yetl-framework-1.7.3.tar` & `yetl-framework-1.7.4.dev1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.115992 yetl-framework-1.7.3/
--rw-r--r--   0 vsts      (1001) docker     (123)     1094 2023-07-14 10:14:36.111992 yetl-framework-1.7.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-14 10:14:36.115992 yetl-framework-1.7.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1461 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.107992 yetl-framework-1.7.3/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.107992 yetl-framework-1.7.3/yetl/_resources/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/_resources/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      299 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/_resources/logging.yaml
--rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/_resources/project.yaml
--rw-r--r--   0 vsts      (1001) docker     (123)    14649 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/_resources/sibytes_yetl_pipeline_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)     2654 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/_resources/sibytes_yetl_project_schema.json
--rw-r--r--   0 vsts      (1001) docker     (123)    14615 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/_resources/sibytes_yetl_tables_schema.json
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.107992 yetl-framework-1.7.3/yetl/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)     3398 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/cli/_init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.107992 yetl-framework-1.7.3/yetl/cli/metadata_provider/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/cli/metadata_provider/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16878 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/cli/metadata_provider/_xlsx.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.111992 yetl-framework-1.7.3/yetl/config/
--rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3362 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2195 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10168 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17636 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/deltalake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.111992 yetl-framework-1.7.3/yetl/config/table/
--rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/table/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4980 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/table/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/table/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6603 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/table/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4712 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/table/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/table/_table_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/config/table/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.111992 yetl-framework-1.7.3/yetl/validation/
--rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/validation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1555 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/validation/_validate.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.111992 yetl-framework-1.7.3/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/workflow/_dlt.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-07-14 10:13:32.000000 yetl-framework-1.7.3/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-14 10:14:36.111992 yetl-framework-1.7.3/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     1094 2023-07-14 10:14:36.000000 yetl-framework-1.7.3/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1361 2023-07-14 10:14:36.000000 yetl-framework-1.7.3/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-14 10:14:36.000000 yetl-framework-1.7.3/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-14 10:14:36.000000 yetl-framework-1.7.3/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       92 2023-07-14 10:14:36.000000 yetl-framework-1.7.3/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-07-14 10:14:36.000000 yetl-framework-1.7.3/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:23:21.913230 yetl-framework-1.7.4.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-07-15 18:23:21.913230 yetl-framework-1.7.4.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      596 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-15 18:23:21.913230 yetl-framework-1.7.4.dev1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1544 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:23:21.909230 yetl-framework-1.7.4.dev1/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      473 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1141 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:23:21.909230 yetl-framework-1.7.4.dev1/yetl/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3367 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/cli/_init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:23:21.909230 yetl-framework-1.7.4.dev1/yetl/cli/metadata_provider/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/cli/metadata_provider/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17152 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/cli/metadata_provider/_xlsx.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:23:21.909230 yetl-framework-1.7.4.dev1/yetl/config/
+-rw-r--r--   0 vsts      (1001) docker     (123)      611 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3362 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2195 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1309 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      194 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      303 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10168 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6294 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5064 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    17641 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:23:21.909230 yetl-framework-1.7.4.dev1/yetl/config/table/
+-rw-r--r--   0 vsts      (1001) docker     (123)      381 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/table/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5005 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/table/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1163 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/table/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6603 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/table/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4712 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/table/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      120 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/table/_table_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      253 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/config/table/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:23:21.909230 yetl-framework-1.7.4.dev1/yetl/resource/
+-rw-r--r--   0 vsts      (1001) docker     (123)      571 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/resource/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      299 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/resource/logging.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/resource/project.yaml
+-rw-r--r--   0 vsts      (1001) docker     (123)    14649 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/resource/sibytes_yetl_pipeline_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     2654 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/resource/sibytes_yetl_project_schema.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    14615 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/resource/sibytes_yetl_tables_schema.json
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:23:21.913230 yetl-framework-1.7.4.dev1/yetl/validation/
+-rw-r--r--   0 vsts      (1001) docker     (123)      353 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/validation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1426 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/validation/_validate.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:23:21.913230 yetl-framework-1.7.4.dev1/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      167 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1312 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/workflow/_dlt.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-07-15 18:22:11.000000 yetl-framework-1.7.4.dev1/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 18:23:21.913230 yetl-framework-1.7.4.dev1/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1199 2023-07-15 18:23:21.000000 yetl-framework-1.7.4.dev1/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1349 2023-07-15 18:23:21.000000 yetl-framework-1.7.4.dev1/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-15 18:23:21.000000 yetl-framework-1.7.4.dev1/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-15 18:23:21.000000 yetl-framework-1.7.4.dev1/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       76 2023-07-15 18:23:21.000000 yetl-framework-1.7.4.dev1/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-07-15 18:23:21.000000 yetl-framework-1.7.4.dev1/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.7.3/README.md` & `yetl-framework-1.7.4.dev1/README.md`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/setup.py` & `yetl-framework-1.7.4.dev1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,50 +6,52 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.7.3",
+    version="1.7.4.dev1",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
     },
     author="Shaun Ryan",
     author_email="shaun_chiburi@hotmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     include_package_data=True,
     package_dir={"": "."},
-    package_data={"yetl._resources": ["*.json", "*.yaml", "*.xsls"]},
+    package_data={"yetl.resource": ["*.json", "*.yaml", "*.xsls"]},
     packages=[
         "yetl",
-        "yetl._resources",
+        "yetl.resource",
         "yetl.validation",
         "yetl.cli",
         "yetl.cli.metadata_provider",
         "yetl.config",
         "yetl.config.table",
         "yetl.workflow",
 
     ],
     install_requires=[
           'PyYAML',
           'jinja2',
-          'pydantic==1.10.6',
-          'jsonschema==4.16.0',
+          'pydantic',
+          'jsonschema',
           'typer',
           'pandas',
           'openpyxl',
           'delta-spark',
           'pyspark'
       ],
     zip_safe=False
```

### Comparing `yetl-framework-1.7.3/yetl/__main__.py` & `yetl-framework-1.7.4.dev1/yetl/__main__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/yetl/_resources/sibytes_yetl_pipeline_schema.json` & `yetl-framework-1.7.4.dev1/yetl/resource/sibytes_yetl_pipeline_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/yetl/_resources/sibytes_yetl_project_schema.json` & `yetl-framework-1.7.4.dev1/yetl/resource/sibytes_yetl_project_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/yetl/_resources/sibytes_yetl_tables_schema.json` & `yetl-framework-1.7.4.dev1/yetl/resource/sibytes_yetl_tables_schema.json`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/yetl/cli/_init.py` & `yetl-framework-1.7.4.dev1/yetl/cli/_init.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import yaml
 import pkg_resources
 from ..validation import (
     SchemaFiles,
     get_schema,
 )
 import json
-from importlib.resources import files
+from ..resource import get_resource_binary, get_resource_text
 
 
 def init(project: str, directory: str = "."):
     project = project.lower()
     project_path = os.path.abspath(directory)
     project_path = f"{project_path}/{project}"
     paths: dict = _make_project_dir(project_path, project)
@@ -40,22 +40,22 @@
         schema_path = os.path.join(json_schema_path, f.value)
         with open(schema_path, "w", encoding="utf-8") as f:
             f.write(json.dumps(schema, indent=4))
 
 
 def _get_default_config(name: str):
     """Get the default configuration"""
-    config = files("yetl._resources").joinpath(name).read_text()
+    config = get_resource_text(name)
 
     return config
 
 
 def _get_binary_template(name: str):
     """Get the binary template object"""
-    data = files("yetl._resources").joinpath(name).read_bytes()
+    data = get_resource_binary(name)
 
     return data
 
 
 def _create_log_file(project_path: str):
     config: dict = yaml.safe_load(_get_default_config("logging.yaml"))
     file_path = os.path.join(project_path, "logging.yaml")
```

### Comparing `yetl-framework-1.7.3/yetl/cli/metadata_provider/_xlsx.py` & `yetl-framework-1.7.4.dev1/yetl/cli/metadata_provider/_xlsx.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,39 +37,41 @@
     max_rows = "max_rows"
     min_rows = "min_rows"
     custom_properties = "custom_properties"
     vacuum = "vacuum"
 
 
 class Metadata(BaseModel):
-    SCHEMA = {
-        ColumnNames.stage: str,
-        ColumnNames.table_type: str,
-        ColumnNames.catalog: str,
-        ColumnNames.database: str,
-        ColumnNames.table: str,
-        ColumnNames.sql: str,
-        ColumnNames.id: str,
-        ColumnNames.depends_on: str,
-        f"{ColumnNames.deltalake}_{ColumnNames.delta_properties}": str,
-        f"{ColumnNames.deltalake}_{ColumnNames.identity}": str,
-        f"{ColumnNames.deltalake}_{ColumnNames.partition_by}": str,
-        f"{ColumnNames.deltalake}_{ColumnNames.cluster_by}": str,
-        f"{ColumnNames.deltalake}_{ColumnNames.delta_constraints}": str,
-        f"{ColumnNames.deltalake}_{ColumnNames.z_order_by}": str,
-        f"{ColumnNames.deltalake}_{ColumnNames.vacuum}": int,
-        f"{ColumnNames.warning_thresholds}_{ColumnNames.invalid_ratio}": np.float64,
-        f"{ColumnNames.warning_thresholds}_{ColumnNames.invalid_rows}": np.float64,
-        f"{ColumnNames.warning_thresholds}_{ColumnNames.max_rows}": np.float64,
-        f"{ColumnNames.warning_thresholds}_{ColumnNames.min_rows}": np.float64,
-        f"{ColumnNames.exception_thresholds}_{ColumnNames.invalid_ratio}": np.float64,
-        f"{ColumnNames.exception_thresholds}_{ColumnNames.invalid_rows}": np.float64,
-        f"{ColumnNames.exception_thresholds}_{ColumnNames.max_rows}": np.float64,
-        f"{ColumnNames.exception_thresholds}_{ColumnNames.min_rows}": np.float64,
-    }
+    SCHEMA: dict = Field(
+        default={
+            ColumnNames.stage: str,
+            ColumnNames.table_type: str,
+            ColumnNames.catalog: str,
+            ColumnNames.database: str,
+            ColumnNames.table: str,
+            ColumnNames.sql: str,
+            ColumnNames.id: str,
+            ColumnNames.depends_on: str,
+            f"{ColumnNames.deltalake}_{ColumnNames.delta_properties}": str,
+            f"{ColumnNames.deltalake}_{ColumnNames.identity}": str,
+            f"{ColumnNames.deltalake}_{ColumnNames.partition_by}": str,
+            f"{ColumnNames.deltalake}_{ColumnNames.cluster_by}": str,
+            f"{ColumnNames.deltalake}_{ColumnNames.delta_constraints}": str,
+            f"{ColumnNames.deltalake}_{ColumnNames.z_order_by}": str,
+            f"{ColumnNames.deltalake}_{ColumnNames.vacuum}": int,
+            f"{ColumnNames.warning_thresholds}_{ColumnNames.invalid_ratio}": np.float64,
+            f"{ColumnNames.warning_thresholds}_{ColumnNames.invalid_rows}": np.float64,
+            f"{ColumnNames.warning_thresholds}_{ColumnNames.max_rows}": np.float64,
+            f"{ColumnNames.warning_thresholds}_{ColumnNames.min_rows}": np.float64,
+            f"{ColumnNames.exception_thresholds}_{ColumnNames.invalid_ratio}": np.float64,
+            f"{ColumnNames.exception_thresholds}_{ColumnNames.invalid_rows}": np.float64,
+            f"{ColumnNames.exception_thresholds}_{ColumnNames.max_rows}": np.float64,
+            f"{ColumnNames.exception_thresholds}_{ColumnNames.min_rows}": np.float64,
+        }
+    )
 
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
 
     stage: StageType = Field(...)
     table_type: TableType = Field(...)
     catalog: str = Field(default=None)
@@ -269,42 +271,44 @@
         ] = self.catalog
         data[self.stage.value][self.table_type.value][self.database][self.table] = table
 
         return data
 
 
 class XlsMetadata(BaseModel):
-    SCHEMA = {
-        ColumnNames.stage: str,
-        ColumnNames.table_type: str,
-        ColumnNames.catalog: str,
-        ColumnNames.database: str,
-        ColumnNames.table: str,
-        ColumnNames.sql: str,
-        ColumnNames.id: str,
-        ColumnNames.depends_on: str,
-        f"{ColumnNames.deltalake}_{ColumnNames.delta_properties}": str,
-        f"{ColumnNames.deltalake}_{ColumnNames.identity}": str,
-        f"{ColumnNames.deltalake}_{ColumnNames.partition_by}": str,
-        f"{ColumnNames.deltalake}_{ColumnNames.cluster_by}": str,
-        f"{ColumnNames.deltalake}_{ColumnNames.delta_constraints}": str,
-        f"{ColumnNames.deltalake}_{ColumnNames.z_order_by}": str,
-        f"{ColumnNames.deltalake}_{ColumnNames.vacuum}": str,
-        f"{ColumnNames.warning_thresholds}_{ColumnNames.invalid_ratio}": np.float64,
-        f"{ColumnNames.warning_thresholds}_{ColumnNames.invalid_rows}": np.float64,
-        f"{ColumnNames.warning_thresholds}_{ColumnNames.max_rows}": np.float64,
-        f"{ColumnNames.warning_thresholds}_{ColumnNames.min_rows}": np.float64,
-        f"{ColumnNames.exception_thresholds}_{ColumnNames.invalid_ratio}": np.float64,
-        f"{ColumnNames.exception_thresholds}_{ColumnNames.invalid_rows}": np.float64,
-        f"{ColumnNames.exception_thresholds}_{ColumnNames.max_rows}": np.float64,
-        f"{ColumnNames.exception_thresholds}_{ColumnNames.min_rows}": np.float64,
-        # "custom_properties.process_group": np."float64",
-        # "custom_properties.rentention_days": np."float64",
-        # "custom_properties.vaccum": np."float64"
-    }
+    SCHEMA: dict = Field(
+        default={
+            ColumnNames.stage: str,
+            ColumnNames.table_type: str,
+            ColumnNames.catalog: str,
+            ColumnNames.database: str,
+            ColumnNames.table: str,
+            ColumnNames.sql: str,
+            ColumnNames.id: str,
+            ColumnNames.depends_on: str,
+            f"{ColumnNames.deltalake}_{ColumnNames.delta_properties}": str,
+            f"{ColumnNames.deltalake}_{ColumnNames.identity}": str,
+            f"{ColumnNames.deltalake}_{ColumnNames.partition_by}": str,
+            f"{ColumnNames.deltalake}_{ColumnNames.cluster_by}": str,
+            f"{ColumnNames.deltalake}_{ColumnNames.delta_constraints}": str,
+            f"{ColumnNames.deltalake}_{ColumnNames.z_order_by}": str,
+            f"{ColumnNames.deltalake}_{ColumnNames.vacuum}": str,
+            f"{ColumnNames.warning_thresholds}_{ColumnNames.invalid_ratio}": np.float64,
+            f"{ColumnNames.warning_thresholds}_{ColumnNames.invalid_rows}": np.float64,
+            f"{ColumnNames.warning_thresholds}_{ColumnNames.max_rows}": np.float64,
+            f"{ColumnNames.warning_thresholds}_{ColumnNames.min_rows}": np.float64,
+            f"{ColumnNames.exception_thresholds}_{ColumnNames.invalid_ratio}": np.float64,
+            f"{ColumnNames.exception_thresholds}_{ColumnNames.invalid_rows}": np.float64,
+            f"{ColumnNames.exception_thresholds}_{ColumnNames.max_rows}": np.float64,
+            f"{ColumnNames.exception_thresholds}_{ColumnNames.min_rows}": np.float64,
+            # "custom_properties.process_group": np."float64",
+            # "custom_properties.rentention_days": np."float64",
+            # "custom_properties.vaccum": np."float64"
+        }
+    )
 
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         df = pd.read_excel(self.source, header=[0, 1])
         df = self.validate_schema(df)
         self.data = self._deserialize(df)
```

### Comparing `yetl-framework-1.7.3/yetl/config/__init__.py` & `yetl-framework-1.7.4.dev1/yetl/config/__init__.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/yetl/config/_config.py` & `yetl-framework-1.7.4.dev1/yetl/config/_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/yetl/config/_decorators.py` & `yetl-framework-1.7.4.dev1/yetl/config/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/yetl/config/_logging_config.py` & `yetl-framework-1.7.4.dev1/yetl/config/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/yetl/config/_project.py` & `yetl-framework-1.7.4.dev1/yetl/config/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/yetl/config/_spark_context.py` & `yetl-framework-1.7.4.dev1/yetl/config/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/yetl/config/_tables.py` & `yetl-framework-1.7.4.dev1/yetl/config/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/yetl/config/_timeslice.py` & `yetl-framework-1.7.4.dev1/yetl/config/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/yetl/config/_utils.py` & `yetl-framework-1.7.4.dev1/yetl/config/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/yetl/config/deltalake.py` & `yetl-framework-1.7.4.dev1/yetl/config/deltalake.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
         )
         # Not whitelist on databricks.
         # table_exists = self.spark.catalog.tableExists(f"`{database}`.`{table}`")
         return _table_exists
 
     def get_delta_properties_sql(self, delta_properties: Dict[str, Union[str, bool]]):
         sql_properties = [
-            f"{k.lower()} = {v.lower()}" for k, v in delta_properties.items()
+            f"{k.lower()} = {str(v).lower()}" for k, v in delta_properties.items()
         ]
         sql_properties = ", ".join(sql_properties)
         return sql_properties
 
     def create_table(
         self,
         database: str,
```

### Comparing `yetl-framework-1.7.3/yetl/config/table/_deltalake.py` & `yetl-framework-1.7.4.dev1/yetl/config/table/_deltalake.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def in_allowed_stages(cls, stage: StageType):
         return stage in (stage.raw, stage.base, stage.curated)
 
     _logger: Any = PrivateAttr(default=None)
     _replacements: Dict[JinjaVariables, str] = PrivateAttr(default=None)
     _spark: DeltaLakeFn = PrivateAttr(default=None)
     depends_on: List[str] = Field(default=[])
-    delta_properties: Dict[str, str] = Field(default=None)
+    delta_properties: Dict[str, Union[str, bool, int, float]] = Field(default=None)
     delta_constraints: Dict[str, str] = Field(default=None)
     partition_by: Union[List[str], str] = Field(default=None)
     cluster_by: Union[List[str], str] = Field(default=None)
     z_order_by: Union[List[str], str] = Field(default=None)
     vacuum: int = Field(default=31)
     options: Union[dict, None] = Field(default=None)
     timeslice: Timeslice = Field(...)
```

### Comparing `yetl-framework-1.7.3/yetl/config/table/_factory.py` & `yetl-framework-1.7.4.dev1/yetl/config/table/_factory.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/yetl/config/table/_read.py` & `yetl-framework-1.7.4.dev1/yetl/config/table/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/yetl/config/table/_table.py` & `yetl-framework-1.7.4.dev1/yetl/config/table/_table.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/yetl/validation/_validate.py` & `yetl-framework-1.7.4.dev1/yetl/validation/_validate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,38 @@
-from importlib.resources import files
 import json
+from ..resource import get_resource_text
 import jsonschema as js
 from enum import Enum
 
 
 class SchemaFiles(Enum):
     tables_schema = "sibytes_yetl_tables_schema.json"
     pipeline_schema = "sibytes_yetl_pipeline_schema.json"
     project_schema = "sibytes_yetl_project_schema.json"
 
 
 def get_table_schema():
     """Get the tables json schema from the package resources"""
-    schema = (
-        files("yetl._resources").joinpath(SchemaFiles.tables_schema.value).read_text()
-    )
+    schema = get_resource_text(SchemaFiles.tables_schema.value)
     json_schema = json.loads(schema)
 
     return json_schema
 
 
 def get_pipeline_schema():
     """Get the pipeline json schema from the package resources"""
-    schema = (
-        files("yetl._resources").joinpath(SchemaFiles.pipeline_schema.value).read_text()
-    )
+    schema = get_resource_text(SchemaFiles.pipeline_schema.value)
     json_schema = json.loads(schema)
 
     return json_schema
 
 
 def get_project_schema():
     """Get the project json schema from the package resources"""
-    schema = (
-        files("yetl._resources").joinpath(SchemaFiles.project_schema.value).read_text()
-    )
+    schema = get_resource_text(SchemaFiles.project_schema.value)
     json_schema = json.loads(schema)
 
     return json_schema
 
 
 def get_schema(schema_file: SchemaFiles):
     if schema_file == SchemaFiles.pipeline_schema:
```

### Comparing `yetl-framework-1.7.3/yetl/workflow/_dlt.py` & `yetl-framework-1.7.4.dev1/yetl/workflow/_dlt.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.7.4.dev1/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.7.3/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.7.4.dev1/yetl_framework.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 README.md
 setup.py
 ./yetl/__init__.py
 ./yetl/__main__.py
-./yetl/_resources/__init__.py
-./yetl/_resources/logging.yaml
-./yetl/_resources/project.yaml
-./yetl/_resources/sibytes_yetl_pipeline_schema.json
-./yetl/_resources/sibytes_yetl_project_schema.json
-./yetl/_resources/sibytes_yetl_tables_schema.json
 ./yetl/cli/_init.py
 ./yetl/cli/metadata_provider/__init__.py
 ./yetl/cli/metadata_provider/_xlsx.py
 ./yetl/config/__init__.py
 ./yetl/config/_config.py
 ./yetl/config/_decorators.py
 ./yetl/config/_logging_config.py
@@ -26,14 +20,20 @@
 ./yetl/config/table/__init__.py
 ./yetl/config/table/_deltalake.py
 ./yetl/config/table/_factory.py
 ./yetl/config/table/_read.py
 ./yetl/config/table/_table.py
 ./yetl/config/table/_table_type.py
 ./yetl/config/table/_write.py
+./yetl/resource/__init__.py
+./yetl/resource/logging.yaml
+./yetl/resource/project.yaml
+./yetl/resource/sibytes_yetl_pipeline_schema.json
+./yetl/resource/sibytes_yetl_project_schema.json
+./yetl/resource/sibytes_yetl_tables_schema.json
 ./yetl/validation/__init__.py
 ./yetl/validation/_validate.py
 ./yetl/workflow/__init__.py
 ./yetl/workflow/_dlt.py
 ./yetl/workflow/_multi_threaded.py
 ./yetl/workflow/_notebook.py
 yetl_framework.egg-info/PKG-INFO
```

