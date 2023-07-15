# Comparing `tmp/together-0.0.6.tar.gz` & `tmp/together-0.0.7.tar.gz`

## Comparing `together-0.0.6.tar` & `together-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 together-0.0.6/.github/workflows/check_code_quality.yml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 together-0.0.6/src/together/__init__.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 together-0.0.6/src/together/api.py
--rw-r--r--   0        0        0     8689 2020-02-02 00:00:00.000000 together-0.0.6/src/together/files.py
--rw-r--r--   0        0        0    10069 2020-02-02 00:00:00.000000 together-0.0.6/src/together/finetune.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 together-0.0.6/src/together/inference.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 together-0.0.6/src/together/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.0.6/src/together/cli/__init__.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 together-0.0.6/src/together/cli/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.0.6/src/together/commands/__init__.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 together-0.0.6/src/together/commands/api.py
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 together-0.0.6/src/together/commands/files.py
--rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 together-0.0.6/src/together/commands/finetune.py
--rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 together-0.0.6/src/together/commands/inference.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 together-0.0.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 together-0.0.6/LICENSE
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 together-0.0.6/README.md
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 together-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 together-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 together-0.0.7/.github/workflows/check_code_quality.yml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 together-0.0.7/src/together/__init__.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 together-0.0.7/src/together/api.py
+-rw-r--r--   0        0        0     8689 2020-02-02 00:00:00.000000 together-0.0.7/src/together/files.py
+-rw-r--r--   0        0        0    10069 2020-02-02 00:00:00.000000 together-0.0.7/src/together/finetune.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 together-0.0.7/src/together/inference.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 together-0.0.7/src/together/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.0.7/src/together/cli/__init__.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 together-0.0.7/src/together/cli/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.0.7/src/together/commands/__init__.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 together-0.0.7/src/together/commands/api.py
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 together-0.0.7/src/together/commands/files.py
+-rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 together-0.0.7/src/together/commands/finetune.py
+-rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 together-0.0.7/src/together/commands/inference.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 together-0.0.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 together-0.0.7/LICENSE
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 together-0.0.7/README.md
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 together-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 together-0.0.7/PKG-INFO
```

### Comparing `together-0.0.6/.github/workflows/check_code_quality.yml` & `together-0.0.7/.github/workflows/check_code_quality.yml`

 * *Files identical despite different names*

### Comparing `together-0.0.6/src/together/api.py` & `together-0.0.7/src/together/api.py`

 * *Files identical despite different names*

### Comparing `together-0.0.6/src/together/files.py` & `together-0.0.7/src/together/files.py`

 * *Files identical despite different names*

### Comparing `together-0.0.6/src/together/finetune.py` & `together-0.0.7/src/together/finetune.py`

 * *Files identical despite different names*

### Comparing `together-0.0.6/src/together/inference.py` & `together-0.0.7/src/together/inference.py`

 * *Files identical despite different names*

### Comparing `together-0.0.6/src/together/utils.py` & `together-0.0.7/src/together/utils.py`

 * *Files identical despite different names*

### Comparing `together-0.0.6/src/together/cli/cli.py` & `together-0.0.7/src/together/cli/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,20 +36,24 @@
     inference.add_parser(subparser, parents=[base_subparser])
     finetune.add_parser(subparser, parents=[base_subparser])
     files.add_parser(subparser, parents=[base_subparser])
 
     args = parser.parse_args()
 
     # Setup logging
-    logger = get_logger(__name__, log_level=args.log)
+    try:
+        logger = get_logger(__name__, log_level=args.log)
+    except Exception:
+        logger = get_logger(__name__, log_level="WARNING")
 
     try:
         args.func(args)
     except AttributeError as e:
         # print error, but ignore if `together` is run.
         if str(e) != "'Namespace' object has no attribute 'func'":
             logger.critical(f"Error raised: {e}")
             exit_1(logger)
+        parser.print_help()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `together-0.0.6/src/together/commands/api.py` & `together-0.0.7/src/together/commands/api.py`

 * *Files identical despite different names*

### Comparing `together-0.0.6/src/together/commands/files.py` & `together-0.0.7/src/together/commands/files.py`

 * *Files identical despite different names*

### Comparing `together-0.0.6/src/together/commands/finetune.py` & `together-0.0.7/src/together/commands/finetune.py`

 * *Files identical despite different names*

### Comparing `together-0.0.6/src/together/commands/inference.py` & `together-0.0.7/src/together/commands/inference.py`

 * *Files identical despite different names*

### Comparing `together-0.0.6/.gitignore` & `together-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `together-0.0.6/LICENSE` & `together-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `together-0.0.6/pyproject.toml` & `together-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "together"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Together Computer", email="community@together.xyz" },
 ]
-description = "Python client for Together's Cloud Platform"
+description = "Python client for Together's Cloud Platform!"
 readme = "README.md"
 license = {file = "LICENSE"}
-requires-python = ">=3.10"
+requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: POSIX :: Linux",
 ]
 
 dependencies = [
```

### Comparing `together-0.0.6/PKG-INFO` & `together-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: together
-Version: 0.0.6
-Summary: Python client for Together's Cloud Platform
+Version: 0.0.7
+Summary: Python client for Together's Cloud Platform!
 Project-URL: Homepage, https://github.com/togethercomputer/together
 Project-URL: Bug Tracker, https://github.com/togethercomputer/together/issues
 Author-email: Together Computer <community@together.xyz>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -206,15 +206,15 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Requires-Python: >=3.6
 Requires-Dist: requests
 Requires-Dist: tqdm
 Requires-Dist: typer
 Provides-Extra: quality
 Requires-Dist: black~=23.1; extra == 'quality'
 Requires-Dist: mypy>=1.3.0; extra == 'quality'
 Requires-Dist: ruff<=0.0.259,>=0.0.241; extra == 'quality'
```

