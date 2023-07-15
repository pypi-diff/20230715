# Comparing `tmp/aws_lambda_env_modeler-1.0.0.tar.gz` & `tmp/aws_lambda_env_modeler-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_lambda_env_modeler-1.0.0.tar", max compression
+gzip compressed data, was "aws_lambda_env_modeler-1.0.1.tar", max compression
```

## Comparing `aws_lambda_env_modeler-1.0.0.tar` & `aws_lambda_env_modeler-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-07-15 20:33:14.961293 aws_lambda_env_modeler-1.0.0/LICENSE
--rw-r--r--   0        0        0     5038 2023-07-15 20:33:14.961293 aws_lambda_env_modeler-1.0.0/README.md
--rw-r--r--   0        0        0      281 2023-07-15 20:33:14.961293 aws_lambda_env_modeler-1.0.0/aws_lambda_env_modeler/__init__.py
--rw-r--r--   0        0        0     2377 2023-07-15 20:33:14.961293 aws_lambda_env_modeler-1.0.0/aws_lambda_env_modeler/modeler.py
--rw-r--r--   0        0        0      123 2023-07-15 20:33:14.961293 aws_lambda_env_modeler-1.0.0/aws_lambda_env_modeler/types.py
--rw-r--r--   0        0        0     1521 2023-07-15 20:33:14.965293 aws_lambda_env_modeler-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6324 1970-01-01 00:00:00.000000 aws_lambda_env_modeler-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-15 21:03:58.895693 aws_lambda_env_modeler-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5030 2023-07-15 21:03:58.895693 aws_lambda_env_modeler-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-15 21:03:58.895693 aws_lambda_env_modeler-1.0.1/aws_lambda_env_modeler/py.typed
+-rw-r--r--   0        0        0     1530 2023-07-15 21:03:58.899693 aws_lambda_env_modeler-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 aws_lambda_env_modeler-1.0.1/PKG-INFO
```

### Comparing `aws_lambda_env_modeler-1.0.0/LICENSE` & `aws_lambda_env_modeler-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_lambda_env_modeler-1.0.0/README.md` & `aws_lambda_env_modeler-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# AWS Lambda Handler Environment Variables Modeler (Python)
+# AWS Lambda Environment Variables Modeler (Python)
 
 [![license](https://img.shields.io/github/license/ran-isenberg/aws-lambda-env-modeler)](https://github.com/ran-isenberg/aws-lambda-env-modeler/blob/master/LICENSE)
 ![PythonSupport](https://img.shields.io/static/v1?label=python&message=3.8.1&color=blue?style=flat-square&logo=python)
 ![PythonSupport](https://img.shields.io/static/v1?label=python&message=3.9&color=blue?style=flat-square&logo=python)
 ![PythonSupport](https://img.shields.io/static/v1?label=python&message=3.10&color=blue?style=flat-square&logo=python)
 [![codecov](https://codecov.io/gh/ran-isenberg/aws-lambda-env-modeler/branch/main/graph/badge.svg?token=P2K7K4KICF)](https://codecov.io/gh/ran-isenberg/aws-lambda-env-modeler)
 ![version](https://img.shields.io/github/v/release/ran-isenberg/aws-lambda-env-modeler)
```

### Comparing `aws_lambda_env_modeler-1.0.0/pyproject.toml` & `aws_lambda_env_modeler-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws_lambda_env_modeler"
-version = "1.0.0"
+version = "1.0.1"
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
-    { include = "aws_lambda_env_modeler" }]
+    { include = "aws_lambda_env_modeler/py.typed" }]
 
 [tool.poetry.urls]
 "Issue tracker" = "https://github.com/ran-isenberg/aws-lambda-env-modeler/issues"
 "Releases" = "https://github.com/ran-isenberg/aws-lambda-env-modeler/releases"
 
 
 [tool.poetry.dependencies]
```

### Comparing `aws_lambda_env_modeler-1.0.0/PKG-INFO` & `aws_lambda_env_modeler-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-lambda-env-modeler
-Version: 1.0.0
+Version: 1.0.1
 Summary: AWS-Lambda-Env-Modeler is a Python library designed to simplify the process of managing and validating environment variables in your AWS Lambda functions.
 Home-page: https://github.com/ran-isenberg/aws-lambda-env-modeler
 License: MIT-0
 Keywords: environment variables parser,aws lambda,serverless best practices,aws serverless
 Author: Ran Isenberg
 Requires-Python: >=3.8.17,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,15 @@
 Requires-Dist: pydantic (>=2.0.0,<3.0.0)
 Project-URL: Issue tracker, https://github.com/ran-isenberg/aws-lambda-env-modeler/issues
 Project-URL: Repository, https://github.com/ran-isenberg/aws-lambda-env-modeler
 Project-URL: Releases, https://github.com/ran-isenberg/aws-lambda-env-modeler/releases
 Description-Content-Type: text/markdown
 
 
-# AWS Lambda Handler Environment Variables Modeler (Python)
+# AWS Lambda Environment Variables Modeler (Python)
 
 [![license](https://img.shields.io/github/license/ran-isenberg/aws-lambda-env-modeler)](https://github.com/ran-isenberg/aws-lambda-env-modeler/blob/master/LICENSE)
 ![PythonSupport](https://img.shields.io/static/v1?label=python&message=3.8.1&color=blue?style=flat-square&logo=python)
 ![PythonSupport](https://img.shields.io/static/v1?label=python&message=3.9&color=blue?style=flat-square&logo=python)
 ![PythonSupport](https://img.shields.io/static/v1?label=python&message=3.10&color=blue?style=flat-square&logo=python)
 [![codecov](https://codecov.io/gh/ran-isenberg/aws-lambda-env-modeler/branch/main/graph/badge.svg?token=P2K7K4KICF)](https://codecov.io/gh/ran-isenberg/aws-lambda-env-modeler)
 ![version](https://img.shields.io/github/v/release/ran-isenberg/aws-lambda-env-modeler)
```

