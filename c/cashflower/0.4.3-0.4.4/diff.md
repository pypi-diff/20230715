# Comparing `tmp/cashflower-0.4.3.tar.gz` & `tmp/cashflower-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashflower-0.4.3.tar", last modified: Thu Jul 13 18:54:42 2023, max compression
+gzip compressed data, was "cashflower-0.4.4.tar", last modified: Sat Jul 15 14:17:55 2023, max compression
```

## Comparing `cashflower-0.4.3.tar` & `cashflower-0.4.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:54:42.657668 cashflower-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-13 18:54:30.000000 cashflower-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-13 18:54:30.000000 cashflower-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-13 18:54:42.657668 cashflower-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-13 18:54:30.000000 cashflower-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:54:42.653668 cashflower-0.4.3/cashflower/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/cashflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:54:42.657668 cashflower-0.4.3/cashflower/model_tpl/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/model_tpl/input.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/model_tpl/model.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/model_tpl/run.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/model_tpl/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7945 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-13 18:54:30.000000 cashflower-0.4.3/cashflower/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:54:42.657668 cashflower-0.4.3/cashflower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-13 18:54:42.000000 cashflower-0.4.3/cashflower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-13 18:54:42.000000 cashflower-0.4.3/cashflower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 18:54:42.000000 cashflower-0.4.3/cashflower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 18:54:42.000000 cashflower-0.4.3/cashflower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 18:54:42.000000 cashflower-0.4.3/cashflower.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 18:54:42.657668 cashflower-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-13 18:54:30.000000 cashflower-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 18:54:42.657668 cashflower-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-13 18:54:30.000000 cashflower-0.4.3/tests/test_cashflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-13 18:54:30.000000 cashflower-0.4.3/tests/test_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-13 18:54:30.000000 cashflower-0.4.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:17:55.696344 cashflower-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-15 14:17:44.000000 cashflower-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-15 14:17:44.000000 cashflower-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-15 14:17:55.696344 cashflower-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-15 14:17:44.000000 cashflower-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:17:55.692344 cashflower-0.4.4/cashflower/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/cashflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:17:55.696344 cashflower-0.4.4/cashflower/model_tpl/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/model_tpl/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/model_tpl/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/model_tpl/run.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/model_tpl/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:17:55.696344 cashflower-0.4.4/cashflower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-15 14:17:55.000000 cashflower-0.4.4/cashflower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-15 14:17:55.000000 cashflower-0.4.4/cashflower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 14:17:55.000000 cashflower-0.4.4/cashflower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-15 14:17:55.000000 cashflower-0.4.4/cashflower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-15 14:17:55.000000 cashflower-0.4.4/cashflower.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 14:17:55.696344 cashflower-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-15 14:17:44.000000 cashflower-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:17:55.696344 cashflower-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-15 14:17:44.000000 cashflower-0.4.4/tests/test_cashflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-15 14:17:44.000000 cashflower-0.4.4/tests/test_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-15 14:17:44.000000 cashflower-0.4.4/tests/test_utils.py
```

### Comparing `cashflower-0.4.3/LICENSE` & `cashflower-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.3/PKG-INFO` & `cashflower-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashflower
-Version: 0.4.3
+Version: 0.4.4
 Summary: Framework for actuarial cash flow models
 Home-page: https://github.com/acturtle/cashflower
 Author: Zuzanna Chmielewska
 Project-URL: Source, https://github.com/acturtle/cashflower
 Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
 Project-URL: Documentation, https://cashflower.acturtle.com
 Requires-Python: >=3.9
```

### Comparing `cashflower-0.4.3/README.md` & `cashflower-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.3/cashflower/cashflow.py` & `cashflower-0.4.4/cashflower/cashflow.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.3/cashflower/graph.py` & `cashflower-0.4.4/cashflower/graph.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.3/cashflower/start.py` & `cashflower-0.4.4/cashflower/start.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,21 +20,18 @@
     template_path = os.path.join(os.path.dirname(__file__), "model_tpl")
     current_path = os.getcwd()
 
     shutil.copytree(template_path, model)
 
     # Some scripts needs words replacements
     run_file = os.path.join(current_path, model, "run.py-tpl")
-    model_file = os.path.join(current_path, model, "model.py-tpl")
     replace_in_file(run_file, "{{ model }}", model)
-    replace_in_file(model_file, "{{ model }}", model)
 
     # Remove -tpl from template
     os.rename(run_file, run_file[:-4])
-    os.rename(model_file, model_file[:-4])
 
 
 def load_settings(settings=None):
     """Add missing settings."""
     initial_settings = {
         "AGGREGATE": True,
         "MULTIPROCESSING": False,
@@ -106,16 +103,16 @@
         variable.settings = settings
         variables.append(variable)
     return variables
 
 
 def prepare_model_input(model_name, settings, argv):
     """Get input for the cash flow model."""
-    input_module = importlib.import_module(model_name + ".input")
-    model_module = importlib.import_module(model_name + ".model")
+    input_module = importlib.import_module("input")
+    model_module = importlib.import_module("model")
 
     # input.py contains runplan and model point sets
     input_members = inspect.getmembers(input_module)
     runplan = get_runplan(input_members)
     model_point_sets, main = get_model_point_sets(input_members, settings)
 
     # model.py contains model variables
```

### Comparing `cashflower-0.4.3/cashflower/utils.py` & `cashflower-0.4.4/cashflower/utils.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.3/cashflower.egg-info/PKG-INFO` & `cashflower-0.4.4/cashflower.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashflower
-Version: 0.4.3
+Version: 0.4.4
 Summary: Framework for actuarial cash flow models
 Home-page: https://github.com/acturtle/cashflower
 Author: Zuzanna Chmielewska
 Project-URL: Source, https://github.com/acturtle/cashflower
 Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
 Project-URL: Documentation, https://cashflower.acturtle.com
 Requires-Python: >=3.9
```

### Comparing `cashflower-0.4.3/cashflower.egg-info/SOURCES.txt` & `cashflower-0.4.4/cashflower.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 cashflower/utils.py
 cashflower.egg-info/PKG-INFO
 cashflower.egg-info/SOURCES.txt
 cashflower.egg-info/dependency_links.txt
 cashflower.egg-info/requires.txt
 cashflower.egg-info/top_level.txt
 cashflower/model_tpl/input.py
-cashflower/model_tpl/model.py-tpl
+cashflower/model_tpl/model.py
 cashflower/model_tpl/run.py-tpl
 cashflower/model_tpl/settings.py
 tests/test_cashflow.py
 tests/test_start.py
 tests/test_utils.py
```

### Comparing `cashflower-0.4.3/setup.py` & `cashflower-0.4.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,9 +20,9 @@
     project_urls={
         'Source': 'https://github.com/acturtle/cashflower',
         'Tracker': 'https://github.com/acturtle/cashflower/issues',
         'Documentation': 'https://cashflower.acturtle.com',
     },
     python_requires='>=3.9',
     url="https://github.com/acturtle/cashflower",
-    version="0.4.3",
+    version="0.4.4",
 )
```

### Comparing `cashflower-0.4.3/tests/test_cashflow.py` & `cashflower-0.4.4/tests/test_cashflow.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.3/tests/test_start.py` & `cashflower-0.4.4/tests/test_start.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.3/tests/test_utils.py` & `cashflower-0.4.4/tests/test_utils.py`

 * *Files identical despite different names*

