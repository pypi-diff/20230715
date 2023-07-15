# Comparing `tmp/aws_lambda_env_modeler-1.0.1.tar.gz` & `tmp/aws_lambda_env_modeler-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_lambda_env_modeler-1.0.1.tar", max compression
+gzip compressed data, was "aws_lambda_env_modeler-1.0.2.tar", max compression
```

## Comparing `aws_lambda_env_modeler-1.0.1.tar` & `aws_lambda_env_modeler-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-07-15 21:03:58.895693 aws_lambda_env_modeler-1.0.1/LICENSE
--rw-r--r--   0        0        0     5030 2023-07-15 21:03:58.895693 aws_lambda_env_modeler-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-15 21:03:58.895693 aws_lambda_env_modeler-1.0.1/aws_lambda_env_modeler/py.typed
--rw-r--r--   0        0        0     1530 2023-07-15 21:03:58.899693 aws_lambda_env_modeler-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 aws_lambda_env_modeler-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-15 21:17:59.659913 aws_lambda_env_modeler-1.0.2/LICENSE
+-rw-r--r--   0        0        0     5030 2023-07-15 21:17:59.659913 aws_lambda_env_modeler-1.0.2/README.md
+-rw-r--r--   0        0        0      281 2023-07-15 21:17:59.659913 aws_lambda_env_modeler-1.0.2/aws_lambda_env_modeler/__init__.py
+-rw-r--r--   0        0        0     2377 2023-07-15 21:17:59.659913 aws_lambda_env_modeler-1.0.2/aws_lambda_env_modeler/modeler.py
+-rw-r--r--   0        0        0        0 2023-07-15 21:17:59.659913 aws_lambda_env_modeler-1.0.2/aws_lambda_env_modeler/py.typed
+-rw-r--r--   0        0        0      136 2023-07-15 21:17:59.659913 aws_lambda_env_modeler-1.0.2/aws_lambda_env_modeler/types.py
+-rw-r--r--   0        0        0     1521 2023-07-15 21:17:59.663913 aws_lambda_env_modeler-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 aws_lambda_env_modeler-1.0.2/PKG-INFO
```

### Comparing `aws_lambda_env_modeler-1.0.1/LICENSE` & `aws_lambda_env_modeler-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_lambda_env_modeler-1.0.1/README.md` & `aws_lambda_env_modeler-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aws_lambda_env_modeler-1.0.1/pyproject.toml` & `aws_lambda_env_modeler-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws_lambda_env_modeler"
-version = "1.0.1"
+version = "1.0.2"
 description = "AWS-Lambda-Env-Modeler is a Python library designed to simplify the process of managing and validating environment variables in your AWS Lambda functions."
 authors = ["Ran Isenberg"]
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
@@ -13,15 +13,15 @@
     "Programming Language :: Python :: 3.10",
 ]
 repository="https://github.com/ran-isenberg/aws-lambda-env-modeler"
 readme = "README.md"
 keywords = ["environment variables parser", "aws lambda", "serverless best practices", "aws serverless"]
 license = "MIT-0"
 packages = [
-    { include = "aws_lambda_env_modeler/py.typed" }]
+    { include = "aws_lambda_env_modeler" }]
 
 [tool.poetry.urls]
 "Issue tracker" = "https://github.com/ran-isenberg/aws-lambda-env-modeler/issues"
 "Releases" = "https://github.com/ran-isenberg/aws-lambda-env-modeler/releases"
 
 
 [tool.poetry.dependencies]
```

### Comparing `aws_lambda_env_modeler-1.0.1/PKG-INFO` & `aws_lambda_env_modeler-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-lambda-env-modeler
-Version: 1.0.1
+Version: 1.0.2
 Summary: AWS-Lambda-Env-Modeler is a Python library designed to simplify the process of managing and validating environment variables in your AWS Lambda functions.
 Home-page: https://github.com/ran-isenberg/aws-lambda-env-modeler
 License: MIT-0
 Keywords: environment variables parser,aws lambda,serverless best practices,aws serverless
 Author: Ran Isenberg
 Requires-Python: >=3.8.17,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

