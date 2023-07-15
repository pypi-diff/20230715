# Comparing `tmp/horde_sdk-0.5.0.tar.gz` & `tmp/horde_sdk-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horde_sdk-0.5.0.tar", last modified: Thu Jul 13 23:40:24 2023, max compression
+gzip compressed data, was "horde_sdk-0.5.2.tar", last modified: Sat Jul 15 02:34:26 2023, max compression
```

## Comparing `horde_sdk-0.5.0.tar` & `horde_sdk-0.5.2.tar`

### file list

```diff
@@ -1,178 +1,174 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.826752 horde_sdk-0.5.0/
--rw-rw-rw-   0        0        0     1183 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    35164 2023-03-31 20:26:08.000000 horde_sdk-0.5.0/LICENSE
--rw-rw-rw-   0        0        0      176 2023-07-13 23:39:46.000000 horde_sdk-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0    42797 2023-07-13 23:40:24.825751 horde_sdk-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     1737 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.641084 horde_sdk-0.5.0/horde_sdk/
--rw-rw-rw-   0        0        0      498 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.672275 horde_sdk-0.5.0/horde_sdk/ai_horde_api/
--rw-rw-rw-   0        0        0      585 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_api/__init__.py
--rw-rw-rw-   0        0        0    14843 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_api/ai_horde_clients.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.676276 horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/
--rw-rw-rw-   0        0        0     1475 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/__init__.py
--rw-rw-rw-   0        0        0     1298 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/_stats.py
--rw-rw-rw-   0        0        0     3315 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/base.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.682357 horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/generate/
--rw-rw-rw-   0        0        0        0 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/generate/__init__.py
--rw-rw-rw-   0        0        0     3840 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/generate/_async.py
--rw-rw-rw-   0        0        0     2329 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/generate/_check.py
--rw-rw-rw-   0        0        0     6483 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/generate/_pop.py
--rw-rw-rw-   0        0        0     3312 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/generate/_status.py
--rw-rw-rw-   0        0        0     1806 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/generate/_submit.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.684357 horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/workers/
--rw-rw-rw-   0        0        0        0 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/workers/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/workers/_workers_all.py
--rw-rw-rw-   0        0        0      979 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_api/consts.py
--rw-rw-rw-   0        0        0     2785 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_api/endpoints.py
--rw-rw-rw-   0        0        0     1818 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_api/fields.py
--rw-rw-rw-   0        0        0      381 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_api/metadata.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.687357 horde_sdk-0.5.0/horde_sdk/ai_horde_worker/
--rw-rw-rw-   0        0        0        0 2023-07-13 23:26:40.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_worker/__init__.py
--rw-rw-rw-   0        0        0    11120 2023-07-13 23:26:40.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_worker/bridge_data.py
--rw-rw-rw-   0        0        0     1119 2023-07-13 23:26:40.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_worker/kudos.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.691357 horde_sdk-0.5.0/horde_sdk/ai_horde_worker/locale_info/
--rw-rw-rw-   0        0        0      190 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_worker/locale_info/README.md
--rw-rw-rw-   0        0        0        0 2023-07-13 23:26:40.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_worker/locale_info/__init__.py
--rw-rw-rw-   0        0        0    10071 2023-07-13 23:26:40.000000 horde_sdk-0.5.0/horde_sdk/ai_horde_worker/locale_info/bridge_data_fields.py
--rw-rw-rw-   0        0        0     2074 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/consts.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.697866 horde_sdk-0.5.0/horde_sdk/generic_api/
--rw-rw-rw-   0        0        0       60 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/generic_api/__init__.py
--rw-rw-rw-   0        0        0      676 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/generic_api/_reflection.py
--rw-rw-rw-   0        0        0    10422 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/generic_api/apimodels.py
--rw-rw-rw-   0        0        0     1237 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/generic_api/endpoints.py
--rw-rw-rw-   0        0        0    31143 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/generic_api/generic_clients.py
--rw-rw-rw-   0        0        0      826 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/generic_api/metadata.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.700377 horde_sdk-0.5.0/horde_sdk/generic_api/utils/
--rw-rw-rw-   0        0        0        0 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/generic_api/utils/__init__.py
--rw-rw-rw-   0        0        0    29120 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/generic_api/utils/swagger.py
--rw-rw-rw-   0        0        0      125 2023-07-13 23:27:48.000000 horde_sdk-0.5.0/horde_sdk/localize.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.707892 horde_sdk-0.5.0/horde_sdk/ratings_api/
--rw-rw-rw-   0        0        0        0 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ratings_api/__init__.py
--rw-rw-rw-   0        0        0     8420 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ratings_api/apimodels.py
--rw-rw-rw-   0        0        0      573 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ratings_api/endpoints.py
--rw-rw-rw-   0        0        0      895 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ratings_api/metadata.py
--rw-rw-rw-   0        0        0      589 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/ratings_api/ratings_client.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.712405 horde_sdk-0.5.0/horde_sdk/scripts/
--rw-rw-rw-   0        0        0        0 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/scripts/__init__.py
--rw-rw-rw-   0        0        0      651 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/scripts/write_all_payload_examples.py
--rw-rw-rw-   0        0        0      653 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/scripts/write_all_response_examples.py
--rw-rw-rw-   0        0        0      431 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/horde_sdk/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.664672 horde_sdk-0.5.0/horde_sdk.egg-info/
--rw-rw-rw-   0        0        0    42797 2023-07-13 23:40:24.000000 horde_sdk-0.5.0/horde_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9066 2023-07-13 23:40:24.000000 horde_sdk-0.5.0/horde_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 23:40:24.000000 horde_sdk-0.5.0/horde_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-13 23:40:24.000000 horde_sdk-0.5.0/horde_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-13 23:40:24.000000 horde_sdk-0.5.0/horde_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1718 2023-07-13 23:40:14.000000 horde_sdk-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-13 23:40:24.826752 horde_sdk-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      352 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.719411 horde_sdk-0.5.0/tests/
--rw-rw-rw-   0        0        0        0 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.724956 horde_sdk-0.5.0/tests/ai_horde_api/
--rw-rw-rw-   0        0        0        0 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/ai_horde_api/__init__.py
--rw-rw-rw-   0        0        0     6790 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/tests/ai_horde_api/test_ai_horde_api_calls.py
--rw-rw-rw-   0        0        0     3901 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/ai_horde_api/test_ai_horde_api_models.py
--rw-rw-rw-   0        0        0     4830 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/ai_horde_api/test_dynamically_validate_against_swagger.py
--rw-rw-rw-   0        0        0     1623 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/ai_horde_api/test_swagger.py
--rw-rw-rw-   0        0        0     1069 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.725955 horde_sdk-0.5.0/tests/ratings_api/
--rw-rw-rw-   0        0        0        0 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/ratings_api/test_init.py
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.726957 horde_sdk-0.5.0/tests/test_data/
--rw-rw-rw-   0        0        0       93 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/RequestErrorResponse.json
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.727959 horde_sdk-0.5.0/tests/test_data/ai_horde_api/
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.754500 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/
--rw-rw-rw-   0        0        0       99 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_filters_filter_id_patch.json
--rw-rw-rw-   0        0        0       47 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_filters_post.json
--rw-rw-rw-   0        0        0       99 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_filters_put.json
--rw-rw-rw-   0        0        0     1298 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_generate_async_post.json
--rw-rw-rw-   0        0        0      488 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_generate_pop_post.json
--rw-rw-rw-   0        0        0      221 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_generate_rate_id_post.json
--rw-rw-rw-   0        0        0      141 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_generate_submit_post.json
--rw-rw-rw-   0        0        0      719 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_async_post.json
--rw-rw-rw-   0        0        0      337 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_pop_post.json
--rw-rw-rw-   0        0        0      101 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_submit_post.json
--rw-rw-rw-   0        0        0      295 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_interrogate_async_post.json
--rw-rw-rw-   0        0        0      238 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_interrogate_pop_post.json
--rw-rw-rw-   0        0        0       57 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_interrogate_submit_post.json
--rw-rw-rw-   0        0        0       44 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_kudos_award_post.json
--rw-rw-rw-   0        0        0       70 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_kudos_kai_user_id_post.json
--rw-rw-rw-   0        0        0       44 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_kudos_transfer_post.json
--rw-rw-rw-   0        0        0      156 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_sharedkeys_put.json
--rw-rw-rw-   0        0        0      156 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_sharedkeys_sharedkey_id_patch.json
--rw-rw-rw-   0        0        0       79 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_status_modes_put.json
--rw-rw-rw-   0        0        0       68 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_teams_post.json
--rw-rw-rw-   0        0        0       68 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_teams_team_id_patch.json
--rw-rw-rw-   0        0        0      391 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_users_user_id_put.json
--rw-rw-rw-   0        0        0      176 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_workers_worker_id_put.json
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.755499 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_production_responses/
--rw-rw-rw-   0        0        0   123568 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_production_responses/_v2_workers_get_200.json
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.817241 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/
--rw-rw-rw-   0        0        0       27 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_filters_filter_id_delete_200.json
--rw-rw-rw-   0        0        0      169 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_filters_filter_id_get_200.json
--rw-rw-rw-   0        0        0      131 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_filters_filter_id_patch_200.json
--rw-rw-rw-   0        0        0      169 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_filters_get_200.json
--rw-rw-rw-   0        0        0       46 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_filters_post_200.json
--rw-rw-rw-   0        0        0      131 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_filters_put_201.json
--rw-rw-rw-   0        0        0       69 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_filters_regex_get_200.json
--rw-rw-rw-   0        0        0     1329 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_find_user_get_200.json
--rw-rw-rw-   0        0        0       57 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_async_post_202.json
--rw-rw-rw-   0        0        0      222 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_check_id_get_200.json
--rw-rw-rw-   0        0        0     1536 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_pop_post_200.json
--rw-rw-rw-   0        0        0       26 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_rate_id_post_200.json
--rw-rw-rw-   0        0        0      515 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_status_id_delete_200.json
--rw-rw-rw-   0        0        0      515 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_status_id_get_200.json
--rw-rw-rw-   0        0        0       26 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_submit_post_200.json
--rw-rw-rw-   0        0        0       57 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_async_post_202.json
--rw-rw-rw-   0        0        0      929 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_pop_post_200.json
--rw-rw-rw-   0        0        0      438 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_status_id_delete_200.json
--rw-rw-rw-   0        0        0      438 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_status_id_get_200.json
--rw-rw-rw-   0        0        0       26 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_submit_post_200.json
--rw-rw-rw-   0        0        0       40 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_async_post_202.json
--rw-rw-rw-   0        0        0      438 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_pop_post_200.json
--rw-rw-rw-   0        0        0      279 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_status_id_delete_200.json
--rw-rw-rw-   0        0        0      279 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_status_id_get_200.json
--rw-rw-rw-   0        0        0       26 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_submit_post_200.json
--rw-rw-rw-   0        0        0       26 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_kudos_award_post_200.json
--rw-rw-rw-   0        0        0       30 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_kudos_transfer_post_200.json
--rw-rw-rw-   0        0        0       27 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_operations_ipaddr_delete_200.json
--rw-rw-rw-   0        0        0      199 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_put_200.json
--rw-rw-rw-   0        0        0       27 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_sharedkey_id_delete_200.json
--rw-rw-rw-   0        0        0      199 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_sharedkey_id_get_200.json
--rw-rw-rw-   0        0        0      199 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_sharedkey_id_patch_200.json
--rw-rw-rw-   0        0        0      351 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_stats_img_models_get_200.json
--rw-rw-rw-   0        0        0      348 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_stats_img_totals_get_200.json
--rw-rw-rw-   0        0        0      351 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_stats_text_models_get_200.json
--rw-rw-rw-   0        0        0      348 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_stats_text_totals_get_200.json
--rw-rw-rw-   0        0        0      181 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_status_models_get_200.json
--rw-rw-rw-   0        0        0      139 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_status_models_model_name_get_200.json
--rw-rw-rw-   0        0        0       94 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_status_modes_get_200.json
--rw-rw-rw-   0        0        0       94 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_status_modes_put_200.json
--rw-rw-rw-   0        0        0      114 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_status_news_get_200.json
--rw-rw-rw-   0        0        0      397 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_status_performance_get_200.json
--rw-rw-rw-   0        0        0      550 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_teams_get_200.json
--rw-rw-rw-   0        0        0       54 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_teams_post_200.json
--rw-rw-rw-   0        0        0       53 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_teams_team_id_delete_200.json
--rw-rw-rw-   0        0        0      448 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_teams_team_id_get_200.json
--rw-rw-rw-   0        0        0       54 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_teams_team_id_patch_200.json
--rw-rw-rw-   0        0        0     1329 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_users_get_200.json
--rw-rw-rw-   0        0        0     1329 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_users_user_id_get_200.json
--rw-rw-rw-   0        0        0      395 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_users_user_id_put_200.json
--rw-rw-rw-   0        0        0     1147 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_workers_get_200.json
--rw-rw-rw-   0        0        0       53 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_delete_200.json
--rw-rw-rw-   0        0        0      977 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_get_200.json
--rw-rw-rw-   0        0        0      118 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_put_200.json
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.820240 horde_sdk-0.5.0/tests/test_data/ai_horde_api/production_responses/
--rw-rw-rw-   0        0        0    20811 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/production_responses/ImgModelStats.json
--rw-rw-rw-   0        0        0        4 2023-07-13 02:41:16.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/production_responses/_v2_workers_get_200_production.json
--rw-rw-rw-   0        0        0   237970 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ai_horde_api/swagger.json
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.626388 horde_sdk-0.5.0/tests/test_data/ratings_api/
-drwxrwxrwx   0        0        0        0 2023-07-13 23:40:24.824753 horde_sdk-0.5.0/tests/test_data/ratings_api/example_responses/
--rw-rw-rw-   0        0        0      666 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ratings_api/example_responses/ImageRatingsResponse.json
--rw-rw-rw-   0        0        0      251 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ratings_api/example_responses/UserCheckResponse.json
--rw-rw-rw-   0        0        0    64737 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ratings_api/example_responses/UserRatingsResponse.json
--rw-rw-rw-   0        0        0     5726 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_data/ratings_api/example_responses/UserValidateResponse.json
--rw-rw-rw-   0        0        0     5982 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/tests/test_dynamically_check_apimodels.py
--rw-rw-rw-   0        0        0      320 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/tests/test_generic.py
--rw-rw-rw-   0        0        0     1650 2023-07-13 23:26:59.000000 horde_sdk-0.5.0/tests/test_ratings_api_models.py
--rw-rw-rw-   0        0        0      474 2023-07-12 15:33:50.000000 horde_sdk-0.5.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:26.041020 horde_sdk-0.5.2/
+-rw-rw-rw-   0        0        0     1183 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    35164 2023-03-31 20:26:08.000000 horde_sdk-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0      213 2023-07-14 12:52:49.000000 horde_sdk-0.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    42796 2023-07-15 02:34:26.041020 horde_sdk-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1736 2023-07-15 00:53:25.000000 horde_sdk-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.866983 horde_sdk-0.5.2/horde_sdk/
+-rw-rw-rw-   0        0        0      498 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.897493 horde_sdk-0.5.2/horde_sdk/ai_horde_api/
+-rw-rw-rw-   0        0        0      585 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ai_horde_api/__init__.py
+-rw-rw-rw-   0        0        0    14843 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ai_horde_api/ai_horde_clients.py
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.901492 horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/
+-rw-rw-rw-   0        0        0     1475 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/__init__.py
+-rw-rw-rw-   0        0        0     1298 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/_stats.py
+-rw-rw-rw-   0        0        0     3315 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/base.py
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.907493 horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/generate/
+-rw-rw-rw-   0        0        0        0 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/generate/__init__.py
+-rw-rw-rw-   0        0        0     3840 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/generate/_async.py
+-rw-rw-rw-   0        0        0     2329 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/generate/_check.py
+-rw-rw-rw-   0        0        0     6487 2023-07-14 12:50:10.000000 horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/generate/_pop.py
+-rw-rw-rw-   0        0        0     3320 2023-07-14 12:50:28.000000 horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/generate/_status.py
+-rw-rw-rw-   0        0        0     1810 2023-07-14 12:50:35.000000 horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/generate/_submit.py
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.909493 horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/workers/
+-rw-rw-rw-   0        0        0        0 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/workers/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/workers/_workers_all.py
+-rw-rw-rw-   0        0        0      979 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ai_horde_api/consts.py
+-rw-rw-rw-   0        0        0     2785 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ai_horde_api/endpoints.py
+-rw-rw-rw-   0        0        0     1818 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ai_horde_api/fields.py
+-rw-rw-rw-   0        0        0      381 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ai_horde_api/metadata.py
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.844106 horde_sdk-0.5.2/horde_sdk/ai_horde_worker/
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.910493 horde_sdk-0.5.2/horde_sdk/ai_horde_worker/locale_info/
+-rw-rw-rw-   0        0        0      190 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ai_horde_worker/locale_info/README.md
+-rw-rw-rw-   0        0        0     2074 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/consts.py
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.917493 horde_sdk-0.5.2/horde_sdk/generic_api/
+-rw-rw-rw-   0        0        0       60 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/generic_api/__init__.py
+-rw-rw-rw-   0        0        0      676 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/generic_api/_reflection.py
+-rw-rw-rw-   0        0        0    10422 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/generic_api/apimodels.py
+-rw-rw-rw-   0        0        0     1237 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/generic_api/endpoints.py
+-rw-rw-rw-   0        0        0    31143 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/generic_api/generic_clients.py
+-rw-rw-rw-   0        0        0      826 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/generic_api/metadata.py
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.919495 horde_sdk-0.5.2/horde_sdk/generic_api/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/generic_api/utils/__init__.py
+-rw-rw-rw-   0        0        0    29120 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/generic_api/utils/swagger.py
+-rw-rw-rw-   0        0        0      125 2023-07-13 23:27:48.000000 horde_sdk-0.5.2/horde_sdk/localize.py
+-rw-rw-rw-   0        0        0        0 2023-07-14 01:13:36.000000 horde_sdk-0.5.2/horde_sdk/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.925493 horde_sdk-0.5.2/horde_sdk/ratings_api/
+-rw-rw-rw-   0        0        0        0 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ratings_api/__init__.py
+-rw-rw-rw-   0        0        0     8436 2023-07-14 12:51:12.000000 horde_sdk-0.5.2/horde_sdk/ratings_api/apimodels.py
+-rw-rw-rw-   0        0        0      573 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ratings_api/endpoints.py
+-rw-rw-rw-   0        0        0      895 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ratings_api/metadata.py
+-rw-rw-rw-   0        0        0      589 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/ratings_api/ratings_client.py
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.928493 horde_sdk-0.5.2/horde_sdk/scripts/
+-rw-rw-rw-   0        0        0        0 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/scripts/__init__.py
+-rw-rw-rw-   0        0        0      651 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/scripts/write_all_payload_examples.py
+-rw-rw-rw-   0        0        0      653 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/scripts/write_all_response_examples.py
+-rw-rw-rw-   0        0        0      431 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/horde_sdk/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.891492 horde_sdk-0.5.2/horde_sdk.egg-info/
+-rw-rw-rw-   0        0        0    42796 2023-07-15 02:34:25.000000 horde_sdk-0.5.2/horde_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8861 2023-07-15 02:34:25.000000 horde_sdk-0.5.2/horde_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 02:34:25.000000 horde_sdk-0.5.2/horde_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-07-15 02:34:25.000000 horde_sdk-0.5.2/horde_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-15 02:34:25.000000 horde_sdk-0.5.2/horde_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1777 2023-07-14 12:52:49.000000 horde_sdk-0.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-15 02:34:26.041020 horde_sdk-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      352 2023-07-14 01:34:15.000000 horde_sdk-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.934502 horde_sdk-0.5.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.940502 horde_sdk-0.5.2/tests/ai_horde_api/
+-rw-rw-rw-   0        0        0        0 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/ai_horde_api/__init__.py
+-rw-rw-rw-   0        0        0     6790 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/tests/ai_horde_api/test_ai_horde_api_calls.py
+-rw-rw-rw-   0        0        0     3901 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/ai_horde_api/test_ai_horde_api_models.py
+-rw-rw-rw-   0        0        0     4830 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/ai_horde_api/test_dynamically_validate_against_swagger.py
+-rw-rw-rw-   0        0        0     1623 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/ai_horde_api/test_swagger.py
+-rw-rw-rw-   0        0        0     1069 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.941500 horde_sdk-0.5.2/tests/ratings_api/
+-rw-rw-rw-   0        0        0        0 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/ratings_api/test_init.py
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.942501 horde_sdk-0.5.2/tests/test_data/
+-rw-rw-rw-   0        0        0       93 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/RequestErrorResponse.json
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.943503 horde_sdk-0.5.2/tests/test_data/ai_horde_api/
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.968506 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/
+-rw-rw-rw-   0        0        0       99 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_filters_filter_id_patch.json
+-rw-rw-rw-   0        0        0       47 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_filters_post.json
+-rw-rw-rw-   0        0        0       99 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_filters_put.json
+-rw-rw-rw-   0        0        0     1298 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_async_post.json
+-rw-rw-rw-   0        0        0      488 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_pop_post.json
+-rw-rw-rw-   0        0        0      221 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_rate_id_post.json
+-rw-rw-rw-   0        0        0      141 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_submit_post.json
+-rw-rw-rw-   0        0        0      719 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_async_post.json
+-rw-rw-rw-   0        0        0      337 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_pop_post.json
+-rw-rw-rw-   0        0        0      101 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_submit_post.json
+-rw-rw-rw-   0        0        0      295 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_interrogate_async_post.json
+-rw-rw-rw-   0        0        0      238 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_interrogate_pop_post.json
+-rw-rw-rw-   0        0        0       57 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_interrogate_submit_post.json
+-rw-rw-rw-   0        0        0       44 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_kudos_award_post.json
+-rw-rw-rw-   0        0        0       70 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_kudos_kai_user_id_post.json
+-rw-rw-rw-   0        0        0       44 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_kudos_transfer_post.json
+-rw-rw-rw-   0        0        0      156 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_sharedkeys_put.json
+-rw-rw-rw-   0        0        0      156 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_sharedkeys_sharedkey_id_patch.json
+-rw-rw-rw-   0        0        0       79 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_status_modes_put.json
+-rw-rw-rw-   0        0        0       68 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_teams_post.json
+-rw-rw-rw-   0        0        0       68 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_teams_team_id_patch.json
+-rw-rw-rw-   0        0        0      391 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_users_user_id_put.json
+-rw-rw-rw-   0        0        0      176 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_workers_worker_id_put.json
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.969507 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_production_responses/
+-rw-rw-rw-   0        0        0   123568 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_production_responses/_v2_workers_get_200.json
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:26.031020 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/
+-rw-rw-rw-   0        0        0       27 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_filters_filter_id_delete_200.json
+-rw-rw-rw-   0        0        0      169 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_filters_filter_id_get_200.json
+-rw-rw-rw-   0        0        0      131 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_filters_filter_id_patch_200.json
+-rw-rw-rw-   0        0        0      169 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_filters_get_200.json
+-rw-rw-rw-   0        0        0       46 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_filters_post_200.json
+-rw-rw-rw-   0        0        0      131 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_filters_put_201.json
+-rw-rw-rw-   0        0        0       69 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_filters_regex_get_200.json
+-rw-rw-rw-   0        0        0     1329 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_find_user_get_200.json
+-rw-rw-rw-   0        0        0       57 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_async_post_202.json
+-rw-rw-rw-   0        0        0      222 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_check_id_get_200.json
+-rw-rw-rw-   0        0        0     1536 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_pop_post_200.json
+-rw-rw-rw-   0        0        0       26 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_rate_id_post_200.json
+-rw-rw-rw-   0        0        0      515 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_status_id_delete_200.json
+-rw-rw-rw-   0        0        0      515 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_status_id_get_200.json
+-rw-rw-rw-   0        0        0       26 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_submit_post_200.json
+-rw-rw-rw-   0        0        0       57 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_async_post_202.json
+-rw-rw-rw-   0        0        0      929 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_pop_post_200.json
+-rw-rw-rw-   0        0        0      438 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_status_id_delete_200.json
+-rw-rw-rw-   0        0        0      438 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_status_id_get_200.json
+-rw-rw-rw-   0        0        0       26 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_submit_post_200.json
+-rw-rw-rw-   0        0        0       40 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_async_post_202.json
+-rw-rw-rw-   0        0        0      438 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_pop_post_200.json
+-rw-rw-rw-   0        0        0      279 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_status_id_delete_200.json
+-rw-rw-rw-   0        0        0      279 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_status_id_get_200.json
+-rw-rw-rw-   0        0        0       26 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_submit_post_200.json
+-rw-rw-rw-   0        0        0       26 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_kudos_award_post_200.json
+-rw-rw-rw-   0        0        0       30 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_kudos_transfer_post_200.json
+-rw-rw-rw-   0        0        0       27 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_operations_ipaddr_delete_200.json
+-rw-rw-rw-   0        0        0      199 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_put_200.json
+-rw-rw-rw-   0        0        0       27 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_sharedkey_id_delete_200.json
+-rw-rw-rw-   0        0        0      199 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_sharedkey_id_get_200.json
+-rw-rw-rw-   0        0        0      199 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_sharedkey_id_patch_200.json
+-rw-rw-rw-   0        0        0      351 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_stats_img_models_get_200.json
+-rw-rw-rw-   0        0        0      348 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_stats_img_totals_get_200.json
+-rw-rw-rw-   0        0        0      351 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_stats_text_models_get_200.json
+-rw-rw-rw-   0        0        0      348 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_stats_text_totals_get_200.json
+-rw-rw-rw-   0        0        0      181 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_status_models_get_200.json
+-rw-rw-rw-   0        0        0      139 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_status_models_model_name_get_200.json
+-rw-rw-rw-   0        0        0       94 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_status_modes_get_200.json
+-rw-rw-rw-   0        0        0       94 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_status_modes_put_200.json
+-rw-rw-rw-   0        0        0      114 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_status_news_get_200.json
+-rw-rw-rw-   0        0        0      397 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_status_performance_get_200.json
+-rw-rw-rw-   0        0        0      550 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_teams_get_200.json
+-rw-rw-rw-   0        0        0       54 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_teams_post_200.json
+-rw-rw-rw-   0        0        0       53 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_teams_team_id_delete_200.json
+-rw-rw-rw-   0        0        0      448 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_teams_team_id_get_200.json
+-rw-rw-rw-   0        0        0       54 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_teams_team_id_patch_200.json
+-rw-rw-rw-   0        0        0     1329 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_users_get_200.json
+-rw-rw-rw-   0        0        0     1329 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_users_user_id_get_200.json
+-rw-rw-rw-   0        0        0      395 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_users_user_id_put_200.json
+-rw-rw-rw-   0        0        0     1147 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_workers_get_200.json
+-rw-rw-rw-   0        0        0       53 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_delete_200.json
+-rw-rw-rw-   0        0        0      977 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_get_200.json
+-rw-rw-rw-   0        0        0      118 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_put_200.json
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:26.034019 horde_sdk-0.5.2/tests/test_data/ai_horde_api/production_responses/
+-rw-rw-rw-   0        0        0    20811 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/production_responses/ImgModelStats.json
+-rw-rw-rw-   0        0        0        4 2023-07-13 02:41:16.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/production_responses/_v2_workers_get_200_production.json
+-rw-rw-rw-   0        0        0   237970 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ai_horde_api/swagger.json
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:25.850734 horde_sdk-0.5.2/tests/test_data/ratings_api/
+drwxrwxrwx   0        0        0        0 2023-07-15 02:34:26.039019 horde_sdk-0.5.2/tests/test_data/ratings_api/example_responses/
+-rw-rw-rw-   0        0        0      666 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ratings_api/example_responses/ImageRatingsResponse.json
+-rw-rw-rw-   0        0        0      251 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ratings_api/example_responses/UserCheckResponse.json
+-rw-rw-rw-   0        0        0    64737 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ratings_api/example_responses/UserRatingsResponse.json
+-rw-rw-rw-   0        0        0     5726 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_data/ratings_api/example_responses/UserValidateResponse.json
+-rw-rw-rw-   0        0        0     5982 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/tests/test_dynamically_check_apimodels.py
+-rw-rw-rw-   0        0        0      320 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/tests/test_generic.py
+-rw-rw-rw-   0        0        0     1650 2023-07-13 23:26:59.000000 horde_sdk-0.5.2/tests/test_ratings_api_models.py
+-rw-rw-rw-   0        0        0      474 2023-07-12 15:33:50.000000 horde_sdk-0.5.2/tests/test_utils.py
```

### Comparing `horde_sdk-0.5.0/CONTRIBUTING.md` & `horde_sdk-0.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/LICENSE` & `horde_sdk-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/PKG-INFO` & `horde_sdk-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horde_sdk
-Version: 0.5.0
+Version: 0.5.2
 Summary: A python toolkit for interacting with the horde APIs, services, and ecosystem.
 Author-email: tazlin <tazlin.on.github@gmail.com>, db0 <mail@dbzer0.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -691,9 +691,9 @@
 - Stable Diffusion Image Generation (driven by [ComfyUI](https://github.com/comfyanonymous/ComfyUI))
 - Image captioning
 - Image rating (currently ratings are for [diffusiondb](https://poloclub.github.io/diffusiondb/), others coming in the future)
 - Text Generation using LLMs (driven by [KoboldAI](https://github.com/KoboldAI/KoboldAI-Client))
 
 From anything to requesting your own images, or rolling your own [worker](https://github.com/Haidra-Org/AI-Horde-Worker) software, this package may suit your needs.
 
-## Documentation 
+## Documentation
 See the complete documentation at https://horde-sdk.readthedocs.io/en/latest/.
```

### Comparing `horde_sdk-0.5.0/README.md` & `horde_sdk-0.5.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 - Stable Diffusion Image Generation (driven by [ComfyUI](https://github.com/comfyanonymous/ComfyUI))
 - Image captioning
 - Image rating (currently ratings are for [diffusiondb](https://poloclub.github.io/diffusiondb/), others coming in the future)
 - Text Generation using LLMs (driven by [KoboldAI](https://github.com/KoboldAI/KoboldAI-Client))
 
 From anything to requesting your own images, or rolling your own [worker](https://github.com/Haidra-Org/AI-Horde-Worker) software, this package may suit your needs.
 
-## Documentation 
+## Documentation
 See the complete documentation at https://horde-sdk.readthedocs.io/en/latest/.
```

### Comparing `horde_sdk-0.5.0/horde_sdk/ai_horde_api/__init__.py` & `horde_sdk-0.5.2/horde_sdk/ai_horde_api/__init__.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/ai_horde_api/ai_horde_clients.py` & `horde_sdk-0.5.2/horde_sdk/ai_horde_api/ai_horde_clients.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/__init__.py` & `horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/__init__.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/_stats.py` & `horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/_stats.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/base.py` & `horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/base.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/generate/_async.py` & `horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/generate/_async.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/generate/_check.py` & `horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/generate/_check.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/generate/_pop.py` & `horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/generate/_pop.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,21 +121,21 @@
 
     @override
     @classmethod
     def get_http_method(cls) -> HTTPMethod:
         return HTTPMethod.POST
 
     @override
-    @staticmethod
-    def get_endpoint_subpath() -> str:
+    @classmethod
+    def get_endpoint_subpath(cls) -> str:
         return AI_HORDE_API_URL_Literals.v2_generate_pop
 
     @override
-    @staticmethod
-    def get_success_response_type() -> type[ImageGenerateJobResponse]:
+    @classmethod
+    def get_success_response_type(cls) -> type[ImageGenerateJobResponse]:
         return ImageGenerateJobResponse
 
 
 class ImageGenerateJobPopPayload(BaseImageGenerateParam):
     prompt: str
 
     @property
```

### Comparing `horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/generate/_status.py` & `horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/generate/_status.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,21 +63,21 @@
 
     @override
     @classmethod
     def get_http_method(cls) -> HTTPMethod:
         return HTTPMethod.DELETE
 
     @override
-    @staticmethod
-    def get_endpoint_subpath() -> str:
+    @classmethod
+    def get_endpoint_subpath(cls) -> str:
         return AI_HORDE_API_URL_Literals.v2_generate_status
 
     @override
-    @staticmethod
-    def get_success_response_type() -> type[ImageGenerateStatusResponse]:
+    @classmethod
+    def get_success_response_type(cls) -> type[ImageGenerateStatusResponse]:
         return ImageGenerateStatusResponse
 
 
 class ImageGenerateStatusRequest(BaseAIHordeRequest, BaseImageJobRequest):
     """Represents a GET request to the `/v2/generate/status/{id}` endpoint."""
 
     @override
@@ -87,15 +87,15 @@
 
     @override
     @classmethod
     def get_http_method(cls) -> HTTPMethod:
         return HTTPMethod.GET
 
     @override
-    @staticmethod
-    def get_endpoint_subpath() -> str:
+    @classmethod
+    def get_endpoint_subpath(cls) -> str:
         return AI_HORDE_API_URL_Literals.v2_generate_status
 
     @override
-    @staticmethod
-    def get_success_response_type() -> type[ImageGenerateStatusResponse]:
+    @classmethod
+    def get_success_response_type(cls) -> type[ImageGenerateStatusResponse]:
         return ImageGenerateStatusResponse
```

### Comparing `horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/generate/_submit.py` & `horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/generate/_submit.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     @override
     @classmethod
     def get_http_method(cls) -> HTTPMethod:
         return HTTPMethod.POST
 
     @override
-    @staticmethod
-    def get_endpoint_subpath() -> str:
+    @classmethod
+    def get_endpoint_subpath(cls) -> str:
         return AI_HORDE_API_URL_Literals.v2_generate_submit
 
     @override
-    @staticmethod
-    def get_success_response_type() -> type[ImageGenerationJobSubmitResponse]:
+    @classmethod
+    def get_success_response_type(cls) -> type[ImageGenerationJobSubmitResponse]:
         return ImageGenerationJobSubmitResponse
```

### Comparing `horde_sdk-0.5.0/horde_sdk/ai_horde_api/apimodels/workers/_workers_all.py` & `horde_sdk-0.5.2/horde_sdk/ai_horde_api/apimodels/workers/_workers_all.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/ai_horde_api/consts.py` & `horde_sdk-0.5.2/horde_sdk/ai_horde_api/consts.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/ai_horde_api/endpoints.py` & `horde_sdk-0.5.2/horde_sdk/ai_horde_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/ai_horde_api/fields.py` & `horde_sdk-0.5.2/horde_sdk/ai_horde_api/fields.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/consts.py` & `horde_sdk-0.5.2/horde_sdk/consts.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/generic_api/_reflection.py` & `horde_sdk-0.5.2/horde_sdk/generic_api/_reflection.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/generic_api/apimodels.py` & `horde_sdk-0.5.2/horde_sdk/generic_api/apimodels.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/generic_api/endpoints.py` & `horde_sdk-0.5.2/horde_sdk/generic_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/generic_api/generic_clients.py` & `horde_sdk-0.5.2/horde_sdk/generic_api/generic_clients.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/generic_api/metadata.py` & `horde_sdk-0.5.2/horde_sdk/generic_api/metadata.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/generic_api/utils/swagger.py` & `horde_sdk-0.5.2/horde_sdk/generic_api/utils/swagger.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/ratings_api/apimodels.py` & `horde_sdk-0.5.2/horde_sdk/ratings_api/apimodels.py`

 * *Files 7% similar despite different names*

```diff
@@ -164,21 +164,21 @@
 
     @override
     @classmethod
     def get_http_method(cls) -> HTTPMethod:
         return HTTPMethod.GET
 
     @override
-    @staticmethod
-    def get_endpoint_subpath() -> str:
+    @classmethod
+    def get_endpoint_subpath(cls) -> str:
         return Rating_API_URL_Literals.v1_image_ratings
 
     @override
-    @staticmethod
-    def get_success_response_type() -> type[ImageRatingsResponse]:
+    @classmethod
+    def get_success_response_type(cls) -> type[ImageRatingsResponse]:
         return ImageRatingsResponse
 
 
 class ImageRatingsComparisonTypes(StrEnum):
     """Ways the API supports selecting a rating range."""
 
     greater_than_equal = "ge"
@@ -215,21 +215,21 @@
 
     @override
     @classmethod
     def get_http_method(cls) -> HTTPMethod:
         return HTTPMethod.GET
 
     @override
-    @staticmethod
-    def get_endpoint_subpath() -> str:
+    @classmethod
+    def get_endpoint_subpath(cls) -> str:
         return Rating_API_URL_Literals.v1_user_validate
 
     @override
-    @staticmethod
-    def get_success_response_type() -> type[UserValidateResponse]:
+    @classmethod
+    def get_success_response_type(cls) -> type[UserValidateResponse]:
         return UserValidateResponse
 
 
 class UserCheckRequest(
     BaseRatingsAPIRequest,
     BaseRequestAuthenticated,
     BaseRequestUserSpecific,
@@ -246,21 +246,21 @@
 
     @override
     @classmethod
     def get_http_method(cls) -> HTTPMethod:
         return HTTPMethod.GET
 
     @override
-    @staticmethod
-    def get_endpoint_subpath() -> str:
+    @classmethod
+    def get_endpoint_subpath(cls) -> str:
         return Rating_API_URL_Literals.v1_user_check
 
     @override
-    @staticmethod
-    def get_success_response_type() -> type[UserCheckResponse]:
+    @classmethod
+    def get_success_response_type(cls) -> type[UserCheckResponse]:
         return UserCheckResponse
 
 
 class UserRatingsRequest(
     BaseRatingsAPIRequest,
     BaseRequestAuthenticated,
     ImageRatingsFilterableRequestBase,
@@ -278,18 +278,18 @@
 
     @override
     @classmethod
     def get_http_method(cls) -> HTTPMethod:
         return HTTPMethod.GET
 
     @override
-    @staticmethod
-    def get_endpoint_subpath() -> str:
+    @classmethod
+    def get_endpoint_subpath(cls) -> str:
         return Rating_API_URL_Literals.v1_user_ratings
 
     @override
-    @staticmethod
-    def get_success_response_type() -> type[UserRatingsResponse]:
+    @classmethod
+    def get_success_response_type(cls) -> type[UserRatingsResponse]:
         return UserRatingsResponse
 
 
 # endregion
```

### Comparing `horde_sdk-0.5.0/horde_sdk/ratings_api/endpoints.py` & `horde_sdk-0.5.2/horde_sdk/ratings_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/ratings_api/metadata.py` & `horde_sdk-0.5.2/horde_sdk/ratings_api/metadata.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/ratings_api/ratings_client.py` & `horde_sdk-0.5.2/horde_sdk/ratings_api/ratings_client.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/scripts/write_all_payload_examples.py` & `horde_sdk-0.5.2/horde_sdk/scripts/write_all_payload_examples.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk/scripts/write_all_response_examples.py` & `horde_sdk-0.5.2/horde_sdk/scripts/write_all_response_examples.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/horde_sdk.egg-info/PKG-INFO` & `horde_sdk-0.5.2/horde_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horde-sdk
-Version: 0.5.0
+Version: 0.5.2
 Summary: A python toolkit for interacting with the horde APIs, services, and ecosystem.
 Author-email: tazlin <tazlin.on.github@gmail.com>, db0 <mail@dbzer0.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -691,9 +691,9 @@
 - Stable Diffusion Image Generation (driven by [ComfyUI](https://github.com/comfyanonymous/ComfyUI))
 - Image captioning
 - Image rating (currently ratings are for [diffusiondb](https://poloclub.github.io/diffusiondb/), others coming in the future)
 - Text Generation using LLMs (driven by [KoboldAI](https://github.com/KoboldAI/KoboldAI-Client))
 
 From anything to requesting your own images, or rolling your own [worker](https://github.com/Haidra-Org/AI-Horde-Worker) software, this package may suit your needs.
 
-## Documentation 
+## Documentation
 See the complete documentation at https://horde-sdk.readthedocs.io/en/latest/.
```

### Comparing `horde_sdk-0.5.0/horde_sdk.egg-info/SOURCES.txt` & `horde_sdk-0.5.2/horde_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 horde_sdk/__init__.py
 horde_sdk/consts.py
 horde_sdk/localize.py
+horde_sdk/py.typed
 horde_sdk/utils.py
 horde_sdk.egg-info/PKG-INFO
 horde_sdk.egg-info/SOURCES.txt
 horde_sdk.egg-info/dependency_links.txt
 horde_sdk.egg-info/requires.txt
 horde_sdk.egg-info/top_level.txt
 horde_sdk/ai_horde_api/__init__.py
@@ -26,20 +27,15 @@
 horde_sdk/ai_horde_api/apimodels/generate/_async.py
 horde_sdk/ai_horde_api/apimodels/generate/_check.py
 horde_sdk/ai_horde_api/apimodels/generate/_pop.py
 horde_sdk/ai_horde_api/apimodels/generate/_status.py
 horde_sdk/ai_horde_api/apimodels/generate/_submit.py
 horde_sdk/ai_horde_api/apimodels/workers/__init__.py
 horde_sdk/ai_horde_api/apimodels/workers/_workers_all.py
-horde_sdk/ai_horde_worker/__init__.py
-horde_sdk/ai_horde_worker/bridge_data.py
-horde_sdk/ai_horde_worker/kudos.py
 horde_sdk/ai_horde_worker/locale_info/README.md
-horde_sdk/ai_horde_worker/locale_info/__init__.py
-horde_sdk/ai_horde_worker/locale_info/bridge_data_fields.py
 horde_sdk/generic_api/__init__.py
 horde_sdk/generic_api/_reflection.py
 horde_sdk/generic_api/apimodels.py
 horde_sdk/generic_api/endpoints.py
 horde_sdk/generic_api/generic_clients.py
 horde_sdk/generic_api/metadata.py
 horde_sdk/generic_api/utils/__init__.py
```

### Comparing `horde_sdk-0.5.0/pyproject.toml` & `horde_sdk-0.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "horde_sdk"
-version = "0.5.0"
+version = "0.5.2"
 description = "A python toolkit for interacting with the horde APIs, services, and ecosystem."
 authors = [
     {name = "tazlin", email = "tazlin.on.github@gmail.com"},
     {name = "db0", email = "mail@dbzer0.com"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
@@ -17,14 +17,15 @@
     "requests",
     "StrEnum",
     "loguru",
     "babel",
     "aiohttp",
     "aiodns",
     "pillow",
+    "python-dotenv",
 ]
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Development Status :: 2 - Pre-Alpha",
@@ -33,14 +34,15 @@
 [tool.setuptools.package-dir]
 horde_sdk = "horde_sdk"
 
 [project.urls]
 "Homepage" = "https://github.com/Haidra-Org/horde-sdk"
 
 [tool.setuptools.package-data]
+horde_sdk = ["py.typed", "lib.pyi"]
 tests = ["*.json"]
 
 [tool.ruff]
 line-length = 119
 select = ["A", "I", "E", "W", "F", "UP", "YTT", "B", "C4", "PIE", "RET", "SIM", "COM"] #, "D", "ANN"] # FIXME
 ignore = [
   # Ignore D rules for non-google docstring standard
```

### Comparing `horde_sdk-0.5.0/tests/ai_horde_api/test_ai_horde_api_calls.py` & `horde_sdk-0.5.2/tests/ai_horde_api/test_ai_horde_api_calls.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/ai_horde_api/test_ai_horde_api_models.py` & `horde_sdk-0.5.2/tests/ai_horde_api/test_ai_horde_api_models.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/ai_horde_api/test_dynamically_validate_against_swagger.py` & `horde_sdk-0.5.2/tests/ai_horde_api/test_dynamically_validate_against_swagger.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/ai_horde_api/test_swagger.py` & `horde_sdk-0.5.2/tests/ai_horde_api/test_swagger.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/conftest.py` & `horde_sdk-0.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_generate_async_post.json` & `horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_async_post.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_async_post.json` & `horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_async_post.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_production_responses/_v2_workers_get_200.json` & `horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_production_responses/_v2_workers_get_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_find_user_get_200.json` & `horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_find_user_get_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_pop_post_200.json` & `horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_pop_post_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_status_id_delete_200.json` & `horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_status_id_delete_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_status_id_get_200.json` & `horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_status_id_get_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_pop_post_200.json` & `horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_pop_post_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_teams_get_200.json` & `horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_teams_get_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_users_get_200.json` & `horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_users_get_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_users_user_id_get_200.json` & `horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_users_user_id_get_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_workers_get_200.json` & `horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_workers_get_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_get_200.json` & `horde_sdk-0.5.2/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_get_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_data/ai_horde_api/production_responses/ImgModelStats.json` & `horde_sdk-0.5.2/tests/test_data/ai_horde_api/production_responses/ImgModelStats.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_data/ai_horde_api/swagger.json` & `horde_sdk-0.5.2/tests/test_data/ai_horde_api/swagger.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_data/ratings_api/example_responses/ImageRatingsResponse.json` & `horde_sdk-0.5.2/tests/test_data/ratings_api/example_responses/ImageRatingsResponse.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_data/ratings_api/example_responses/UserRatingsResponse.json` & `horde_sdk-0.5.2/tests/test_data/ratings_api/example_responses/UserRatingsResponse.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_data/ratings_api/example_responses/UserValidateResponse.json` & `horde_sdk-0.5.2/tests/test_data/ratings_api/example_responses/UserValidateResponse.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_dynamically_check_apimodels.py` & `horde_sdk-0.5.2/tests/test_dynamically_check_apimodels.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.5.0/tests/test_ratings_api_models.py` & `horde_sdk-0.5.2/tests/test_ratings_api_models.py`

 * *Files identical despite different names*

