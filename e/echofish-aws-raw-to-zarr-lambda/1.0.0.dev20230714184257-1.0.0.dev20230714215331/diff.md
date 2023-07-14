# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257.tar", last modified: Fri Jul 14 18:44:04 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331.tar", last modified: Fri Jul 14 21:54:32 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:44:04.391390 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-14 18:42:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 18:44:04.391390 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-14 18:42:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 18:44:04.391390 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-07-14 18:43:59.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:44:04.387390 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:44:04.387390 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 18:42:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-07-14 18:42:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
--rw-r--r--   0 root         (0) root         (0)    15406 2023-07-14 18:42:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)     1148 2023-07-14 18:42:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
--rw-r--r--   0 root         (0) root         (0)     3398 2023-07-14 18:42:52.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 18:44:04.391390 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 18:44:04.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      587 2023-07-14 18:44:04.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 18:44:04.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-07-14 18:44:04.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-14 18:44:04.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 21:54:32.362311 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-14 21:53:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 21:54:32.362311 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-14 21:53:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 21:54:32.362311 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-07-14 21:54:28.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 21:54:32.358312 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 21:54:32.362311 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 21:53:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-07-14 21:53:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15781 2023-07-14 21:53:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1302 2023-07-14 21:53:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3398 2023-07-14 21:53:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+-rw-r--r--   0 root         (0) root         (0)      212 2023-07-14 21:53:26.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/sns_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 21:54:32.362311 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 21:54:32.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      641 2023-07-14 21:54:32.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 21:54:32.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-07-14 21:54:32.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-14 21:54:32.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230714184257
+Version: 1.0.0.dev20230714215331
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230714184257",
+  version="1.0.0.dev20230714215331",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,39 +2,44 @@
 import os
 import glob
 import shutil
 import echopype as ep
 import numpy as np
 import pandas as pd
 import geopandas
+import json
 from datetime import datetime
 
 TEMPDIR = "/tmp"
 
 
 class LambdaExecutor:
 
     ############################################################################
     def __init__(
             self,
             s3_operations,
             dynamo_operations,
+            sns_operations,
             input_bucket,
             output_bucket,
             table_name,
             output_bucket_access_key,
             output_bucket_secret_access_key,
+            done_topic_arn,
     ):
         self.__s3 = s3_operations
         self.__dynamo = dynamo_operations
+        self.__sns_operations = sns_operations
         self.__input_bucket = input_bucket
         self.__output_bucket = output_bucket
         self.__table_name = table_name
         self.__output_bucket_access_key = output_bucket_access_key
         self.__output_bucket_secret_access_key = output_bucket_secret_access_key
+        self.__done_topic_arn = done_topic_arn
 
     ############################################################################
     def __delete_all_local_raw_and_zarr_files(self):  # good
         """Used to clean up any residual files from warm lambdas
         to keep the storage footprint below the 512 MB allocation.
 
         Returns
@@ -344,14 +349,18 @@
                     bucket_name=self.__output_bucket,
                     key=s3_key,
                     access_key_id=self.__output_bucket_access_key,
                     secret_access_key=self.__output_bucket_secret_access_key
                 )
         # print('Done uploading files')
 
+    def __publish_done_message(self, message):
+        print("Sending done message")
+        self.__sns_operations.publish(self.__done_topic_arn, json.dumps(message))
+
     ############################################################################
     def execute(self, message):
         ship_name = message['shipName']
         cruise_name = message['cruiseName']
         sensor_name = message['sensorName']
         input_file_name = message['fileName']
 
@@ -391,9 +400,10 @@
         self.__update_processing_status(
             cruise_name=cruise_name,
             file_name=input_file_name,
             new_status='SUCCESS'
         )
         self.__delete_all_local_raw_and_zarr_files()
         #
+        self.__publish_done_message(message)
         print(f'Done processing {input_file_name}')
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # lambda_handler.py
 import os
 import json
 from .lambda_executor import LambdaExecutor
 from .s3_operations import S3Operations
 from .dynamo_operations import DynamoOperations
+from .sns_operations import SnsOperations
 
 
 input_bucket = os.environ['INPUT_BUCKET']
 output_bucket = os.environ['OUTPUT_BUCKET']
 table_name = os.environ['TABLE_NAME']
 output_bucket_access_key = os.environ['OUTPUT_BUCKET_ACCESS_KEY']
 output_bucket_secret_access_key = os.environ['OUTPUT_BUCKET_SECRET_ACCESS_KEY']
+done_topic_arn = os.environ['TOPIC_ARN']
 
 executor = LambdaExecutor(
     s3_operations=S3Operations(),
     dynamo_operations=DynamoOperations(),
+    sns_operations=SnsOperations(),
     input_bucket=input_bucket,
     output_bucket=output_bucket,
     table_name=table_name,
     output_bucket_access_key=output_bucket_access_key,
-    output_bucket_secret_access_key=output_bucket_secret_access_key
+    output_bucket_secret_access_key=output_bucket_secret_access_key,
+    done_topic_arn=done_topic_arn
 )
 
 def handler(sns_event, context):
     print("Event : " + str(sns_event))
     print("Context : " + str(context))
     for record in sns_event['Records']:
         message = json.loads(record['Sns']['Message'])
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230714184257
+Version: 1.0.0.dev20230714215331
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714184257/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230714215331/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,12 +2,13 @@
 README.md
 setup.py
 src/echofish_aws_raw_to_zarr_lambda/__init__.py
 src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
 src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
 src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
 src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+src/echofish_aws_raw_to_zarr_lambda/sns_operations.py
 src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
 src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
 src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
 src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
 src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

