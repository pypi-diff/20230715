# Comparing `tmp/hyfi_template-0.4.3.tar.gz` & `tmp/hyfi_template-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi_template-0.4.3.tar", max compression
+gzip compressed data, was "hyfi_template-0.4.4.tar", max compression
```

## Comparing `hyfi_template-0.4.3.tar` & `hyfi_template-0.4.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1071 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/LICENSE
--rw-r--r--   0        0        0     2215 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/README.md
--rw-r--r--   0        0        0     3012 2023-07-10 18:50:16.557195 hyfi_template-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      286 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/src/hyfit/__cli__.py
--rw-r--r--   0        0        0      379 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/src/hyfit/__init__.py
--rw-r--r--   0        0        0       22 2023-07-10 18:50:16.505195 hyfi_template-0.4.3/src/hyfit/_version.py
--rw-r--r--   0        0        0        0 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/src/hyfit/conf/__init__.py
--rw-r--r--   0        0        0      249 2023-07-10 18:50:16.505195 hyfi_template-0.4.3/src/hyfit/conf/about/__init__.yaml
--rw-r--r--   0        0        0      553 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/src/hyfit/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/src/hyfit/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/src/hyfit/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/src/hyfit/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/src/hyfit/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/src/hyfit/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      328 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/src/hyfit/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/src/hyfit/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/src/hyfit/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      322 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/src/hyfit/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/src/hyfit/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/src/hyfit/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      137 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/src/hyfit/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/src/hyfit/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      901 2023-07-10 18:49:49.361474 hyfi_template-0.4.3/src/hyfit/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/module/__init__.yaml
--rw-r--r--   0        0        0       73 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      880 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/path/__init__.yaml
--rw-r--r--   0        0        0      133 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/path/__task__.yaml
--rw-r--r--   0        0        0      291 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      128 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      236 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      241 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       90 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       69 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/pipeline/__test_dataframe__.yaml
--rw-r--r--   0        0        0      268 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/pipeline/__test_general__.yaml
--rw-r--r--   0        0        0      744 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/project/__init__.yaml
--rw-r--r--   0        0        0      185 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/project/__test__.yaml
--rw-r--r--   0        0        0       38 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/running/__init__.yaml
--rw-r--r--   0        0        0      161 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      305 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/task/__init__.yaml
--rw-r--r--   0        0        0      208 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/task/__test__.yaml
--rw-r--r--   0        0        0      114 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0      113 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0        0 2023-07-10 18:49:49.365474 hyfi_template-0.4.3/src/hyfit/py.typed
--rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 hyfi_template-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-15 05:55:11.921012 hyfi_template-0.4.4/LICENSE
+-rw-r--r--   0        0        0     2215 2023-07-15 05:55:11.921012 hyfi_template-0.4.4/README.md
+-rw-r--r--   0        0        0     3012 2023-07-15 05:55:42.195733 hyfi_template-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      286 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/__cli__.py
+-rw-r--r--   0        0        0      379 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-15 05:55:42.131728 hyfi_template-0.4.4/src/hyfit/_version.py
+-rw-r--r--   0        0        0        0 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/__init__.py
+-rw-r--r--   0        0        0      249 2023-07-15 05:55:42.131728 hyfi_template-0.4.4/src/hyfit/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      328 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      322 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      137 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      901 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      880 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      125 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      291 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      128 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      236 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      241 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       90 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       69 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/pipeline/__test_dataframe__.yaml
+-rw-r--r--   0        0        0      268 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/pipeline/__test_general__.yaml
+-rw-r--r--   0        0        0      744 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      160 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/project/__test__.yaml
+-rw-r--r--   0        0        0       38 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      298 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      183 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/task/__test__.yaml
+-rw-r--r--   0        0        0      124 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0      128 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/conf/workflow/__test__.yaml
+-rw-r--r--   0        0        0        0 2023-07-15 05:55:11.925013 hyfi_template-0.4.4/src/hyfit/py.typed
+-rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 hyfi_template-0.4.4/PKG-INFO
```

### Comparing `hyfi_template-0.4.3/LICENSE` & `hyfi_template-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.3/README.md` & `hyfi_template-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.3/pyproject.toml` & `hyfi_template-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "hyfi-template"
-version = "0.4.3"
+version = "0.4.4"
 description = "A GitHub Template Repository for HyFI-based Projects"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi-template.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi-template"
 readme = "README.md"
 packages = [{ include = "hyfit", from = "src" }]
 
 [tool.poetry.scripts]
 hyfit = 'hyfit.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^1.2.2"
+hyfi = "^1.2.6"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `hyfi_template-0.4.3/src/hyfit/conf/batch/__init__.yaml` & `hyfi_template-0.4.4/src/hyfit/conf/batch/__init__.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-batch_name: ${oc.select:..batch_name,demo-batch}
+_config_name_: __init__
+batch_name: ${oc.select:..batch_name,__init__}
 batch_num:
-batch_root: ${oc.select:..path.batch_outputs,tmp/batch-outputs/${.batch_name}}
+batch_root: ${oc.select:..task_root,workspace}/${oc.select:..path.dirnames.outputs,outputs}
 output_suffix:
 output_extention:
 random_seed: true
 seed: -1
 resume_run: false
 resume_latest: false
 device: cpu
```

### Comparing `hyfi_template-0.4.3/src/hyfit/conf/copier/conf.yaml` & `hyfi_template-0.4.4/src/hyfit/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.3/src/hyfit/conf/dotenv/__init__.yaml` & `hyfi_template-0.4.4/src/hyfit/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.3/src/hyfit/conf/hydra/help/help.yaml` & `hyfi_template-0.4.4/src/hyfit/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.3/src/hyfit/conf/mode/__init__.yaml` & `hyfi_template-0.4.4/src/hyfit/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.3/src/hyfit/conf/path/__init__.yaml` & `hyfi_template-0.4.4/src/hyfit/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.3/src/hyfit/conf/project/__init__.yaml` & `hyfi_template-0.4.4/src/hyfit/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.4.3/PKG-INFO` & `hyfi_template-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: hyfi-template
-Version: 0.4.3
+Version: 0.4.4
 Summary: A GitHub Template Repository for HyFI-based Projects
 Home-page: https://hyfi-template.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=1.2.2,<2.0.0)
+Requires-Dist: hyfi (>=1.2.6,<2.0.0)
 Project-URL: Repository, https://github.com/entelecheia/hyfi-template
 Description-Content-Type: text/markdown
 
 # HyFI Template
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
```

