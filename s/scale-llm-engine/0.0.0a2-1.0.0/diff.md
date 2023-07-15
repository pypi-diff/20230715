# Comparing `tmp/scale_llm_engine-0.0.0a2.tar.gz` & `tmp/scale-llm-engine-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_llm_engine-0.0.0a2.tar", max compression
+gzip compressed data, was "/Users/yixu/projects/llm-engine/dist/.tmp-vr6ch88r/scale-llm-engine-1.0.0.tar", last modified: Sat Jul 15 01:50:08 2023, max compression
```

## Comparing `scale_llm_engine-0.0.0a2.tar` & `scale-llm-engine-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,252 @@
--rw-r--r--   0        0        0     1023 2023-07-15 04:30:27.117123 scale_llm_engine-0.0.0a2/README.md
--rw-r--r--   0        0        0     1060 2023-07-15 04:30:27.118047 scale_llm_engine-0.0.0a2/llmengine/__init__.py
--rw-r--r--   0        0        0     5614 2023-07-15 04:30:27.118543 scale_llm_engine-0.0.0a2/llmengine/api_engine.py
--rw-r--r--   0        0        0    17831 2023-07-15 04:30:27.119127 scale_llm_engine-0.0.0a2/llmengine/client.py
--rw-r--r--   0        0        0     7962 2023-07-15 04:30:27.119749 scale_llm_engine-0.0.0a2/llmengine/completion.py
--rw-r--r--   0        0        0     8169 2023-07-15 04:30:27.119988 scale_llm_engine-0.0.0a2/llmengine/data_types.py
--rw-r--r--   0        0        0     1533 2023-07-15 04:30:27.120141 scale_llm_engine-0.0.0a2/llmengine/errors.py
--rw-r--r--   0        0        0     4238 2023-07-15 04:30:27.120624 scale_llm_engine-0.0.0a2/llmengine/fine_tuning.py
--rw-r--r--   0        0        0     2069 2023-07-15 04:30:27.120996 scale_llm_engine-0.0.0a2/llmengine/model.py
--rw-r--r--   0        0        0     8026 2023-07-15 04:30:27.121202 scale_llm_engine-0.0.0a2/llmengine/types.py
--rw-r--r--   0        0        0      808 2023-07-15 04:34:29.613024 scale_llm_engine-0.0.0a2/pyproject.toml
--rw-r--r--   0        0        0     1920 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0a2/PKG-INFO
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.565219 scale-llm-engine-1.0.0/
+-rw-r--r--   0 yixu       (502) staff       (20)      554 2023-07-15 00:37:13.000000 scale-llm-engine-1.0.0/LICENSE
+-rw-r--r--   0 yixu       (502) staff       (20)       82 2023-07-15 01:50:08.565400 scale-llm-engine-1.0.0/PKG-INFO
+-rw-r--r--   0 yixu       (502) staff       (20)     1925 2023-07-15 00:37:13.000000 scale-llm-engine-1.0.0/README.md
+-rw-r--r--   0 yixu       (502) staff       (20)      101 2023-07-15 00:37:13.000000 scale-llm-engine-1.0.0/pyproject.toml
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.472773 scale-llm-engine-1.0.0/scale_llm_engine.egg-info/
+-rw-r--r--   0 yixu       (502) staff       (20)       82 2023-07-15 01:50:08.000000 scale-llm-engine-1.0.0/scale_llm_engine.egg-info/PKG-INFO
+-rw-r--r--   0 yixu       (502) staff       (20)    10691 2023-07-15 01:50:08.000000 scale-llm-engine-1.0.0/scale_llm_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 yixu       (502) staff       (20)        1 2023-07-15 01:50:08.000000 scale-llm-engine-1.0.0/scale_llm_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 yixu       (502) staff       (20)      493 2023-07-15 01:50:08.000000 scale-llm-engine-1.0.0/scale_llm_engine.egg-info/entry_points.txt
+-rw-r--r--   0 yixu       (502) staff       (20)       16 2023-07-15 01:50:08.000000 scale-llm-engine-1.0.0/scale_llm_engine.egg-info/top_level.txt
+-rw-r--r--   0 yixu       (502) staff       (20)      332 2023-07-15 01:50:08.566419 scale-llm-engine-1.0.0/setup.cfg
+-rw-r--r--   0 yixu       (502) staff       (20)      837 2023-07-15 01:49:52.000000 scale-llm-engine-1.0.0/setup.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.473079 scale-llm-engine-1.0.0/spellbook_serve/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/__init__.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.477998 scale-llm-engine-1.0.0/spellbook_serve/api/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/api/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1487 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/api/app.py
+-rw-r--r--   0 yixu       (502) staff       (20)     8267 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/api/batch_jobs_v1.py
+-rw-r--r--   0 yixu       (502) staff       (20)    10411 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/api/dependencies.py
+-rw-r--r--   0 yixu       (502) staff       (20)     5852 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/api/docker_image_batch_job_bundles_v1.py
+-rw-r--r--   0 yixu       (502) staff       (20)    10914 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/api/llms_v1.py
+-rw-r--r--   0 yixu       (502) staff       (20)     6602 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/api/model_bundles_v1.py
+-rw-r--r--   0 yixu       (502) staff       (20)     6602 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/api/model_bundles_v2.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1854 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/api/model_endpoints_docs_v1.py
+-rw-r--r--   0 yixu       (502) staff       (20)     8690 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/api/model_endpoints_v1.py
+-rw-r--r--   0 yixu       (502) staff       (20)     6701 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/api/tasks_v1.py
+-rw-r--r--   0 yixu       (502) staff       (20)      538 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/api/worker.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.482970 scale-llm-engine-1.0.0/spellbook_serve/common/
+-rw-r--r--   0 yixu       (502) staff       (20)      125 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1453 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/config.py
+-rw-r--r--   0 yixu       (502) staff       (20)      567 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/constants.py
+-rw-r--r--   0 yixu       (502) staff       (20)      375 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/datadog_utils.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.486545 scale-llm-engine-1.0.0/spellbook_serve/common/dtos/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/dtos/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     5139 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/dtos/batch_jobs.py
+-rw-r--r--   0 yixu       (502) staff       (20)      460 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/dtos/docker_repository.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1145 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/dtos/endpoint_builder.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2616 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/dtos/llms.py
+-rw-r--r--   0 yixu       (502) staff       (20)     3572 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/dtos/model_bundles.py
+-rw-r--r--   0 yixu       (502) staff       (20)     4566 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/dtos/model_endpoints.py
+-rw-r--r--   0 yixu       (502) staff       (20)      225 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/dtos/resource_manager.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1088 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/dtos/tasks.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1979 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/env_vars.py
+-rw-r--r--   0 yixu       (502) staff       (20)      213 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/errors.py
+-rw-r--r--   0 yixu       (502) staff       (20)      460 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/io.py
+-rw-r--r--   0 yixu       (502) staff       (20)     3819 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/resource_limits.py
+-rw-r--r--   0 yixu       (502) staff       (20)      909 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/serialization_utils.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2338 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/service_requests.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1941 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/settings.py
+-rw-r--r--   0 yixu       (502) staff       (20)     4113 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/common/types.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.490418 scale-llm-engine-1.0.0/spellbook_serve/core/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/__init__.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.492145 scale-llm-engine-1.0.0/spellbook_serve/core/auth/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/auth/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1217 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/auth/authentication_repository.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1147 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/auth/fake_authentication_repository.py
+-rw-r--r--   0 yixu       (502) staff       (20)      799 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/auth/known_users.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.494050 scale-llm-engine-1.0.0/spellbook_serve/core/aws/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/aws/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     8844 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/aws/roles.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1078 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/aws/secrets.py
+-rw-r--r--   0 yixu       (502) staff       (20)      793 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/aws/sfn_client.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2801 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/aws/storage_client.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.495270 scale-llm-engine-1.0.0/spellbook_serve/core/celery/
+-rw-r--r--   0 yixu       (502) staff       (20)      143 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/celery/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)    26939 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/celery/app.py
+-rw-r--r--   0 yixu       (502) staff       (20)     3877 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/celery/s3.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2610 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/config.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.496699 scale-llm-engine-1.0.0/spellbook_serve/core/docker/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/docker/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     6586 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/docker/docker_image.py
+-rw-r--r--   0 yixu       (502) staff       (20)     3297 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/docker/ecr.py
+-rw-r--r--   0 yixu       (502) staff       (20)    20348 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/docker/remote_build.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1384 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/domain_exceptions.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1017 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/fake_notification_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2503 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/kubernetes.py
+-rw-r--r--   0 yixu       (502) staff       (20)    12103 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/loggers.py
+-rw-r--r--   0 yixu       (502) staff       (20)      903 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/notification_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     4728 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/testing_utilities.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.498862 scale-llm-engine-1.0.0/spellbook_serve/core/utils/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/utils/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     5451 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/utils/env.py
+-rw-r--r--   0 yixu       (502) staff       (20)     3250 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/utils/format.py
+-rw-r--r--   0 yixu       (502) staff       (20)      105 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/utils/git.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1875 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/utils/python_utils.py
+-rw-r--r--   0 yixu       (502) staff       (20)     5095 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/utils/timer.py
+-rw-r--r--   0 yixu       (502) staff       (20)     3736 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/core/utils/url.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.500653 scale-llm-engine-1.0.0/spellbook_serve/db/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/db/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     4951 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/db/base.py
+-rw-r--r--   0 yixu       (502) staff       (20)     5679 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/db/endpoint_row_lock.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1723 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/db/local_setup.py
+-rw-r--r--   0 yixu       (502) staff       (20)      421 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/db/ml_infra_pg.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.502719 scale-llm-engine-1.0.0/spellbook_serve/db/models/
+-rw-r--r--   0 yixu       (502) staff       (20)      329 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/db/models/__init__.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.503639 scale-llm-engine-1.0.0/spellbook_serve/db/models/common/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/db/models/common/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)      379 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/db/models/common/query.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2411 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/db/models/common/record.py
+-rw-r--r--   0 yixu       (502) staff       (20)       82 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/db/models/constants.py
+-rw-r--r--   0 yixu       (502) staff       (20)      221 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/db/models/exceptions.py
+-rw-r--r--   0 yixu       (502) staff       (20)    11565 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/db/models/model.py
+-rw-r--r--   0 yixu       (502) staff       (20)    34786 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/db/models/spellbook_serve.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.504473 scale-llm-engine-1.0.0/spellbook_serve/db/models/utils/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/db/models/utils/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)      106 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/db/models/utils/misc.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.505251 scale-llm-engine-1.0.0/spellbook_serve/domain/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/__init__.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.505864 scale-llm-engine-1.0.0/spellbook_serve/domain/authorization/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/authorization/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2977 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/authorization/scale_authorization_module.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.509710 scale-llm-engine-1.0.0/spellbook_serve/domain/entities/
+-rw-r--r--   0 yixu       (502) staff       (20)     2357 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/entities/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1587 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/entities/batch_job_entity.py
+-rw-r--r--   0 yixu       (502) staff       (20)      169 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/entities/common_types.py
+-rw-r--r--   0 yixu       (502) staff       (20)      623 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/entities/docker_image_batch_job_bundle_entity.py
+-rw-r--r--   0 yixu       (502) staff       (20)      228 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/entities/gpu_type.py
+-rw-r--r--   0 yixu       (502) staff       (20)      370 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/entities/llm_entity.py
+-rw-r--r--   0 yixu       (502) staff       (20)     7646 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/entities/model_bundle_entity.py
+-rw-r--r--   0 yixu       (502) staff       (20)     4506 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/entities/model_endpoint_entity.py
+-rw-r--r--   0 yixu       (502) staff       (20)      200 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/entities/owned_entity.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2018 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/exceptions.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.513796 scale-llm-engine-1.0.0/spellbook_serve/domain/gateways/
+-rw-r--r--   0 yixu       (502) staff       (20)      583 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/gateways/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1088 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/gateways/async_model_endpoint_inference_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2396 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/gateways/docker_image_batch_job_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)      652 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/gateways/model_endpoints_schema_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)      976 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/gateways/model_primitive_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1008 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/gateways/monitoring_metrics_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)      976 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/gateways/streaming_model_endpoint_inference_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)      909 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/gateways/sync_model_endpoint_inference_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1226 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/gateways/task_queue_gateway.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.515519 scale-llm-engine-1.0.0/spellbook_serve/domain/repositories/
+-rw-r--r--   0 yixu       (502) staff       (20)      352 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/repositories/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     3264 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/repositories/docker_image_batch_job_bundle_repository.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1465 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/repositories/docker_repository.py
+-rw-r--r--   0 yixu       (502) staff       (20)     3156 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/repositories/model_bundle_repository.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.517560 scale-llm-engine-1.0.0/spellbook_serve/domain/services/
+-rw-r--r--   0 yixu       (502) staff       (20)      400 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/services/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2154 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/services/batch_job_service.py
+-rw-r--r--   0 yixu       (502) staff       (20)      575 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/services/endpoint_builder_service.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1295 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/services/llm_model_endpoint_service.py
+-rw-r--r--   0 yixu       (502) staff       (20)    10248 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/services/model_endpoint_service.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.522089 scale-llm-engine-1.0.0/spellbook_serve/domain/use_cases/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/use_cases/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     3870 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/use_cases/async_inference_use_cases.py
+-rw-r--r--   0 yixu       (502) staff       (20)    12426 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/use_cases/batch_job_use_cases.py
+-rw-r--r--   0 yixu       (502) staff       (20)     5296 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/use_cases/docker_image_batch_job_bundle_use_cases.py
+-rw-r--r--   0 yixu       (502) staff       (20)    20759 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/use_cases/llm_model_endpoint_use_cases.py
+-rw-r--r--   0 yixu       (502) staff       (20)    23574 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/use_cases/model_bundle_use_cases.py
+-rw-r--r--   0 yixu       (502) staff       (20)    19516 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/use_cases/model_endpoint_use_cases.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1113 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/use_cases/model_endpoints_schema_use_cases.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2615 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/use_cases/streaming_inference_use_cases.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2776 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/domain/use_cases/sync_inference_use_cases.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.525455 scale-llm-engine-1.0.0/spellbook_serve/entrypoints/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/entrypoints/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1630 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/entrypoints/init_database.py
+-rw-r--r--   0 yixu       (502) staff       (20)     7791 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/entrypoints/init_spellbook_models.py
+-rw-r--r--   0 yixu       (502) staff       (20)     5673 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/entrypoints/k8s_cache.py
+-rw-r--r--   0 yixu       (502) staff       (20)     5950 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/entrypoints/start_batch_job_orchestration.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2141 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/entrypoints/start_docker_image_batch_job_init_container.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1328 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/entrypoints/start_fastapi_server.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.527979 scale-llm-engine-1.0.0/spellbook_serve/inference/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/inference/__init__.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.529270 scale-llm-engine-1.0.0/spellbook_serve/inference/async_inference/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/inference/async_inference/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1251 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/inference/async_inference/celery.py
+-rw-r--r--   0 yixu       (502) staff       (20)     3894 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/inference/async_inference/tasks.py
+-rw-r--r--   0 yixu       (502) staff       (20)    11040 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/inference/common.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1528 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/inference/download_and_inject_bundle.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.530848 scale-llm-engine-1.0.0/spellbook_serve/inference/forwarding/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/inference/forwarding/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)    18191 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/inference/forwarding/forwarding.py
+-rw-r--r--   0 yixu       (502) staff       (20)     4824 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/inference/forwarding/http_forwarder.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.531328 scale-llm-engine-1.0.0/spellbook_serve/inference/infra/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/inference/infra/__init__.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.532072 scale-llm-engine-1.0.0/spellbook_serve/inference/infra/gateways/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/inference/infra/gateways/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)      543 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/inference/infra/gateways/datadog_inference_monitoring_metrics_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     4422 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/inference/post_inference_hooks.py
+-rw-r--r--   0 yixu       (502) staff       (20)     6137 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/inference/service_requests.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.533767 scale-llm-engine-1.0.0/spellbook_serve/inference/sync_inference/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/inference/sync_inference/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)      357 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/inference/sync_inference/constants.py
+-rw-r--r--   0 yixu       (502) staff       (20)     4065 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/inference/sync_inference/fastapi_server.py
+-rw-r--r--   0 yixu       (502) staff       (20)      722 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/inference/sync_inference/start_fastapi_server.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.534655 scale-llm-engine-1.0.0/spellbook_serve/infra/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/__init__.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.544900 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/
+-rw-r--r--   0 yixu       (502) staff       (20)     1845 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)    12162 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/aiohttp_sse_client.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1494 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/batch_job_orchestration_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)      902 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/batch_job_progress_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2985 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/celery_task_queue_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1003 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/datadog_monitoring_metrics_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)      812 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/fake_model_primitive_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1378 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/fake_monitoring_metrics_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)      523 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/filesystem_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2361 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/k8s_resource_parser.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1817 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/live_async_model_endpoint_inference_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     3614 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/live_batch_job_orchestration_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1876 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/live_batch_job_progress_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)    12705 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/live_docker_image_batch_job_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     9540 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/live_model_endpoint_infra_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     9449 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/live_model_endpoints_schema_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     7527 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/live_streaming_model_endpoint_inference_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     6407 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/live_sync_model_endpoint_inference_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     7183 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/model_endpoint_infra_gateway.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.549485 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/resources/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/resources/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     3641 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/resources/endpoint_resource_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1443 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/resources/fake_sqs_endpoint_resource_delegate.py
+-rw-r--r--   0 yixu       (502) staff       (20)     4993 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/resources/image_cache_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)    59818 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/resources/k8s_endpoint_resource_delegate.py
+-rw-r--r--   0 yixu       (502) staff       (20)    55522 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/resources/k8s_resource_types.py
+-rw-r--r--   0 yixu       (502) staff       (20)     4780 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/resources/live_endpoint_resource_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     6073 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/resources/live_sqs_endpoint_resource_delegate.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1370 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/resources/sqs_endpoint_resource_delegate.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1225 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/gateways/s3_filesystem_gateway.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1361 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/infra_utils.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.556542 scale-llm-engine-1.0.0/spellbook_serve/infra/repositories/
+-rw-r--r--   0 yixu       (502) staff       (20)     1240 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/repositories/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2940 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/repositories/batch_job_record_repository.py
+-rw-r--r--   0 yixu       (502) staff       (20)     5773 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/repositories/db_batch_job_record_repository.py
+-rw-r--r--   0 yixu       (502) staff       (20)     6275 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/repositories/db_docker_image_batch_job_bundle_repository.py
+-rw-r--r--   0 yixu       (502) staff       (20)    10886 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/repositories/db_model_bundle_repository.py
+-rw-r--r--   0 yixu       (502) staff       (20)    14026 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/repositories/db_model_endpoint_record_repository.py
+-rw-r--r--   0 yixu       (502) staff       (20)      563 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/repositories/db_repository_mixin.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1738 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/repositories/ecr_docker_repository.py
+-rw-r--r--   0 yixu       (502) staff       (20)      808 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/repositories/feature_flag_repository.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1144 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/repositories/model_endpoint_cache_repository.py
+-rw-r--r--   0 yixu       (502) staff       (20)     6086 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/repositories/model_endpoint_record_repository.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1967 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/repositories/redis_feature_flag_repository.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2320 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/repositories/redis_model_endpoint_cache_repository.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.561908 scale-llm-engine-1.0.0/spellbook_serve/infra/services/
+-rw-r--r--   0 yixu       (502) staff       (20)      275 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/services/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)      848 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/services/batch_job_orchestration_service.py
+-rw-r--r--   0 yixu       (502) staff       (20)     4320 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/services/image_cache_service.py
+-rw-r--r--   0 yixu       (502) staff       (20)    15491 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/services/live_batch_job_orchestration_service.py
+-rw-r--r--   0 yixu       (502) staff       (20)     7935 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/services/live_batch_job_service.py
+-rw-r--r--   0 yixu       (502) staff       (20)    36482 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/services/live_endpoint_builder_service.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2341 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/services/live_llm_model_endpoint_service.py
+-rw-r--r--   0 yixu       (502) staff       (20)    15862 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/services/live_model_endpoint_service.py
+-rw-r--r--   0 yixu       (502) staff       (20)     2014 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/infra/services/model_endpoint_cache_service.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.562953 scale-llm-engine-1.0.0/spellbook_serve/scripts/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/scripts/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)     1144 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/scripts/autogenerate_client_and_docs.py
+drwxr-xr-x   0 yixu       (502) staff       (20)        0 2023-07-15 01:50:08.564743 scale-llm-engine-1.0.0/spellbook_serve/service_builder/
+-rw-r--r--   0 yixu       (502) staff       (20)        0 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/service_builder/__init__.py
+-rw-r--r--   0 yixu       (502) staff       (20)      372 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/service_builder/celery.py
+-rw-r--r--   0 yixu       (502) staff       (20)     4034 2023-07-15 01:15:04.000000 scale-llm-engine-1.0.0/spellbook_serve/service_builder/tasks_v1.py
```

