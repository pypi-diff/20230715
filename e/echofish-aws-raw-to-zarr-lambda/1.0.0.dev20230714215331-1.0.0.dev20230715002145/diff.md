# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331.tar", last modified: Fri Jul 14 21:54:32 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145.tar", last modified: Sat Jul 15 00:22:49 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 21:54:32.362311 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-14 21:53:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 21:54:32.362311 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-14 21:53:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 21:54:32.362311 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-14 21:54:28.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 21:54:32.358312 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 21:54:32.362311 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 21:53:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-14 21:53:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15781 2023-07-14 21:53:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1302 2023-07-14 21:53:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3398 2023-07-14 21:53:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
--rw-r--r--   0 root         (0) root         (0)      212 2023-07-14 21:53:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/sns_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 21:54:32.362311 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 21:54:32.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      641 2023-07-14 21:54:32.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 21:54:32.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-14 21:54:32.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-14 21:54:32.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 00:22:49.343997 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-15 00:21:40.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-15 00:22:49.343997 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-15 00:21:40.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-15 00:22:49.343997 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-15 00:22:44.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 00:22:49.339997 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 00:22:49.339997 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-15 00:21:40.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-15 00:21:40.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15781 2023-07-15 00:21:40.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-07-15 00:21:40.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3398 2023-07-15 00:21:40.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-15 00:21:40.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda/sns_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 00:22:49.343997 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-15 00:22:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      641 2023-07-15 00:22:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 00:22:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-15 00:22:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-15 00:22:49.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230714215331
+Version: 1.0.0.dev20230715002145
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230714215331",
+  version="1.0.0.dev20230715002145",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230714215331
+Version: 1.0.0.dev20230715002145
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230715002145/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

