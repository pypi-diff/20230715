# Comparing `tmp/clear_skies_aws-1.7.6.tar.gz` & `tmp/clear_skies_aws-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear_skies_aws-1.7.6.tar", max compression
+gzip compressed data, was "clear_skies_aws-1.7.7.tar", max compression
```

## Comparing `clear_skies_aws-1.7.6.tar` & `clear_skies_aws-1.7.7.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1053 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/LICENSE
--rw-r--r--   0        0        0     7780 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/README.md
--rw-r--r--   0        0        0      789 2023-07-14 19:20:04.221882 clear_skies_aws-1.7.6/pyproject.toml
--rw-r--r--   0        0        0       58 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/__init__.py
--rw-r--r--   0        0        0     2141 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/actions/__init__.py
--rw-r--r--   0        0        0     3357 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/actions/action_aws.py
--rw-r--r--   0        0        0     4085 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/actions/assume_role.py
--rw-r--r--   0        0        0     2450 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/actions/assume_role_test.py
--rw-r--r--   0        0        0     6921 2023-07-12 17:17:53.471558 clear_skies_aws-1.7.6/src/clearskies_aws/actions/ses.py
--rw-r--r--   0        0        0     1630 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/actions/ses_test.py
--rw-r--r--   0        0        0     2197 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/actions/sns.py
--rw-r--r--   0        0        0     2194 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/actions/sns_test.py
--rw-r--r--   0        0        0     2340 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/actions/sqs.py
--rw-r--r--   0        0        0     2234 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/actions/sqs_test.py
--rw-r--r--   0        0        0       83 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/backends/__init__.py
--rw-r--r--   0        0        0    29126 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/backends/dynamo_db_backend.py
--rw-r--r--   0        0        0    13150 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/backends/dynamo_db_backend_test.py
--rw-r--r--   0        0        0     2726 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/backends/sqs_backend.py
--rw-r--r--   0        0        0     1138 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/backends/sqs_backend_test.py
--rw-r--r--   0        0        0      348 2023-07-14 10:53:10.727298 clear_skies_aws-1.7.6/src/clearskies_aws/contexts/__init__.py
--rw-r--r--   0        0        0     1305 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     1276 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     1251 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc
--rw-r--r--   0        0        0      506 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/contexts/cli.py
--rw-r--r--   0        0        0     1002 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/contexts/lambda_api_gateway.py
--rw-r--r--   0        0        0      952 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/contexts/lambda_elb.py
--rw-r--r--   0        0        0     1009 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/contexts/lambda_http_gateway.py
--rw-r--r--   0        0        0     1183 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/contexts/lambda_invocation.py
--rw-r--r--   0        0        0     1317 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/contexts/lambda_sns.py
--rw-r--r--   0        0        0     1685 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py
--rw-r--r--   0        0        0     1999 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py
--rw-r--r--   0        0        0      510 2023-07-14 10:52:55.860805 clear_skies_aws-1.7.6/src/clearskies_aws/contexts/wsgi.py
--rw-r--r--   0        0        0       56 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/di/__init__.py
--rw-r--r--   0        0        0      775 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/di/standard_dependencies.py
--rw-r--r--   0        0        0      267 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/__init__.py
--rw-r--r--   0        0        0      943 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     3710 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     2761 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc
--rw-r--r--   0        0        0      901 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc
--rw-r--r--   0        0        0     3065 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/lambda_api_gateway.py
--rw-r--r--   0        0        0     2845 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py
--rw-r--r--   0        0        0      662 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/lambda_elb.py
--rw-r--r--   0        0        0      692 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/lambda_http_gateway.py
--rw-r--r--   0        0        0      715 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/lambda_invocation.py
--rw-r--r--   0        0        0     2163 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/lambda_sns.py
--rw-r--r--   0        0        0     2082 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/lambda_sqs_standard.py
--rw-r--r--   0        0        0       22 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/mocks/__init__.py
--rw-r--r--   0        0        0       21 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/mocks/actions/__init__.py
--rw-r--r--   0        0        0      937 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/mocks/actions/ses.py
--rw-r--r--   0        0        0      326 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/secrets/__init__.py
--rw-r--r--   0        0        0     1919 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/secrets/additional_configs/__init__.py
--rw-r--r--   0        0        0     1082 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py
--rw-r--r--   0        0        0     3467 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py
--rw-r--r--   0        0        0     3776 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py
--rw-r--r--   0        0        0     6444 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py
--rw-r--r--   0        0        0     1443 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/secrets/akeyless_with_ssm_cache.py
--rw-r--r--   0        0        0     1655 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/secrets/parameter_store.py
--rw-r--r--   0        0        0      761 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/secrets/parameter_store_test.py
--rw-r--r--   0        0        0     2898 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/secrets/secrets_manager.py
--rw-r--r--   0        0        0      786 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.6/src/clearskies_aws/secrets/secrets_manager_test.py
--rw-r--r--   0        0        0     8579 1970-01-01 00:00:00.000000 clear_skies_aws-1.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/LICENSE
+-rw-r--r--   0        0        0     7780 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/README.md
+-rw-r--r--   0        0        0      789 2023-07-15 19:54:59.160374 clear_skies_aws-1.7.7/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/__init__.py
+-rw-r--r--   0        0        0     2141 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/actions/__init__.py
+-rw-r--r--   0        0        0     3357 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/actions/action_aws.py
+-rw-r--r--   0        0        0     4085 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/actions/assume_role.py
+-rw-r--r--   0        0        0     2450 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/actions/assume_role_test.py
+-rw-r--r--   0        0        0     6921 2023-07-12 17:17:53.471558 clear_skies_aws-1.7.7/src/clearskies_aws/actions/ses.py
+-rw-r--r--   0        0        0     1630 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/actions/ses_test.py
+-rw-r--r--   0        0        0     2197 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/actions/sns.py
+-rw-r--r--   0        0        0     2194 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/actions/sns_test.py
+-rw-r--r--   0        0        0     2340 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/actions/sqs.py
+-rw-r--r--   0        0        0     2234 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/actions/sqs_test.py
+-rw-r--r--   0        0        0       83 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/backends/__init__.py
+-rw-r--r--   0        0        0    29126 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/backends/dynamo_db_backend.py
+-rw-r--r--   0        0        0    13150 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/backends/dynamo_db_backend_test.py
+-rw-r--r--   0        0        0     2726 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/backends/sqs_backend.py
+-rw-r--r--   0        0        0     1138 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/backends/sqs_backend_test.py
+-rw-r--r--   0        0        0      348 2023-07-14 10:53:10.727298 clear_skies_aws-1.7.7/src/clearskies_aws/contexts/__init__.py
+-rw-r--r--   0        0        0     1305 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     1276 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     1251 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc
+-rw-r--r--   0        0        0      506 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/contexts/cli.py
+-rw-r--r--   0        0        0     1002 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/contexts/lambda_api_gateway.py
+-rw-r--r--   0        0        0      952 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/contexts/lambda_elb.py
+-rw-r--r--   0        0        0     1009 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/contexts/lambda_http_gateway.py
+-rw-r--r--   0        0        0     1183 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/contexts/lambda_invocation.py
+-rw-r--r--   0        0        0     1317 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/contexts/lambda_sns.py
+-rw-r--r--   0        0        0     1685 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py
+-rw-r--r--   0        0        0     1999 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py
+-rw-r--r--   0        0        0      510 2023-07-14 10:52:55.860805 clear_skies_aws-1.7.7/src/clearskies_aws/contexts/wsgi.py
+-rw-r--r--   0        0        0       56 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/di/__init__.py
+-rw-r--r--   0        0        0      775 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/di/standard_dependencies.py
+-rw-r--r--   0        0        0      267 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/__init__.py
+-rw-r--r--   0        0        0      943 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     3710 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     2761 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc
+-rw-r--r--   0        0        0      901 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc
+-rw-r--r--   0        0        0     3184 2023-07-15 19:39:08.598719 clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/lambda_api_gateway.py
+-rw-r--r--   0        0        0     2845 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py
+-rw-r--r--   0        0        0      662 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/lambda_elb.py
+-rw-r--r--   0        0        0      692 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/lambda_http_gateway.py
+-rw-r--r--   0        0        0      715 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/lambda_invocation.py
+-rw-r--r--   0        0        0     2163 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/lambda_sns.py
+-rw-r--r--   0        0        0     2082 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/lambda_sqs_standard.py
+-rw-r--r--   0        0        0       22 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/mocks/__init__.py
+-rw-r--r--   0        0        0       21 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/mocks/actions/__init__.py
+-rw-r--r--   0        0        0      937 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/mocks/actions/ses.py
+-rw-r--r--   0        0        0      326 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/secrets/__init__.py
+-rw-r--r--   0        0        0     1919 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/secrets/additional_configs/__init__.py
+-rw-r--r--   0        0        0     1082 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py
+-rw-r--r--   0        0        0     3467 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py
+-rw-r--r--   0        0        0     3776 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py
+-rw-r--r--   0        0        0     6444 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py
+-rw-r--r--   0        0        0     1443 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/secrets/akeyless_with_ssm_cache.py
+-rw-r--r--   0        0        0     1655 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/secrets/parameter_store.py
+-rw-r--r--   0        0        0      761 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/secrets/parameter_store_test.py
+-rw-r--r--   0        0        0     2898 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/secrets/secrets_manager.py
+-rw-r--r--   0        0        0      786 2023-07-12 17:16:37.845253 clear_skies_aws-1.7.7/src/clearskies_aws/secrets/secrets_manager_test.py
+-rw-r--r--   0        0        0     8579 1970-01-01 00:00:00.000000 clear_skies_aws-1.7.7/PKG-INFO
```

### Comparing `clear_skies_aws-1.7.6/LICENSE` & `clear_skies_aws-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/README.md` & `clear_skies_aws-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/pyproject.toml` & `clear_skies_aws-1.7.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "clear-skies-aws"
-version = "1.7.6"
+version = "1.7.7"
 description = "clearskies bindings for working in AWS"
 authors = [
     "Conor Mancone <cmancone@gmail.com>",
     "tnijboer"
 ]
 repository = "https://github.com/cmancone/clearskies-aws"
 license = "MIT"
```

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/actions/__init__.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/actions/action_aws.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/actions/action_aws.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/actions/assume_role.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/actions/assume_role.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/actions/assume_role_test.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/actions/assume_role_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/actions/ses.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/actions/ses.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/actions/ses_test.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/actions/ses_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/actions/sns.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/actions/sns.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/actions/sns_test.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/actions/sns_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/actions/sqs.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/actions/sqs.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/actions/sqs_test.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/actions/sqs_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/backends/dynamo_db_backend.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/backends/dynamo_db_backend.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/backends/dynamo_db_backend_test.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/backends/dynamo_db_backend_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/backends/sqs_backend.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/backends/sqs_backend.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/backends/sqs_backend_test.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/backends/sqs_backend_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.7.7/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.7.7/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc` & `clear_skies_aws-1.7.7/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/contexts/lambda_api_gateway.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/contexts/lambda_api_gateway.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/contexts/lambda_elb.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/contexts/lambda_elb.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/contexts/lambda_http_gateway.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/contexts/lambda_http_gateway.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/contexts/lambda_invocation.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/contexts/lambda_invocation.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/contexts/lambda_sns.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/contexts/lambda_sns.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/di/standard_dependencies.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/di/standard_dependencies.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc` & `clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc` & `clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/lambda_api_gateway.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/lambda_api_gateway.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,7 +89,10 @@
         return self._query_parameters
 
     def context_specifics(self):
         return {
             "event": self._event,
             "context": self._context,
         }
+
+    def get_client_ip(self):
+        return self._event.get('requestContext', {}).get('identity', {}).get('sourceIp')
```

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/lambda_elb.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/lambda_elb.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/lambda_http_gateway.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/lambda_http_gateway.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/lambda_invocation.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/lambda_invocation.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/lambda_sns.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/lambda_sns.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/input_outputs/lambda_sqs_standard.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/input_outputs/lambda_sqs_standard.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/mocks/actions/ses.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/mocks/actions/ses.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/secrets/additional_configs/__init__.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/secrets/additional_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/secrets/akeyless_with_ssm_cache.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/secrets/akeyless_with_ssm_cache.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/secrets/parameter_store.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/secrets/parameter_store.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/secrets/parameter_store_test.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/secrets/parameter_store_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/secrets/secrets_manager.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/secrets/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/src/clearskies_aws/secrets/secrets_manager_test.py` & `clear_skies_aws-1.7.7/src/clearskies_aws/secrets/secrets_manager_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.7.6/PKG-INFO` & `clear_skies_aws-1.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-aws
-Version: 1.7.6
+Version: 1.7.7
 Summary: clearskies bindings for working in AWS
 Home-page: https://github.com/cmancone/clearskies-aws
 License: MIT
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

