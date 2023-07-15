# Comparing `tmp/skypilot-nightly-1.0.0.dev20230713.tar.gz` & `tmp/skypilot-nightly-1.0.0.dev20230714.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot-nightly-1.0.0.dev20230713.tar", last modified: Thu Jul 13 16:17:35 2023, max compression
+gzip compressed data, was "skypilot-nightly-1.0.0.dev20230714.tar", last modified: Fri Jul 14 10:42:07 2023, max compression
```

## Comparing `skypilot-nightly-1.0.0.dev20230713.tar` & `skypilot-nightly-1.0.0.dev20230714.tar`

### file list

```diff
@@ -1,223 +1,223 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.560316 skypilot-nightly-1.0.0.dev20230713/
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-13 16:17:35.556316 skypilot-nightly-1.0.0.dev20230713/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 16:17:35.560316 skypilot-nightly-1.0.0.dev20230713/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-13 16:17:27.000000 skypilot-nightly-1.0.0.dev20230713/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.536315 skypilot-nightly-1.0.0.dev20230713/sky/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-13 16:17:27.000000 skypilot-nightly-1.0.0.dev20230713/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.536315 skypilot-nightly-1.0.0.dev20230713/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.536315 skypilot-nightly-1.0.0.dev20230713/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)   112593 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   201662 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.536315 skypilot-nightly-1.0.0.dev20230713/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/backends/onprem_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.540315 skypilot-nightly-1.0.0.dev20230713/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (123)   167453 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.540315 skypilot-nightly-1.0.0.dev20230713/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41085 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    25564 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    24158 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    42911 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    24297 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.540315 skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    22995 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.540315 skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    18601 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    19812 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.544315 skypilot-nightly-1.0.0.dev20230713/sky/data/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    89247 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    41325 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    45228 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.544315 skypilot-nightly-1.0.0.dev20230713/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.544315 skypilot-nightly-1.0.0.dev20230713/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/provision/aws/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    45043 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.544315 skypilot-nightly-1.0.0.dev20230713/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-13 16:17:27.000000 skypilot-nightly-1.0.0.dev20230713/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.544315 skypilot-nightly-1.0.0.dev20230713/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/log_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.532315 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.544315 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.544315 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/aws/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/aws/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    52192 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/aws/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.548315 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/azure/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.548315 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/gcp/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/gcp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.548315 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.548315 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/lambda_cloud/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.548315 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/oci/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.548315 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/scp/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/scp/scp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.552316 skypilot-nightly-1.0.0.dev20230713/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/ray_patches/job_head.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/skypilot_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.552316 skypilot-nightly-1.0.0.dev20230713/sky/spot/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/spot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/spot/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.552316 skypilot-nightly-1.0.0.dev20230713/sky/spot/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/spot/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.552316 skypilot-nightly-1.0.0.dev20230713/sky/spot/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/spot/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.552316 skypilot-nightly-1.0.0.dev20230713/sky/spot/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/spot/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    21256 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/spot/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/spot/spot_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/spot/spot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.552316 skypilot-nightly-1.0.0.dev20230713/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/templates/gcp-tpu-create.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/templates/gcp-tpu-delete.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/templates/spot-controller.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.552316 skypilot-nightly-1.0.0.dev20230713/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.556316 skypilot-nightly-1.0.0.dev20230713/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.556316 skypilot-nightly-1.0.0.dev20230713/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/utils/env_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/utils/tpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.556316 skypilot-nightly-1.0.0.dev20230713/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-13 16:17:35.000000 skypilot-nightly-1.0.0.dev20230713/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-07-13 16:17:35.000000 skypilot-nightly-1.0.0.dev20230713/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 16:17:35.000000 skypilot-nightly-1.0.0.dev20230713/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-13 16:17:35.000000 skypilot-nightly-1.0.0.dev20230713/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-13 16:17:35.000000 skypilot-nightly-1.0.0.dev20230713/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-13 16:17:35.000000 skypilot-nightly-1.0.0.dev20230713/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 16:17:35.556316 skypilot-nightly-1.0.0.dev20230713/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/tests/test_onprem.py
--rw-r--r--   0 runner    (1001) docker     (123)    20799 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/tests/test_pycryptodome_version.py
--rw-r--r--   0 runner    (1001) docker     (123)   123678 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/tests/test_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-13 16:17:25.000000 skypilot-nightly-1.0.0.dev20230713/tests/test_wheels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.746555 skypilot-nightly-1.0.0.dev20230714/
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-14 10:42:07.746555 skypilot-nightly-1.0.0.dev20230714/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:42:07.746555 skypilot-nightly-1.0.0.dev20230714/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-14 10:41:58.000000 skypilot-nightly-1.0.0.dev20230714/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.718555 skypilot-nightly-1.0.0.dev20230714/sky/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-14 10:41:58.000000 skypilot-nightly-1.0.0.dev20230714/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.722555 skypilot-nightly-1.0.0.dev20230714/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.722555 skypilot-nightly-1.0.0.dev20230714/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112593 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   201662 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.722555 skypilot-nightly-1.0.0.dev20230714/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/backends/onprem_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.722555 skypilot-nightly-1.0.0.dev20230714/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167453 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.726555 skypilot-nightly-1.0.0.dev20230714/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41085 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25564 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24158 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42911 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24297 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.726555 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22995 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.726555 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18601 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19812 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.730555 skypilot-nightly-1.0.0.dev20230714/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89247 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41325 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45228 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.730555 skypilot-nightly-1.0.0.dev20230714/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.730555 skypilot-nightly-1.0.0.dev20230714/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/provision/aws/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45043 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.730555 skypilot-nightly-1.0.0.dev20230714/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7977 2023-07-14 10:41:58.000000 skypilot-nightly-1.0.0.dev20230714/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.730555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/log_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.714555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.730555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.730555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52192 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.734555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.734555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.734555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.734555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/lambda_cloud/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.734555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/oci/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.734555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/scp/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/scp/scp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.738555 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/job_head.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/skypilot_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.738555 skypilot-nightly-1.0.0.dev20230714/sky/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/spot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/spot/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.738555 skypilot-nightly-1.0.0.dev20230714/sky/spot/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/spot/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.738555 skypilot-nightly-1.0.0.dev20230714/sky/spot/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/spot/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.738555 skypilot-nightly-1.0.0.dev20230714/sky/spot/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/spot/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21256 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/spot/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/spot/spot_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/spot/spot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.738555 skypilot-nightly-1.0.0.dev20230714/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/gcp-tpu-create.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/gcp-tpu-delete.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/templates/spot-controller.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.742555 skypilot-nightly-1.0.0.dev20230714/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.742555 skypilot-nightly-1.0.0.dev20230714/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.742555 skypilot-nightly-1.0.0.dev20230714/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/env_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/tpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.742555 skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-14 10:42:07.000000 skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-07-14 10:42:07.000000 skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:42:07.000000 skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-14 10:42:07.000000 skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-14 10:42:07.000000 skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-14 10:42:07.000000 skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:42:07.746555 skypilot-nightly-1.0.0.dev20230714/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_onprem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20799 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_pycryptodome_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   123678 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 10:41:52.000000 skypilot-nightly-1.0.0.dev20230714/tests/test_wheels.py
```

### Comparing `skypilot-nightly-1.0.0.dev20230713/LICENSE` & `skypilot-nightly-1.0.0.dev20230714/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230714/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230714/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230713
+Version: 1.0.0.dev20230714
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230713
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230714
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230713/README.md` & `skypilot-nightly-1.0.0.dev20230714/README.md`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/pyproject.toml` & `skypilot-nightly-1.0.0.dev20230714/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/setup.py` & `skypilot-nightly-1.0.0.dev20230714/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/__init__.py` & `skypilot-nightly-1.0.0.dev20230714/sky/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The SkyPilot package."""
 import os
 
 # Replaced with the current commit when building the wheels.
-__commit__ = '5864399925058b0ffdd68d4c9319bd2ea3610912'
-__version__ = '1.0.0-dev20230713'
+__commit__ = 'f35f65d802f575c7e12b7573196b66ac1ced3a38'
+__version__ = '1.0.0-dev20230714'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 # Keep this order to avoid cyclic imports
 from sky import backends
 from sky import benchmark
 from sky import clouds
 from sky.clouds.service_catalog import list_accelerators
```

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/adaptors/aws.py` & `skypilot-nightly-1.0.0.dev20230714/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/adaptors/azure.py` & `skypilot-nightly-1.0.0.dev20230714/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/adaptors/cloudflare.py` & `skypilot-nightly-1.0.0.dev20230714/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/adaptors/docker.py` & `skypilot-nightly-1.0.0.dev20230714/sky/adaptors/docker.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/adaptors/gcp.py` & `skypilot-nightly-1.0.0.dev20230714/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/adaptors/ibm.py` & `skypilot-nightly-1.0.0.dev20230714/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/adaptors/oci.py` & `skypilot-nightly-1.0.0.dev20230714/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/authentication.py` & `skypilot-nightly-1.0.0.dev20230714/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/backends/backend.py` & `skypilot-nightly-1.0.0.dev20230714/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/backends/backend_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/backends/backend_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/backends/cloud_vm_ray_backend.py` & `skypilot-nightly-1.0.0.dev20230714/sky/backends/cloud_vm_ray_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/backends/docker_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/backends/local_docker_backend.py` & `skypilot-nightly-1.0.0.dev20230714/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot-nightly-1.0.0.dev20230714/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/backends/onprem_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/backends/onprem_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/backends/wheel_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/benchmark/benchmark_state.py` & `skypilot-nightly-1.0.0.dev20230714/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/benchmark/benchmark_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/check.py` & `skypilot-nightly-1.0.0.dev20230714/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/cli.py` & `skypilot-nightly-1.0.0.dev20230714/sky/cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/cloud_stores.py` & `skypilot-nightly-1.0.0.dev20230714/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/__init__.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/aws.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/azure.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/cloud.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/gcp.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/ibm.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/local.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/local.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/oci.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/scp.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/scp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/__init__.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/aws_catalog.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/azure_catalog.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/common.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/config.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/oci_catalog.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/clouds/service_catalog/scp_catalog.py` & `skypilot-nightly-1.0.0.dev20230714/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/core.py` & `skypilot-nightly-1.0.0.dev20230714/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/dag.py` & `skypilot-nightly-1.0.0.dev20230714/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/data/data_transfer.py` & `skypilot-nightly-1.0.0.dev20230714/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/data/data_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/data/mounting_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/data/storage.py` & `skypilot-nightly-1.0.0.dev20230714/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/data/storage_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/exceptions.py` & `skypilot-nightly-1.0.0.dev20230714/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/execution.py` & `skypilot-nightly-1.0.0.dev20230714/sky/execution.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/global_user_state.py` & `skypilot-nightly-1.0.0.dev20230714/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/optimizer.py` & `skypilot-nightly-1.0.0.dev20230714/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/provision/__init__.py` & `skypilot-nightly-1.0.0.dev20230714/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/provision/aws/instance.py` & `skypilot-nightly-1.0.0.dev20230714/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/resources.py` & `skypilot-nightly-1.0.0.dev20230714/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/setup_files/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230714/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/setup_files/setup.py` & `skypilot-nightly-1.0.0.dev20230714/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/sky_logging.py` & `skypilot-nightly-1.0.0.dev20230714/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/LICENSE` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/attempt_skylet.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/autostop_lib.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/configs.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/constants.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/events.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/job_lib.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/log_lib.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/aws/config.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/aws/node_provider.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/aws/utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/azure/azure-config-template.json` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/azure/config.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/azure/node_provider.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/gcp/config.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/gcp/constants.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/gcp/node.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/node.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/gcp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/gcp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/ibm/node_provider.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/ibm/utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/lambda_cloud/lambda_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/lambda_cloud/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/oci/config.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/oci/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/oci/node_provider.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/oci/query_helper.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/scp/config.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/scp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/providers/scp/scp_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/providers/scp/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/ray_patches/__init__.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/ray_patches/worker.py.patch` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/skylet.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skylet/subprocess_daemon.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/skypilot_config.py` & `skypilot-nightly-1.0.0.dev20230714/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/spot/__init__.py` & `skypilot-nightly-1.0.0.dev20230714/sky/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/spot/constants.py` & `skypilot-nightly-1.0.0.dev20230714/sky/spot/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/spot/controller.py` & `skypilot-nightly-1.0.0.dev20230714/sky/spot/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/spot/dashboard/dashboard.py` & `skypilot-nightly-1.0.0.dev20230714/sky/spot/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/spot/dashboard/static/favicon.ico` & `skypilot-nightly-1.0.0.dev20230714/sky/spot/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/spot/dashboard/templates/index.html` & `skypilot-nightly-1.0.0.dev20230714/sky/spot/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/spot/recovery_strategy.py` & `skypilot-nightly-1.0.0.dev20230714/sky/spot/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/spot/spot_state.py` & `skypilot-nightly-1.0.0.dev20230714/sky/spot/spot_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/spot/spot_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/spot/spot_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/status_lib.py` & `skypilot-nightly-1.0.0.dev20230714/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/task.py` & `skypilot-nightly-1.0.0.dev20230714/sky/task.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/templates/aws-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230714/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/templates/azure-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230714/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/templates/gcp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230714/sky/templates/gcp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/templates/ibm-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230714/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/templates/lambda-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230714/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/templates/local-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230714/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/templates/oci-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230714/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/templates/scp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230714/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/templates/spot-controller.yaml.j2` & `skypilot-nightly-1.0.0.dev20230714/sky/templates/spot-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/usage/constants.py` & `skypilot-nightly-1.0.0.dev20230714/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/usage/usage_lib.py` & `skypilot-nightly-1.0.0.dev20230714/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/utils/accelerator_registry.py` & `skypilot-nightly-1.0.0.dev20230714/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/utils/cli_utils/status_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/utils/command_runner.py` & `skypilot-nightly-1.0.0.dev20230714/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/utils/common_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/utils/dag_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/utils/db_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/utils/env_options.py` & `skypilot-nightly-1.0.0.dev20230714/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/utils/log_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/utils/schemas.py` & `skypilot-nightly-1.0.0.dev20230714/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/utils/subprocess_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/utils/timeline.py` & `skypilot-nightly-1.0.0.dev20230714/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/utils/tpu_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/utils/tpu_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/utils/ux_utils.py` & `skypilot-nightly-1.0.0.dev20230714/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/sky/utils/validator.py` & `skypilot-nightly-1.0.0.dev20230714/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/skypilot_nightly.egg-info/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230713
+Version: 1.0.0.dev20230714
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230713
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230714
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230713/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/skypilot_nightly.egg-info/requires.txt` & `skypilot-nightly-1.0.0.dev20230714/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/tests/test_cli.py` & `skypilot-nightly-1.0.0.dev20230714/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/tests/test_config.py` & `skypilot-nightly-1.0.0.dev20230714/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/tests/test_list_accelerators.py` & `skypilot-nightly-1.0.0.dev20230714/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/tests/test_onprem.py` & `skypilot-nightly-1.0.0.dev20230714/tests/test_onprem.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/tests/test_optimizer_dryruns.py` & `skypilot-nightly-1.0.0.dev20230714/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/tests/test_optimizer_random_dag.py` & `skypilot-nightly-1.0.0.dev20230714/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/tests/test_smoke.py` & `skypilot-nightly-1.0.0.dev20230714/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/tests/test_spot.py` & `skypilot-nightly-1.0.0.dev20230714/tests/test_spot.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/tests/test_storage.py` & `skypilot-nightly-1.0.0.dev20230714/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230713/tests/test_wheels.py` & `skypilot-nightly-1.0.0.dev20230714/tests/test_wheels.py`

 * *Files identical despite different names*

