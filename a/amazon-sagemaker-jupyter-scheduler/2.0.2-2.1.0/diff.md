# Comparing `tmp/amazon_sagemaker_jupyter_scheduler-2.0.2.tar.gz` & `tmp/amazon_sagemaker_jupyter_scheduler-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon_sagemaker_jupyter_scheduler-2.0.2.tar", last modified: Sat Jul  8 01:27:42 2023, max compression
+gzip compressed data, was "amazon_sagemaker_jupyter_scheduler-2.1.0.tar", last modified: Thu Jul 13 17:45:27 2023, max compression
```

## Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2.tar` & `amazon_sagemaker_jupyter_scheduler-2.1.0.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.172769 amazon_sagemaker_jupyter_scheduler-2.0.2/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       66 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/.eslintignore
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1026 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/.eslintrc.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1605 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/.gitignore
--rw-r--r--   0 p4admin  (12569) amazon     (100)      102 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/.prettierignore
--rw-r--r--   0 p4admin  (12569) amazon     (100)      102 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/.prettierrc
--rw-r--r--   0 p4admin  (12569) amazon     (100)      739 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/Config
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2329 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/DEVELOPMENT.md
--rw-r--r--   0 p4admin  (12569) amazon     (100)      686 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/MANIFEST.in
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1174 2023-07-08 01:27:42.172769 amazon_sagemaker_jupyter_scheduler-2.0.2/PKG-INFO
--rw-r--r--   0 p4admin  (12569) amazon     (100)      347 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/README.md
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2046 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/RELEASE.md
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.148769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      806 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      455 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/_version.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.152769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/advanced_environments/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/advanced_environments/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      163 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/advanced_environments/base_advanced_environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5969 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_advanced_environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    13864 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_studio_advanced_environment.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2541 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/app_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      465 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/aws_config.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.140769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/botocore_model/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.140769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.152769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/
--rw-r--r--   0 p4admin  (12569) amazon     (100)  1377688 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/service-2.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)    19161 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/clients.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2538 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/cron_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2060 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/deletable_resource.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1501 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/environment_detector.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5211 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3338 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/error_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      820 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/extension.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5757 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/file_uploader.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6084 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/handlers.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    65897 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/host_region_mapping.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1533 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/internal_metadata_adapter.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.152769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4948 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/package.json
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.140769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/schemas/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.140769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.152769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1130 2023-07-08 01:27:32.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/advanced-options.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4834 2023-07-08 01:27:32.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/package.json.orig
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.156769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1875 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/144.9be27e93647ef0e84863.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   242036 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      166 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)    26299 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)   106222 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      412 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)    13283 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/509.b1db44e3c8c1ddb64444.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1875 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/615.d5639a877b54ff655d41.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)   209775 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      706 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4059 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js.LICENSE.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)    50576 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/993.faa5510ce9696a850c76.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8346 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.9f672e548acd2153a221.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      118 2023-07-08 01:27:32.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/style.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)    66200 2023-07-08 01:27:41.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6440 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/logging.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    30236 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/model_converter.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3796 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/models.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.156769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      759 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      528 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/revenue.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9468 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4682 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3788 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/tags.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2295 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/runtime_environment_parameters.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      498 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/s3_uri.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    43813 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/scheduler.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.160769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/__init__.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.160769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/helpers/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/helpers/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      913 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/helpers/utils.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.160769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/providers/
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/providers/__init__.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9555 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/providers/test_image_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     8033 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/providers/test_tags.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    14065 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_advanced_environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3180 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_app_metadata.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1145 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_aws_config.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    17404 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_clients.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1694 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_cron_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2149 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_deletable_resource.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1895 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_environment_detector.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1529 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_environments.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1512 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_error_util.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6823 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_file_uploader.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2280 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_handlers.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3519 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_internal_metadata_adapter.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     5843 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_logging.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    24154 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_model_converter.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1747 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_runtime_environment_parameters.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)    33726 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_scheduler.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)      427 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_utils.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2805 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/utils.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.152769 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler.egg-info/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1174 2023-07-08 01:27:42.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9270 2023-07-08 01:27:42.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2023-07-08 01:27:42.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2023-07-08 01:27:42.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 p4admin  (12569) amazon     (100)      208 2023-07-08 01:27:42.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler.egg-info/requires.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-07-08 01:27:42.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler.egg-info/top_level.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)      261 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/babel.config.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)       73 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/custom.d.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      827 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/jest.config.base.js
--rw-r--r--   0 p4admin  (12569) amazon     (100)      510 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/jest.config.js
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.160769 amazon_sagemaker_jupyter_scheduler-2.0.2/jupyter-config/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.160769 amazon_sagemaker_jupyter_scheduler-2.0.2/jupyter-config/jupyter_server_config.d/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      109 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/jupyter-config/jupyter_server_config.d/amazon_sagemaker_jupyter_scheduler.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)      306 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/jupyter-config/jupyter_server_config.py
--rw-r--r--   0 p4admin  (12569) amazon     (100)   965893 2023-07-08 01:27:31.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/package-lock.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4834 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/package.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)      127 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/pyproject.toml
--rw-r--r--   0 p4admin  (12569) amazon     (100)      133 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/requirements.txt
--rw-r--r--   0 p4admin  (12569) amazon     (100)       38 2023-07-08 01:27:42.172769 amazon_sagemaker_jupyter_scheduler-2.0.2/setup.cfg
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3069 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/setup.py
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/__mocks__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/__mocks__/fileMock.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/__tests__/
--rwxr-xr-x   0 p4admin  (12569) amazon     (100)    12302 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/__tests__/CreateNotebookJobForm.spec.tsx
--rwxr-xr-x   0 p4admin  (12569) amazon     (100)     4348 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/__tests__/VpcCheckbox.spec.tsx
--rwxr-xr-x   0 p4admin  (12569) amazon     (100)    13449 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/__tests__/initalValueHelpers.spec.ts
--rwxr-xr-x   0 p4admin  (12569) amazon     (100)    11135 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/__tests__/validationHelpers.spec.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.140769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      964 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/Link.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      754 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/RouterLink.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/__test__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1005 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/__test__/Link.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      609 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/__test__/RouterLink.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      184 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/types.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/selectinput/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1583 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/selectinput/SelectInput.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       56 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/selectinput/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      967 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/selectinput/types.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1626 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/TextInput.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1656 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/__tests__/TextInput.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       54 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2932 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      206 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/types.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/tooltip/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1348 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/tooltip/Tooltip.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.164769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/tooltip/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1040 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/tooltip/__tests__/Tooltip.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       27 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/tooltip/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      553 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/tooltip/styles.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.168769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/constants/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     7978 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/constants/common.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       53 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/constants/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       99 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/constants/kernels.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      186 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/index.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.168769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/plugins/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3429 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/plugins/ScheduleNotebookDisablerPlugin.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1455 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/plugins/ScheduleNotebookPlugin.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       92 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/plugins/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3328 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/themeProvider.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.168769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/types/
--rw-r--r--   0 p4admin  (12569) amazon     (100)      420 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/types/images.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       82 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/types/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      141 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/types/kernels.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      132 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/types/sagemaker.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.168769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1929 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/PluginEnvironmentProvider.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.168769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/__tests__/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1833 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/__tests__/PluginEnvironmentProvider.spec.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      123 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/common.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1528 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/images.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      108 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1205 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/kernels.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1017 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/rendering.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.168769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4226 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJob.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.168769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.172769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/
--rw-r--r--   0 p4admin  (12569) amazon     (100)    15893 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/AdvancedOptions.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.172769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3900 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariable.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3230 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariables.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1094 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/styles.ts
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.172769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3551 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/VpcCheckbox.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)       55 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      285 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     4808 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/validationHelpers.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)    13805 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/CreateNotebookJobform.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1229 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/InputContainer.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.172769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/JobEnvironment/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2737 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/JobEnvironment/DefaultJobEnvironment.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      712 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/JobEnvironment/JobEnvironmentContainer.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      118 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/JobEnvironment/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1280 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/JobEnvironment/jobEnvironment.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     3138 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/MultiSelectContainer.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1554 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/SelectInputContainer.tsx
-drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:27:42.172769 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1613 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/StudioImageSelectorOption.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)     6035 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/StudioJobEnvironment.tsx
--rw-r--r--   0 p4admin  (12569) amazon     (100)      552 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioApi.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)    12172 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioHelpers.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)    64113 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioMock.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)      781 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioModel.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1305 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioStyles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)       41 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     7544 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/initialValueHelpers.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     1727 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/index.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2216 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/mockResponses.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     2723 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/styles.ts
--rw-r--r--   0 p4admin  (12569) amazon     (100)     9250 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/tsconfig.base.json
--rw-r--r--   0 p4admin  (12569) amazon     (100)      304 2023-07-08 01:25:34.000000 amazon_sagemaker_jupyter_scheduler-2.0.2/tsconfig.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.709317 amazon_sagemaker_jupyter_scheduler-2.1.0/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       66 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/.eslintignore
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1026 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/.eslintrc.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1605 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/.gitignore
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      102 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/.prettierignore
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      102 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/.prettierrc
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      739 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/Config
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2329 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/DEVELOPMENT.md
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      686 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/MANIFEST.in
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1174 2023-07-13 17:45:27.709317 amazon_sagemaker_jupyter_scheduler-2.1.0/PKG-INFO
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      347 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/README.md
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2046 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/RELEASE.md
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.681318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      806 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      455 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/_version.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.681318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      163 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/base_advanced_environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5969 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_advanced_environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    13333 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_studio_advanced_environment.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2541 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/app_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      465 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/aws_config.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.669318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/botocore_model/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.669318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.681318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)  1377688 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/service-2.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    19161 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/clients.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2538 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/cron_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2060 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/deletable_resource.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1501 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/environment_detector.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5211 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3338 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/error_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      820 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/extension.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5757 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/file_uploader.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6084 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/handlers.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    65897 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/host_region_mapping.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1533 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/internal_metadata_adapter.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.685318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4948 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/package.json
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.669318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.669318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.685318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1130 2023-07-13 17:45:16.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/advanced-options.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4834 2023-07-13 17:45:16.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/package.json.orig
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.689318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1875 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/144.9be27e93647ef0e84863.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   242036 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      166 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    26299 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   106222 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      412 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    13283 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/509.b1db44e3c8c1ddb64444.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1875 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/615.d5639a877b54ff655d41.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   209775 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      706 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4059 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js.LICENSE.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    52588 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/993.84c00bb76b4448d8ce3f.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8346 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.299f9d522c52a504280b.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      118 2023-07-13 17:45:16.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/style.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    66200 2023-07-13 17:45:26.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6440 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/logging.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    31271 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/model_converter.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3898 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/models.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.689318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      759 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      528 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/revenue.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9468 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4682 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3788 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/tags.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2930 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/runtime_environment_parameters.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      498 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/s3_uri.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    44823 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/scheduler.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.693318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/__init__.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.693318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/helpers/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/helpers/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      913 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/helpers/utils.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.693318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/providers/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/providers/__init__.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9555 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/providers/test_image_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8033 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/providers/test_tags.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    14065 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_advanced_environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3180 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_app_metadata.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1145 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_aws_config.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    17404 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_clients.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1694 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_cron_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2149 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_deletable_resource.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1895 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_environment_detector.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1529 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_environments.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1512 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_error_util.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6823 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_file_uploader.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2280 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_handlers.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3519 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_internal_metadata_adapter.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5843 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_logging.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    28697 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_model_converter.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2101 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_runtime_environment_parameters.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    34195 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_scheduler.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      427 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_utils.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2805 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/utils.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.681318 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler.egg-info/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1174 2023-07-13 17:45:27.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9270 2023-07-13 17:45:27.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2023-07-13 17:45:27.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        1 2023-07-13 17:45:27.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      208 2023-07-13 17:45:27.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler.egg-info/requires.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-07-13 17:45:27.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler.egg-info/top_level.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      261 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/babel.config.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       73 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/custom.d.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      827 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/jest.config.base.js
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      510 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/jest.config.js
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.693318 amazon_sagemaker_jupyter_scheduler-2.1.0/jupyter-config/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.693318 amazon_sagemaker_jupyter_scheduler-2.1.0/jupyter-config/jupyter_server_config.d/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      109 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/jupyter-config/jupyter_server_config.d/amazon_sagemaker_jupyter_scheduler.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      306 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/jupyter-config/jupyter_server_config.py
+-rw-r--r--   0 p4admin  (12569) amazon     (100)   965893 2023-07-13 17:45:15.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/package-lock.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4834 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/package.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      127 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/pyproject.toml
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      133 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/requirements.txt
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       38 2023-07-13 17:45:27.709317 amazon_sagemaker_jupyter_scheduler-2.1.0/setup.cfg
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3069 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/setup.py
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.693318 amazon_sagemaker_jupyter_scheduler-2.1.0/src/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.693318 amazon_sagemaker_jupyter_scheduler-2.1.0/src/__mocks__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/__mocks__/fileMock.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.697317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/__tests__/
+-rwxr-xr-x   0 p4admin  (12569) amazon     (100)    12302 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/__tests__/CreateNotebookJobForm.spec.tsx
+-rwxr-xr-x   0 p4admin  (12569) amazon     (100)     4348 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/__tests__/VpcCheckbox.spec.tsx
+-rwxr-xr-x   0 p4admin  (12569) amazon     (100)    13449 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/__tests__/initalValueHelpers.spec.ts
+-rwxr-xr-x   0 p4admin  (12569) amazon     (100)    11135 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/__tests__/validationHelpers.spec.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.669318 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.697317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      964 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/Link.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      754 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/RouterLink.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.697317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/__test__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1005 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/__test__/Link.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      609 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/__test__/RouterLink.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      246 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      184 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/types.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.697317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/selectinput/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1583 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/selectinput/SelectInput.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       56 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/selectinput/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      967 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/selectinput/types.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.697317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1626 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/TextInput.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.697317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1656 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/__tests__/TextInput.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       54 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2932 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      206 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/types.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.697317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/tooltip/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1348 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/tooltip/Tooltip.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.697317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/tooltip/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1040 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/tooltip/__tests__/Tooltip.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       27 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/tooltip/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      553 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/tooltip/styles.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.697317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/constants/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8440 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/constants/common.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       53 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/constants/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       99 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/constants/kernels.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      186 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/index.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.701317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/plugins/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3429 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/plugins/ScheduleNotebookDisablerPlugin.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1455 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/plugins/ScheduleNotebookPlugin.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       92 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/plugins/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3328 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/themeProvider.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.701317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/types/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      420 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/types/images.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       82 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/types/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      141 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/types/kernels.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      132 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/types/sagemaker.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.701317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1929 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/PluginEnvironmentProvider.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.701317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/__tests__/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1833 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/__tests__/PluginEnvironmentProvider.spec.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      123 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/common.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1528 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/images.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      108 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1205 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/kernels.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1017 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/rendering.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.701317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     4427 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJob.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.705317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.705317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    17765 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/AdvancedOptions.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.705317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3900 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariable.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3230 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariables.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       79 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1094 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/styles.ts
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.705317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3551 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/VpcCheckbox.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       55 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      285 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       35 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     5596 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/validationHelpers.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    14732 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/CreateNotebookJobform.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1229 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/InputContainer.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.705317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/JobEnvironment/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2737 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/JobEnvironment/DefaultJobEnvironment.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      712 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/JobEnvironment/JobEnvironmentContainer.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      118 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/JobEnvironment/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1280 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/JobEnvironment/jobEnvironment.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     3138 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/MultiSelectContainer.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1554 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/SelectInputContainer.tsx
+drwxr-xr-x   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:45:27.709317 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1613 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/StudioImageSelectorOption.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     6035 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/StudioJobEnvironment.tsx
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      552 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioApi.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    12172 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioHelpers.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)    64113 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioMock.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      781 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioModel.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1305 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioStyles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)       41 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     8199 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/initialValueHelpers.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     1727 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)        0 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/index.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2216 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/mockResponses.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     2815 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/styles.ts
+-rw-r--r--   0 p4admin  (12569) amazon     (100)     9250 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/tsconfig.base.json
+-rw-r--r--   0 p4admin  (12569) amazon     (100)      304 2023-07-13 17:43:10.000000 amazon_sagemaker_jupyter_scheduler-2.1.0/tsconfig.json
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/.eslintrc.js` & `amazon_sagemaker_jupyter_scheduler-2.1.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/.gitignore` & `amazon_sagemaker_jupyter_scheduler-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/Config` & `amazon_sagemaker_jupyter_scheduler-2.1.0/Config`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/DEVELOPMENT.md` & `amazon_sagemaker_jupyter_scheduler-2.1.0/DEVELOPMENT.md`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/MANIFEST.in` & `amazon_sagemaker_jupyter_scheduler-2.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/PKG-INFO` & `amazon_sagemaker_jupyter_scheduler-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon_sagemaker_jupyter_scheduler
-Version: 2.0.2
+Version: 2.1.0
 Summary: Amazon SageMaker Jupyter Scheduler based on the https://pypi.org/project/jupyter-scheduler/
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3,Scheduling Notebooks,Notebooks,Amazon Sagemaker
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/RELEASE.md` & `amazon_sagemaker_jupyter_scheduler-2.1.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/__init__.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_advanced_environments.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_advanced_environments.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_studio_advanced_environment.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/advanced_environments/sagemaker_studio_advanced_environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,103 +143,98 @@
         role_arns = []  # TODO: sync with UI to modify this to a single value
         accountId = await get_aws_account_id()
         s3_bucket_name = (
             f"{self.SAGEMAKER_DEFAULT_S3_PREFIX}-{accountId}-{get_region_name()}"
         )
         s3_uri = f"s3://{s3_bucket_name}/"
 
-        try:
-            DEFAULT_USER_SETTINGS_KEY = "DefaultUserSettings"
-            USER_SETTINGS_KEY = "UserSettings"
-            # we could in a shared space app
-            # TODO: Refactor shared space as a supported runtime environment
-            api_calls = [sm_client.describe_domain(get_domain_id())]
-
-            if get_user_profile_name():
-                api_calls.append(
-                    sm_client.describe_user_profile(
-                        get_domain_id(), get_user_profile_name()
-                    )
-                )
-            else:
-                api_calls.append(
-                    sm_client.describe_space(get_domain_id(), get_shared_space_name())
+        DEFAULT_USER_SETTINGS_KEY = "DefaultUserSettings"
+        USER_SETTINGS_KEY = "UserSettings"
+        # we could in a shared space app
+        # TODO: Refactor shared space as a supported runtime environment
+        api_calls = [sm_client.describe_domain(get_domain_id())]
+
+        if get_user_profile_name():
+            api_calls.append(
+                sm_client.describe_user_profile(
+                    get_domain_id(), get_user_profile_name()
                 )
-                DEFAULT_USER_SETTINGS_KEY = "DefaultSpaceSettings"
-                USER_SETTINGS_KEY = "SpaceSettings"
-
-            # user details is synonymous to space details
-            [domain_details, user_details] = await asyncio.gather(*api_calls)
-            logger.info(
-                f"domain level details: {domain_details}, user details: {user_details}"
             )
+        else:
+            api_calls.append(
+                sm_client.describe_space(get_domain_id(), get_shared_space_name())
+            )
+            DEFAULT_USER_SETTINGS_KEY = "DefaultSpaceSettings"
+            USER_SETTINGS_KEY = "SpaceSettings"
+
+        # user details is synonymous to space details
+        [domain_details, user_details] = await asyncio.gather(*api_calls)
+        logger.info(
+            f"domain level details: {domain_details}, user details: {user_details}"
+        )
 
-            # Domains created before VpcOnly mode was released will not have AppNetworkAccessType set.
-            domain_app_network_access_type = domain_details.get(
-                "AppNetworkAccessType", "PublicInternetOnly"
-            )
+        # Domains created before VpcOnly mode was released will not have AppNetworkAccessType set.
+        domain_app_network_access_type = domain_details.get(
+            "AppNetworkAccessType", "PublicInternetOnly"
+        )
 
-            all_compatible_subnets = await self._get_compatible_subnets(
+        all_compatible_subnets = await self._get_compatible_subnets(
+            vpc_id=domain_details["VpcId"]
+        )
+        logger.info(
+            f"all compatible logs from the vpc - {domain_details['VpcId']}: {all_compatible_subnets}"
+        )
+
+        # if the Studio domain subnet is in compatible list then make it true,
+        # any subnet that is in domain but not compatible, dont add it to the return value
+        for subnet_id in domain_details["SubnetIds"]:
+            for index, compatible_subnet in enumerate(all_compatible_subnets):
+                if compatible_subnet["name"] == subnet_id:
+                    all_compatible_subnets[index]["is_selected"] = True
+
+        # NOTE: In case of SpaceSettings they dont support security group as part of reInvent 2022,
+        # it will be empty, our logic can handle it
+        domain_attached_security_group_ids = self._merge_security_groups(
+            domain_details.get(DEFAULT_USER_SETTINGS_KEY, {}),
+            user_details.get(USER_SETTINGS_KEY, {}),
+        )
+        for sg_id in domain_attached_security_group_ids:
+            security_group_ids.append({"name": sg_id, "is_selected": True})
+        if not security_group_ids:
+            # If customer choose quick setup, by default Studio is only configured with subnets from default VPC.
+            # There is no security group attached by default.
+            # Even customer chooses the standard setup, it allows customer to leave the security groups blank.
+            # So if we detect that the security group is empty we will make a call to ec2 and get the default security group of the attached VPC
+            ec2_client = get_ec2_client()
+            security_groups = await ec2_client.list_security_groups_by_vpc_id(
                 vpc_id=domain_details["VpcId"]
             )
-            logger.info(
-                f"all compatible logs from the vpc - {domain_details['VpcId']}: {all_compatible_subnets}"
-            )
 
-            # if the Studio domain subnet is in compatible list then make it true,
-            # any subnet that is in domain but not compatible, dont add it to the return value
-            for subnet_id in domain_details["SubnetIds"]:
-                for index, compatible_subnet in enumerate(all_compatible_subnets):
-                    if compatible_subnet["name"] == subnet_id:
-                        all_compatible_subnets[index]["is_selected"] = True
-
-            # NOTE: In case of SpaceSettings they dont support security group as part of reInvent 2022,
-            # it will be empty, our logic can handle it
-            domain_attached_security_group_ids = self._merge_security_groups(
-                domain_details.get(DEFAULT_USER_SETTINGS_KEY, {}),
-                user_details.get(USER_SETTINGS_KEY, {}),
-            )
-            for sg_id in domain_attached_security_group_ids:
-                security_group_ids.append({"name": sg_id, "is_selected": True})
-            if not security_group_ids:
-                # If customer choose quick setup, by default Studio is only configured with subnets from default VPC.
-                # There is no security group attached by default.
-                # Even customer chooses the standard setup, it allows customer to leave the security groups blank.
-                # So if we detect that the security group is empty we will make a call to ec2 and get the default security group of the attached VPC
-                ec2_client = get_ec2_client()
-                security_groups = await ec2_client.list_security_groups_by_vpc_id(
-                    vpc_id=domain_details["VpcId"]
+            for sg in security_groups["SecurityGroups"]:
+                security_group_ids.append(
+                    {
+                        "name": sg["GroupId"],
+                        "is_selected": sg["GroupName"] == "default",
+                    }
                 )
+        logger.info(
+            f"security group details: {domain_attached_security_group_ids}, Domain VPC ID: {domain_details['VpcId']}, {security_group_ids}"
+        )
 
-                for sg in security_groups["SecurityGroups"]:
-                    security_group_ids.append(
-                        {
-                            "name": sg["GroupId"],
-                            "is_selected": sg["GroupName"] == "default",
-                        }
-                    )
-            logger.info(
-                f"security group details: {domain_attached_security_group_ids}, Domain VPC ID: {domain_details['VpcId']}, {security_group_ids}"
-            )
-
-            lcc_arns = self._get_lcc_arns(
-                domain_details.get(DEFAULT_USER_SETTINGS_KEY, {}),
-                user_details.get(USER_SETTINGS_KEY, {}),
-            )
-
-            # NOTE: In case of SpaceSettings they dont support execution role as part of reInvent 2022,
-            # it will be empty, our logic can handle it
-            role_arns = self._get_role_arns(
-                domain_details.get(DEFAULT_USER_SETTINGS_KEY, {}),
-                user_details.get(USER_SETTINGS_KEY, {}),
-            )
+        lcc_arns = self._get_lcc_arns(
+            domain_details.get(DEFAULT_USER_SETTINGS_KEY, {}),
+            user_details.get(USER_SETTINGS_KEY, {}),
+        )
 
-        except Exception as error:
-            logger.error(f"error when calling advanced environments - {error}")
-            # fail silently, we want to atleast give back empty values for the customer to fill it up
+        # NOTE: In case of SpaceSettings they dont support execution role as part of reInvent 2022,
+        # it will be empty, our logic can handle it
+        role_arns = self._get_role_arns(
+            domain_details.get(DEFAULT_USER_SETTINGS_KEY, {}),
+            user_details.get(USER_SETTINGS_KEY, {}),
+        )
 
         try:
             response = await get_s3_client().create_bucket(
                 s3_bucket_name, get_region_name()
             )
             logger.info(f"S3 bucket created succesfully {s3_uri} - {response}")
             # If the bucket already exists, the versioning & encryption calls is not needed
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/app_metadata.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/app_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/service-2.json` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/botocore_model/sagemaker/2017-07-24/service-2.json`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/clients.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/clients.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/cron_util.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/cron_util.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/deletable_resource.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/deletable_resource.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/environment_detector.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/environment_detector.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/environments.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/environments.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/error_util.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/error_util.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/extension.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/extension.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/file_uploader.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/file_uploader.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/handlers.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/handlers.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/host_region_mapping.json` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/host_region_mapping.json`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/internal_metadata_adapter.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/internal_metadata_adapter.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/package.json` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.961111111111111%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}", "'version'": "'2.1.0'"}*

```diff
@@ -59,18 +59,14 @@
     "files": [
         "dist/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://aws.amazon.com/sagemaker/",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.9f672e548acd2153a221.js"
-        },
         "disabledExtensions": [
             "@jupyterlab/scheduler:IAdvancedOptions"
         ],
         "extension": true,
         "outputDir": "amazon_sagemaker_jupyter_scheduler/labextension",
         "schemaDir": "schema",
         "sharedPackages": {
@@ -110,9 +106,9 @@
         "test": "jest",
         "test:debug": "node --inspect node_modules/.bin/jest --watch --runInBand",
         "test:server-extension": ":",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
-    "version": "2.0.2"
+    "version": "2.1.0"
 }
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/advanced-options.json` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/advanced-options.json`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/schemas/@amzn/sagemaker-jupyter-scheduler/package.json.orig` & `amazon_sagemaker_jupyter_scheduler-2.1.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'2.1.0'"}*

```diff
@@ -106,9 +106,9 @@
         "test": "jest",
         "test:debug": "node --inspect node_modules/.bin/jest --watch --runInBand",
         "test:server-extension": ":",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
-    "version": "2.0.2"
+    "version": "2.1.0"
 }
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/144.9be27e93647ef0e84863.js` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/144.9be27e93647ef0e84863.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/193.04adf0a714b67e82f263.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/240.762850093662386d80d3.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/509.b1db44e3c8c1ddb64444.js` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/509.b1db44e3c8c1ddb64444.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/615.d5639a877b54ff655d41.js` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/615.d5639a877b54ff655d41.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js.LICENSE.txt` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/993.faa5510ce9696a850c76.js` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/993.84c00bb76b4448d8ce3f.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 "use strict";
 (self.webpackChunk_amzn_sagemaker_jupyter_scheduler = self.webpackChunk_amzn_sagemaker_jupyter_scheduler || []).push([
     [993], {
         7993: (e, t, r) => {
             r.r(t), r.d(t, {
-                default: () => Vt
+                default: () => Rt
             });
             var n = r(6271),
                 o = r.n(n),
                 a = r(7363),
                 l = r(5015);
             const i = "nbScheduler",
                 s = {
@@ -22,14 +22,16 @@
                                 RoleArn: "Role ARN",
                                 Image: "Image",
                                 Kernel: "Kernel",
                                 securityGroup: "Security Group(s)",
                                 subnet: "Subnet(s)",
                                 s3InputFolder: "Input Folder",
                                 s3OutputFolder: "Output Folder",
+                                maxRetryAttempts: "Max retry attempts",
+                                maxRunTimeInSeconds: "Max run time (in seconds)",
                                 selectAdditionalDepency: "Select additional dependencies",
                                 efsPlaceholder: "Enter EFS file path",
                                 efsLabel: "Initialization script location (optional)",
                                 startUpScript: "Start-up script",
                                 executionEnv: "Execution enviroment",
                                 useVPC: "Use a Virtual Private Cloud (VPC) to run this job",
                                 enableEncryption: "Configure job encryption",
@@ -69,15 +71,17 @@
                                     SubnetMinError: "At least one Subnet must be selected when Security Group is selected.",
                                     SubnetsMaxError: "Can only have maximum of 16 subnets.",
                                     SubnetLengthError: "Subnet must be less than 32 characters.",
                                     SubnetsFormatError: "One or more subnets has invalid format.",
                                     EnvironmentVariableEmptyError: "Key or Value cannot be empty.",
                                     EnvironmentVariableLengthError: "Key or Value cannot be more than 512 characters.",
                                     EnvironmentVariableFormatError: "Key or Value has invalid format.",
-                                    KMSKeyError: "KMS key has invalid format."
+                                    KMSKeyError: "KMS key has invalid format.",
+                                    MaxRetryAttemptsError: "Invalid max retry attempts must have a minimum value of 1 and a maximum value of 30.",
+                                    MaxRunTimeInSecondsError: "Invalid max run time must have a minimum value of 1."
                                 },
                                 VPCErrors: {
                                     RequiresPrivateSubnet: "Running notebook jobs in a VPC requires the virtual network to use a private subnet.",
                                     NoPrivateSubnetsInSageMakerDomain: "There are no private subnets associated with your SageMaker Studio domain",
                                     YouMayChooseOtherSubnets: "You may choose to run the job using other private subnets associated with this VPC"
                                 }
                             },
@@ -92,15 +96,17 @@
                                 SubnetTooltip: "Specify or add Private subnet(s) of the desired VPC.",
                                 InputFolderTooltip: "Enter the S3 location to store the input artifacts like notebook and script.",
                                 OutputFolderTooltip: "Enter the S3 location to store the output artifacts.",
                                 InitialScriptTooltip: "Enter the file path of a local script to run before the notebook execution.",
                                 EnvironmentVariablesTooltip: "Enter key-value pairs that will be accessible in your notebook.",
                                 kmsKeyTooltip: "If you want Amazon SageMaker to encrypt the output of your notebook job using your own AWS KMS encryption key instead of the default S3 service key, provide its ID or ARN",
                                 ebsKeyTooltip: "Encrypt data on the storage volume attached to the compute instance that runs the scheduled job.",
-                                LearnMore: "Learn more"
+                                LearnMore: "Learn more",
+                                MaxRetryAttempts: "Enter a minimum value of 1 and a maximum value of 30.",
+                                MaxRunTimeInSeconds: "Enter a minimum value of 1."
                             },
                             StudioTooltips: {
                                 ImageTooltipText: "Select available SageMaker image.",
                                 KernelTooltipText: "Select available SageMaker Kernel.",
                                 RoleArnTooltip: "Specify a role with permission to create a notebook job.",
                                 SecurityGroupsTooltip: "Specify or add security group(s) that have been created for the default VPC. For better security, we recommend that you use a private VPC.",
                                 SubnetTooltip: "Specify or add subnet(s) that have been created for the default VPC. For better security, we recommend that you use a private VPC.",
@@ -134,27 +140,27 @@
                             buttons: {
                                 goToIamConsole: "Go to IAM console",
                                 enterKeysInTerminal: "Run `aws configure` in Terminal"
                             }
                         }
                     }
                 },
-                c = {
+                u = {
                     expiredToken: "ExpiredToken",
                     invalidClientTokenId: "InvalidClientTokenId",
                     noCredentials: "NoCredentials"
                 },
-                u = "terminal:create-new";
-            var d, m = r(5185),
+                c = "terminal:create-new";
+            var m, d = r(5185),
                 p = r(5306),
                 v = r(1396),
                 g = r(6247);
             ! function(e) {
                 e.PublicInternetOnly = "PublicInternetOnly", e.VpcOnly = "VpcOnly"
-            }(d || (d = {}));
+            }(m || (m = {}));
             var b, h, f = r(9208),
                 E = r(1982),
                 y = r(9692);
             ! function(e) {
                 e[e.Large = 0] = "Large", e[e.Medium = 1] = "Medium", e[e.Small = 2] = "Small"
             }(b || (b = {})),
             function(e) {
@@ -242,54 +248,54 @@
                     className: t,
                     InputProps: r,
                     FormHelperTextProps: n,
                     size: a = b.Medium,
                     variant: l,
                     ...i
                 }) => {
-                    var s, c, u;
-                    const d = (0, E.cx)(E.css`
+                    var s, u, c;
+                    const m = (0, E.cx)(E.css`
   .MuiFormHelperText-root.Mui-error::before {
     display: inline-block;
     vertical-align: middle;
     background-size: 1rem 1rem;
     height: var(--text-input-error-icon-height);
     width: var(--text-input-error-icon-width);
     background-image: var(--text-input-helper-text-alert-icon);
     background-repeat: no-repeat;
     content: ' ';
   }
 `, t, null == e ? void 0 : e.root);
                     return o().createElement(p.TextField, {
                         classes: {
-                            root: d,
+                            root: m,
                             ...e
                         },
                         variant: l,
                         InputProps: {
                             ...r,
                             classes: {
                                 root: (0, E.cx)(k({
                                     size: a
                                 }).root, null === (s = null == r ? void 0 : r.classes) || void 0 === s ? void 0 : s.root),
                                 input: (0, E.cx)(k({
                                     size: a
-                                }).input, null === (c = null == r ? void 0 : r.classes) || void 0 === c ? void 0 : c.input)
+                                }).input, null === (u = null == r ? void 0 : r.classes) || void 0 === u ? void 0 : u.input)
                             }
                         },
                         FormHelperTextProps: {
                             ...n,
                             classes: {
-                                root: (0, E.cx)(x().root, null === (u = null == n ? void 0 : n.classes) || void 0 === u ? void 0 : u.root)
+                                root: (0, E.cx)(x().root, null === (c = null == n ? void 0 : n.classes) || void 0 === c ? void 0 : c.root)
                             }
                         },
                         ...i
                     })
                 },
-                P = (0, y.Z)((() => ({
+                M = (0, y.Z)((() => ({
                     popper: {
                         "& .MuiTooltip-tooltip": {
                             backgroundColor: "var(--color-light)",
                             boxShadow: "var(--tooltip-shadow)",
                             color: "var(--tooltip-text-color",
                             padding: "var(--padding-16)",
                             fontSize: "var(--font-size-0)"
@@ -300,110 +306,110 @@
                             color: "var(--tooltip-surface)",
                             "&:before": {
                                 boxShadow: "var(--tooltip-shadow)"
                             }
                         }
                     }
                 })));
-            var M, T = r(30);
+            var P, T = r(30);
             ! function(e) {
                 e.TopStart = "top-start", e.Top = "top", e.TopEnd = "top-end", e.RightStart = "right-start", e.Right = "right", e.RightEnd = "right-end", e.BottomStart = "bottom-start", e.Bottom = "bottom", e.BottomEnd = "bottom-end", e.LeftStart = "left-start", e.Left = "left", e.LeftEnd = "left-end"
-            }(M || (M = {}));
+            }(P || (P = {}));
             const j = ({
                     children: e,
                     classes: t,
                     className: r,
-                    placement: n = M.Right,
+                    placement: n = P.Right,
                     ...a
                 }) => {
-                    const l = (0, E.cx)(r, P().popper, null == t ? void 0 : t.popper);
+                    const l = (0, E.cx)(r, M().popper, null == t ? void 0 : t.popper);
                     return o().createElement(T.ZP, {
                         ...a,
                         arrow: !0,
                         classes: {
                             popper: l,
-                            tooltip: P().tooltip
+                            tooltip: M().tooltip
                         },
                         placement: n
                     }, e)
                 },
                 C = E.css`
   display: flex;
   flex-direction: column;
 `,
-                N = E.css`
+                I = E.css`
   display: flex;
   flex-direction: column;
 `,
-                I = E.css`
+                N = E.css`
   display: inline-flex;
   svg {
     width: 0.75em;
     height: 0.75em;
     transform: translateY(-2px);
   }
 `,
                 O = E.css`
   svg {
     width: 0.75em;
     height: 0.75em;
     transform: translateY(1px);
   }
 `,
-                F = (e = !1) => E.css`
+                V = (e = !1) => E.css`
   display: flex;
   flex-direction: column;
   ${e?"":"max-width : 500px;"}
   .MuiCheckbox-colorPrimary.Mui-checked {
     color: var(--jp-brand-color1);
   }
   .MuiButton-containedPrimary:hover {
     background-color: var(--jp-brand-color1);
   }
 `,
-                V = E.css`
+                A = E.css`
   font-size: var(--jp-content-font-size1);
 `,
-                A = E.css`
+                F = E.css`
   display: flex;
   justify-content: flex-start;
   align-items: center;
   gap: 0.5rem;
   svg {
     width: var(--jp-ui-font-size1);
     height: var(--jp-ui-font-size1);
     path {
       fill: var(--jp-error-color1);
     }
   }
 `,
-                z = (e = !1) => E.css`
+                R = (e = !1) => E.css`
   color: var(--jp-color-root-light-800);
   font-weight: 400;
   font-size: var(--jp-ui-font-size1);
   line-height: var(--jp-ui-font-size1);
   margin-bottom: var(--jp-ui-font-size1);
   ${e&&"\n    &:after {\n      content: '*';\n      color: var(--jp-error-color1);\n    }\n  "}
 `;
-            var R, K, L = r(6689);
+            var z, K, D = r(6689);
             ! function(e) {
                 e.External = "_blank", e.Content = "_self"
-            }(R || (R = {})),
+            }(z || (z = {})),
             function(e) {
                 e.None = "none", e.Hover = "hover", e.Always = "always"
             }(K || (K = {}));
-            const D = ({
+            const L = ({
                 className: e,
                 disabled: t = !1,
                 children: r,
                 onClick: n,
-                target: a = R.Content,
+                target: a = z.Content,
                 ...l
             }) => {
-                const i = a === R.External,
+                const i = a === z.External,
                     s = {
                         ...l,
                         className: (0, E.cx)(E.css`
   cursor: pointer;
   text-decoration: none;
   color: var(--jp-brand-color1);
 
@@ -412,15 +418,15 @@
     color: var(--jp-brand-color1);
   }
 `, e),
                         target: a,
                         onClick: t ? void 0 : n,
                         rel: i ? "noopener noreferrer" : void 0
                     };
-                return o().createElement(L.Z, {
+                return o().createElement(D.Z, {
                     ...s
                 }, r)
             };
             r(78);
             const J = e => "string" == typeof e && e.length > 0;
             var B = r(5505),
                 G = r.n(B);
@@ -446,39 +452,39 @@
                     return {
                         kernel: null,
                         arnEnvironment: null,
                         version: null
                     }
                 }
             }
-            const Z = ({
+            const q = ({
                 labelInfo: e,
                 required: t,
                 toolTipText: r,
                 errorMessage: n,
                 ...a
             }) => o().createElement("div", {
-                className: N
-            }, o().createElement("div", {
                 className: I
+            }, o().createElement("div", {
+                className: N
             }, o().createElement("label", {
-                className: z(t)
+                className: R(t)
             }, " ", e, " "), r && !a.readOnly && o().createElement(j, {
                 title: r,
                 className: O
             }, o().createElement(f.Z, null))), o().createElement(w, {
                 ...a,
                 error: J(n),
                 helperText: n,
                 InputProps: {
                     readOnly: a.readOnly,
                     ...a.InputProps
                 }
             }));
-            var q = r(6433);
+            var Z = r(6433);
             E.css`
   box-sizing: border-box;
   width: 100%;
   padding: var(--jp-padding-large);
   flex-direction: column;
   display: flex;
   color: var(--jp-ui-font-color0);
@@ -575,127 +581,131 @@
   color: var(--jp-ui-font-color0);
 `,
                 te = E.css`
   display: flex;
   flex-direction: column;
   gap: var(--jp-ui-font-size1);
 `,
-                re = s.ScheduleNoteBook.MainPanel.ErrorMessages.VPCErrors,
-                ne = s.ScheduleNoteBook.MainPanel.AdvancedOptions,
-                oe = s.ScheduleNoteBook.MainPanel.Tooltips,
-                ae = o().createElement("div", null, o().createElement("span", {
+                re = E.css`
+  color: var(--jp-error-color1);
+  padding: 12px;
+`,
+                ne = s.ScheduleNoteBook.MainPanel.ErrorMessages.VPCErrors,
+                oe = s.ScheduleNoteBook.MainPanel.AdvancedOptions,
+                ae = s.ScheduleNoteBook.MainPanel.Tooltips,
+                le = o().createElement("div", null, o().createElement("span", {
                     className: W
-                }, " ", oe.VPCTooltip, " "), o().createElement(D, {
+                }, " ", ae.VPCTooltip, " "), o().createElement(L, {
                     href: "https://docs.aws.amazon.com/sagemaker/latest/dg/create-notebook-auto-execution-advanced.html",
-                    target: R.External
+                    target: z.External
                 }, o().createElement("p", {
                     className: Q
                 }, s.ScheduleNoteBook.MainPanel.Tooltips.LearnMore))),
-                le = ({
+                ie = ({
                     isChecked: e,
                     formState: t,
                     formErrors: r,
                     initialSecurityGroups: n,
                     initialSubnets: a,
                     availableSubnets: l,
                     setFormErrors: i,
                     setChecked: s,
-                    setFormState: c,
-                    ...u
+                    setFormState: u,
+                    ...c
                 }) => o().createElement("div", {
                     className: Y
-                }, o().createElement(q.Z, {
+                }, o().createElement(Z.Z, {
                     name: "vpc-check-box",
                     className: X,
                     color: "primary",
                     checked: e,
                     onChange: e => {
                         const o = e.target.checked;
                         if (s(o), o) {
-                            if (c({
+                            if (u({
                                     ...t,
                                     vpc_security_group_ids: n,
                                     vpc_subnets: a
                                 }), 0 === a.length && l.length > 0) return void i({
                                 ...r,
-                                subnetError: `${re.RequiresPrivateSubnet} ${re.NoPrivateSubnetsInSageMakerDomain}. ${re.YouMayChooseOtherSubnets}`
+                                subnetError: `${ne.RequiresPrivateSubnet} ${ne.NoPrivateSubnetsInSageMakerDomain}. ${ne.YouMayChooseOtherSubnets}`
                             });
                             0 === l.length && i({
                                 ...r,
-                                subnetError: `${re.RequiresPrivateSubnet} ${re.NoPrivateSubnetsInSageMakerDomain}`
+                                subnetError: `${ne.RequiresPrivateSubnet} ${ne.NoPrivateSubnetsInSageMakerDomain}`
                             })
-                        } else c({
+                        } else u({
                             ...t,
                             vpc_security_group_ids: [],
                             vpc_subnets: []
                         }), i({
                             ...r,
                             subnetError: "",
                             securityGroupError: ""
                         })
                     },
-                    ...u
-                }), o().createElement("label", null, ne.useVPC), o().createElement(j, {
+                    ...c
+                }), o().createElement("label", null, oe.useVPC), o().createElement(j, {
                     classes: {
                         popperInteractive: ee
                     },
-                    title: ae,
+                    title: le,
                     interactive: !0
                 }, o().createElement(f.Z, {
                     fontSize: "small"
                 })));
-            var ie = r(9419),
-                se = r(2679),
+            var se = r(9419),
+                ue = r(2679),
                 ce = r(4085);
-            const ue = E.css`
+            const me = E.css`
   display: flex;
   align-items: flex-end;
   padding-right: 1em;
   gap: 20px;
 `,
                 de = E.css`
   display: flex;
   flex-direction: column;
 `,
-                me = E.css`
+                pe = E.css`
   width: 170px;
 `,
-                pe = (E.css`
+                ve = (E.css`
   display: flex;
   flex-direction: column;
   margin-bottom: var(--jp-padding-large);
 `, E.css`
   display: flex;
   flex-direction: column;
   gap: 16px;
 `),
-                ve = E.css`
+                ge = E.css`
   font-weight: 400;
   font-size: var(--jp-ui-font-size1);
   line-height: var(--jp-ui-font-size1);
 `,
-                ge = E.css`
+                be = E.css`
   background-color: var(--jp-brand-color1);
   font-size: var(--jp-ui-font-size1);
   text-transform: none;
 `,
-                be = E.css`
+                he = E.css`
   display: inline-flex;
   align-items: center;
   gap: 6px;
   svg {
     width: 0.75em;
     height: 0.75em;
   }
 `,
-                he = new RegExp("[a-zA-Z_][a-zA-Z0-9_]*"),
-                fe = new RegExp("[\\S\\s]*"),
-                Ee = s.ScheduleNoteBook.MainPanel.ErrorMessages.AdvancedOptions,
-                ye = s.ScheduleNoteBook.MainPanel.AdvancedOptions,
-                Se = ({
+                fe = new RegExp("[a-zA-Z_][a-zA-Z0-9_]*"),
+                Ee = new RegExp("[\\S\\s]*"),
+                ye = s.ScheduleNoteBook.MainPanel.ErrorMessages.AdvancedOptions,
+                Se = s.ScheduleNoteBook.MainPanel.AdvancedOptions,
+                _e = ({
                     isDisabled: e,
                     environmentParameters: t,
                     setEnvironmentParameters: r,
                     index: n,
                     formErrors: a,
                     setFormErrors: l
                 }) => {
@@ -710,765 +720,816 @@
                                 } : {
                                     key: t[l].key,
                                     value: o
                                 },
                                 s = [...t];
                             s.splice(l, 1, i), r(s)
                         },
-                        c = () => {
+                        u = () => {
                             const {
                                 key: e,
                                 value: t
                             } = i;
                             e.length < 1 || t.length < 1 ? l({
                                 ...a,
-                                environmentVariablesError: Ee.EnvironmentVariableEmptyError
+                                environmentVariablesError: ye.EnvironmentVariableEmptyError
                             }) : e.length > 512 || t.length > 512 ? l({
                                 ...a,
-                                environmentVariablesError: Ee.EnvironmentVariableLengthError
-                            }) : he.test(e) && fe.test(t) ? l({
+                                environmentVariablesError: ye.EnvironmentVariableLengthError
+                            }) : fe.test(e) && Ee.test(t) ? l({
                                 ...a,
                                 environmentVariablesError: ""
                             }) : l({
                                 ...a,
-                                environmentVariablesError: Ee.EnvironmentVariableFormatError
+                                environmentVariablesError: ye.EnvironmentVariableFormatError
                             })
                         };
                     return o().createElement("div", {
-                        className: ue
-                    }, o().createElement(Z, {
-                        className: me,
+                        className: me
+                    }, o().createElement(q, {
+                        className: pe,
                         readOnly: e,
                         name: `envKey-${n}`,
-                        labelInfo: ye.Key,
+                        labelInfo: Se.Key,
                         value: t[n].key,
                         onChange: s,
-                        onBlur: c
-                    }), o().createElement(Z, {
-                        className: me,
+                        onBlur: u
+                    }), o().createElement(q, {
+                        className: pe,
                         readOnly: e,
                         name: `envValue-${n}`,
-                        labelInfo: ye.Value,
+                        labelInfo: Se.Value,
                         value: t[n].value,
                         onChange: s,
-                        onBlur: c
+                        onBlur: u
                     }), o().createElement("div", null, !e && o().createElement(ce.Z, {
                         onClick: () => {
                             (e => {
                                 const n = [...t];
                                 n.splice(e, 1), r(n), l({
                                     ...a,
                                     environmentVariablesError: ""
                                 })
                             })(n), l({
                                 ...a,
                                 environmentVariablesError: ""
                             })
                         }
-                    }, o().createElement(se.Z, null))))
+                    }, o().createElement(ue.Z, null))))
                 },
-                _e = s.ScheduleNoteBook.MainPanel.AdvancedOptions,
-                ke = s.ScheduleNoteBook.MainPanel.Tooltips,
-                xe = ({
+                ke = s.ScheduleNoteBook.MainPanel.AdvancedOptions,
+                xe = s.ScheduleNoteBook.MainPanel.Tooltips,
+                we = ({
                     allFieldsDisabled: e,
                     isButtonDisabled: t,
                     environmentVariables: r,
                     setEnvironmentVariables: n,
                     formErrors: a,
                     ...l
                 }) => {
                     const i = !!a.environmentVariablesError,
                         s = o().createElement("div", {
-                            className: A
-                        }, o().createElement(ie.Z, {
+                            className: F
+                        }, o().createElement(se.Z, {
                             severity: "error"
                         }, a.environmentVariablesError));
                     return o().createElement("div", {
-                        className: pe
+                        className: ve
                     }, o().createElement("div", {
-                        className: be
+                        className: he
                     }, o().createElement("label", {
-                        className: ve
-                    }, _e.environmentVariables), e ? null : o().createElement(j, {
-                        title: ke.EnvironmentVariablesTooltip
+                        className: ge
+                    }, ke.environmentVariables), e ? null : o().createElement(j, {
+                        title: xe.EnvironmentVariablesTooltip
                     }, o().createElement(f.Z, null))), e && 0 === r.length ? o().createElement("div", {
                         className: de
                     }, o().createElement(w, {
                         InputProps: {
                             readOnly: !0
                         },
-                        placeholder: _e.Placeholders.NoneSelected
-                    })) : o().createElement(o().Fragment, null, r.map(((t, i) => o().createElement(Se, {
+                        placeholder: ke.Placeholders.NoneSelected
+                    })) : o().createElement(o().Fragment, null, r.map(((t, i) => o().createElement(_e, {
                         isDisabled: e,
                         key: i,
                         environmentParameters: r,
                         setEnvironmentParameters: n,
                         index: i,
                         formErrors: a,
                         ...l
                     })))), i && o().createElement("div", null, s), !e && o().createElement("div", null, o().createElement(p.Button, {
                         disabled: t,
-                        className: ge,
+                        className: be,
                         variant: "contained",
                         color: "primary",
                         size: "small",
                         onClick: () => {
                             n([...r, {
                                 key: "",
                                 value: ""
                             }])
                         }
-                    }, _e.addEnvironmentvariable)))
+                    }, ke.addEnvironmentvariable)))
                 };
-            var we = r(1518),
+            var Me = r(1518),
                 Pe = r(5861),
-                Me = r(3640);
-            const Te = (0, we.D)(),
-                je = ({
+                Te = r(3640);
+            const je = (0, Me.D)(),
+                Ce = ({
                     label: e,
                     required: t,
                     errorMessage: r,
                     disabled: n,
                     renderInput: a,
                     tooltip: l,
                     disabledTooltip: i,
                     freeSolo: s,
-                    options: c,
-                    ...u
+                    options: u,
+                    ...c
                 }) => {
-                    var d, m;
-                    null != a || (a = t => o().createElement(Me.Z, {
+                    var m, d;
+                    null != a || (a = t => o().createElement(Te.Z, {
                         ...t,
                         variant: "outlined",
                         size: "small",
                         margin: "dense",
                         placeholder: e
                     }));
                     const p = n ? i ? o().createElement(j, {
                             title: i,
                             className: O
                         }, o().createElement(f.Z, null)) : o().createElement(o().Fragment, null) : l ? o().createElement(j, {
                             title: l,
                             className: O
                         }, o().createElement(f.Z, null)) : o().createElement(o().Fragment, null),
                         v = r ? o().createElement("div", {
-                            className: A
-                        }, o().createElement(ie.Z, {
+                            className: F
+                        }, o().createElement(se.Z, {
                             severity: "error"
                         }, r)) : o().createElement(o().Fragment, null);
                     return o().createElement("div", {
                         className: C
                     }, o().createElement("div", {
-                        className: I
+                        className: N
                     }, o().createElement("label", {
-                        className: z(t)
+                        className: R(t)
                     }, e), p), o().createElement(Pe.Z, {
-                        ...u,
+                        ...c,
                         multiple: !0,
                         renderInput: a,
                         freeSolo: s,
                         readOnly: n,
-                        options: c,
+                        options: u,
                         filterOptions: (e, t) => {
-                            const r = Te(e, t);
+                            const r = je(e, t);
                             return "" === t.inputValue || e.includes(t.inputValue) || r.push(t.inputValue), r
                         },
-                        renderOption: (e, t, r) => (c.includes(t) || (t = `Add "${t}"`), o().createElement("li", {
+                        renderOption: (e, t, r) => (u.includes(t) || (t = `Add "${t}"`), o().createElement("li", {
                             ...e
                         }, t)),
                         componentsProps: {
-                            ...u.componentsProps,
+                            ...c.componentsProps,
                             popupIndicator: {
-                                ...null === (d = u.componentsProps) || void 0 === d ? void 0 : d.popupIndicator,
+                                ...null === (m = c.componentsProps) || void 0 === m ? void 0 : m.popupIndicator,
                                 size: "small"
                             },
                             clearIndicator: {
-                                ...null === (m = u.componentsProps) || void 0 === m ? void 0 : m.clearIndicator,
+                                ...null === (d = c.componentsProps) || void 0 === d ? void 0 : d.clearIndicator,
                                 size: "small"
                             }
                         }
                     }), v)
                 },
-                Ce = new RegExp("^(https|s3)://([^/]+)/?(.*)$"),
+                Ie = new RegExp("^(https|s3)://([^/]+)/?(.*)$"),
                 Ne = new RegExp("[-0-9a-zA-Z]+"),
-                Ie = new RegExp("^arn:aws[a-z\\-]*:iam::\\d{12}:role/?[a-zA-Z_0-9+=,.@\\-_/]+$"),
-                Oe = new RegExp("^arn:aws:kms:\\w+(?:-\\w+)+:\\d{12}:key\\/[A-Za-z0-9]+(?:-[A-Za-z0-9]+)+$"),
-                Fe = new RegExp("^[0-9a-z]{8}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{12}$"),
-                Ve = s.ScheduleNoteBook.MainPanel.ErrorMessages,
-                Ae = Ve.VPCErrors,
-                ze = e => e.length < 20 || e.length > 2048 ? Ve.AdvancedOptions.RoleArnLengthError : Ie.test(e) ? "" : Ve.AdvancedOptions.RoleArnFormatError,
-                Re = e => 0 === e.trim().length ? Ve.AdvancedOptions.S3LengthError : Ce.test(e) ? "" : Ve.AdvancedOptions.S3FormatError,
-                Ke = e => 0 === e.length || Oe.test(e) || Fe.test(e) ? "" : Ve.AdvancedOptions.KMSKeyError;
+                Oe = new RegExp("^arn:aws[a-z\\-]*:iam::\\d{12}:role/?[a-zA-Z_0-9+=,.@\\-_/]+$"),
+                Ve = new RegExp("^arn:aws:kms:\\w+(?:-\\w+)+:\\d{12}:key\\/[A-Za-z0-9]+(?:-[A-Za-z0-9]+)+$"),
+                Ae = new RegExp("^[0-9a-z]{8}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{12}$"),
+                Fe = s.ScheduleNoteBook.MainPanel.ErrorMessages,
+                Re = Fe.VPCErrors,
+                ze = e => e.length < 20 || e.length > 2048 ? Fe.AdvancedOptions.RoleArnLengthError : Oe.test(e) ? "" : Fe.AdvancedOptions.RoleArnFormatError,
+                Ke = e => 0 === e.trim().length ? Fe.AdvancedOptions.S3LengthError : Ie.test(e) ? "" : Fe.AdvancedOptions.S3FormatError,
+                De = e => 0 === e.length || Ve.test(e) || Ae.test(e) ? "" : Fe.AdvancedOptions.KMSKeyError;
             var Le;
             ! function(e) {
                 e.LocalJL = "local-jupyter-lab", e.Studio = "studio"
             }(Le || (Le = {}));
-            class De {
+            class Je {
                 get isStudio() {
                     return this.type === Le.Studio
                 }
                 get isLocalJL() {
                     return this.type === Le.LocalJL
                 }
                 constructor(e) {
                     this.type = e
                 }
             }
-            const Je = (0, n.createContext)(void 0);
+            const Be = (0, n.createContext)(void 0);
 
-            function Be({
+            function Ge({
                 app: e,
                 children: t
             }) {
                 const [r, a] = (0, n.useState)((() => function(e) {
-                    return e.hasPlugin("@amzn/sagemaker-ui:project") ? new De(Le.Studio) : new De(Le.LocalJL)
+                    return e.hasPlugin("@amzn/sagemaker-ui:project") ? new Je(Le.Studio) : new Je(Le.LocalJL)
                 }(e))), l = {
                     pluginEnvironment: r,
                     setPluginEnvironment: a
                 };
-                return o().createElement(Je.Provider, {
+                return o().createElement(Be.Provider, {
                     value: l
                 }, t)
             }
 
-            function Ge() {
-                const e = (0, n.useContext)(Je);
+            function $e() {
+                const e = (0, n.useContext)(Be);
                 if (void 0 === e) throw new Error("usePluginEnvironment must be used within a PluginEnvironmentProvider");
                 return e
             }
-            var $e = r(8202),
+            var qe = r(8202),
                 Ze = r(3274),
-                qe = r(8102);
-            const He = s.ScheduleNoteBook.MainPanel.AdvancedOptions,
-                Ue = s.ScheduleNoteBook.MainPanel.Tooltips,
-                Ye = s.ScheduleNoteBook.MainPanel.StudioTooltips,
-                We = s.ScheduleNoteBook.MainPanel.ErrorMessages,
-                Qe = o().createElement("div", null, o().createElement("span", {
+                He = r(8102);
+            const Ue = s.ScheduleNoteBook.MainPanel.AdvancedOptions,
+                Ye = s.ScheduleNoteBook.MainPanel.Tooltips,
+                We = s.ScheduleNoteBook.MainPanel.StudioTooltips,
+                Qe = s.ScheduleNoteBook.MainPanel.ErrorMessages,
+                Xe = o().createElement("div", null, o().createElement("span", {
                     className: W
-                }, Ue.kmsKeyTooltip), o().createElement(D, {
+                }, Ye.kmsKeyTooltip), o().createElement(L, {
                     href: "https://docs.aws.amazon.com/sagemaker/latest/dg/create-notebook-auto-execution-advanced.html",
-                    target: R.External
+                    target: z.External
                 }, o().createElement("p", {
                     className: Q
-                }, Ue.LearnMore))),
-                Xe = o().createElement("div", null, o().createElement("span", {
+                }, Ye.LearnMore))),
+                et = o().createElement("div", null, o().createElement("span", {
                     className: W
-                }, Ue.LCCScriptTooltipText), o().createElement(D, {
+                }, Ye.LCCScriptTooltipText), o().createElement(L, {
                     href: "https://aws.amazon.com/blogs/machine-learning/customize-amazon-sagemaker-studio-using-lifecycle-configurations/",
-                    target: R.External
+                    target: z.External
                 }, o().createElement("p", {
                     className: Q
-                }, Ue.LearnMore))),
-                et = ({
+                }, Ye.LearnMore))),
+                tt = ({
                     isDisabled: e,
                     formState: t,
                     formErrors: r,
                     environmentVariables: a,
                     setEnvironmentVariables: l,
                     lccOptions: i,
                     availableSecurityGroups: s,
-                    availableSubnets: c,
-                    initialSubnets: u,
-                    initialSecurityGroups: d,
-                    isVPCDomain: m,
+                    availableSubnets: u,
+                    initialSubnets: c,
+                    initialSecurityGroups: m,
+                    isVPCDomain: d,
                     requestClient: b,
                     enableVPCSetting: h,
                     userDefaultValues: E,
                     setFormState: y,
                     handleChange: S,
-                    setSubnets: _,
-                    setSecurityGroups: k,
-                    onSelectLCCScript: x,
-                    setFormValidationErrors: w,
+                    handleNumberValueChange: _,
+                    setSubnets: k,
+                    setSecurityGroups: x,
+                    onSelectLCCScript: w,
+                    setFormValidationErrors: M,
                     setEnableVPCSetting: P,
-                    setRoleArn: M
+                    setRoleArn: T
                 }) => {
                     const {
-                        pluginEnvironment: T
-                    } = Ge(), [C, N] = (0, n.useState)(!1), [I, O] = (0, n.useState)(!1), F = e => {
+                        pluginEnvironment: C
+                    } = $e(), [I, N] = (0, n.useState)(!1), [O, V] = (0, n.useState)(!1), A = e => {
                         const t = e.target.name,
-                            n = Re(e.target.value);
-                        w({
+                            n = Ke(e.target.value);
+                        M({
                             ...r,
                             ["s3_input" === t ? "s3InputFolderError" : "s3OutputFolderError"]: n
                         })
-                    }, V = e => {
+                    }, F = e => {
                         const t = e.target.name,
-                            n = Ke(e.target.value);
-                        w({
+                            n = De(e.target.value);
+                        M({
                             ...r,
                             ["sm_output_kms_key" === t ? "outputKMSError" : "ebsKMSError"]: n
                         })
                     };
                     return o().createElement("div", {
                         className: H
-                    }, o().createElement(Z, {
+                    }, o().createElement(q, {
                         "aria-label": "role_arn",
                         name: "role_arn",
-                        disabled: I,
+                        disabled: O,
                         readOnly: e,
                         required: !0,
-                        labelInfo: He.RoleArn,
+                        labelInfo: Ue.RoleArn,
                         errorMessage: r.roleError,
-                        placeholder: He.Placeholders.RolePlaceHolder,
+                        placeholder: Ue.Placeholders.RolePlaceHolder,
                         onChange: S,
                         value: t.role_arn,
                         onBlur: e => {
                             const {
                                 value: t
                             } = e.target, n = ze(t);
-                            M(t), w({
+                            T(t), M({
                                 ...r,
                                 roleError: n
                             })
                         },
-                        toolTipText: T.isStudio ? Ye.RoleArnTooltip : Ue.RoleArnTooltip
-                    }), o().createElement(Z, {
+                        toolTipText: C.isStudio ? We.RoleArnTooltip : Ye.RoleArnTooltip
+                    }), o().createElement(q, {
                         name: "s3_input",
                         onChange: S,
                         required: !0,
-                        disabled: I,
+                        disabled: O,
                         readOnly: e,
                         value: t.s3_input,
-                        placeholder: He.Placeholders.S3BucketPlaceHolder,
-                        labelInfo: He.s3InputFolder,
+                        placeholder: Ue.Placeholders.S3BucketPlaceHolder,
+                        labelInfo: Ue.s3InputFolder,
                         errorMessage: r.s3InputFolderError,
-                        onBlur: F,
-                        toolTipText: T.isStudio ? Ye.InputFolderTooltip : Ue.InputFolderTooltip
-                    }), o().createElement(Z, {
+                        onBlur: A,
+                        toolTipText: C.isStudio ? We.InputFolderTooltip : Ye.InputFolderTooltip
+                    }), o().createElement(q, {
                         name: "s3_output",
                         onChange: S,
                         required: !0,
-                        disabled: I,
+                        disabled: O,
                         readOnly: e,
                         value: t.s3_output,
-                        placeholder: He.Placeholders.S3BucketPlaceHolder,
-                        labelInfo: He.s3OutputFolder,
+                        placeholder: Ue.Placeholders.S3BucketPlaceHolder,
+                        labelInfo: Ue.s3OutputFolder,
                         errorMessage: r.s3OutputFolderError,
-                        onBlur: F,
-                        toolTipText: T.isStudio ? Ye.OutputFolderTooltip : Ue.OutputFolderTooltip
+                        onBlur: A,
+                        toolTipText: C.isStudio ? We.OutputFolderTooltip : Ye.OutputFolderTooltip
                     }), !e && o().createElement("div", {
                         className: Y
                     }, o().createElement(p.Checkbox, {
                         "data-testid": "kms_checkbox",
                         name: "kms_checkbox",
                         className: X,
                         color: "primary",
-                        checked: C,
+                        checked: I,
                         onChange: e => {
                             const n = e.target.checked;
                             N(n);
                             const o = n ? E.sm_output_kms_key : "",
                                 a = n ? E.sm_volume_kms_key : "";
                             y({
                                 ...t,
                                 sm_output_kms_key: o,
                                 sm_volume_kms_key: a
-                            }), w({
+                            }), M({
                                 ...r,
-                                outputKMSError: Ke(o),
-                                ebsKMSError: Ke(a)
+                                outputKMSError: De(o),
+                                ebsKMSError: De(a)
                             })
                         }
-                    }), o().createElement("label", null, He.enableEncryption), o().createElement(j, {
+                    }), o().createElement("label", null, Ue.enableEncryption), o().createElement(j, {
                         classes: {
                             popperInteractive: ee
                         },
-                        title: Qe,
+                        title: Xe,
                         interactive: !0
                     }, o().createElement(f.Z, {
                         fontSize: "small"
-                    }))), (e || C) && o().createElement(o().Fragment, null, o().createElement(Z, {
+                    }))), (e || I) && o().createElement(o().Fragment, null, o().createElement(q, {
                         name: "sm_output_kms_key",
                         onChange: S,
                         required: !1,
                         readOnly: e,
-                        disabled: I,
+                        disabled: O,
                         value: t.sm_output_kms_key,
-                        placeholder: e ? He.Placeholders.NoneSelected : He.enterKMSArnOrID,
-                        labelInfo: He.kmsKey,
+                        placeholder: e ? Ue.Placeholders.NoneSelected : Ue.enterKMSArnOrID,
+                        labelInfo: Ue.kmsKey,
                         errorMessage: r.outputKMSError,
-                        onBlur: V,
-                        toolTipText: e ? void 0 : Ue.kmsKeyTooltip
-                    }), o().createElement(Z, {
+                        onBlur: F,
+                        toolTipText: e ? void 0 : Ye.kmsKeyTooltip
+                    }), o().createElement(q, {
                         name: "sm_volume_kms_key",
                         onChange: S,
                         required: !1,
                         readOnly: e,
-                        disabled: I,
+                        disabled: O,
                         value: t.sm_volume_kms_key,
-                        placeholder: e ? He.Placeholders.NoneSelected : He.enterKMSArnOrID,
-                        labelInfo: He.ebsKey,
+                        placeholder: e ? Ue.Placeholders.NoneSelected : Ue.enterKMSArnOrID,
+                        labelInfo: Ue.ebsKey,
                         errorMessage: r.ebsKMSError,
-                        onBlur: V,
-                        toolTipText: e ? void 0 : Ue.ebsKeyTooltip
-                    })), m && !e && o().createElement(le, {
+                        onBlur: F,
+                        toolTipText: e ? void 0 : Ye.ebsKeyTooltip
+                    })), d && !e && o().createElement(ie, {
                         isChecked: h,
                         setChecked: P,
-                        initialSecurityGroups: d,
-                        initialSubnets: u,
-                        availableSubnets: c,
+                        initialSecurityGroups: m,
+                        initialSubnets: c,
+                        availableSubnets: u,
                         formState: t,
                         formErrors: r,
-                        setFormErrors: w,
+                        setFormErrors: M,
                         setFormState: y,
                         "data-testid": "vpc-checkbox"
-                    }), (m && h || e) && o().createElement(o().Fragment, null, o().createElement(je, {
+                    }), (d && h || e) && o().createElement(o().Fragment, null, o().createElement(Ce, {
                         required: !0,
                         name: "vpc_subnets",
-                        disabled: e || 0 === c.length,
-                        label: He.subnet,
-                        options: c,
+                        disabled: e || 0 === u.length,
+                        label: Ue.subnet,
+                        options: u,
                         value: t.vpc_subnets,
                         onChange: (e, n, o) => {
                             const [a, l] = ((e, t) => {
-                                if (0 === e.length) return 0 === t.length ? ["", ""] : [Ve.AdvancedOptions.SubnetMinError, void 0];
+                                if (0 === e.length) return 0 === t.length ? ["", ""] : [Fe.AdvancedOptions.SubnetMinError, void 0];
                                 if (e && e.length > 0) {
-                                    if (e.length > 16) return [Ve.AdvancedOptions.SubnetsMaxError, void 0];
+                                    if (e.length > 16) return [Fe.AdvancedOptions.SubnetsMaxError, void 0];
                                     for (const t of e) {
-                                        if (t.length > 32) return [Ve.AdvancedOptions.SubnetLengthError, void 0];
-                                        if (!Ne.test(t)) return [Ve.AdvancedOptions.SubnetsFormatError, void 0]
+                                        if (t.length > 32) return [Fe.AdvancedOptions.SubnetLengthError, void 0];
+                                        if (!Ne.test(t)) return [Fe.AdvancedOptions.SubnetsFormatError, void 0]
                                     }
-                                    if (0 === t.length) return ["", Ve.AdvancedOptions.SecurityGroupMinError]
+                                    if (0 === t.length) return ["", Fe.AdvancedOptions.SecurityGroupMinError]
                                 }
                                 return ["", void 0]
                             })(n, t.vpc_security_group_ids);
-                            _(n), w({
+                            k(n), M({
                                 ...r,
                                 securityGroupError: null != l ? l : r.securityGroupError,
                                 subnetError: null != a ? a : ""
                             })
                         },
                         errorMessage: r.subnetError,
-                        placeholder: `${He.Placeholders.SelectPrivateSubnets}`,
-                        tooltip: T.isStudio ? Ye.SubnetTooltip : Ue.SubnetTooltip,
-                        disabledTooltip: `${He.Placeholders.NoPrivateSubnets}`,
+                        placeholder: `${Ue.Placeholders.SelectPrivateSubnets}`,
+                        tooltip: C.isStudio ? We.SubnetTooltip : Ye.SubnetTooltip,
+                        disabledTooltip: `${Ue.Placeholders.NoPrivateSubnets}`,
                         freeSolo: !0
-                    }), o().createElement(je, {
+                    }), o().createElement(Ce, {
                         required: !0,
                         className: "securityGroupSelector",
                         name: "vpc_security_group_ids",
-                        disabled: e || 0 === c.length,
-                        label: He.securityGroup,
+                        disabled: e || 0 === u.length,
+                        label: Ue.securityGroup,
                         options: s,
                         value: t.vpc_security_group_ids,
                         onChange: (e, n, o) => {
                             const [a, l] = ((e, t) => {
-                                if (0 === e.length) return 0 === t.length ? ["", ""] : [Ve.AdvancedOptions.SecurityGroupMinError, void 0];
+                                if (0 === e.length) return 0 === t.length ? ["", ""] : [Fe.AdvancedOptions.SecurityGroupMinError, void 0];
                                 if (e.length > 0) {
-                                    if (e.length > 5) return [Ve.AdvancedOptions.SecurityGroupsMaxError, void 0];
+                                    if (e.length > 5) return [Fe.AdvancedOptions.SecurityGroupsMaxError, void 0];
                                     for (const t of e) {
-                                        if (!t.startsWith("sg-")) return [Ve.AdvancedOptions.SecurityGroupSGError, void 0];
-                                        if (t.length > 32) return [Ve.AdvancedOptions.SecurityGroupLengthError, void 0];
-                                        if (!Ne.test(t)) return [Ve.AdvancedOptions.SecurityGroupFormatError, void 0]
+                                        if (!t.startsWith("sg-")) return [Fe.AdvancedOptions.SecurityGroupSGError, void 0];
+                                        if (t.length > 32) return [Fe.AdvancedOptions.SecurityGroupLengthError, void 0];
+                                        if (!Ne.test(t)) return [Fe.AdvancedOptions.SecurityGroupFormatError, void 0]
                                     }
-                                    if (0 === t.length) return ["", Ve.AdvancedOptions.SubnetMinError]
+                                    if (0 === t.length) return ["", Fe.AdvancedOptions.SubnetMinError]
                                 }
                                 return ["", void 0]
                             })(n, t.vpc_subnets);
-                            k(n), w({
+                            x(n), M({
                                 ...r,
                                 securityGroupError: null != a ? a : "",
                                 subnetError: null != l ? l : r.subnetError
                             })
                         },
                         errorMessage: r.securityGroupError,
-                        placeholder: `${He.Placeholders.selectOrAdd} ${He.securityGroup}`,
-                        tooltip: T.isStudio ? Ye.SecurityGroupsTooltip : Ue.SecurityGroupsTooltip,
-                        disabledTooltip: `${He.Placeholders.No} ${He.securityGroup}`,
+                        placeholder: `${Ue.Placeholders.selectOrAdd} ${Ue.securityGroup}`,
+                        tooltip: C.isStudio ? We.SecurityGroupsTooltip : Ye.SecurityGroupsTooltip,
+                        disabledTooltip: `${Ue.Placeholders.No} ${Ue.securityGroup}`,
                         freeSolo: !0
-                    })), T.isStudio && o().createElement("div", {
+                    })), C.isStudio && o().createElement("div", {
                         className: te
-                    }, o().createElement(qe.Z, {
+                    }, o().createElement(He.Z, {
                         id: "startup-script-select-label"
-                    }, He.startUpScript, o().createElement(j, {
-                        title: Xe,
+                    }, Ue.startUpScript, o().createElement(j, {
+                        title: et,
                         interactive: !0
                     }, o().createElement(f.Z, {
                         fontSize: "small"
-                    }))), o().createElement($e.Z, {
+                    }))), o().createElement(qe.Z, {
                         labelId: "startup-script-select-label",
                         id: "startup-script-select",
-                        disabled: I,
+                        disabled: O,
                         readOnly: e,
                         value: t.sm_lcc_init_script_arn,
-                        onChange: e => x(e.target.value)
+                        onChange: e => w(e.target.value)
                     }, i && i.map((e => o().createElement(Ze.Z, {
                         key: e,
                         value: e
-                    }, e))))), o().createElement(xe, {
+                    }, e))))), o().createElement(we, {
                         isButtonDisabled: e || a.length >= 48 || !!r.environmentVariablesError,
                         allFieldsDisabled: e,
                         environmentVariables: a,
                         setEnvironmentVariables: l,
                         formErrors: r,
-                        setFormErrors: w
-                    }), o().createElement("div", null, o().createElement(Z, {
-                        placeholder: e ? He.Placeholders.NoneSelected : He.efsPlaceholder,
-                        labelInfo: He.efsLabel,
+                        setFormErrors: M
+                    }), o().createElement("div", null, o().createElement(q, {
+                        placeholder: e ? Ue.Placeholders.NoneSelected : Ue.efsPlaceholder,
+                        labelInfo: Ue.efsLabel,
                         required: !1,
                         value: t.sm_init_script,
                         name: "sm_init_script",
                         readOnly: e,
-                        disabled: I,
+                        disabled: O,
                         errorMessage: r.efsFilePathError,
                         onChange: S,
                         onBlur: e => {
                             const t = e.target.value;
-                            0 === t.trim().length ? w({
+                            0 === t.trim().length ? M({
                                 ...r,
                                 efsFilePathError: ""
                             }) : (async e => {
                                 const t = v.URLExt.join(b.baseUrl, "/validate_volume_path");
-                                O(!0);
+                                V(!0);
                                 const n = await g.ServerConnection.makeRequest(t, {
                                     method: "POST",
                                     body: JSON.stringify({
                                         file_path: e
                                     })
                                 }, b);
-                                O(!1), 200 !== n.status || !0 === (await n.json()).file_path_exist ? w({
+                                V(!1), 200 !== n.status || !0 === (await n.json()).file_path_exist ? M({
                                     ...r,
                                     efsFilePathError: ""
-                                }) : w({
+                                }) : M({
                                     ...r,
-                                    efsFilePathError: We.AdvancedOptions.EFSFilePathError
+                                    efsFilePathError: Qe.AdvancedOptions.EFSFilePathError
                                 })
                             })(t)
                         },
-                        toolTipText: e ? void 0 : T.isStudio ? Ye.InitialScriptTooltip : Ue.InitialScriptTooltip
-                    })))
+                        toolTipText: e ? void 0 : C.isStudio ? We.InitialScriptTooltip : Ye.InitialScriptTooltip
+                    })), o().createElement(q, {
+                        name: "max_retry_attempts",
+                        type: "number",
+                        onChange: _,
+                        required: !0,
+                        disabled: O,
+                        readOnly: e,
+                        value: t.max_retry_attempts,
+                        placeholder: Ue.maxRetryAttempts,
+                        labelInfo: Ue.maxRetryAttempts,
+                        errorMessage: r.maxRetryAttemptsError,
+                        onBlur: e => {
+                            const t = (e => {
+                                const t = parseInt(e);
+                                return isNaN(t) || t < 0 || t > 30 ? Fe.AdvancedOptions.MaxRetryAttemptsError : ""
+                            })(e.target.value);
+                            M({
+                                ...r,
+                                maxRetryAttemptsError: t
+                            })
+                        },
+                        toolTipText: Ye.MaxRetryAttempts
+                    }), o().createElement(q, {
+                        name: "max_run_time_in_seconds",
+                        type: "number",
+                        onChange: _,
+                        required: !0,
+                        disabled: O,
+                        readOnly: e,
+                        value: t.max_run_time_in_seconds,
+                        placeholder: Ue.maxRunTimeInSeconds,
+                        labelInfo: Ue.maxRunTimeInSeconds,
+                        errorMessage: r.maxRunTimeInSecondsError,
+                        onBlur: e => {
+                            const t = (e => {
+                                const t = parseInt(e);
+                                return isNaN(t) || t < 0 ? Fe.AdvancedOptions.MaxRunTimeInSecondsError : ""
+                            })(e.target.value);
+                            M({
+                                ...r,
+                                maxRunTimeInSecondsError: t
+                            })
+                        },
+                        toolTipText: Ye.MaxRunTimeInSeconds
+                    }))
                 },
-                tt = "No script",
-                rt = new Set(["sm_kernel", "sm_image", "sm_lcc_init_script_arn", "role_arn", "vpc_security_group_ids", "vpc_subnets", "s3_input", "s3_output", "sm_init_script", "sm_output_kms_key", "sm_volume_kms_key"]),
-                nt = (e, t, r, n) => {
+                rt = "No script",
+                nt = new Set(["sm_kernel", "sm_image", "sm_lcc_init_script_arn", "role_arn", "vpc_security_group_ids", "vpc_subnets", "s3_input", "s3_output", "sm_init_script", "sm_output_kms_key", "sm_volume_kms_key", "max_run_time_in_seconds", "max_retry_attempts"]),
+                ot = (e, t, r, n) => {
                     var o, a;
                     if (r === l.JobsView.JobDetail || r === l.JobsView.JobDefinitionDetail) {
                         if (e) return e[n] ? e[n].split(",") : []
                     } else if (r === l.JobsView.CreateForm) {
                         if (e && n in e) {
                             const t = e[n];
                             return t ? t.split(",") : []
                         }
                         const r = null === (o = null == t ? void 0 : t.find((e => e.name === n))) || void 0 === o ? void 0 : o.value;
                         return (null === (a = null == r ? void 0 : r.filter((e => e.is_selected))) || void 0 === a ? void 0 : a.map((e => e.name))) || []
                     }
                     return []
                 },
-                ot = (e, t, r, n) => {
+                at = (e, t, r, n) => {
                     var o;
                     if (r === l.JobsView.JobDetail || r === l.JobsView.JobDefinitionDetail) {
                         if (e) return e[n]
                     } else if (r === l.JobsView.CreateForm) return e && n in e ? e[n] : (null === (o = null == t ? void 0 : t.find((e => e.name === n))) || void 0 === o ? void 0 : o.value) || "";
                     return ""
                 },
-                at = (e, t, r) => {
+                lt = (e, t, r, n) => {
+                    if (t === l.JobsView.JobDetail || t === l.JobsView.JobDefinitionDetail) {
+                        if (e) return e[n]
+                    } else if (t === l.JobsView.CreateForm && e && n in e) return e[n];
+                    return r
+                },
+                it = (e, t, r) => {
                     if (t === l.JobsView.JobDetail || t === l.JobsView.JobDefinitionDetail) {
                         if (e) return e[r]
                     } else if (t === l.JobsView.CreateForm && e && r in e) return e[r];
                     return ""
                 },
-                lt = ({
+                st = ({
                     label: e,
                     value: t,
                     options: r,
                     onChange: n,
                     freeSolo: a,
                     customListItemRender: l,
                     renderInput: i,
                     ...s
                 }) => {
-                    var c;
-                    const u = Object.fromEntries(r.map((e => [e.value, e])));
-                    let d = t;
-                    return !a && "string" == typeof t && t in u && (d = u[t]), o().createElement(o().Fragment, null, o().createElement(Pe.Z, {
+                    var u;
+                    const c = Object.fromEntries(r.map((e => [e.value, e])));
+                    let m = t;
+                    return !a && "string" == typeof t && t in c && (m = c[t]), o().createElement(o().Fragment, null, o().createElement(Pe.Z, {
                         ...s,
                         id: `${e}-selectinput`,
                         renderOption: (e, t, r) => o().createElement("li", {
                             ...e
                         }, l ? l(t, t.label, r.selected) : t.label),
                         componentsProps: {
                             ...s.componentsProps,
                             popupIndicator: {
-                                ...null === (c = s.componentsProps) || void 0 === c ? void 0 : c.popupIndicator,
+                                ...null === (u = s.componentsProps) || void 0 === u ? void 0 : u.popupIndicator,
                                 size: "small"
                             }
                         },
                         options: r,
                         onChange: (e, t, r) => {
                             (t && "string" != typeof t || a) && n && n(t || "")
                         },
-                        value: d,
-                        renderInput: i || (e => o().createElement(Me.Z, {
+                        value: m,
+                        renderInput: i || (e => o().createElement(Te.Z, {
                             ...e,
                             variant: "outlined",
                             size: "small",
                             margin: "dense"
                         }))
                     }))
                 },
-                it = ({
+                ut = ({
                     label: e,
                     required: t = !0,
                     toolTipText: r,
                     toolTipArea: n,
                     errorMessage: a,
                     ...l
                 }) => {
                     const i = n && o().createElement("div", null, o().createElement("span", {
                         className: W
                     }, n.descriptionText), n.toolTipComponent);
                     return o().createElement("div", {
                         className: C
                     }, o().createElement("div", {
-                        className: I
+                        className: N
                     }, o().createElement("label", {
-                        className: z(t)
+                        className: R(t)
                     }, e), (r || n) && !l.readOnly && o().createElement(j, {
                         title: i || r || "",
                         className: O,
                         interactive: null !== n
-                    }, o().createElement(f.Z, null))), o().createElement(lt, {
+                    }, o().createElement(f.Z, null))), o().createElement(st, {
                         label: e,
                         disableClearable: !0,
                         ...l
                     }))
                 },
-                st = E.css`
+                ct = E.css`
   display: flex;
   flex-direction: column;
   padding: 10px;
 `,
-                ct = E.css`
+                mt = E.css`
   display: flex;
   flex-direction: column;
   gap: 20px;
 `,
-                ut = E.css`
+                dt = E.css`
   display: flex;
   flex-direction: column;
 `,
-                dt = (E.css`
+                pt = (E.css`
   transform: rotate(90deg);
 `, E.css`
   display: flex;
   flex-flow: row nowrap;
   justify-content: space-between;
   align-items: center;
   width: 100%;
 `),
-                mt = E.css`
+                vt = E.css`
   font-size: var(--jp-ui-font-size0);
   min-width: max-content;
 `,
-                pt = E.css`
+                gt = E.css`
   font-size: var(--jp-ui-font-size0);
   color: var(--jp-inverse-layout-color4);
   padding-right: 5px;
   text-overflow: ellipsis;
   overflow: hidden;
   white-space: nowrap;
 `,
-                vt = E.css`
+                bt = E.css`
   width: 100%;
 `,
-                gt = E.css`
+                ht = E.css`
   display: flex;
   flex-direction: row;
   justify-content: space-between;
   &[data-selected='true'] {
     background-image: var(--jp-check-icon);
     background-size: 15px;
     background-repeat: no-repeat;
     background-position: 100% center;
   }
   & > p {
     max-width: calc(100% - 10px);
   }
 `,
-                bt = (e, t, r) => o().createElement("span", {
-                    className: vt
+                ft = (e, t, r) => o().createElement("span", {
+                    className: bt
                 }, o().createElement("div", {
-                    className: gt,
+                    className: ht,
                     "data-selected": r
-                }, o().createElement("p", null, t || e.label)), ht(e.optionMetadata && e.optionMetadata.description)),
-                ht = e => {
+                }, o().createElement("p", null, t || e.label)), Et(e.optionMetadata && e.optionMetadata.description)),
+                Et = e => {
                     if (!e) return;
                     const t = e.match(/(((https?:\/\/)|(www\.))[^\s]+)/g);
                     if (t)
                         for (const r of t) e = e.replace(r, " ");
                     const r = e.trim();
                     return o().createElement("div", {
-                        className: dt
-                    }, o().createElement("span", {
                         className: pt
-                    }, r), t && t.map((e => o().createElement(D, {
-                        className: mt,
+                    }, o().createElement("span", {
+                        className: gt
+                    }, r), t && t.map((e => o().createElement(L, {
+                        className: vt,
                         key: e,
                         href: e,
-                        target: R.External
+                        target: z.External
                     }, s.KernelSelector.imageSelectorOption.linkText))))
                 };
             r(9850);
-            const ft = ["datascience-1.0", "sagemaker-data-science-38", "1.8.1-cpu-py36", "pytorch-1.8-gpu-py36", "sagemaker-sparkmagic", "tensorflow-2.6-cpu-py38-ubuntu20.04-v1", "tensorflow-2.6-gpu-py38-cu112-ubuntu20.04-v1", "sagemaker-sparkanalytics-v1"];
-            var Et;
+            const yt = ["datascience-1.0", "sagemaker-data-science-38", "1.8.1-cpu-py36", "pytorch-1.8-gpu-py36", "sagemaker-sparkmagic", "tensorflow-2.6-cpu-py38-ubuntu20.04-v1", "tensorflow-2.6-gpu-py38-cu112-ubuntu20.04-v1", "sagemaker-sparkanalytics-v1"];
+            var St;
             ! function(e) {
                 e.Custom = "customImage", e.Sagemaker = "smeImage", e.Session = "session"
-            }(Et || (Et = {}));
-            const yt = {
+            }(St || (St = {}));
+            const _t = {
                 smeImage: "Sagemaker Image",
                 customImage: "Custom Image",
                 prefered: "Use image from preferred session",
                 session: "Use image from other session"
             };
 
-            function St(e, t, r) {
+            function kt(e, t, r) {
                 const n = Object.values(e).filter((e => {
                     const n = e.arnEnvironment.split("/")[1];
-                    return r ? (null == e ? void 0 : e.group) === t && ft.includes(n) : ((null == e ? void 0 : e.group) !== Et.Sagemaker || !e.label.includes("Geospatial")) && (null == e ? void 0 : e.group) === t
+                    return r ? (null == e ? void 0 : e.group) === t && yt.includes(n) : ((null == e ? void 0 : e.group) !== St.Sagemaker || !e.label.includes("Geospatial")) && (null == e ? void 0 : e.group) === t
                 }));
                 return {
-                    label: yt[t],
+                    label: _t[t],
                     value: "",
                     options: n.map((e => ({
                         label: e.label,
-                        value: t === Et.Session ? e.label : e.arnEnvironment,
-                        group: yt[t],
+                        value: t === St.Session ? e.label : e.arnEnvironment,
+                        group: _t[t],
                         optionMetadata: e,
                         options: e.versionOptions
                     })))
                 }
             }
-            const _t = s.ScheduleNoteBook.MainPanel.Tooltips,
-                kt = s.ScheduleNoteBook.MainPanel.StudioTooltips,
-                xt = ({
+            const xt = s.ScheduleNoteBook.MainPanel.Tooltips,
+                wt = s.ScheduleNoteBook.MainPanel.StudioTooltips,
+                Mt = ({
                     isDisabled: e,
                     formState: t,
                     formErrors: r,
                     setFormState: a,
                     setFormErrors: i,
-                    model: c,
-                    jobsView: u,
-                    requestClient: d,
-                    contentsManager: m
+                    model: u,
+                    jobsView: c,
+                    requestClient: m,
+                    contentsManager: d
                 }) => {
                     var p, b;
                     const {
                         pluginEnvironment: h
-                    } = Ge(), [f, E] = (0, n.useState)({
+                    } = $e(), [f, E] = (0, n.useState)({
                         arnEnvironment: null,
                         kernel: null,
                         version: null
                     }), [y, S] = (0, n.useState)({});
                     (0, n.useEffect)((() => {
                         (async function(e) {
                             const t = v.URLExt.join(e.baseUrl, "api/kernelspecs"),
                                 r = await g.ServerConnection.makeRequest(t, {}, e);
                             if (200 === r.status) return await r.json()
-                        })(d).then((async e => {
+                        })(m).then((async e => {
                             var r;
                             e && S(function(e) {
                                 const t = {},
                                     r = e.kernelspecs;
                                 return Object.values(r).forEach((e => {
                                     var r;
                                     if (!e) return;
@@ -1496,27 +1557,27 @@
                                         }(e.spec.display_name),
                                         {
                                             kernel: l,
                                             arnEnvironment: i,
                                             version: s
                                         } = $(e.name);
                                     if (!(l && i && o && a)) return;
-                                    const c = {
+                                    const u = {
                                         arnEnvironment: i,
                                         kernelOptions: [{
                                             label: a,
                                             value: l
                                         }],
                                         versionOptions: s ? [{
                                             label: `v${s}`,
                                             value: s
                                         }] : void 0,
                                         label: s ? `${o} v${s}` : o,
                                         description: (null == n ? void 0 : n.description) ? n.description : void 0,
-                                        group: n && n.is_template ? Et.Sagemaker : Et.Custom
+                                        group: n && n.is_template ? St.Sagemaker : St.Custom
                                     };
                                     if (t[i]) {
                                         const {
                                             kernelOptions: e
                                         } = t[i];
                                         if (!e.some((e => e.value === l))) {
                                             const r = [...e, {
@@ -1534,25 +1595,25 @@
                                                         label: `v${s}`,
                                                         value: s.toString()
                                                     },
                                                     n = Array.isArray(e) ? [...e, r] : [r];
                                                 t[i].versionOptions = n
                                             }
                                         }
-                                    } else t[i] = c
+                                    } else t[i] = u
                                 })), t
                             }(e));
                             const n = await async function(e, t) {
                                 if (e.endsWith(".ipynb")) try {
                                     return (await t.get(e)).content.metadata.kernelspec.name
                                 } catch (e) {
                                     return ""
                                 }
                                 return ""
-                            }(c.inputFile, m), o = n in (null !== (r = null == e ? void 0 : e.kernelspecs) && void 0 !== r ? r : {}) ? n : "", i = ((e, t, r) => {
+                            }(u.inputFile, d), o = n in (null !== (r = null == e ? void 0 : e.kernelspecs) && void 0 !== r ? r : {}) ? n : "", i = ((e, t, r) => {
                                 if (r === l.JobsView.JobDetail || r === l.JobsView.JobDefinitionDetail) {
                                     if (e) {
                                         const {
                                             sm_kernel: t,
                                             sm_image: r
                                         } = e;
                                         return $(`${t}__SAGEMAKER_INTERNAL__${r}`)
@@ -1578,50 +1639,50 @@
                                     }
                                 }
                                 return $(t) || {
                                     kernel: null,
                                     arnEnvironment: null,
                                     version: null
                                 }
-                            })(c.runtimeEnvironmentParameters, o, u);
+                            })(u.runtimeEnvironmentParameters, o, c);
                             E(i), a({
                                 ...t,
                                 sm_kernel: i.kernel || "",
                                 sm_image: i.arnEnvironment || ""
                             })
                         }))
                     }), []);
-                    const _ = [...null !== (p = St(y, Et.Sagemaker, !1).options) && void 0 !== p ? p : [], ...null !== (b = St(y, Et.Custom).options) && void 0 !== b ? b : []],
+                    const _ = [...null !== (p = kt(y, St.Sagemaker, !1).options) && void 0 !== p ? p : [], ...null !== (b = kt(y, St.Custom).options) && void 0 !== b ? b : []],
                         k = (0, n.useMemo)((() => {
                             var e;
                             return f.arnEnvironment && (null === (e = y[f.arnEnvironment]) || void 0 === e ? void 0 : e.kernelOptions) || []
                         }), [y, f]),
                         x = !!r.jobEnvironmentError,
                         w = o().createElement("div", {
-                            className: A
-                        }, o().createElement(ie.Z, {
+                            className: F
+                        }, o().createElement(se.Z, {
                             severity: "error"
                         }, r.jobEnvironmentError));
                     return (0, n.useEffect)((() => {
                         f.arnEnvironment && f.kernel && r.jobEnvironmentError && i({
                             ...r,
                             jobEnvironmentError: ""
                         })
                     }), [f.arnEnvironment, f.kernel]), 0 === Object.keys(y).length ? null : o().createElement("div", {
-                        className: st
-                    }, o().createElement("div", {
                         className: ct
                     }, o().createElement("div", {
-                        className: ut
-                    }, o().createElement(it, {
+                        className: mt
+                    }, o().createElement("div", {
+                        className: dt
+                    }, o().createElement(ut, {
                         "data-testid": "sm_image_dropdown",
                         options: _,
                         value: f.arnEnvironment,
                         label: s.ImageSelector.label,
-                        customListItemRender: bt,
+                        customListItemRender: ft,
                         onChange: (e, r) => {
                             var n;
                             if (!e || "string" == typeof e) return;
                             const o = (null === (n = e.optionMetadata) || void 0 === n ? void 0 : n.kernelOptions) || [],
                                 l = o.length > 0 ? o[0].value : null,
                                 i = r ? r.value : null;
                             a({
@@ -1635,46 +1696,46 @@
                             })
                         },
                         readOnly: e,
                         groupBy: e => {
                             var t;
                             return null !== (t = e.group) && void 0 !== t ? t : ""
                         },
-                        toolTipText: h.isStudio ? kt.ImageTooltipText : _t.ImageTooltipText
+                        toolTipText: h.isStudio ? wt.ImageTooltipText : xt.ImageTooltipText
                     }), r.jobEnvironmentError && o().createElement("div", {
-                        className: V
-                    }, x && w)), o().createElement(it, {
+                        className: A
+                    }, x && w)), o().createElement(ut, {
                         options: k,
                         value: f.kernel,
                         label: s.KernelSelector.label,
                         onChange: e => {
                             e && "string" != typeof e && e && (a({
                                 ...t,
                                 sm_kernel: e.value
                             }), E({
                                 ...f,
                                 kernel: e.value
                             }))
                         },
                         readOnly: e,
-                        toolTipText: h.isStudio ? kt.KernelTooltipText : _t.KernelTooltipText
+                        toolTipText: h.isStudio ? wt.KernelTooltipText : xt.KernelTooltipText
                     })))
                 },
-                wt = s.ScheduleNoteBook.MainPanel.AdvancedOptions,
-                Pt = s.ScheduleNoteBook.MainPanel.Tooltips,
-                Mt = ({
+                Pt = s.ScheduleNoteBook.MainPanel.AdvancedOptions,
+                Tt = s.ScheduleNoteBook.MainPanel.Tooltips,
+                jt = ({
                     setFormState: e,
                     formState: t,
                     isDisabled: r,
                     formErrors: a,
                     setFormErrors: l,
                     model: i,
                     executionEnvironments: s
                 }) => {
-                    const c = (0, n.useMemo)((() => ((e, t) => {
+                    const u = (0, n.useMemo)((() => ((e, t) => {
                         var r, n;
                         if (e) {
                             const {
                                 sm_kernel: t,
                                 sm_image: r
                             } = e;
                             return $(`${t}__SAGEMAKER_INTERNAL__${r}`)
@@ -1686,326 +1747,336 @@
                             arnEnvironment: null,
                             version: null
                         }
                     })(i.runtimeEnvironmentParameters, null == s ? void 0 : s.auto_detected_config)), []);
                     (0, n.useEffect)((() => {
                         e({
                             ...t,
-                            sm_kernel: c.kernel || "",
-                            sm_image: c.arnEnvironment || ""
+                            sm_kernel: u.kernel || "",
+                            sm_image: u.arnEnvironment || ""
                         })
-                    }), [c]);
-                    const u = r => {
+                    }), [u]);
+                    const c = r => {
                         const n = r.target.name,
                             o = r.target.value;
                         e({
                             ...t,
                             [n]: o
                         })
                     };
                     return o().createElement("div", {
                         className: H
-                    }, o().createElement(Z, {
+                    }, o().createElement(q, {
                         name: "sm_image",
-                        onChange: u,
+                        onChange: c,
                         readOnly: r,
                         required: !0,
                         value: t.sm_image,
-                        placeholder: wt.Placeholders.ImagePlaceHolder,
-                        labelInfo: wt.Image,
+                        placeholder: Pt.Placeholders.ImagePlaceHolder,
+                        labelInfo: Pt.Image,
                         errorMessage: a.ImageError,
                         onBlur: e => {
                             const {
                                 value: t
-                            } = e.target, r = t.length <= 0 ? Ve.AdvancedOptions.ImageError : "";
+                            } = e.target, r = t.length <= 0 ? Fe.AdvancedOptions.ImageError : "";
                             l({
                                 ...a,
                                 ImageError: r
                             })
                         },
-                        toolTipText: Pt.ImageTooltipText
-                    }), o().createElement(Z, {
+                        toolTipText: Tt.ImageTooltipText
+                    }), o().createElement(q, {
                         name: "sm_kernel",
-                        onChange: u,
+                        onChange: c,
                         readOnly: r,
                         required: !0,
                         value: t.sm_kernel,
-                        placeholder: wt.Placeholders.KernelPlaceHolder,
-                        labelInfo: wt.Kernel,
+                        placeholder: Pt.Placeholders.KernelPlaceHolder,
+                        labelInfo: Pt.Kernel,
                         errorMessage: a.KernelError,
                         onBlur: e => {
                             const {
                                 value: t
-                            } = e.target, r = t.length <= 0 ? Ve.AdvancedOptions.KernelError : "";
+                            } = e.target, r = t.length <= 0 ? Fe.AdvancedOptions.KernelError : "";
                             l({
                                 ...a,
                                 KernelError: r
                             })
                         },
-                        toolTipText: Pt.KernelTooltipText
+                        toolTipText: Tt.KernelTooltipText
                     }))
                 },
-                Tt = e => {
+                Ct = e => {
                     const {
                         pluginEnvironment: t
-                    } = Ge();
-                    return o().createElement(o().Fragment, null, t.isStudio && o().createElement(xt, {
+                    } = $e();
+                    return o().createElement(o().Fragment, null, t.isStudio && o().createElement(Mt, {
                         ...e
-                    }), t.isLocalJL && o().createElement(Mt, {
+                    }), t.isLocalJL && o().createElement(jt, {
                         ...e
                     }))
                 },
-                jt = e => {
+                It = e => {
                     const {
                         executionEnvironments: t,
                         settingRegistry: r,
                         jobsView: a,
                         requestClient: i,
                         errors: s,
-                        handleErrorsChange: c,
-                        model: u,
-                        handleModelChange: m
+                        handleErrorsChange: u,
+                        model: c,
+                        handleModelChange: d
                     } = e, p = (0, n.useMemo)((() => {
                         return e = null == t ? void 0 : t.auto_detected_config, a === l.JobsView.CreateForm && (null === (r = null == e ? void 0 : e.find((e => "app_network_access_type" === e.name))) || void 0 === r ? void 0 : r.value) || "";
                         var e, r
                     }), []), v = (0, n.useMemo)((() => {
                         var e, r;
                         const n = [],
                             o = (null === (r = null === (e = t.auto_detected_config) || void 0 === e ? void 0 : e.find((e => "lcc_arn" === e.name))) || void 0 === r ? void 0 : r.value) || [];
-                        n.push(tt), n.push(...o);
-                        const i = (s = u.runtimeEnvironmentParameters, ((c = a) === l.JobsView.JobDetail || c === l.JobsView.JobDefinitionDetail) && s && s.sm_lcc_init_script_arn || tt);
-                        var s, c;
-                        return u.runtimeEnvironmentParameters && i !== tt && n.push(i), {
+                        n.push(rt), n.push(...o);
+                        const i = (s = c.runtimeEnvironmentParameters, ((u = a) === l.JobsView.JobDetail || u === l.JobsView.JobDefinitionDetail) && s && s.sm_lcc_init_script_arn || rt);
+                        var s, u;
+                        return c.runtimeEnvironmentParameters && i !== rt && n.push(i), {
                             allLCCOptions: n,
                             selectedLccValue: i
                         }
                     }), []), g = (0, n.useMemo)((() => ((e, t, r) => {
                         var n;
                         if (r === l.JobsView.JobDetail || r === l.JobsView.JobDefinitionDetail) {
                             if (e) return e.role_arn
                         } else if (r === l.JobsView.CreateForm) {
                             if (e && "role_arn" in e) return e.role_arn;
                             const r = null === (n = null == t ? void 0 : t.find((e => "role_arn" === e.name))) || void 0 === n ? void 0 : n.value;
                             if ((null == r ? void 0 : r.length) > 0) return r[0]
                         }
                         return ""
-                    })(u.runtimeEnvironmentParameters, t.auto_detected_config, a)), []), b = (0, n.useMemo)((() => ot(u.runtimeEnvironmentParameters, t.auto_detected_config, a, "s3_output")), []), h = (0, n.useMemo)((() => ot(u.runtimeEnvironmentParameters, t.auto_detected_config, a, "s3_input")), []), f = (0, n.useMemo)((() => {
+                    })(c.runtimeEnvironmentParameters, t.auto_detected_config, a)), []), b = (0, n.useMemo)((() => at(c.runtimeEnvironmentParameters, t.auto_detected_config, a, "s3_output")), []), h = (0, n.useMemo)((() => at(c.runtimeEnvironmentParameters, t.auto_detected_config, a, "s3_input")), []), f = (0, n.useMemo)((() => lt(c.runtimeEnvironmentParameters, a, 1, "max_retry_attempts")), []), E = (0, n.useMemo)((() => lt(c.runtimeEnvironmentParameters, a, 172800, "max_run_time_in_seconds")), []), y = (0, n.useMemo)((() => {
                         var e, r;
                         const n = (null === (r = null === (e = t.auto_detected_config) || void 0 === e ? void 0 : e.find((e => "vpc_security_group_ids" === e.name))) || void 0 === r ? void 0 : r.value) || [];
                         return null == n ? void 0 : n.map((e => e.name))
-                    }), []), E = (0, n.useMemo)((() => {
+                    }), []), S = (0, n.useMemo)((() => {
                         var e, r;
                         const n = (null === (r = null === (e = t.auto_detected_config) || void 0 === e ? void 0 : e.find((e => "vpc_subnets" === e.name))) || void 0 === r ? void 0 : r.value) || [];
                         return null == n ? void 0 : n.map((e => e.name))
-                    }), []), y = (0, n.useMemo)((() => p === d.PublicInternetOnly ? {
+                    }), []), _ = (0, n.useMemo)((() => p === m.PublicInternetOnly ? {
                         securityGroups: [],
                         subnets: []
                     } : {
-                        securityGroups: 0 === E.length && a === l.JobsView.CreateForm ? [] : nt(u.runtimeEnvironmentParameters, t.auto_detected_config, a, "vpc_security_group_ids"),
-                        subnets: nt(u.runtimeEnvironmentParameters, t.auto_detected_config, a, "vpc_subnets")
-                    }), []), S = (0, n.useMemo)((() => ((e, t) => {
+                        securityGroups: 0 === S.length && a === l.JobsView.CreateForm ? [] : ot(c.runtimeEnvironmentParameters, t.auto_detected_config, a, "vpc_security_group_ids"),
+                        subnets: ot(c.runtimeEnvironmentParameters, t.auto_detected_config, a, "vpc_subnets")
+                    }), []), k = (0, n.useMemo)((() => ((e, t) => {
                         if (t === l.JobsView.JobDetail || t === l.JobsView.JobDefinitionDetail) {
                             if (e) return e.sm_init_script
                         } else if (t === l.JobsView.CreateForm && e && "sm_init_script" in e) return e.sm_init_script;
                         return ""
-                    })(u.runtimeEnvironmentParameters, a)), []), _ = (0, n.useMemo)((() => (e => {
+                    })(c.runtimeEnvironmentParameters, a)), []), x = (0, n.useMemo)((() => (e => {
                         const t = [];
                         if (e)
                             for (const r in e)
-                                if (!rt.has(r)) {
+                                if (!nt.has(r)) {
                                     const n = {
                                         key: r,
                                         value: e[r]
                                     };
                                     t.push(n)
                                 } return t
-                    })(u.runtimeEnvironmentParameters)), []), k = (0, n.useMemo)((() => at(u.runtimeEnvironmentParameters, a, "sm_output_kms_key")), []), x = (0, n.useMemo)((() => at(u.runtimeEnvironmentParameters, a, "sm_volume_kms_key")), []), w = (0, n.useMemo)((() => {
-                        if (p === d.PublicInternetOnly) return !1;
-                        const e = y.subnets;
-                        return 0 !== E.length && (0 === e.length && E.length, !0)
-                    }), []), [P, M] = (0, n.useState)({
+                    })(c.runtimeEnvironmentParameters)), []), w = (0, n.useMemo)((() => it(c.runtimeEnvironmentParameters, a, "sm_output_kms_key")), []), M = (0, n.useMemo)((() => it(c.runtimeEnvironmentParameters, a, "sm_volume_kms_key")), []), P = (0, n.useMemo)((() => {
+                        if (p === m.PublicInternetOnly) return !1;
+                        const e = _.subnets;
+                        return 0 !== S.length && (0 === e.length && S.length, !0)
+                    }), []), [T, j] = (0, n.useState)({
                         sm_lcc_init_script_arn: v.selectedLccValue || "",
                         role_arn: g || "",
-                        vpc_security_group_ids: y.securityGroups || "",
-                        vpc_subnets: y.subnets || "",
+                        vpc_security_group_ids: _.securityGroups || "",
+                        vpc_subnets: _.subnets || "",
                         s3_input: h || "",
                         s3_output: b || "",
                         sm_kernel: "",
                         sm_image: "",
-                        sm_init_script: S || "",
-                        sm_output_kms_key: k || "",
-                        sm_volume_kms_key: x || ""
-                    }), [T, j] = (0, n.useState)({
-                        ...P,
+                        sm_init_script: k || "",
+                        sm_output_kms_key: w || "",
+                        sm_volume_kms_key: M || "",
+                        max_retry_attempts: f,
+                        max_run_time_in_seconds: E
+                    }), [C, I] = (0, n.useState)({
+                        ...T,
                         sm_output_kms_key: "",
                         sm_volume_kms_key: ""
                     });
                     (0, n.useEffect)((() => {
-                        const e = (e => e && 0 === e.length ? `${Ae.RequiresPrivateSubnet} ${Ae.NoPrivateSubnetsInSageMakerDomain}` : "")(E),
-                            t = (r = y.subnets) && 0 === r.length ? `${Ae.RequiresPrivateSubnet} ${Ae.NoPrivateSubnetsInSageMakerDomain}. ${Ae.YouMayChooseOtherSubnets}` : "";
+                        const e = (e => e && 0 === e.length ? `${Re.RequiresPrivateSubnet} ${Re.NoPrivateSubnetsInSageMakerDomain}` : "")(S),
+                            t = (r = _.subnets) && 0 === r.length ? `${Re.RequiresPrivateSubnet} ${Re.NoPrivateSubnetsInSageMakerDomain}. ${Re.YouMayChooseOtherSubnets}` : "";
                         var r;
-                        c({
+                        u({
                             ...s,
                             roleError: ze(g),
-                            s3InputFolderError: Re(h),
-                            s3OutputFolderError: Re(b),
+                            s3InputFolderError: Ke(h),
+                            s3OutputFolderError: Ke(b),
                             environmentsStillLoading: "",
                             kernelsStillLoading: "",
-                            subnetError: w && (e || t) || ""
+                            subnetError: P && (e || t) || ""
                         })
                     }), []);
-                    const [C, N] = (0, n.useState)();
+                    const [N, O] = (0, n.useState)();
                     (0, n.useEffect)((() => {
                         (async function(e) {
                             return (await e.get("@amzn/sagemaker-jupyter-scheduler:advanced-options", "advancedOptions")).composite
                         })(r).then((e => {
-                            N(e)
+                            O(e)
                         }))
                     }), []), (0, n.useEffect)((() => {
                         var e, t, r, n;
                         let o = {},
                             a = {},
                             l = {};
-                        const i = null !== (e = null == C ? void 0 : C.role_arn) && void 0 !== e ? e : "";
+                        const i = null !== (e = null == N ? void 0 : N.role_arn) && void 0 !== e ? e : "";
                         i && i !== g && (o = {
                             ...o,
                             role_arn: i
                         }, a = {
                             ...a,
                             roleError: ze(i)
                         });
-                        const u = null !== (t = null == C ? void 0 : C.s3_input) && void 0 !== t ? t : "";
-                        u && u !== h && (o = {
+                        const c = null !== (t = null == N ? void 0 : N.s3_input) && void 0 !== t ? t : "";
+                        c && c !== h && (o = {
                             ...o,
-                            s3_input: u
+                            s3_input: c
                         }, a = {
                             ...a,
-                            s3InputFolderError: Re(u)
+                            s3InputFolderError: Ke(c)
                         });
-                        const d = null !== (r = null == C ? void 0 : C.s3_output) && void 0 !== r ? r : "";
-                        d && d !== b && (o = {
+                        const m = null !== (r = null == N ? void 0 : N.s3_output) && void 0 !== r ? r : "";
+                        m && m !== b && (o = {
                             ...o,
-                            s3_output: d
+                            s3_output: m
                         }, a = {
                             ...a,
-                            s3OutputFolderError: Re(d)
+                            s3OutputFolderError: Ke(m)
                         });
-                        const m = null !== (n = null == C ? void 0 : C.sm_output_kms_key) && void 0 !== n ? n : "";
-                        m && m !== k && (l = {
+                        const d = null !== (n = null == N ? void 0 : N.sm_output_kms_key) && void 0 !== n ? n : "";
+                        d && d !== w && (l = {
                             ...l,
-                            sm_output_kms_key: m
+                            sm_output_kms_key: d
                         }), l = {
                             ...o,
                             ...l
-                        }, Object.keys(o).length > 0 && j({
-                            ...T,
+                        }, Object.keys(o).length > 0 && I({
+                            ...C,
                             ...o
-                        }), Object.keys(l).length > 0 && M({
-                            ...P,
+                        }), Object.keys(l).length > 0 && j({
+                            ...T,
                             ...l
-                        }), Object.keys(a).length > 0 && c({
+                        }), Object.keys(a).length > 0 && u({
                             ...s,
                             ...a
                         })
-                    }), [C]);
-                    const [I, O] = (0, n.useState)(_), [V, A] = (0, n.useState)(w), z = (0, n.useMemo)((() => {
+                    }), [N]);
+                    const [A, F] = (0, n.useState)(x), [R, z] = (0, n.useState)(P), K = (0, n.useMemo)((() => {
                         const e = {};
-                        return null == I || I.map((t => {
+                        return null == A || A.map((t => {
                             const {
                                 key: r,
                                 value: n
                             } = t;
                             0 !== r.trim().length && 0 !== n.trim().length && (e[r] = n)
                         })), e
-                    }), [I]);
+                    }), [A]);
                     (0, n.useEffect)((() => {
                         var e, t;
-                        const r = (null === (e = T.vpc_security_group_ids) || void 0 === e ? void 0 : e.join(",")) || "",
-                            n = (null === (t = T.vpc_subnets) || void 0 === t ? void 0 : t.join(",")) || "";
-                        m({
-                            ...u,
+                        const r = (null === (e = C.vpc_security_group_ids) || void 0 === e ? void 0 : e.join(",")) || "",
+                            n = (null === (t = C.vpc_subnets) || void 0 === t ? void 0 : t.join(",")) || "";
+                        d({
+                            ...c,
                             runtimeEnvironmentParameters: {
-                                ...T,
+                                ...C,
                                 vpc_security_group_ids: r,
                                 vpc_subnets: n,
-                                ...z
+                                ...K
                             }
                         })
-                    }), [T, z]);
-                    const R = a === l.JobsView.JobDefinitionDetail || a === l.JobsView.JobDetail;
+                    }), [C, K]);
+                    const D = a === l.JobsView.JobDefinitionDetail || a === l.JobsView.JobDetail;
                     return o().createElement("div", {
-                        className: F(R)
-                    }, o().createElement(Tt, {
-                        isDisabled: R,
-                        formState: T,
-                        setFormState: j,
+                        className: V(D)
+                    }, o().createElement(Ct, {
+                        isDisabled: D,
+                        formState: C,
+                        setFormState: I,
                         formErrors: s,
-                        setFormErrors: c,
+                        setFormErrors: u,
                         ...e
-                    }), o().createElement(et, {
-                        isDisabled: R,
-                        formState: T,
-                        setFormState: j,
+                    }), o().createElement(tt, {
+                        isDisabled: D,
+                        formState: C,
+                        setFormState: I,
                         handleChange: e => {
                             const t = e.target.name,
                                 r = e.target.value;
-                            j({
-                                ...T,
+                            I({
+                                ...C,
                                 [t]: r
                             })
                         },
+                        handleNumberValueChange: e => {
+                            const t = e.target.name,
+                                r = parseInt(e.target.value);
+                            I({
+                                ...C,
+                                [t]: isNaN(r) ? "" : r
+                            })
+                        },
                         requestClient: i,
                         formErrors: s,
-                        setFormValidationErrors: c,
-                        environmentVariables: I,
-                        userDefaultValues: P,
-                        setEnvironmentVariables: O,
+                        setFormValidationErrors: u,
+                        environmentVariables: A,
+                        userDefaultValues: T,
+                        setEnvironmentVariables: F,
                         lccOptions: v.allLCCOptions,
-                        availableSecurityGroups: f,
-                        availableSubnets: E,
-                        initialSecurityGroups: y.securityGroups,
-                        initialSubnets: y.subnets,
+                        availableSecurityGroups: y,
+                        availableSubnets: S,
+                        initialSecurityGroups: _.securityGroups,
+                        initialSubnets: _.subnets,
                         setSubnets: e => {
-                            j({
-                                ...T,
+                            I({
+                                ...C,
                                 vpc_subnets: e
                             })
                         },
                         setRoleArn: e => {
-                            j({
-                                ...T,
+                            I({
+                                ...C,
                                 role_arn: e
                             })
                         },
                         setSecurityGroups: e => {
-                            j({
-                                ...T,
+                            I({
+                                ...C,
                                 vpc_security_group_ids: e
                             })
                         },
                         onSelectLCCScript: e => {
-                            j({
-                                ...T,
+                            I({
+                                ...C,
                                 sm_lcc_init_script_arn: e
                             })
                         },
-                        isVPCDomain: p === d.VpcOnly,
-                        enableVPCSetting: V,
-                        setEnableVPCSetting: A
+                        isVPCDomain: p === m.VpcOnly,
+                        enableVPCSetting: R,
+                        setEnableVPCSetting: z
                     }))
                 };
-            var Ct = r(2453);
+            var Nt = r(2453);
 
-            function Nt(e) {
+            function Ot(e) {
                 return getComputedStyle(document.body).getPropertyValue(e).trim()
             }
 
-            function It() {
+            function Vt() {
                 const e = document.body.getAttribute("data-jp-theme-light");
-                return (0, Ct.Z)({
+                return (0, Nt.Z)({
                     spacing: 4,
                     components: {
                         MuiButton: {
                             defaultProps: {
                                 size: "small"
                             }
                         },
@@ -2088,135 +2159,140 @@
                             defaultProps: {
                                 variant: "dense"
                             }
                         }
                     },
                     palette: {
                         background: {
-                            paper: Nt("--jp-layout-color1"),
-                            default: Nt("--jp-layout-color1")
+                            paper: Ot("--jp-layout-color1"),
+                            default: Ot("--jp-layout-color1")
                         },
                         mode: "true" === e ? "light" : "dark",
                         primary: {
-                            main: Nt("--jp-brand-color1"),
-                            light: Nt("--jp-brand-color2"),
-                            dark: Nt("--jp-brand-color0")
+                            main: Ot("--jp-brand-color1"),
+                            light: Ot("--jp-brand-color2"),
+                            dark: Ot("--jp-brand-color0")
                         },
                         error: {
-                            main: Nt("--jp-error-color1"),
-                            light: Nt("--jp-error-color2"),
-                            dark: Nt("--jp-error-color0")
+                            main: Ot("--jp-error-color1"),
+                            light: Ot("--jp-error-color2"),
+                            dark: Ot("--jp-error-color0")
                         },
                         warning: {
-                            main: Nt("--jp-warn-color1"),
-                            light: Nt("--jp-warn-color2"),
-                            dark: Nt("--jp-warn-color0")
+                            main: Ot("--jp-warn-color1"),
+                            light: Ot("--jp-warn-color2"),
+                            dark: Ot("--jp-warn-color0")
                         },
                         success: {
-                            main: Nt("--jp-success-color1"),
-                            light: Nt("--jp-success-color2"),
-                            dark: Nt("--jp-success-color0")
+                            main: Ot("--jp-success-color1"),
+                            light: Ot("--jp-success-color2"),
+                            dark: Ot("--jp-success-color0")
                         },
                         text: {
-                            primary: Nt("--jp-ui-font-color1"),
-                            secondary: Nt("--jp-ui-font-color2"),
-                            disabled: Nt("--jp-ui-font-color3")
+                            primary: Ot("--jp-ui-font-color1"),
+                            secondary: Ot("--jp-ui-font-color2"),
+                            disabled: Ot("--jp-ui-font-color3")
                         }
                     },
                     shape: {
                         borderRadius: 2
                     },
                     typography: {
-                        fontFamily: Nt("--jp-ui-font-family"),
+                        fontFamily: Ot("--jp-ui-font-family"),
                         fontSize: 12,
                         htmlFontSize: 16,
                         button: {
                             textTransform: "capitalize"
                         }
                     }
                 })
             }
-            var Ot = r(5395);
+            var At = r(5395);
             const Ft = ({
                     requestClient: e,
                     contentsManager: t,
                     commands: r,
                     jobsView: a,
                     errors: i,
-                    handleErrorsChange: d,
+                    handleErrorsChange: m,
                     ...b
                 }) => {
+                    const [h, f] = (0, n.useState)("");
                     (0, n.useEffect)((() => {
                         const t = {
                             ...i,
                             environmentsStillLoading: "EnvironmentsStillLoadingError",
                             kernelsStillLoading: "KernelsStillLoadingError"
                         };
-                        d(t), a === l.JobsView.CreateForm ? (async () => {
+                        m(t), a === l.JobsView.CreateForm ? (async () => {
                             const t = v.URLExt.join(e.baseUrl, "/advanced_environments"),
                                 n = await g.ServerConnection.makeRequest(t, {}, e);
                             if (200 !== n.status) {
                                 const e = (await n.json()).error_code;
-                                return Object.values(c).indexOf(e) >= 0 && (async e => {
+                                throw Object.values(u).indexOf(e) >= 0 && (async e => {
                                     const t = o().createElement(o().Fragment, null, s.Dialog.awsCredentialsError.body.text.map(((e, t) => o().createElement("p", {
                                             key: t,
                                             className: U
                                         }, ((e, t) => {
                                             const r = e.split("%");
                                             return o().createElement(o().Fragment, null, r.map((e => {
                                                 if (e.startsWith("{")) {
                                                     const [r, ...n] = e.replace("{", "").split("}"), a = t[r], l = n.join("");
-                                                    return a ? o().createElement(o().Fragment, null, o().createElement(D, {
+                                                    return a ? o().createElement(o().Fragment, null, o().createElement(L, {
                                                         key: r,
                                                         href: a.linkHref,
-                                                        target: R.External
+                                                        target: z.External
                                                     }, a.linkString), l) : o().createElement(o().Fragment, null, e)
                                                 }
                                                 return o().createElement(o().Fragment, null, e)
                                             })))
                                         })(e, s.Dialog.awsCredentialsError.body.links))))),
-                                        r = new m.Dialog({
+                                        r = new d.Dialog({
                                             title: s.Dialog.awsCredentialsError.title,
                                             body: t,
-                                            buttons: [m.Dialog.cancelButton(), m.Dialog.okButton({
+                                            buttons: [d.Dialog.cancelButton(), d.Dialog.okButton({
                                                 label: s.Dialog.awsCredentialsError.buttons.enterKeysInTerminal
                                             })]
                                         });
-                                    (await r.launch()).button.label === s.Dialog.awsCredentialsError.buttons.enterKeysInTerminal && e.execute(u)
-                                })(r), null
+                                    (await r.launch()).button.label === s.Dialog.awsCredentialsError.buttons.enterKeysInTerminal && e.execute(c)
+                                })(r), new Error(n.statusText)
                             }
                             return await n.json()
                         })().then((async e => {
-                            y(!1), f(e)
-                        })).catch((e => console.error(e))) : y(!1)
+                            _(!1), y(e)
+                        })).catch((e => {
+                            f(e.message)
+                        })) : _(!1)
                     }), [a, b.model.inputFile]);
-                    const [h, f] = (0, n.useState)({}), [E, y] = (0, n.useState)(!0);
-                    return E ? null : a !== l.JobsView.CreateForm || (null == h ? void 0 : h.auto_detected_config) ? o().createElement(Ot.Z, {
-                        theme: It()
+                    const [E, y] = (0, n.useState)({}), [S, _] = (0, n.useState)(!0);
+                    return h ? o().createElement("div", {
+                        className: re
+                    }, h) : S ? null : a !== l.JobsView.CreateForm || (null == E ? void 0 : E.auto_detected_config) ? o().createElement(At.Z, {
+                        theme: Vt()
                     }, o().createElement(p.StylesProvider, {
                         injectFirst: !0
-                    }, o().createElement(jt, {
-                        executionEnvironments: h,
+                    }, o().createElement(It, {
+                        executionEnvironments: E,
                         requestClient: e,
                         contentsManager: t,
                         jobsView: a,
                         errors: i,
-                        handleErrorsChange: d,
+                        handleErrorsChange: m,
                         ...b
                     }))) : null
                 },
-                Vt = [{
+                Rt = [{
                     id: "@amzn/sagemaker-scheduler:scheduler",
                     autoStart: !1,
                     requires: [a.ISettingRegistry],
                     provides: l.Scheduler.IAdvancedOptions,
                     activate: (e, t) => r => {
                         const n = e.serviceManager.serverSettings,
                             a = e.serviceManager.contents;
-                        return o().createElement(Be, {
+                        return o().createElement(Ge, {
                             app: e
                         }, o().createElement(Ft, {
                             requestClient: n,
                             contentsManager: a,
                             settingRegistry: t,
                             commands: e.commands,
                             ...r
@@ -2247,15 +2323,15 @@
                                     const e = (document.cookie || "").split(";");
                                     for (let t = 0; t < e.length; t++) {
                                         const r = e[t].split("=");
                                         if ("enabledFeatureFlags" === r[0].trim()) return JSON.parse(decodeURIComponent(r[1]))
                                     }
                                     return null
                                 })(),
-                                c = !!s && s.indexOf(i) >= 0;
-                            (o < 1669824e6 || l) && !c && (document.styleSheets[0].insertRule('li[data-command="scheduling:create-from-filebrowser"] { display: none !important; }'), document.styleSheets[0].insertRule('\n          button[title="Create a notebook job"] { display: none !important; }\n        '), document.styleSheets[0].insertRule('\n          div[class="jp-LauncherCard"][title="Notebook Jobs"] { display: none !important; }\n        '))
+                                u = !!s && s.indexOf(i) >= 0;
+                            (o < 1669824e6 || l) && !u && (document.styleSheets[0].insertRule('li[data-command="scheduling:create-from-filebrowser"] { display: none !important; }'), document.styleSheets[0].insertRule('\n          button[title="Create a notebook job"] { display: none !important; }\n        '), document.styleSheets[0].insertRule('\n          div[class="jp-LauncherCard"][title="Notebook Jobs"] { display: none !important; }\n        '))
                         })()
                     }
                 }]
         }
     }
 ]);
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.9f672e548acd2153a221.js` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.299f9d522c52a504280b.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, a, n, o, i, u, l, f, d, s, c, p, h, b, m, v, g = {
-            5700: (e, r, t) => {
+            3194: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(349), t.e(509), t.e(86), t.e(271), t.e(456), t.e(993)]).then((() => () => t(7993))),
                         "./extension": () => Promise.all([t.e(349), t.e(509), t.e(86), t.e(271), t.e(456), t.e(993)]).then((() => () => t(7993)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
@@ -51,27 +51,27 @@
         240: "762850093662386d80d3",
         271: "a546aebb6445a3b38e60",
         349: "eb375dbeb301592df698",
         456: "f9df645a48dde143e1a9",
         509: "b1db44e3c8c1ddb64444",
         615: "d5639a877b54ff655d41",
         915: "83ac080d036e9c56d7e0",
-        993: "faa5510ce9696a850c76"
+        993: "84c00bb76b4448d8ce3f"
     } [e] + ".js?v=" + {
         86: "99a29e600153377570fa",
         144: "9be27e93647ef0e84863",
         193: "04adf0a714b67e82f263",
         240: "762850093662386d80d3",
         271: "a546aebb6445a3b38e60",
         349: "eb375dbeb301592df698",
         456: "f9df645a48dde143e1a9",
         509: "b1db44e3c8c1ddb64444",
         615: "d5639a877b54ff655d41",
         915: "83ac080d036e9c56d7e0",
-        993: "faa5510ce9696a850c76"
+        993: "84c00bb76b4448d8ce3f"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -123,15 +123,15 @@
                         (!u || !u.loaded && (!a != !u.eager ? a : i > u.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (u("@amzn/sagemaker-jupyter-scheduler", "2.0.2", (() => Promise.all([w.e(349), w.e(509), w.e(86), w.e(271), w.e(456), w.e(993)]).then((() => () => w(7993))))), u("@emotion/css", "11.10.5", (() => Promise.all([w.e(509), w.e(615)]).then((() => () => w(4615))))), u("@material-ui/core", "4.12.4", (() => Promise.all([w.e(193), w.e(349), w.e(271), w.e(456)]).then((() => () => w(3193))))), u("react-router-dom", "5.3.4", (() => Promise.all([w.e(240), w.e(271), w.e(915)]).then((() => () => w(7240)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@amzn/sagemaker-jupyter-scheduler", "2.1.0", (() => Promise.all([w.e(349), w.e(509), w.e(86), w.e(271), w.e(456), w.e(993)]).then((() => () => w(7993))))), u("@emotion/css", "11.10.5", (() => Promise.all([w.e(509), w.e(615)]).then((() => () => w(4615))))), u("@material-ui/core", "4.12.4", (() => Promise.all([w.e(193), w.e(349), w.e(271), w.e(456)]).then((() => () => w(3193))))), u("react-router-dom", "5.3.4", (() => Promise.all([w.e(240), w.e(271), w.e(915)]).then((() => () => w(7240)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -299,10 +299,10 @@
                     u && u(w)
                 }
                 for (r && r(t); l < o.length; l++) n = o[l], w.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_amzn_sagemaker_jupyter_scheduler = self.webpackChunk_amzn_sagemaker_jupyter_scheduler || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var j = w(5700);
+    var j = w(3194);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amzn/sagemaker-jupyter-scheduler"] = j
 })();
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/logging.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/logging.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/model_converter.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/model_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -201,21 +201,25 @@
                 "InstanceType": "ml.m5.xlarge"
                 if isinstance(upstream_model, UpdateJobDefinition)
                 else upstream_model.compute_type,
                 "VolumeSizeInGB": 30,
             },
             # "RetryStrategy": {"MaximumRetryAttempts": upstream_model.max_retries},
             "RetryStrategy": {
-                "MaximumRetryAttempts": 1
+                "MaximumRetryAttempts": runtime_environment_parameters.max_retry_attempts
+                if hasattr(runtime_environment_parameters, "max_retry_attempts")
+                else 1
             },  # TODO: currently OSS UI is not providing an option to set this, setting it for default 1
             "RoleArn": runtime_environment_parameters.role_arn,
             "StoppingCondition": {
                 # TODO: Stop hard-coding these values, when they are added back to the model.
                 # 60 * 60 * 48 = 172800 seconds (48 hours)
-                "MaxRuntimeInSeconds": 172800,
+                "MaxRuntimeInSeconds": runtime_environment_parameters.max_run_time_in_seconds
+                if hasattr(runtime_environment_parameters, "max_run_time_in_seconds")
+                else 172800,
                 "MaxWaitTimeInSeconds": 172800,
                 # "MaxRuntimeInSeconds": upstream_model.timeout_seconds,
                 # "MaxWaitTimeInSeconds": upstream_model.timeout_seconds,
             },
         }
 
         if upstream_model.parameters is not None and len(upstream_model.parameters):
@@ -316,14 +320,20 @@
             ).customer_environment_variables,
             RuntimeEnvironmentParameterName.SM_IMAGE.value: training_job_environment.get(
                 JobEnvironmentVariableName.SM_FIRST_PARTY_IMAGE_ARN.value, ""
             ),
             RuntimeEnvironmentParameterName.S3_INPUT.value: s3_uri.split(
                 f"/{training_job_name}"
             )[0],
+            RuntimeEnvironmentParameterName.MAX_RETRY_ATTEMPTS.value: training_job_response.get("RetryStrategy", {}).get(
+                "MaximumRetryAttempts", 0
+            ),
+            RuntimeEnvironmentParameterName.MAX_RUN_TIME_IN_SECONDS.value: training_job_response.get("StoppingCondition", {}).get(
+                "MaxRuntimeInSeconds", 172800
+            ),
             RuntimeEnvironmentParameterName.S3_OUTPUT.value: s3_output,
             RuntimeEnvironmentParameterName.SM_KERNEL.value: training_job_environment.get(
                 JobEnvironmentVariableName.SM_KERNEL_NAME.value, ""
             ),
             RuntimeEnvironmentParameterName.SM_INIT_SCRIPT.value: training_job_environment.get(
                 JobEnvironmentVariableName.SM_INIT_SCRIPT.value, ""
             ),
@@ -426,14 +436,16 @@
 
         # Reduce output formats to those that are available, while preserving original order.
         output_formats = [
             output_format
             for output_format in output_formats
             if output_format in available_output_formats
         ]
+        secondary_status = training_job_response.get("SecondaryStatus", '')
+        training_job_status = training_job_response["TrainingJobStatus"]
 
         describe_job_response = DescribeJob(
             job_id=training_job_response.get("TrainingJobName"),
             output_formats=output_formats,
             input_filename=environment.get(
                 JobEnvironmentVariableName.SM_INPUT_NOTEBOOK_NAME.value, ""
             ),
@@ -460,21 +472,21 @@
             ),
             max_retries=training_job_response.get("RetryStrategy", {}).get(
                 "MaximumRetryAttempts", 0
             ),
             compute_type=training_job_response.get("ResourceConfig", {}).get(
                 "InstanceType"
             ),
-            status=status,
             create_time=training_job_response["CreationTime"].timestamp() * 1000,
             update_time=training_job_response["LastModifiedTime"].timestamp() * 1000,
             start_time=start_time.timestamp() * 1000 if start_time else None,
             end_time=end_time.timestamp() * 1000 if end_time else None,
-            status_message=failure_reason,
-            url="https://amazon.com",  # TODO
+            url = "https://amazon.com",
+            status_message = secondary_status if secondary_status == "MaxRuntimeExceeded" and training_job_status == "Stopped" else failure_reason,
+            status = Status.FAILED if secondary_status == "MaxRuntimeExceeded" and training_job_status == "Stopped" else status,
             # idempotency_token = TODO: TBD OSS
             # tags = TODO: How should we translate list of key:value pairs to list of strings?
         )
 
         if outputs:
             # This indicates to the UI where the output files are located, if they have been downloaded.
             scheduler.add_job_files(describe_job_response)
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/models.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,16 @@
     S3_INPUT = "s3_input"
     S3_OUTPUT = "s3_output"
     ROLE_ARN = "role_arn"
     VPC_SECURITY_GROUP_IDS = "vpc_security_group_ids"
     VPC_SUBNETS = "vpc_subnets"
     SM_OUTPUT_KMS_KEY = "sm_output_kms_key"
     SM_VOLUME_KMS_KEY = "sm_volume_kms_key"
+    MAX_RETRY_ATTEMPTS = "max_retry_attempts"
+    MAX_RUN_TIME_IN_SECONDS = "max_run_time_in_seconds"
 
     def __str__(self):
         return self.value
 
 
 class JobEnvironmentVariableName(Enum):
     SM_JOB_DEF_VERSION = "SM_JOB_DEF_VERSION"
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/revenue.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/revenue.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/providers/tags.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/providers/tags.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/runtime_environment_parameters.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/runtime_environment_parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,22 @@
         return self.parameters.get(RuntimeEnvironmentParameterName.S3_INPUT.value)
 
     @property
     def s3_output(self):
         return self.parameters.get(RuntimeEnvironmentParameterName.S3_OUTPUT.value)
 
     @property
+    def max_run_time_in_seconds(self):
+        return self.parameters.get(RuntimeEnvironmentParameterName.MAX_RUN_TIME_IN_SECONDS.value)
+    
+    @property
+    def max_retry_attempts(self):
+        return self.parameters.get(RuntimeEnvironmentParameterName.MAX_RETRY_ATTEMPTS.value)
+
+    @property
     def role_arn(self):
         return self.parameters.get(RuntimeEnvironmentParameterName.ROLE_ARN.value)
 
     @property
     def security_group_ids(self):
         return self.parameters.get(
             RuntimeEnvironmentParameterName.VPC_SECURITY_GROUP_IDS.value
@@ -72,7 +80,18 @@
     @property
     def customer_environment_variables(self):
         return self._remove_dict_keys(
             self.parameters,
             [str(item) for item in RuntimeEnvironmentParameterName]
             + [str(item) for item in JobEnvironmentVariableName],
         )
+    @property
+    def max_retry_attempts(self):
+        return self.parameters.get(
+            RuntimeEnvironmentParameterName.MAX_RETRY_ATTEMPTS.value
+        )
+
+    @property
+    def max_run_time_in_seconds(self):
+        return self.parameters.get(
+            RuntimeEnvironmentParameterName.MAX_RUN_TIME_IN_SECONDS.value
+        )
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/scheduler.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -604,14 +604,15 @@
                 await self.converter.to_create_training_job_input(
                     training_job_name=job_definition_id,
                     upstream_model=model,
                     s3_file_uploader=s3_file_uploader,
                     s3_dependency_uri=s3_dependency_uri,
                 )
             )
+            create_training_job_input["RetryStrategy"]["MaximumRetryAttempts"] = 1
 
             common_tags = []
 
             try:
                 common_tags = await get_resource_create_tags(
                     job_name=model.name,
                     notebook_name=s3_file_uploader.notebook_name,
@@ -637,28 +638,41 @@
                     s3_file_uploader.notebook_name
                 )
                 create_training_job_input["Environment"][
                     JobEnvironmentVariableName.SM_OUTPUT_NOTEBOOK_NAME.value
                 ] = get_pipeline_expression_output_name(
                     model.name, notebook_name_without_ext, notebook_extension
                 )
-
+                maxAttempts = runtime_environment_parameters.max_retry_attempts if hasattr(runtime_environment_parameters, "max_retry_attempts") else 1
+                maxAttempts = int(maxAttempts)
                 pipeline_result = await self.sagemaker_client().create_pipeline(
                     pipeline_name=job_definition_id,
                     pipeline_display_name=sanitize_string(model.name, 63),
                     pipeline_description=self.get_created_resources_description_text(),
                     pipeline_definition=json.dumps(
                         {
                             "Version": "2020-12-01",
                             "Parameters": [],
                             "Steps": [
                                 {
                                     "Name": f"{sanitize_string(model.name, 10)}-{sanitize_string(notebook_name_without_ext, 10)}",
                                     "Type": "Training",
                                     "Arguments": create_training_job_input,
+                                    "RetryPolicies": [
+                                        {
+                                            "ExceptionType": [
+                                                "Step.SERVICE_FAULT",
+                                                "Step.THROTTLING",
+                                                "SageMaker.JOB_INTERNAL_ERROR",
+                                                "SageMaker.CAPACITY_ERROR",
+                                                "SageMaker.RESOURCE_LIMIT"
+                                            ],
+                                            "MaxAttempts": maxAttempts,
+                                        },
+                                    ],
                                 }
                             ],
                         }
                     ),
                     role_arn=runtime_environment_parameters.role_arn,
                     tags=common_tags,
                 )
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/helpers/utils.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/providers/test_image_metadata.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/providers/test_image_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/providers/test_tags.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/providers/test_tags.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_advanced_environments.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_advanced_environments.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_app_metadata.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_app_metadata.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_aws_config.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_aws_config.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_clients.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_cron_util.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_cron_util.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_deletable_resource.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_deletable_resource.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_environment_detector.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_environment_detector.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_environments.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_error_util.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_error_util.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_file_uploader.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_file_uploader.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_handlers.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_internal_metadata_adapter.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_internal_metadata_adapter.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_logging.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_model_converter.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_model_converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -172,23 +172,111 @@
         "sm_init_script": "",
         "sm_kernel": "",
         "sm_lcc_init_script_arn": "",
         "vpc_security_group_ids": "",
         "vpc_subnets": "",
         "sm_output_kms_key": "arn:aws:kms:us-west-2:344324978117:key/e5cdae90-20db-4e1c-8741-038652abcf94",
         "sm_volume_kms_key": "arn:aws:kms:us-west-2:344324978117:key/e5cdae90-20db-4e1c-038652abcf94",
+        'max_retry_attempts': 3, 
+        'max_run_time_in_seconds': 300,
     }
     assert describe_jupyter_job_output.compute_type == "ml.m5.2xlarge"
     assert describe_jupyter_job_output.status.value == "FAILED"
     assert describe_jupyter_job_output.create_time == 1664472266000
     assert describe_jupyter_job_output.start_time == 1664472372000
     assert describe_jupyter_job_output.end_time == 1664472499000
     assert describe_jupyter_job_output.update_time == 1664472501000
     assert describe_jupyter_job_output.status_message == "Algorithm error: 123"
 
+@patch("builtins.open", custom_mock_open)
+def test_to_jupyter_describe_job_output_status_message():
+    mock_scheduler = Mock()
+    mock_scheduler.environments_manager.output_formats_mapping.return_value = {
+        "ipynb": "Notebook",
+    }
+    describe_jupyter_job_output = ModelConverter(Mock()).to_jupyter_describe_job_output(
+        scheduler=mock_scheduler,
+        outputs=True,
+        training_job_response={
+            "TrainingJobName": "a-b-c-d",
+            "InputDataConfig": [
+                {"DataSource": {"S3DataSource": {"S3Uri": "s3://data-source-uri"}}}
+            ],
+            "OutputDataConfig": {
+                "S3OutputPath": "s3://output-path",
+                "KmsKeyId": "arn:aws:kms:us-west-2:344324978117:key/e5cdae90-20db-4e1c-8741-038652abcf94",
+            },
+            "HyperParameters": {
+                "hyper param 1": "hyper param 1 value",
+                "hyper param 2": "hyper param 2 value",
+            },
+            "Environment": {
+                "SM_ENV_NAME": "sagemaker-default-env",
+                "SM_OUTPUT_FORMATS": "ipynb",
+                "environment property 1": "environment property 1 value",
+                "environment property 2": "environment property 2 value",
+            },
+            "RoleArn": "arn:aws:iam::177118115371:role/service-role/AmazonSageMaker-ExecutionRole-20220125T140052",
+            "StoppingCondition": {"MaxRuntimeInSeconds": 300},
+            "RetryStrategy": {"MaximumRetryAttempts": 3},
+            "ResourceConfig": {
+                "InstanceType": "ml.m5.2xlarge",
+                "VolumeKmsKeyId": "arn:aws:kms:us-west-2:344324978117:key/e5cdae90-20db-4e1c-038652abcf94",
+            },
+            "TrainingJobStatus": "Stopped",
+            "SecondaryStatus": "MaxRuntimeExceeded",
+            "CreationTime": datetime.fromisoformat("2022-09-29T10:24:26-07:00"),
+            "TrainingStartTime": datetime.fromisoformat("2022-09-29T10:26:12-07:00"),
+            "TrainingEndTime": datetime.fromisoformat("2022-09-29T10:28:19-07:00"),
+            "LastModifiedTime": datetime.fromisoformat("2022-09-29T10:28:21-07:00"),
+            "FailureReason": "Algorithm error: [SM-111] 123",
+        },
+        tag_dict={
+            "sagemaker:name": "My Training Job",
+            "sagemaker:job-definition-id": "my-job-definition",
+        },
+    )
+
+    assert describe_jupyter_job_output.job_id == "a-b-c-d"
+    assert describe_jupyter_job_output.output_formats == ["ipynb", "log"]
+    assert describe_jupyter_job_output.input_filename == ""
+    assert (
+        describe_jupyter_job_output.runtime_environment_name == "sagemaker-default-env"
+    )
+    assert describe_jupyter_job_output.name == "My Training Job"
+    assert describe_jupyter_job_output.job_definition_id == "my-job-definition"
+    assert describe_jupyter_job_output.parameters == {
+        "hyper param 1": "hyper param 1 value",
+        "hyper param 2": "hyper param 2 value",
+    }
+    assert describe_jupyter_job_output.runtime_environment_parameters == {
+        "environment property 1": "environment property 1 value",
+        "environment property 2": "environment property 2 value",
+        "role_arn": "arn:aws:iam::177118115371:role/service-role/AmazonSageMaker-ExecutionRole-20220125T140052",
+        "s3_input": "s3://data-source-uri",
+        "s3_output": "s3://output-path",
+        # TODO: Mock these values in the input, and update the assertion here.
+        "sm_image": "",
+        "sm_init_script": "",
+        "sm_kernel": "",
+        "sm_lcc_init_script_arn": "",
+        "vpc_security_group_ids": "",
+        "vpc_subnets": "",
+        "sm_output_kms_key": "arn:aws:kms:us-west-2:344324978117:key/e5cdae90-20db-4e1c-8741-038652abcf94",
+        "sm_volume_kms_key": "arn:aws:kms:us-west-2:344324978117:key/e5cdae90-20db-4e1c-038652abcf94",
+        'max_retry_attempts': 3, 
+        'max_run_time_in_seconds': 300,
+    }
+    assert describe_jupyter_job_output.compute_type == "ml.m5.2xlarge"
+    assert describe_jupyter_job_output.status.value == "FAILED"
+    assert describe_jupyter_job_output.create_time == 1664472266000
+    assert describe_jupyter_job_output.start_time == 1664472372000
+    assert describe_jupyter_job_output.end_time == 1664472499000
+    assert describe_jupyter_job_output.update_time == 1664472501000
+    assert describe_jupyter_job_output.status_message == "MaxRuntimeExceeded"
 
 mock_create_job = CreateJob(
     input_uri="Untitled.ipynb",
     output_formats=["ipynb"],
     runtime_environment_name="sagemaker-default-env",
     runtime_environment_parameters={
         "sm_lcc_init_script_arn": "No script",
@@ -199,14 +287,16 @@
         "s3_output": "s3://sagemaker-notebook-execution-748478975813/",
         "sm_kernel": "python3",
         "sm_image": "arn:aws:sagemaker:us-west-2:236514542706:image/datascience-1.0",
         "executionEnvironment": "",
         "sm_init_script": "",
         "sm_output_kms_key": "arn:aws:kms:us-west-2:344324978117:key/e5cdae90-20db-4e1c-8741-038652abcf94",
         "sm_volume_kms_key": "arn:aws:kms:us-west-2:344324978117:key/e5cdae90-20db-4e1c-8741-038652abcf94",
+        "max_retry_attempts": 1,
+        "max_run_time_in_seconds": 172800,
     },
     name="NotebookA.ipynb",
     compute_type="ml.m4.xlarge",
 )
 
 
 @pytest.mark.asyncio
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_runtime_environment_parameters.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_runtime_environment_parameters.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,16 @@
         "s3_input": "mock-s3_input",
         "s3_output": "mock-s3_output",
         "role_arn": "mock-role_arn",
         "vpc_security_group_ids": "mock-vpc_security_group_ids",
         "vpc_subnets": "mock-vpc_subnets",
         "other_param": "mock-other_param",
         "yet_another_param": "mock-yet_another_param",
+        "max_retry_attempts": "mock-max_retry_attempts",
+        "max_run_time_in_seconds": "mock-max_run_time_in_seconds",
     }
 
     # When
     runtime_environment_parameters = RuntimeEnvironmentParameters(raw_parameters)
 
     # Then
     assert runtime_environment_parameters.sm_image == "mock-sm_image"
@@ -38,7 +40,14 @@
         == "mock-vpc_security_group_ids"
     )
     assert runtime_environment_parameters.subnets == "mock-vpc_subnets"
     assert runtime_environment_parameters.customer_environment_variables == {
         "other_param": "mock-other_param",
         "yet_another_param": "mock-yet_another_param",
     }
+    assert (
+        runtime_environment_parameters.max_retry_attempts == "mock-max_retry_attempts"
+    )
+    assert (
+        runtime_environment_parameters.max_run_time_in_seconds
+        == "mock-max_run_time_in_seconds"
+    )
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/tests/test_scheduler.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/tests/test_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -704,26 +704,29 @@
     input = MagicMock()
     TEST_JOB_NAME = "JobName"
     TEST_NOTEBOOK_NAME = "HelloWorld.ipynb"
     TEST_INPUT_URI = f"a/b/c/{TEST_NOTEBOOK_NAME}"
     input.name = TEST_JOB_NAME
     input.input_uri = TEST_INPUT_URI
     input.schedule = "0 0 * * MON-FRI"
+    # TODO Fix this unit tests
+    # input.runtime_environment_parameters.max_retry_attempts = 3
     # to make the create_job call, we need to mock a bunch of things
     # 1. s3 bucket upload, getting dependency, converter create_job input
     # to_job_tags and get_addtion_tags
 
     mock_s3_file_uploader = MagicMock()
     mock_s3_file_uploader.notebook_name = TEST_NOTEBOOK_NAME
     scheduler._prepare_job_artifacts = AsyncMock(return_value=mock_s3_file_uploader)
 
     scheduler._get_system_dependencies_version = AsyncMock()
 
     mock_training_job = {
-        "Environment": {JobEnvironmentVariableName.SM_OUTPUT_NOTEBOOK_NAME.value: ""}
+        "Environment": {JobEnvironmentVariableName.SM_OUTPUT_NOTEBOOK_NAME.value: ""},
+        "RetryStrategy": { "MaximumRetryAttempts" : 1 }
     }
     scheduler.converter.to_create_training_job_input = AsyncMock(
         return_value=mock_training_job
     )
 
     mock_sagemaker_client = AsyncMock(spec=SageMakerAsyncBoto3Client)
     scheduler._sagemaker_client = mock_sagemaker_client
@@ -748,14 +751,17 @@
     ]
     training_job = json.loads(
         mock_sagemaker_client.create_pipeline.call_args_list[0].kwargs[
             "pipeline_definition"
         ]
     )
     training_job_tags = training_job["Steps"][0]["Arguments"]["Tags"]
+    assert training_job["Steps"][0]["RetryPolicies"][0]["ExceptionType"] == ["Step.SERVICE_FAULT", "Step.THROTTLING", "SageMaker.JOB_INTERNAL_ERROR", "SageMaker.CAPACITY_ERROR", "SageMaker.RESOURCE_LIMIT"]
+    # TODO Fix this unit tests
+    # assert training_job["Steps"][0]["RetryPolicies"][0]["MaxAttempts"] == 3
     event_bridge_rule_tags = mock_eventbridge_client.put_rule.call_args_list[0].kwargs[
         "tags"
     ]
 
     compare_tag_list(pipeline_tags, expected_tags)
     compare_tag_list(
         training_job_tags,
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler/utils.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler.egg-info/PKG-INFO` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-sagemaker-jupyter-scheduler
-Version: 2.0.2
+Version: 2.1.0
 Summary: Amazon SageMaker Jupyter Scheduler based on the https://pypi.org/project/jupyter-scheduler/
 Home-page: https://aws.amazon.com/sagemaker/
 Author: Amazon
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3,Scheduling Notebooks,Notebooks,Amazon Sagemaker
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/amazon_sagemaker_jupyter_scheduler.egg-info/SOURCES.txt` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,16 @@
 amazon_sagemaker_jupyter_scheduler/labextension/static/349.eb375dbeb301592df698.js.LICENSE.txt
 amazon_sagemaker_jupyter_scheduler/labextension/static/509.b1db44e3c8c1ddb64444.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/615.d5639a877b54ff655d41.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/86.99a29e600153377570fa.js.LICENSE.txt
 amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/915.83ac080d036e9c56d7e0.js.LICENSE.txt
-amazon_sagemaker_jupyter_scheduler/labextension/static/993.faa5510ce9696a850c76.js
-amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.9f672e548acd2153a221.js
+amazon_sagemaker_jupyter_scheduler/labextension/static/993.84c00bb76b4448d8ce3f.js
+amazon_sagemaker_jupyter_scheduler/labextension/static/remoteEntry.299f9d522c52a504280b.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/style.js
 amazon_sagemaker_jupyter_scheduler/labextension/static/third-party-licenses.json
 amazon_sagemaker_jupyter_scheduler/providers/__init__.py
 amazon_sagemaker_jupyter_scheduler/providers/image_metadata.py
 amazon_sagemaker_jupyter_scheduler/providers/revenue.py
 amazon_sagemaker_jupyter_scheduler/providers/standalone_image_metadata.py
 amazon_sagemaker_jupyter_scheduler/providers/studio_image_metadata.py
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/jest.config.base.js` & `amazon_sagemaker_jupyter_scheduler-2.1.0/jest.config.base.js`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/package-lock.json` & `amazon_sagemaker_jupyter_scheduler-2.1.0/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.916663640764948%*

 * *Differences: {"'packages'": "{'': {'version': '2.1.0'}}", "'version'": "'2.1.0'"}*

```diff
@@ -11856,15 +11856,15 @@
                 "jest": "^27.2.4",
                 "npm-run-all": "^4.1.5",
                 "ts-jest": "^27.0.5",
                 "typescript": "^4.9.5"
             },
             "license": "Apache 2.0",
             "name": "@amzn/sagemaker-jupyter-scheduler",
-            "version": "2.0.2"
+            "version": "2.1.0"
         },
         "node_modules/@adobe/css-tools": {
             "dev": true,
             "integrity": "sha512-E09FiIft46CmH5Qnjb0wsW54/YQd69LsxeKUOWawmws1XWvyFGURnAChH0mlr7YPFR1ofwvUQfcL0J3lMxXqPA==",
             "license": "MIT",
             "version": "4.2.0"
         },
@@ -29020,9 +29020,9 @@
             },
             "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
             "license": "MIT",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "2.0.2"
+    "version": "2.1.0"
 }
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/package.json` & `amazon_sagemaker_jupyter_scheduler-2.1.0/amazon_sagemaker_jupyter_scheduler/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.961111111111111%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.299f9d522c52a504280b.js'), "*

 * *                 "('extension', './extension')])}",*

 * * "'version'": "'2.1.0'"}*

```diff
@@ -59,14 +59,18 @@
     "files": [
         "dist/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://aws.amazon.com/sagemaker/",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.299f9d522c52a504280b.js"
+        },
         "disabledExtensions": [
             "@jupyterlab/scheduler:IAdvancedOptions"
         ],
         "extension": true,
         "outputDir": "amazon_sagemaker_jupyter_scheduler/labextension",
         "schemaDir": "schema",
         "sharedPackages": {
@@ -106,9 +110,9 @@
         "test": "jest",
         "test:debug": "node --inspect node_modules/.bin/jest --watch --runInBand",
         "test:server-extension": ":",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
-    "version": "2.0.2"
+    "version": "2.1.0"
 }
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/setup.py` & `amazon_sagemaker_jupyter_scheduler-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/__tests__/CreateNotebookJobForm.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/__tests__/CreateNotebookJobForm.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/__tests__/VpcCheckbox.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/__tests__/VpcCheckbox.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/__tests__/initalValueHelpers.spec.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/__tests__/initalValueHelpers.spec.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/__tests__/validationHelpers.spec.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/__tests__/validationHelpers.spec.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/Link.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/Link.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/RouterLink.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/RouterLink.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/__test__/Link.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/__test__/Link.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/link/__test__/RouterLink.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/link/__test__/RouterLink.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/selectinput/SelectInput.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/selectinput/SelectInput.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/selectinput/types.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/selectinput/types.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/TextInput.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/TextInput.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/__tests__/TextInput.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/__tests__/TextInput.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/textinput/styles.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/textinput/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/tooltip/Tooltip.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/tooltip/Tooltip.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/tooltip/__tests__/Tooltip.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/tooltip/__tests__/Tooltip.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/components/tooltip/styles.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/components/tooltip/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/constants/common.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/constants/common.ts`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,16 @@
         RoleArn: 'Role ARN',
         Image: 'Image',
         Kernel: 'Kernel',
         securityGroup: 'Security Group(s)',
         subnet: 'Subnet(s)',
         s3InputFolder: 'Input Folder',
         s3OutputFolder: 'Output Folder',
+        maxRetryAttempts: 'Max retry attempts',
+        maxRunTimeInSeconds: 'Max run time (in seconds)',
         selectAdditionalDepency: 'Select additional dependencies',
         efsPlaceholder: 'Enter EFS file path',
         efsLabel: 'Initialization script location (optional)',
         startUpScript: 'Start-up script',
         executionEnv: 'Execution enviroment',
         useVPC: 'Use a Virtual Private Cloud (VPC) to run this job',
         enableEncryption: 'Configure job encryption',
@@ -67,14 +69,16 @@
           SubnetsMaxError: 'Can only have maximum of 16 subnets.',
           SubnetLengthError: 'Subnet must be less than 32 characters.',
           SubnetsFormatError: 'One or more subnets has invalid format.',
           EnvironmentVariableEmptyError: 'Key or Value cannot be empty.',
           EnvironmentVariableLengthError: 'Key or Value cannot be more than 512 characters.',
           EnvironmentVariableFormatError: 'Key or Value has invalid format.',
           KMSKeyError: 'KMS key has invalid format.',
+          MaxRetryAttemptsError: 'Invalid max retry attempts must have a minimum value of 1 and a maximum value of 30.',
+          MaxRunTimeInSecondsError: 'Invalid max run time must have a minimum value of 1.',
         },
         VPCErrors: {
           RequiresPrivateSubnet: 'Running notebook jobs in a VPC requires the virtual network to use a private subnet.',
           NoPrivateSubnetsInSageMakerDomain:
             'There are no private subnets associated with your SageMaker Studio domain',
           YouMayChooseOtherSubnets:
             'You may choose to run the job using other private subnets associated with this VPC',
@@ -97,14 +101,16 @@
           'Enter the file path of a local script to run before the notebook execution.',
         EnvironmentVariablesTooltip: 'Enter key-value pairs that will be accessible in your notebook.',
         kmsKeyTooltip:
           'If you want Amazon SageMaker to encrypt the output of your notebook job using your own AWS KMS encryption key instead of the default S3 service key, provide its ID or ARN',
         ebsKeyTooltip:
           'Encrypt data on the storage volume attached to the compute instance that runs the scheduled job.',
         LearnMore: 'Learn more',
+        MaxRetryAttempts: 'Enter a minimum value of 1 and a maximum value of 30.',
+        MaxRunTimeInSeconds: 'Enter a minimum value of 1.',
       },
       StudioTooltips: {
         ImageTooltipText: 'Select available SageMaker image.',
         KernelTooltipText: 'Select available SageMaker Kernel.',
         RoleArnTooltip: 'Specify a role with permission to create a notebook job.',
         SecurityGroupsTooltip:
           'Specify or add security group(s) that have been created for the default VPC. For better security, we recommend that you use a private VPC.',
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/plugins/ScheduleNotebookDisablerPlugin.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/plugins/ScheduleNotebookDisablerPlugin.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/plugins/ScheduleNotebookPlugin.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/plugins/ScheduleNotebookPlugin.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/themeProvider.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/themeProvider.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/PluginEnvironmentProvider.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/PluginEnvironmentProvider.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/__tests__/PluginEnvironmentProvider.spec.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/__tests__/PluginEnvironmentProvider.spec.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/images.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/images.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/kernels.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/kernels.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/utils/rendering.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/utils/rendering.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJob.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJob.tsx`

 * *Files 6% similar despite different names*

```diff
@@ -54,26 +54,27 @@
   contentsManager,
   commands,
   jobsView,
   errors,
   handleErrorsChange,
   ...rest
 }) => {
+  const [apiError, setApiError] = useState<string>('');
   const fetchExecutionEnvironments = async () => {
     const url = URLExt.join(requestClient.baseUrl, '/advanced_environments');
     const response = await ServerConnection.makeRequest(url, {}, requestClient);
 
     if (response.status !== 200) {
       const responseJson = await response.json();
       const responseErrorCode = responseJson.error_code;
       const awsCredentialsErrors = Object.values(errorCodes.awsCredentials);
       if (awsCredentialsErrors.indexOf(responseErrorCode) >= 0) {
         showCredentialsErrorDialog(commands);
       }
-      return null;
+      throw new Error(response.statusText);
     } else {
       const executionEnvironmentsResponse = await response.json();
       return executionEnvironmentsResponse;
     }
   };
 
   useEffect(() => {
@@ -87,24 +88,30 @@
 
     if (jobsView === JobsView.CreateForm) {
       fetchExecutionEnvironments()
         .then(async (executionEnvironments: any) => {
           setEnvironmentsLoading(false);
           setExecutionEnvironments(executionEnvironments);
         })
-        .catch((error) => console.error(error));
+        .catch(error => {
+          setApiError(error.message);
+        });
     } else {
       setEnvironmentsLoading(false);
     }
   }, [jobsView, rest.model.inputFile]);
 
   const [executionEnvironments, setExecutionEnvironments] = useState<any>({});
 
   const [environmentsLoading, setEnvironmentsLoading] = useState<boolean>(true);
 
+  if (apiError) {
+    return <div className={Styles.ErrorMessageBlock}>{apiError}</div>
+  }
+
   const loading = environmentsLoading;
 
   if (loading) {
     return null;
   }
 
   if (jobsView === JobsView.CreateForm && !executionEnvironments?.auto_detected_config) {
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/AdvancedOptions.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/AdvancedOptions.tsx`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 import {
   validateRoleArn,
   validateS3Url,
   validateSecurityGroups,
   validateSubnets,
   validateKMS,
+  validateMaxRetryAttempts,
+  validateMaxRunTimeInSeconds,
 } from './validationHelpers';
 
 import * as Styles from '../../styles';
 import { usePluginEnvironment } from '../../../utils/PluginEnvironmentProvider';
 import Select from '@mui/material/Select';
 import MenuItem from '@mui/material/MenuItem';
 import InputLabel from '@mui/material/InputLabel';
@@ -51,14 +53,15 @@
   initialSecurityGroups: string[];
   userDefaultValues: FormState;
   setSubnets: (subnets: string[]) => void;
   setRoleArn: (roleArn: string) => void;
   setSecurityGroups: (securityGroups: string[]) => void;
   onSelectLCCScript: (event: string) => void;
   handleChange: (e: React.ChangeEvent<HTMLInputElement | HTMLTextAreaElement>) => void;
+  handleNumberValueChange: (e: React.ChangeEvent<HTMLInputElement | HTMLTextAreaElement>) => void;
   setFormValidationErrors: (errors: Scheduler.ErrorsType) => void;
   isVPCDomain: boolean;
   enableVPCSetting: boolean;
   setEnableVPCSetting: (checkBoxState: boolean) => void;
 }
 
 const kmsTooltipArea = (
@@ -92,14 +95,15 @@
   initialSecurityGroups,
   isVPCDomain,
   requestClient,
   enableVPCSetting,
   userDefaultValues,
   setFormState,
   handleChange,
+  handleNumberValueChange,
   setSubnets,
   setSecurityGroups,
   onSelectLCCScript,
   setFormValidationErrors,
   setEnableVPCSetting,
   setRoleArn,
 }) => {
@@ -157,14 +161,34 @@
 
     setFormValidationErrors({
       ...formErrors,
       [name === 's3_input' ? 's3InputFolderError' : 's3OutputFolderError']: errorMessage,
     });
   };
 
+  const handleMaxRetryAttemptsFieldOnBlur = (e: React.ChangeEvent<HTMLInputElement | HTMLTextAreaElement>) => {
+  		  
+    const errorMessage = validateMaxRetryAttempts(e.target.value);
+ 
+    setFormValidationErrors({
+      ...formErrors,
+      maxRetryAttemptsError: errorMessage,
+    });
+  };
+
+  const handleMaxRunTimeInSecondsFieldOnBlur = (e: React.ChangeEvent<HTMLInputElement | HTMLTextAreaElement>) => {
+  		  
+    const errorMessage = validateMaxRunTimeInSeconds(e.target.value);
+ 
+    setFormValidationErrors({
+      ...formErrors,
+      maxRunTimeInSecondsError: errorMessage,
+    });
+  };
+
   const handleKMSOnBlur = (e: React.ChangeEvent<HTMLInputElement | HTMLTextAreaElement>) => {
     const name = e.target.name;
     const errorMessage = validateKMS(e.target.value);
     setFormValidationErrors({
       ...formErrors,
       [name === 'sm_output_kms_key' ? 'outputKMSError' : 'ebsKMSError']: errorMessage,
     });
@@ -414,12 +438,43 @@
           errorMessage={formErrors.efsFilePathError}
           onChange={handleChange}
           onBlur={validateInitScript}
           toolTipText={!isDisabled ? ( pluginEnvironment.isStudio ? studioTooltipsStrings.InitialScriptTooltip : tooltipsStrings.InitialScriptTooltip) : undefined}
         />
         {/* {loading && <ActivityIndicator />} */}
       </div>
+
+      <InputContainer
+        name={'max_retry_attempts'}
+        type="number"
+        onChange={handleNumberValueChange}
+        required
+        disabled={loading}
+        readOnly={isDisabled}
+        value={formState.max_retry_attempts}
+        placeholder={widgetStrings.maxRetryAttempts}
+        labelInfo={widgetStrings.maxRetryAttempts}
+        errorMessage={formErrors.maxRetryAttemptsError}
+        onBlur={handleMaxRetryAttemptsFieldOnBlur}
+        toolTipText={tooltipsStrings.MaxRetryAttempts}
+      />
+
+      <InputContainer
+          name={'max_run_time_in_seconds'}
+          type="number"
+          onChange={handleNumberValueChange}
+          required
+          disabled={loading}
+          readOnly={isDisabled}
+          value={formState.max_run_time_in_seconds}
+          placeholder={widgetStrings.maxRunTimeInSeconds}
+          labelInfo={widgetStrings.maxRunTimeInSeconds}
+          errorMessage={formErrors.maxRunTimeInSecondsError}
+          onBlur={handleMaxRunTimeInSecondsFieldOnBlur}
+          toolTipText={tooltipsStrings.MaxRunTimeInSeconds}
+      />
+
     </div>
   );
 };
 
 export default AdvancedOptions;
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariable.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariable.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariables.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/EnvironmentVariables.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/styles.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/EnvironmentVariables/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/VpcCheckbox.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/VpcCheckbox/VpcCheckbox.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/AdvancedOptions/validationHelpers.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/AdvancedOptions/validationHelpers.ts`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 const securityGroupAndSubnetPattern = new RegExp('[-0-9a-zA-Z]+');
 const roleArnPattern = new RegExp('^arn:aws[a-z\\-]*:iam::\\d{12}:role/?[a-zA-Z_0-9+=,.@\\-_/]+$');
 const keyArnPattern = new RegExp('^arn:aws:kms:\\w+(?:-\\w+)+:\\d{12}:key\\/[A-Za-z0-9]+(?:-[A-Za-z0-9]+)+$');
 const keyIDPattern = new RegExp('^[0-9a-z]{8}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{4}-[0-9a-z]{12}$');
 
 const errorStrings = i18nStrings.ScheduleNoteBook.MainPanel.ErrorMessages;
 const vpcErrorStrings = errorStrings.VPCErrors;
+const maxRetryAttemptsMinValue = 0;
+const maxRetryAttemptsMaxValue = 30;
+const maxRunTimeMinValue = 0;
 
 export const validateImage = (image: string): string => {
   return image.length <= 0 ? errorStrings.AdvancedOptions.ImageError : '';
 }
 
 export const validateKernel = (kernel: string): string => {
   return kernel.length <= 0 ? errorStrings.AdvancedOptions.KernelError : '';
@@ -38,14 +41,30 @@
   if (!s3PathPattern.test(s3Path)) {
     return errorStrings.AdvancedOptions.S3FormatError;
   }
 
   return '';
 };
 
+export const validateMaxRetryAttempts = (maxRetryAttemptsString: string): string => {
+  const maxRetryAttempts = parseInt(maxRetryAttemptsString)
+  if (isNaN(maxRetryAttempts) || maxRetryAttempts < maxRetryAttemptsMinValue || maxRetryAttempts > maxRetryAttemptsMaxValue){
+    return errorStrings.AdvancedOptions.MaxRetryAttemptsError;
+  }
+  return '';
+};
+
+export const validateMaxRunTimeInSeconds = (maxRuntTimeInSecondsString: string): string => {
+  const maxRuntTimeInSeconds = parseInt(maxRuntTimeInSecondsString)
+  if (isNaN(maxRuntTimeInSeconds) || maxRuntTimeInSeconds < maxRunTimeMinValue){
+    return errorStrings.AdvancedOptions.MaxRunTimeInSecondsError;
+  }
+  return '';
+};
+
 export const validateSubnetOptions = (subnetOptions: string[]): string => {
   if (subnetOptions) {
     if (subnetOptions.length === 0) {
       return `${vpcErrorStrings.RequiresPrivateSubnet} ${vpcErrorStrings.NoPrivateSubnetsInSageMakerDomain}`
     }
   }
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/CreateNotebookJobform.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/CreateNotebookJobform.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
   getInitialS3Values,
   getInitialSubnetOrSecurityGroupValues,
   getNetworkAccessType,
   ISubnetSecurityGroupValues,
   getInitialKMSKeys,
   getAdvancedOptionsFromSettingRegistry,
   NO_SCRIPT,
+  getInitialKeyValue,
 } from './initialValueHelpers';
 import * as validationHelpers from './AdvancedOptions/validationHelpers';
 import { ContentsManager, ServerConnection } from '@jupyterlab/services';
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { JobEnvironmentContainer } from './JobEnvironment/JobEnvironmentContainer';
 import { IAutoDetectedConfig } from './JobEnvironment';
 
@@ -31,14 +32,16 @@
   vpc_subnets: string[];
   sm_kernel: string;
   sm_image: string;
   s3_input: string;
   s3_output: string;
   sm_output_kms_key: string;
   sm_volume_kms_key: string;
+  max_retry_attempts: number;
+  max_run_time_in_seconds: number;
 }
 
 export type CreateNotebookJobFormProps = Scheduler.IAdvancedOptionsProps & {
   requestClient: ServerConnection.ISettings;
   settingRegistry: ISettingRegistry;
   executionEnvironments: {
     environment_configs: IAutoDetectedConfig[] | null;
@@ -112,14 +115,32 @@
       model.runtimeEnvironmentParameters,
       executionEnvironments.auto_detected_config,
       jobsView,
       's3_input',
     );
   }, []);
 
+  const initialMaxRetryAttemtpsValue = useMemo(() => {
+    return getInitialKeyValue(
+      model.runtimeEnvironmentParameters,
+      jobsView,
+      1,
+      'max_retry_attempts',
+    );
+  }, []);
+
+  const initialMaxRunTimeInSecondsValue = useMemo(() => {
+    return getInitialKeyValue(
+      model.runtimeEnvironmentParameters,
+      jobsView,
+      172800,
+      'max_run_time_in_seconds',
+    );
+  }, []);
+
   const securityGroupOptions = useMemo(() => {
     const ALL_SECURITY_GROUPS =
       (executionEnvironments.auto_detected_config?.find((c) => c.name === 'vpc_security_group_ids')
         ?.value as ISubnetSecurityGroupValues) || [];
 
     return ALL_SECURITY_GROUPS?.map((item: { name: any }) => item.name);
   }, []);
@@ -203,14 +224,16 @@
     s3_input: initialS3InputValue || '',
     s3_output: initialS3OutputValue || '',
     sm_kernel: '',
     sm_image: '',
     sm_init_script: initialInitScriptValue || '',
     sm_output_kms_key: initialOutputKMSKey || '',
     sm_volume_kms_key: initialVolumeKMSKey || '',
+    max_retry_attempts: initialMaxRetryAttemtpsValue,
+    max_run_time_in_seconds: initialMaxRunTimeInSecondsValue,
   });
 
   // initially output and volume kms keys should be empty even if we have the initial values coming from the user defaults,
   // because initially the kms encryption is disabled. When the kms encryption gets enabled the user default values will get picked up.
   const [formState, setFormState] = useState<FormState>({
     ...userDefaultValues,
     sm_output_kms_key: '',
@@ -333,14 +356,20 @@
 
   const handleChange = (e: React.ChangeEvent<HTMLInputElement | HTMLTextAreaElement>) => {
     const name = e.target.name;
     const value = e.target.value;
     setFormState({ ...formState, [name]: value });
   };
 
+  const handleNumberValueChange = (e: React.ChangeEvent<HTMLInputElement | HTMLTextAreaElement>) => {
+    const name = e.target.name;
+    const value = parseInt(e.target.value);
+    setFormState({ ...formState, [name]: isNaN(value) ? '' : value });
+  };
+
   const onSelectLCCScript = (startupScript: string) => {
     setFormState({
       ...formState,
       sm_lcc_init_script_arn: startupScript
     });
   };
 
@@ -372,14 +401,15 @@
         {...props} />
 
       <AdvancedOptions
         isDisabled={areFieldsDisabled}
         formState={formState}
         setFormState={setFormState}
         handleChange={handleChange}
+        handleNumberValueChange={handleNumberValueChange}
         requestClient={requestClient}
         formErrors={formErrors}
         setFormValidationErrors={setFormErrors}
         environmentVariables={environmentVariables}
         userDefaultValues={userDefaultValues}
         setEnvironmentVariables={setEnvironmentVariables}
         lccOptions={initialLccValues.allLCCOptions}
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/InputContainer.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/InputContainer.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/JobEnvironment/DefaultJobEnvironment.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/JobEnvironment/DefaultJobEnvironment.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/JobEnvironment/JobEnvironmentContainer.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/JobEnvironment/JobEnvironmentContainer.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/JobEnvironment/jobEnvironment.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/JobEnvironment/jobEnvironment.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/MultiSelectContainer.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/MultiSelectContainer.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/SelectInputContainer.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/SelectInputContainer.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/StudioImageSelectorOption.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/StudioImageSelectorOption.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/StudioJobEnvironment.tsx` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/StudioJobEnvironment.tsx`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioApi.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioApi.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioHelpers.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioHelpers.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioMock.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioMock.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioModel.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioModel.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/Studio/studioStyles.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/Studio/studioStyles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/initialValueHelpers.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/initialValueHelpers.ts`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,16 @@
   'vpc_security_group_ids',
   'vpc_subnets',
   's3_input',
   's3_output',
   'sm_init_script',
   'sm_output_kms_key',
   'sm_volume_kms_key',
+  'max_run_time_in_seconds',
+  'max_retry_attempts',
 ]);
 
 const SETTING_REGISTRY_PLUGIN = '@amzn/sagemaker-jupyter-scheduler:advanced-options';
 const SETTING_REGISTRY_ADVANCED_OPTIONS_KEY = 'advancedOptions';
 
 export interface ISubnetSecurityGroupShape {
   name: string;
@@ -176,14 +178,33 @@
 
     return autoDetectedConfig?.find((c) => c.name === key)?.value || '';
   }
 
   return '';
 };
 
+export const getInitialKeyValue = (
+  runtimeEnvironmentParameters: RuntimeEnvParams,
+  view: JobsView,
+  defaultValue: number,
+  key: 'max_retry_attempts' | 'max_run_time_in_seconds',
+): number => {
+  if (view === JobsView.JobDetail || view === JobsView.JobDefinitionDetail) {
+    if (runtimeEnvironmentParameters) {
+      return runtimeEnvironmentParameters[key] as number;
+    }
+  } else if (view === JobsView.CreateForm) {
+    if (runtimeEnvironmentParameters && key in runtimeEnvironmentParameters) {
+      return runtimeEnvironmentParameters[key] as number;
+    }
+  }
+
+  return defaultValue;
+};
+
 export const getInitialKMSKeys = (
   runtimeEnvironmentParameters: RuntimeEnvParams,
   view: JobsView,
   key: 'sm_output_kms_key' | 'sm_volume_kms_key',
 ): string => {
   if (view === JobsView.JobDetail || view === JobsView.JobDefinitionDetail) {
     if (runtimeEnvironmentParameters) {
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/CreateNotebookJobForm/styles.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/CreateNotebookJobForm/styles.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/mockResponses.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/mockResponses.ts`

 * *Files identical despite different names*

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/src/widgets/styles.ts` & `amazon_sagemaker_jupyter_scheduler-2.1.0/src/widgets/styles.ts`

 * *Files 2% similar despite different names*

```diff
@@ -130,7 +130,12 @@
 `;
 
 export const AdvancedOptionsSelectContainer = css`
   display: flex;
   flex-direction: column;
   gap: var(--jp-ui-font-size1);
 `;
+
+export const ErrorMessageBlock = css`
+  color: var(--jp-error-color1);
+  padding: 12px;
+`;
```

### Comparing `amazon_sagemaker_jupyter_scheduler-2.0.2/tsconfig.base.json` & `amazon_sagemaker_jupyter_scheduler-2.1.0/tsconfig.base.json`

 * *Files identical despite different names*

