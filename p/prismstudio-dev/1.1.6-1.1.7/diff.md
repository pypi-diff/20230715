# Comparing `tmp/prismstudio-dev-1.1.6.tar.gz` & `tmp/prismstudio-dev-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prismstudio-dev-1.1.6.tar", last modified: Sun Jul  9 04:11:13 2023, max compression
+gzip compressed data, was "prismstudio-dev-1.1.7.tar", last modified: Sat Jul 15 01:01:27 2023, max compression
```

## Comparing `prismstudio-dev-1.1.6.tar` & `prismstudio-dev-1.1.7.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 04:11:13.992268 prismstudio-dev-1.1.6/
--rw-rw-r--   0 prism     (1000) prism     (1000)    23016 2023-07-07 08:31:20.000000 prismstudio-dev-1.1.6/LICENSE.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)      444 2023-07-09 04:11:13.992268 prismstudio-dev-1.1.6/PKG-INFO
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 04:11:13.988268 prismstudio-dev-1.1.6/prism/
--rw-rw-r--   0 prism     (1000) prism     (1000)     1177 2023-07-07 08:39:02.000000 prismstudio-dev-1.1.6/prism/__init__.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 04:11:13.988268 prismstudio-dev-1.1.6/prism/_common/
--rw-rw-r--   0 prism     (1000) prism     (1000)       28 2023-07-09 04:11:11.000000 prismstudio-dev-1.1.6/prism/_common/.env
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_common/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3459 2023-07-07 09:03:28.000000 prismstudio-dev-1.1.6/prism/_common/config.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    10161 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.6/prism/_common/const.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 04:11:13.988268 prismstudio-dev-1.1.6/prism/_core/
--rw-rw-r--   0 prism     (1000) prism     (1000)      251 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_core/__init__.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 04:11:13.988268 prismstudio-dev-1.1.6/prism/_core/_data/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_core/_data/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    41177 2023-06-16 00:01:45.000000 prismstudio-dev-1.1.6/prism/_core/_data/estimate.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     7950 2023-06-16 00:01:45.000000 prismstudio-dev-1.1.6/prism/_core/_data/event.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    70894 2023-07-07 05:15:34.000000 prismstudio-dev-1.1.6/prism/_core/_data/financial.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    12859 2023-06-27 09:00:21.000000 prismstudio-dev-1.1.6/prism/_core/_data/index.py
--rw-rw-r--   0 prism     (1000) prism     (1000)   121051 2023-06-16 00:01:45.000000 prismstudio-dev-1.1.6/prism/_core/_data/industry.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    36768 2023-07-07 02:42:51.000000 prismstudio-dev-1.1.6/prism/_core/_data/market.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     6446 2023-06-16 00:01:45.000000 prismstudio-dev-1.1.6/prism/_core/_data/precalculated.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3840 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.6/prism/_core/_data/securitymaster.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    15625 2023-06-15 23:39:09.000000 prismstudio-dev-1.1.6/prism/_core/_fn.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 04:11:13.992268 prismstudio-dev-1.1.6/prism/_core/_req_builder/
--rw-rw-r--   0 prism     (1000) prism     (1000)     1458 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_core/_req_builder/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1450 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_core/_req_builder/_auth.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    22657 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_core/_req_builder/_dataquery.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2058 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_core/_req_builder/_dbinfo.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     7633 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_core/_req_builder/_exportdata.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3633 2023-06-15 23:39:09.000000 prismstudio-dev-1.1.6/prism/_core/_req_builder/_gui.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    15003 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.6/prism/_core/_req_builder/_job.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     4582 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.6/prism/_core/_req_builder/_list.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    15321 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_core/_req_builder/_portfolio.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     4295 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_core/_req_builder/_securitymaster.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    25699 2023-06-15 23:39:09.000000 prismstudio-dev-1.1.6/prism/_core/_req_builder/_task.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    10877 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_core/_req_builder/_taskquery.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    24533 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.6/prism/_core/_req_builder/_universe.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     8696 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_core/_req_builder/preference.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     9606 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_core/ols.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 04:11:13.992268 prismstudio-dev-1.1.6/prism/_prismcomponent/
--rw-rw-r--   0 prism     (1000) prism     (1000)      353 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_prismcomponent/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     7323 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_prismcomponent/abstract_prismcomponent.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    14370 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.6/prism/_prismcomponent/datacomponent.py
--rw-rw-r--   0 prism     (1000) prism     (1000)   185597 2023-06-15 23:39:09.000000 prismstudio-dev-1.1.6/prism/_prismcomponent/prismcomponent.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    21567 2023-07-07 02:42:51.000000 prismstudio-dev-1.1.6/prism/_prismcomponent/taskcomponent.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 04:11:13.992268 prismstudio-dev-1.1.6/prism/_utils/
--rw-rw-r--   0 prism     (1000) prism     (1000)      480 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_utils/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2248 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_utils/auth_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3629 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_utils/exceptions.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2028 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_utils/loader.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3706 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_utils/prismcomponent_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     5532 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_utils/req_builder_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    14289 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_utils/validate_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     7232 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/prism/_utils/validate_utils_refactored.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1438 2023-07-07 02:42:51.000000 prismstudio-dev-1.1.6/prism/_utils/version.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 04:11:13.992268 prismstudio-dev-1.1.6/prismstudio_dev.egg-info/
--rw-rw-r--   0 prism     (1000) prism     (1000)      444 2023-07-09 04:11:13.000000 prismstudio-dev-1.1.6/prismstudio_dev.egg-info/PKG-INFO
--rw-rw-r--   0 prism     (1000) prism     (1000)     3042 2023-07-09 04:11:13.000000 prismstudio-dev-1.1.6/prismstudio_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)        1 2023-07-09 04:11:13.000000 prismstudio-dev-1.1.6/prismstudio_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)      256 2023-07-09 04:11:13.000000 prismstudio-dev-1.1.6/prismstudio_dev.egg-info/requires.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)       12 2023-07-09 04:11:13.000000 prismstudio-dev-1.1.6/prismstudio_dev.egg-info/top_level.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)       91 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/pyproject.toml
--rw-rw-r--   0 prism     (1000) prism     (1000)       38 2023-07-09 04:11:13.992268 prismstudio-dev-1.1.6/setup.cfg
--rw-rw-r--   0 prism     (1000) prism     (1000)     1341 2023-07-07 08:31:20.000000 prismstudio-dev-1.1.6/setup.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 04:11:13.992268 prismstudio-dev-1.1.6/tests/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/__init__.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 04:11:13.992268 prismstudio-dev-1.1.6/tests/test_util/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/__init__.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 04:11:13.992268 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2200 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_common_functions.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1539 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_fillna.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 04:11:13.992268 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     5990 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_01_frequency.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2004 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_02_datetype.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2719 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_03_periodtype.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1615 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_04_adjustment.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2304 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_05_shownid.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1946 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_06_rank_method.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2302 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_07_method.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     6448 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3854 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_09_contains_universename.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1717 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_10_contains_min_periods.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1118 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_11_base.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1792 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_12_preliminary.py
--rw-rw-r--   0 prism     (1000) prism     (1000)      889 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_13_setting.py
--rw-rw-r--   0 prism     (1000) prism     (1000)      956 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_14_settings.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1770 2023-07-07 02:42:51.000000 prismstudio-dev-1.1.6/tests/test_util/test_version.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/
+-rw-rw-r--   0 prism     (1000) prism     (1000)    23016 2023-07-09 08:09:32.000000 prismstudio-dev-1.1.7/LICENSE.txt
+-rw-rw-r--   0 prism     (1000) prism     (1000)      444 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/PKG-INFO
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/prism/
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1177 2023-07-07 08:39:02.000000 prismstudio-dev-1.1.7/prism/__init__.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/prism/_common/
+-rw-rw-r--   0 prism     (1000) prism     (1000)       28 2023-07-15 01:01:24.000000 prismstudio-dev-1.1.7/prism/_common/.env
+-rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_common/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3472 2023-07-09 08:26:49.000000 prismstudio-dev-1.1.7/prism/_common/config.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    10482 2023-07-15 01:00:00.000000 prismstudio-dev-1.1.7/prism/_common/const.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/prism/_core/
+-rw-rw-r--   0 prism     (1000) prism     (1000)      251 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/__init__.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/prism/_core/_data/
+-rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/_data/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    41177 2023-06-16 00:01:45.000000 prismstudio-dev-1.1.7/prism/_core/_data/estimate.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     7950 2023-06-16 00:01:45.000000 prismstudio-dev-1.1.7/prism/_core/_data/event.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    70894 2023-07-09 08:09:32.000000 prismstudio-dev-1.1.7/prism/_core/_data/financial.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    12927 2023-07-15 00:59:57.000000 prismstudio-dev-1.1.7/prism/_core/_data/index.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)   121051 2023-06-16 00:01:45.000000 prismstudio-dev-1.1.7/prism/_core/_data/industry.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    36768 2023-07-07 02:42:51.000000 prismstudio-dev-1.1.7/prism/_core/_data/market.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     6446 2023-06-16 00:01:45.000000 prismstudio-dev-1.1.7/prism/_core/_data/precalculated.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3840 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.7/prism/_core/_data/securitymaster.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    15625 2023-06-15 23:39:09.000000 prismstudio-dev-1.1.7/prism/_core/_fn.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/prism/_core/_req_builder/
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1458 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1450 2023-07-13 01:40:27.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_auth.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    22657 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_dataquery.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2058 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_dbinfo.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     7633 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_exportdata.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3633 2023-06-15 23:39:09.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_gui.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    15003 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_job.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     4582 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_list.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    15321 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_portfolio.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     4295 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_securitymaster.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    25699 2023-06-15 23:39:09.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_task.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    10877 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_taskquery.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    24533 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/_universe.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     8696 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/_req_builder/preference.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     9606 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_core/ols.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/prism/_prismcomponent/
+-rw-rw-r--   0 prism     (1000) prism     (1000)      353 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_prismcomponent/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     7644 2023-07-15 01:00:00.000000 prismstudio-dev-1.1.7/prism/_prismcomponent/abstract_prismcomponent.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    11256 2023-07-15 01:00:00.000000 prismstudio-dev-1.1.7/prism/_prismcomponent/datacomponent.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)   185816 2023-07-15 01:00:00.000000 prismstudio-dev-1.1.7/prism/_prismcomponent/prismcomponent.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    21567 2023-07-07 02:42:51.000000 prismstudio-dev-1.1.7/prism/_prismcomponent/taskcomponent.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/prism/_utils/
+-rw-rw-r--   0 prism     (1000) prism     (1000)      480 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_utils/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2248 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_utils/auth_utils.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3629 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_utils/exceptions.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2028 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_utils/loader.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3706 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_utils/prismcomponent_utils.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     5532 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_utils/req_builder_utils.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)    14289 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_utils/validate_utils.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     7232 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/prism/_utils/validate_utils_refactored.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1438 2023-07-07 02:42:51.000000 prismstudio-dev-1.1.7/prism/_utils/version.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/prismstudio_dev.egg-info/
+-rw-rw-r--   0 prism     (1000) prism     (1000)      444 2023-07-15 01:01:27.000000 prismstudio-dev-1.1.7/prismstudio_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3042 2023-07-15 01:01:27.000000 prismstudio-dev-1.1.7/prismstudio_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 prism     (1000) prism     (1000)        1 2023-07-15 01:01:27.000000 prismstudio-dev-1.1.7/prismstudio_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 prism     (1000) prism     (1000)      256 2023-07-15 01:01:27.000000 prismstudio-dev-1.1.7/prismstudio_dev.egg-info/requires.txt
+-rw-rw-r--   0 prism     (1000) prism     (1000)       12 2023-07-15 01:01:27.000000 prismstudio-dev-1.1.7/prismstudio_dev.egg-info/top_level.txt
+-rw-rw-r--   0 prism     (1000) prism     (1000)       91 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/pyproject.toml
+-rw-rw-r--   0 prism     (1000) prism     (1000)       38 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/setup.cfg
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1341 2023-07-09 08:09:32.000000 prismstudio-dev-1.1.7/setup.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/tests/
+-rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/__init__.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/tests/test_util/
+-rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/__init__.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/
+-rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2200 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_common_functions.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1539 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_fillna.py
+drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-15 01:01:27.633500 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/
+-rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/__init__.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     5990 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_01_frequency.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2004 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_02_datetype.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2719 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_03_periodtype.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1615 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_04_adjustment.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2304 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_05_shownid.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1946 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_06_rank_method.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     2302 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_07_method.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     6448 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     3854 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_09_contains_universename.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1717 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_10_contains_min_periods.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1118 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_11_base.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1792 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_12_preliminary.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)      889 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_13_setting.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)      956 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_14_settings.py
+-rw-rw-r--   0 prism     (1000) prism     (1000)     1770 2023-07-07 02:42:51.000000 prismstudio-dev-1.1.7/tests/test_util/test_version.py
```

### Comparing `prismstudio-dev-1.1.6/LICENSE.txt` & `prismstudio-dev-1.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/__init__.py` & `prismstudio-dev-1.1.7/prism/__init__.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_common/config.py` & `prismstudio-dev-1.1.7/prism/_common/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     DEVELOPMENT = "dev"
     STAGING = "stg"
     PRODUCTION = "production"
     DEMO = "demo"
 
 
 class StateSettings(BaseSettings):
-    ENV_STATE: str = 'production'
+    ENV_STATE: EnvironmentState = 'production'
     VERSION: str = '1.1.6'
     URL_STABLE: str = 'https://api.prism39.com'
     URL_DEV: str = 'https://ops.prism39.com'
     dev: str = ':30495'
     stg: str = ':30496'
     demo: str = ':40452'
```

### Comparing `prismstudio-dev-1.1.6/prism/_common/const.py` & `prismstudio-dev-1.1.7/prism/_common/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     'BeyondType',
     'COMPONENT2CATEGORY',
     'FUNCTIONS',
     'FILEEXTENSION',
     'AggregateComponents',
     'PACKAGE_NAME',
     'SPECIALVALUEMAP',
+    'DataCategoryType',
 ]
 
 BEGINNING_DATE = pd.to_datetime('1700-01-01')
 ACTIVE_DATE = pd.to_datetime('2199-12-31')
 
 
 class PrismComponentType(str, Enum):
@@ -127,14 +128,27 @@
 
 class TaskComponentType(str, Enum):
     SCREEN = 'screen'
     FACTOR_BACKTEST = 'factor_backtest'
     STRATEGY_BACKTEST = 'strategy_backtest'
     EXPORT_DATA = 'export_data'
 
+
+class DataCategoryType(str, Enum):
+    FINANCIAL = "Financial"
+    PRECALCAULATED = "Precalculated"
+    EVENT = "Event"
+    SM = "Securitymaster"
+    MARKET = "Market"
+    ESTIMATE = "Estimate"
+    INDEX = "Index"
+    INDUSTRY_ESTIMATE = "Industry Estimate"
+    INDUSTRY_FINANCIAL = "Industry"
+
+
 class FinancialDataComponentType(str, Enum):
     BALANCE_SHEET = 'Balance Sheet'
     CASH_FLOW = 'Cash Flow'
     DPS = 'DPS'
     EPS = 'EPS'
     FINANCIAL_DATE = 'Financial Date'
     INCOME_STATEMENT = 'Income Statement'
```

### Comparing `prismstudio-dev-1.1.6/prism/_core/_data/estimate.py` & `prismstudio-dev-1.1.7/prism/_core/_data/estimate.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_data/event.py` & `prismstudio-dev-1.1.7/prism/_core/_data/event.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_data/financial.py` & `prismstudio-dev-1.1.7/prism/_core/_data/financial.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_data/index.py` & `prismstudio-dev-1.1.7/prism/_core/_data/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,16 @@
     | Default frequency is business daily.
 
     Parameters
     ----------
         dataitemid : int
             | Unique identifier for the different data item. This identifies the type of the balance sheet value (Revenue, Expense, etc.)
 
-        leveltype : str, {'Price Return', 'Total Return Gross'}
+        leveltype : str, default None, {'Price Return', 'Total Return Gross'}
+            | Default value None gives all leveltype.
 
     Returns
     -------
         prism._PrismComponent
 
     Examples
     --------
```

### Comparing `prismstudio-dev-1.1.6/prism/_core/_data/industry.py` & `prismstudio-dev-1.1.7/prism/_core/_data/industry.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_data/market.py` & `prismstudio-dev-1.1.7/prism/_core/_data/market.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_data/precalculated.py` & `prismstudio-dev-1.1.7/prism/_core/_data/precalculated.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_data/securitymaster.py` & `prismstudio-dev-1.1.7/prism/_core/_data/securitymaster.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_fn.py` & `prismstudio-dev-1.1.7/prism/_core/_fn.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_req_builder/__init__.py` & `prismstudio-dev-1.1.7/prism/_core/_req_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_req_builder/_auth.py` & `prismstudio-dev-1.1.7/prism/_core/_req_builder/_auth.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_req_builder/_dataquery.py` & `prismstudio-dev-1.1.7/prism/_core/_req_builder/_dataquery.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_req_builder/_dbinfo.py` & `prismstudio-dev-1.1.7/prism/_core/_req_builder/_dbinfo.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_req_builder/_exportdata.py` & `prismstudio-dev-1.1.7/prism/_core/_req_builder/_exportdata.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_req_builder/_gui.py` & `prismstudio-dev-1.1.7/prism/_core/_req_builder/_gui.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_req_builder/_job.py` & `prismstudio-dev-1.1.7/prism/_core/_req_builder/_job.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_req_builder/_list.py` & `prismstudio-dev-1.1.7/prism/_core/_req_builder/_list.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_req_builder/_portfolio.py` & `prismstudio-dev-1.1.7/prism/_core/_req_builder/_portfolio.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_req_builder/_securitymaster.py` & `prismstudio-dev-1.1.7/prism/_core/_req_builder/_securitymaster.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_req_builder/_task.py` & `prismstudio-dev-1.1.7/prism/_core/_req_builder/_task.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_req_builder/_taskquery.py` & `prismstudio-dev-1.1.7/prism/_core/_req_builder/_taskquery.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_req_builder/_universe.py` & `prismstudio-dev-1.1.7/prism/_core/_req_builder/_universe.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/_req_builder/preference.py` & `prismstudio-dev-1.1.7/prism/_core/_req_builder/preference.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_core/ols.py` & `prismstudio-dev-1.1.7/prism/_core/ols.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_prismcomponent/abstract_prismcomponent.py` & `prismstudio-dev-1.1.7/prism/_prismcomponent/abstract_prismcomponent.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,23 +22,27 @@
     def __init__(
         self,
         *,
         component_type: str,
         component_name: str,
         component_args: dict = {},
         children: list,
+        component_category: str = None,
         nodeid: UUID = None,
         query_name: str = None,
     ):
         # if not hasattr(self, '_func_name'): self._func_name = func_name
         if component_type == PrismComponentType.FUNCTION_COMPONENT:
             if not hasattr(self, "_component_name"):
                 self._component_name = component_name
+            if not hasattr(self, "_component_category"):
+                self._component_category = component_category
         self._query = {
             "component_type": component_type,
+            "component_category": component_category,
             "component_name": component_name,
             "component_args": component_args,
             "children": children,
             "nodeid": nodeid,
         }
         try:
             json.dumps(self._query)
@@ -59,15 +63,15 @@
             except:
                 pass
         else:
             try:
                 print(
                     "\t" * depth,
                     "====",
-                    query["component_name"],
+                    query["component_category"] + "/" + query["component_name"] if query["component_category"] is not None else query["component_name"],
                 )
                 if len(query["component_args"]) > 0:
                     print(
                         "\t" * (depth + 1),
                         "parameters: {",
                     )
                     for k, v in query["component_args"].items():
```

### Comparing `prismstudio-dev-1.1.6/prism/_prismcomponent/prismcomponent.py` & `prismstudio-dev-1.1.7/prism/_prismcomponent/prismcomponent.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
             755975  344286611  2011-10-31   45.6     ITT
         """
         ...
 
     @operation
     def floor(self):
         """
-        The floor value of each element. The floor of x i.e., the largest integer not greater than x. 
+        The floor value of each element. The floor of x i.e., the largest integer not greater than x.
 
         Returns
         -------
             prism._PrismComponent
                 The floor of each element, with ``float`` dtype. This is a scalar if element is a scalar.
 
         Examples
@@ -4168,14 +4168,15 @@
 
     _component_type = PrismComponentType.DATA_COMPONENT
 
     def __init__(self, **kwargs):
         component_args = dict(kwargs)
         query = {
             "component_type": self._component_type,
+            "component_category": self._component_category,
             "component_name": self._component_name,
             "component_args": component_args,
             "children": [],
             "nodeid": str(uuid.uuid4()),
         }
         val_res = requests.post(url=URL_DATAQUERIES + "/validate", json=query, headers=_authentication())
         if val_res.status_code >= 400:
@@ -4193,18 +4194,29 @@
 
     @property
     @classmethod
     @abstractmethod
     def _component_name():
         raise NotImplementedError()
 
+
+    @property
+    @classmethod
+    @abstractmethod
+    def _component_category():
+        raise NotImplementedError()
+
+
     def __setattr__(self, name, value):
         if name == "_component_name":
             raise AttributeError("Can't modify {}".format(name))
 
+        if name == "_component_category":
+            raise AttributeError("Can't modify {}".format(name))
+
         super().__setattr__(name, value)
 
 
 class _PrismTaskComponent(_AbstractPrismComponent, ABC):
     _component_type = PrismComponentType.TASK_COMPONENT
 
     def __init__(self, **kwargs):
@@ -4241,16 +4253,14 @@
             "component_args": component_args,
             "children": [],
         }
         super().__init__(**query)
 
 
 class _PrismFinancialComponent(_PrismComponent):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
 
     @_validate_args
     @n_period_operation
     @operation
     def n_fiscal_quarters_max(self, n: int, weights: list = None):
         """
         Return the maximum of the values over given fiscal quarter n.
```

### Comparing `prismstudio-dev-1.1.6/prism/_prismcomponent/taskcomponent.py` & `prismstudio-dev-1.1.7/prism/_prismcomponent/taskcomponent.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_utils/auth_utils.py` & `prismstudio-dev-1.1.7/prism/_utils/auth_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_utils/exceptions.py` & `prismstudio-dev-1.1.7/prism/_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_utils/loader.py` & `prismstudio-dev-1.1.7/prism/_utils/loader.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_utils/prismcomponent_utils.py` & `prismstudio-dev-1.1.7/prism/_utils/prismcomponent_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_utils/req_builder_utils.py` & `prismstudio-dev-1.1.7/prism/_utils/req_builder_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_utils/validate_utils.py` & `prismstudio-dev-1.1.7/prism/_utils/validate_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_utils/validate_utils_refactored.py` & `prismstudio-dev-1.1.7/prism/_utils/validate_utils_refactored.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prism/_utils/version.py` & `prismstudio-dev-1.1.7/prism/_utils/version.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/prismstudio_dev.egg-info/SOURCES.txt` & `prismstudio-dev-1.1.7/prismstudio_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/setup.py` & `prismstudio-dev-1.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_common_functions.py` & `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_common_functions.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_fillna.py` & `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_fillna.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_01_frequency.py` & `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_01_frequency.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_02_datetype.py` & `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_02_datetype.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_03_periodtype.py` & `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_03_periodtype.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_04_adjustment.py` & `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_04_adjustment.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_05_shownid.py` & `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_05_shownid.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_06_rank_method.py` & `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_06_rank_method.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_07_method.py` & `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_07_method.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py` & `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_09_contains_universename.py` & `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_09_contains_universename.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_10_contains_min_periods.py` & `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_10_contains_min_periods.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_11_base.py` & `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_11_base.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_12_preliminary.py` & `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_12_preliminary.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_13_setting.py` & `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_13_setting.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/tests/test_util/test__validate_args/test_params/test_param_14_settings.py` & `prismstudio-dev-1.1.7/tests/test_util/test__validate_args/test_params/test_param_14_settings.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.6/tests/test_util/test_version.py` & `prismstudio-dev-1.1.7/tests/test_util/test_version.py`

 * *Files identical despite different names*

