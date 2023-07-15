# Comparing `tmp/cirun-0.22.tar.gz` & `tmp/cirun-0.23.tar.gz`

## Comparing `cirun-0.22.tar` & `cirun-0.23.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 cirun-0.22/requirements.txt
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cirun-0.22/cirun/__about__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cirun-0.22/cirun/__init__.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 cirun-0.22/cirun/client.py
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 cirun-0.22/cirun/cloud.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cirun-0.22/cirun/main.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 cirun-0.22/cirun/repo.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 cirun-0.22/cirun/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cirun-0.22/cirun/tests/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 cirun-0.22/cirun/tests/test_client.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cirun-0.22/tests/__init__.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 cirun-0.22/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cirun-0.22/LICENSE.txt
--rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 cirun-0.22/README.md
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 cirun-0.22/pyproject.toml
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 cirun-0.22/PKG-INFO
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 cirun-0.23/requirements.txt
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cirun-0.23/cirun/__about__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cirun-0.23/cirun/__init__.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 cirun-0.23/cirun/client.py
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 cirun-0.23/cirun/cloud.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 cirun-0.23/cirun/main.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 cirun-0.23/cirun/repo.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 cirun-0.23/cirun/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cirun-0.23/cirun/tests/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 cirun-0.23/cirun/tests/test_client.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cirun-0.23/tests/__init__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 cirun-0.23/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cirun-0.23/LICENSE.txt
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 cirun-0.23/README.md
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 cirun-0.23/pyproject.toml
+-rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 cirun-0.23/PKG-INFO
```

### Comparing `cirun-0.22/cirun/client.py` & `cirun-0.23/cirun/client.py`

 * *Files identical despite different names*

### Comparing `cirun-0.22/cirun/cloud.py` & `cirun-0.23/cirun/cloud.py`

 * *Files identical despite different names*

### Comparing `cirun-0.22/cirun/repo.py` & `cirun-0.23/cirun/repo.py`

 * *Files identical despite different names*

### Comparing `cirun-0.22/.gitignore` & `cirun-0.23/.gitignore`

 * *Files identical despite different names*

### Comparing `cirun-0.22/LICENSE.txt` & `cirun-0.23/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cirun-0.22/README.md` & `cirun-0.23/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 
 ## Installation
 
 ```console
 pip install cirun
 ```
 
+or via `conda-forge`
+
+```console
+conda install -c conda-forge cirun
+```
+
 ## Usage
 
 **cirun-py** can be used as a CLI as well as a Python client programmatically.
 
 - Create an API key from the Cirun Dashboard https://cirun.io/admin/api
 - Set that API Key as an environment variable named `CIRUN_API_KEY`
```

### Comparing `cirun-0.22/pyproject.toml` & `cirun-0.23/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -29,17 +29,17 @@
   "typer",
   "hatch",
   "requests",
 ]
 dynamic = ["version"]
 
 [project.urls]
-Documentation = "https://github.com/aktechlabs/cirun#readme"
-Issues = "https://github.com/aktechlabs/cirun-docs/issues"
-Source = "https://github.com/aktechlabs/cirun-docs"
+Documentation = "https://github.com/aktechlabs/cirun-py#readme"
+Issues = "https://github.com/aktechlabs/cirun-py/issues"
+Source = "https://github.com/aktechlabs/cirun-py"
 
 [tool.hatch.version]
 path = "cirun/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
```

### Comparing `cirun-0.22/PKG-INFO` & `cirun-0.23/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: cirun
-Version: 0.22
+Version: 0.23
 Summary: Cirun Python Client
-Project-URL: Documentation, https://github.com/aktechlabs/cirun#readme
-Project-URL: Issues, https://github.com/aktechlabs/cirun-docs/issues
-Project-URL: Source, https://github.com/aktechlabs/cirun-docs
+Project-URL: Documentation, https://github.com/aktechlabs/cirun-py#readme
+Project-URL: Issues, https://github.com/aktechlabs/cirun-py/issues
+Project-URL: Source, https://github.com/aktechlabs/cirun-py
 Author-email: Amit Kumar <amit@cirun.io>
+License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -39,14 +40,20 @@
 
 ## Installation
 
 ```console
 pip install cirun
 ```
 
+or via `conda-forge`
+
+```console
+conda install -c conda-forge cirun
+```
+
 ## Usage
 
 **cirun-py** can be used as a CLI as well as a Python client programmatically.
 
 - Create an API key from the Cirun Dashboard https://cirun.io/admin/api
 - Set that API Key as an environment variable named `CIRUN_API_KEY`
```

