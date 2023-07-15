# Comparing `tmp/langsmith-0.0.6.tar.gz` & `tmp/langsmith-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langsmith-0.0.6.tar", max compression
+gzip compressed data, was "langsmith-0.0.7.tar", max compression
```

## Comparing `langsmith-0.0.6.tar` & `langsmith-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     8031 2023-07-14 06:11:43.024263 langsmith-0.0.6/README.md
--rw-r--r--   0        0        0      478 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/cli/__init__.py
--rw-r--r--   0        0        0      363 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/cli/conf/nginx.conf
--rw-r--r--   0        0        0      143 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/cli/docker-compose.dev.yaml
--rw-r--r--   0        0        0      315 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/cli/docker-compose.ngrok.yaml
--rw-r--r--   0        0        0     1186 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/cli/docker-compose.yaml
--rw-r--r--   0        0        0    14283 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/cli/main.py
--rw-r--r--   0        0        0    31862 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/client.py
--rw-r--r--   0        0        0      234 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/evaluation/__init__.py
--rw-r--r--   0        0        0     1411 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/evaluation/evaluator.py
--rw-r--r--   0        0        0     1529 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/evaluation/string_evaluator.py
--rw-r--r--   0        0        0     9462 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/run_helpers.py
--rw-r--r--   0        0        0     6116 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/run_trees.py
--rw-r--r--   0        0        0     6499 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/schemas.py
--rw-r--r--   0        0        0     4180 2023-07-14 06:11:43.024263 langsmith-0.0.6/langsmith/utils.py
--rw-r--r--   0        0        0      858 2023-07-14 06:11:43.024263 langsmith-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     8593 1970-01-01 00:00:00.000000 langsmith-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     8031 2023-07-12 19:19:22.829561 langsmith-0.0.7/README.md
+-rw-r--r--   0        0        0      478 2023-07-10 20:55:19.191988 langsmith-0.0.7/langsmith/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:54:45.352774 langsmith-0.0.7/langsmith/cli/__init__.py
+-rw-r--r--   0        0        0      363 2023-07-05 17:54:45.353156 langsmith-0.0.7/langsmith/cli/conf/nginx.conf
+-rw-r--r--   0        0        0      143 2023-07-12 06:25:39.153595 langsmith-0.0.7/langsmith/cli/docker-compose.dev.yaml
+-rw-r--r--   0        0        0      315 2023-07-05 17:54:45.353418 langsmith-0.0.7/langsmith/cli/docker-compose.ngrok.yaml
+-rw-r--r--   0        0        0     1186 2023-07-12 00:52:45.305623 langsmith-0.0.7/langsmith/cli/docker-compose.yaml
+-rw-r--r--   0        0        0    14420 2023-07-15 15:32:37.213445 langsmith-0.0.7/langsmith/cli/main.py
+-rw-r--r--   0        0        0    31862 2023-07-15 15:34:27.624335 langsmith-0.0.7/langsmith/client.py
+-rw-r--r--   0        0        0      234 2023-07-05 17:54:45.355050 langsmith-0.0.7/langsmith/evaluation/__init__.py
+-rw-r--r--   0        0        0     1411 2023-07-05 17:54:45.355316 langsmith-0.0.7/langsmith/evaluation/evaluator.py
+-rw-r--r--   0        0        0     1529 2023-07-05 17:54:45.355546 langsmith-0.0.7/langsmith/evaluation/string_evaluator.py
+-rw-r--r--   0        0        0     9462 2023-07-05 17:54:45.355760 langsmith-0.0.7/langsmith/run_helpers.py
+-rw-r--r--   0        0        0     6116 2023-07-12 00:52:45.306853 langsmith-0.0.7/langsmith/run_trees.py
+-rw-r--r--   0        0        0     6499 2023-07-13 17:24:35.594023 langsmith-0.0.7/langsmith/schemas.py
+-rw-r--r--   0        0        0     4180 2023-07-15 15:34:27.624819 langsmith-0.0.7/langsmith/utils.py
+-rw-r--r--   0        0        0      858 2023-07-15 15:52:31.855998 langsmith-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     8593 1970-01-01 00:00:00.000000 langsmith-0.0.7/PKG-INFO
```

### Comparing `langsmith-0.0.6/README.md` & `langsmith-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.6/langsmith/cli/docker-compose.yaml` & `langsmith-0.0.7/langsmith/cli/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.6/langsmith/cli/main.py` & `langsmith-0.0.7/langsmith/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,14 +344,17 @@
     logger.info("LangChain Environment:")
     for k, v in env.items():
         logger.info(f"{k:{max_key_length}}: {v}")
 
 
 def main() -> None:
     """Main entrypoint for the CLI."""
+    print("BY USING THIS SOFTWARE YOU AGREE TO THE TERMS OF SERVICE AT:")
+    print("https://smith.langchain.com/terms-of-service.pdf")
+
     parser = argparse.ArgumentParser()
     subparsers = parser.add_subparsers(description="LangSmith CLI commands")
 
     server_command = LangSmithCommand()
     server_start_parser = subparsers.add_parser(
         "start", description="Start the LangSmith server."
     )
```

### Comparing `langsmith-0.0.6/langsmith/client.py` & `langsmith-0.0.7/langsmith/client.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.6/langsmith/evaluation/evaluator.py` & `langsmith-0.0.7/langsmith/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.6/langsmith/evaluation/string_evaluator.py` & `langsmith-0.0.7/langsmith/evaluation/string_evaluator.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.6/langsmith/run_helpers.py` & `langsmith-0.0.7/langsmith/run_helpers.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.6/langsmith/run_trees.py` & `langsmith-0.0.7/langsmith/run_trees.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.6/langsmith/schemas.py` & `langsmith-0.0.7/langsmith/schemas.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.6/langsmith/utils.py` & `langsmith-0.0.7/langsmith/utils.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.6/pyproject.toml` & `langsmith-0.0.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langsmith"
-version = "0.0.6"
+version = "0.0.7"
 description = "Client library to connect to the LangSmith LLM Tracing and Evaluation Platform."
 authors = ["LangChain"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "langsmith"}]
 
 [tool.poetry.scripts]
```

### Comparing `langsmith-0.0.6/PKG-INFO` & `langsmith-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langsmith
-Version: 0.0.6
+Version: 0.0.7
 Summary: Client library to connect to the LangSmith LLM Tracing and Evaluation Platform.
 License: MIT
 Author: LangChain
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

