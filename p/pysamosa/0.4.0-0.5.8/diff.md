# Comparing `tmp/pysamosa-0.4.0.tar.gz` & `tmp/pysamosa-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysamosa-0.4.0.tar", last modified: Fri Jun 23 09:14:43 2023, max compression
+gzip compressed data, was "pysamosa-0.5.8.tar", last modified: Sat Jul 15 04:49:19 2023, max compression
```

## Comparing `pysamosa-0.4.0.tar` & `pysamosa-0.5.8.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-23 09:14:43.218287 pysamosa-0.4.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7651 2023-06-23 09:07:23.000000 pysamosa-0.4.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)      306 2023-06-23 09:07:23.000000 pysamosa-0.4.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    13974 2023-06-23 09:14:43.218287 pysamosa-0.4.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    12753 2023-06-23 09:07:23.000000 pysamosa-0.4.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-23 09:14:43.174284 pysamosa-0.4.0/notebooks/
--rw-rw-r--   0 travis    (2000) travis    (2000)  1309734 2023-06-23 09:07:23.000000 pysamosa-0.4.0/notebooks/retracking_example.ipynb
--rw-rw-r--   0 travis    (2000) travis    (2000)      132 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-23 09:14:43.198285 pysamosa-0.4.0/pysamosa/
--rw-rw-r--   0 travis    (2000) travis    (2000)      184 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12843 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/common_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      334 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/conf_params.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26159 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/data_access.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3162 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/dist2coast.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      462 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/download_aux_data.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5229 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/l1b_simulator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3086 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/leading_edge_detector.py
--rw-rw-r--   0 travis    (2000) travis    (2000)  9928947 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/luts_samosa.pickle
--rw-rw-r--   0 travis    (2000) travis    (2000)     6053 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/main_coastalffsar.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6164 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/main_coral_paper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1862 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/main_cs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1532 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/main_s3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1737 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/main_s6.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2731 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/main_s6jtex.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2987 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/main_s6jtex_raw_vs_rmc.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17889 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1614 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/model_helpers.pyx
--rw-rw-r--   0 travis    (2000) travis    (2000)     7209 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/montecarlo_simulator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/pysamosa.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1622 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/qual_flag_estimator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24082 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/retracker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12275 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/retracker_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23266 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/retracker_processor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6887 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/rip.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      232 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/settings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3527 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/settings_manager.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1684 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/simple_logger.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9195 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       47 2023-06-23 09:07:23.000000 pysamosa-0.4.0/pysamosa/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-23 09:14:43.198285 pysamosa-0.4.0/pysamosa.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13974 2023-06-23 09:14:43.000000 pysamosa-0.4.0/pysamosa.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1855 2023-06-23 09:14:43.000000 pysamosa-0.4.0/pysamosa.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-23 09:14:43.000000 pysamosa-0.4.0/pysamosa.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-23 09:14:43.000000 pysamosa-0.4.0/pysamosa.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2023-06-23 09:14:43.000000 pysamosa-0.4.0/pysamosa.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2023-06-23 09:14:43.000000 pysamosa-0.4.0/pysamosa.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      308 2023-06-23 09:07:23.000000 pysamosa-0.4.0/requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-23 09:14:43.198285 pysamosa-0.4.0/scripts/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1671 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/cs_l2_conversion.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-23 09:14:43.214287 pysamosa-0.4.0/scripts/luts/
--rw-rw-r--   0 travis    (2000) travis    (2000)   217134 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/luts/AUX_RLUT_S6A_002.nc
--rw-rw-r--   0 travis    (2000) travis    (2000)   214215 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/luts/AUX_RLUT_S6A_003.nc
--rwxrwxr-x   0 travis    (2000) travis    (2000)  4818008 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/luts/F0.txt
--rwxrwxr-x   0 travis    (2000) travis    (2000)  4827430 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/luts/F1.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    30520 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/luts/LUT_Alpha_P_CS-2.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)   993604 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC
--rw-rw-r--   0 travis    (2000) travis    (2000)    30520 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/luts/convert_luts.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9610 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/thesis_plots.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6110 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/track_browser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9809 2023-06-23 09:07:23.000000 pysamosa-0.4.0/scripts/track_browser_footprint.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      436 2023-06-23 09:14:43.222287 pysamosa-0.4.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2405 2023-06-23 09:07:23.000000 pysamosa-0.4.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-23 09:14:43.218287 pysamosa-0.4.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10885 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2431 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/settings_dumper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2429 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_common_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3305 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_dist2coast.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5903 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_dynamic_fg_epoch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4328 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_l1b_sim_retracker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2093 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_l1b_simulator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1253 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_leading_edge_detector.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9363 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9434 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_montecarlo_sim.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8236 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_retrack_multi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9035 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_retrack_single.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4791 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_samplusplus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1111 2023-06-23 09:07:23.000000 pysamosa-0.4.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:49:19.290581 pysamosa-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-15 04:49:07.000000 pysamosa-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-15 04:49:07.000000 pysamosa-0.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-07-15 04:49:19.290581 pysamosa-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-07-15 04:49:07.000000 pysamosa-0.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:49:19.246581 pysamosa-0.5.8/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)  1309734 2023-07-15 04:49:07.000000 pysamosa-0.5.8/notebooks/retracking_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:49:19.266581 pysamosa-0.5.8/pysamosa/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/conf_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26159 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/data_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/dist2coast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/download_aux_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/l1b_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/leading_edge_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)  9928947 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/luts_samosa.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/main_coastalffsar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/main_coral_paper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/main_cs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/main_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/main_s6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/main_s6jtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/main_s6jtex_raw_vs_rmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17889 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/model_helpers.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/montecarlo_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/pysamosa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/qual_flag_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24082 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/retracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/retracker_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/retracker_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/rip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/settings_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/simple_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-15 04:49:07.000000 pysamosa-0.5.8/pysamosa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:49:19.266581 pysamosa-0.5.8/pysamosa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-07-15 04:49:19.000000 pysamosa-0.5.8/pysamosa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-15 04:49:19.000000 pysamosa-0.5.8/pysamosa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 04:49:19.000000 pysamosa-0.5.8/pysamosa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 04:49:18.000000 pysamosa-0.5.8/pysamosa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-15 04:49:19.000000 pysamosa-0.5.8/pysamosa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-15 04:49:19.000000 pysamosa-0.5.8/pysamosa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-15 04:49:07.000000 pysamosa-0.5.8/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:49:19.270581 pysamosa-0.5.8/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-15 04:49:07.000000 pysamosa-0.5.8/scripts/cs_l2_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:49:19.286581 pysamosa-0.5.8/scripts/luts/
+-rw-r--r--   0 runner    (1001) docker     (123)   217134 2023-07-15 04:49:07.000000 pysamosa-0.5.8/scripts/luts/AUX_RLUT_S6A_002.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   214215 2023-07-15 04:49:07.000000 pysamosa-0.5.8/scripts/luts/AUX_RLUT_S6A_003.nc
+-rwxr-xr-x   0 runner    (1001) docker     (123)  4818008 2023-07-15 04:49:07.000000 pysamosa-0.5.8/scripts/luts/F0.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)  4827430 2023-07-15 04:49:07.000000 pysamosa-0.5.8/scripts/luts/F1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    30520 2023-07-15 04:49:07.000000 pysamosa-0.5.8/scripts/luts/LUT_Alpha_P_CS-2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   993604 2023-07-15 04:49:07.000000 pysamosa-0.5.8/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC
+-rw-r--r--   0 runner    (1001) docker     (123)    30520 2023-07-15 04:49:07.000000 pysamosa-0.5.8/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-15 04:49:07.000000 pysamosa-0.5.8/scripts/luts/convert_luts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9610 2023-07-15 04:49:07.000000 pysamosa-0.5.8/scripts/thesis_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-15 04:49:07.000000 pysamosa-0.5.8/scripts/track_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9809 2023-07-15 04:49:07.000000 pysamosa-0.5.8/scripts/track_browser_footprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-15 04:49:19.290581 pysamosa-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-15 04:49:07.000000 pysamosa-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 04:49:19.290581 pysamosa-0.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 04:49:07.000000 pysamosa-0.5.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10885 2023-07-15 04:49:07.000000 pysamosa-0.5.8/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-15 04:49:07.000000 pysamosa-0.5.8/tests/settings_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-15 04:49:07.000000 pysamosa-0.5.8/tests/test_common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-15 04:49:07.000000 pysamosa-0.5.8/tests/test_dist2coast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-15 04:49:07.000000 pysamosa-0.5.8/tests/test_dynamic_fg_epoch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-07-15 04:49:07.000000 pysamosa-0.5.8/tests/test_l1b_sim_retracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-15 04:49:07.000000 pysamosa-0.5.8/tests/test_l1b_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-15 04:49:07.000000 pysamosa-0.5.8/tests/test_leading_edge_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9393 2023-07-15 04:49:07.000000 pysamosa-0.5.8/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-07-15 04:49:07.000000 pysamosa-0.5.8/tests/test_montecarlo_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-07-15 04:49:07.000000 pysamosa-0.5.8/tests/test_retrack_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-07-15 04:49:07.000000 pysamosa-0.5.8/tests/test_retrack_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-15 04:49:07.000000 pysamosa-0.5.8/tests/test_samplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-15 04:49:07.000000 pysamosa-0.5.8/tests/test_utils.py
```

### Comparing `pysamosa-0.4.0/LICENSE` & `pysamosa-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/PKG-INFO` & `pysamosa-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysamosa
-Version: 0.4.0
+Version: 0.5.8
 Summary: PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation.
 Home-page: https://github.com/floschl/pysamosa
 Author: Florian Schlembach
 Author-email: florian.schlembach@tum.de
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: satellite altimetry retracking samosa+ samosa coastal open ocean sentinel esasar altimetry ff-sar fully focused
 Classifier: Development Status :: 4 - Beta
@@ -18,18 +18,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PySAMOSA
 
-[![Build Status](https://app.travis-ci.com/floschl/pysamosa.svg?branch=main)](https://app.travis-ci.com/floschl/pysamosa)
+![CI](https://github.com/floschl/pysamosa/actions/workflows/ci.yml/badge.svg)
+![Release](https://github.com/floschl/pysamosa/actions/workflows/release.yml/badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/pysamosa)
 [![DOI](https://zenodo.org/badge/646028227.svg)](https://zenodo.org/badge/latestdoi/646028227)
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 
 ![]() <div align="center"><img src="https://github.com/floschl/pysamosa/blob/main/resources/logo_name.png?raw=true"
 width="500"></div>
 
 PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to
 measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation. More details on satellite altimetry can be found in this [PDF](https://www.altimetry.info/file/Radar_Altimetry_Tutorial.pdf).
 
@@ -129,25 +130,14 @@
 
     $ git clone {repo_url}
 
 Enter cloned directory
 
     $ cd pysamosa
 
-Create your isolated Python environment, e.g. anything from Python 3.8
-either via conda
-
-    $ conda create -n pysamosa python=3.8 pip
-
-or via pyenv/pipenv/venv.
-
-Activate pysamosa conda environment
-
-    $ conda activate pysamosa
-
 Install dependencies into your conda env/virtualenv
 
     $ pip install -r requirements.txt
 
 Compile the .pyx files (e.g. model_helpers.pyx) by running cython to build the extensions
 For Windows users: An installed C/C++ compiler may be required for installation, e.g. MSCV, which comes with
 the free [Visual Studio Community](https://visualstudio.microsoft.com/vs/community/)
```

### Comparing `pysamosa-0.4.0/README.md` & `pysamosa-0.5.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # PySAMOSA
 
-[![Build Status](https://app.travis-ci.com/floschl/pysamosa.svg?branch=main)](https://app.travis-ci.com/floschl/pysamosa)
+![CI](https://github.com/floschl/pysamosa/actions/workflows/ci.yml/badge.svg)
+![Release](https://github.com/floschl/pysamosa/actions/workflows/release.yml/badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/pysamosa)
 [![DOI](https://zenodo.org/badge/646028227.svg)](https://zenodo.org/badge/latestdoi/646028227)
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 
 ![]() <div align="center"><img src="https://github.com/floschl/pysamosa/blob/main/resources/logo_name.png?raw=true"
 width="500"></div>
 
 PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to
 measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation. More details on satellite altimetry can be found in this [PDF](https://www.altimetry.info/file/Radar_Altimetry_Tutorial.pdf).
 
@@ -107,25 +108,14 @@
 
     $ git clone {repo_url}
 
 Enter cloned directory
 
     $ cd pysamosa
 
-Create your isolated Python environment, e.g. anything from Python 3.8
-either via conda
-
-    $ conda create -n pysamosa python=3.8 pip
-
-or via pyenv/pipenv/venv.
-
-Activate pysamosa conda environment
-
-    $ conda activate pysamosa
-
 Install dependencies into your conda env/virtualenv
 
     $ pip install -r requirements.txt
 
 Compile the .pyx files (e.g. model_helpers.pyx) by running cython to build the extensions
 For Windows users: An installed C/C++ compiler may be required for installation, e.g. MSCV, which comes with
 the free [Visual Studio Community](https://visualstudio.microsoft.com/vs/community/)
```

### Comparing `pysamosa-0.4.0/notebooks/retracking_example.ipynb` & `pysamosa-0.5.8/notebooks/retracking_example.ipynb`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/common_types.py` & `pysamosa-0.5.8/pysamosa/common_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from enum import Enum
 from pathlib import Path
 from typing import Optional
 
 import numpy as np
-from pydantic import BaseModel, root_validator, validator
+from pydantic import BaseModel, model_validator
 
 
 class SensorType(Enum):
     S3 = "s3"
     CS = "cs"
     S6_F04 = "s6_f04"
     S6_F06 = "s6_f06"
@@ -81,17 +81,18 @@
         return sensor_sets
 
 
 SENSOR_SETS_DEFAULT_S3 = SensorSettings.get_default_sets(SensorType.S3)
 
 
 class WaveformSettings(BaseModel):
-    zp_oversampling_factor: int = None
+    zp_oversampling_factor: int = 1
     internal_oversampling_factor: int = 1
-    np: Optional[int]
+    # np: Optional[int]
+    np: int = None
 
     def get_default_src_type(st: L1bSourceType, **kwargs):
         if st is L1bSourceType.GPOD:
             return WaveformSettings(
                 **{**{"zp_oversampling_factor": 2, "np": 256, **kwargs}}
             )
         elif st is L1bSourceType.EUM_S3:
@@ -103,26 +104,19 @@
                 **{**{"zp_oversampling_factor": 2, "np": 128, **kwargs}}
             )
         elif "s6" in str(st).lower():
             return WaveformSettings(
                 **{**{"zp_oversampling_factor": 2, "np": 256, **kwargs}}
             )
 
-    @validator("zp_oversampling_factor", pre=True, always=True)
-    def set_default_zp_oversampling_factor(cls, v, *, values, **kwargs):
-        return v or 1
-
-    @validator("np", pre=True, always=True)
-    def set_default_np(cls, v, *, values, **kwargs):
-        np = 128 if v is None else v
-        return (
-            np
-            * values["zp_oversampling_factor"]
-            * values["internal_oversampling_factor"]
-        )
+    @model_validator(mode="after")
+    def set_def_np(self):
+        np = self.np if self.np is not None else 128
+        self.np = np * self.zp_oversampling_factor * self.internal_oversampling_factor
+        return self
 
 
 class RetrackerProcessorSettings(BaseModel):
     n_offset: int = 0
     n_inds: int = 5  # 0 = all
     n_procs: int = None  # None = all available
     nc_dest_dir: Path = Path().cwd().parent / ".testrun"
@@ -220,24 +214,24 @@
     beam_ang_stack_rad: np.ndarray = np.array([])
     epoch_ref_gate: float = 65.0
     dist2coast: float = 42.0
     rip: np.ndarray = np.array([])
     pri_hz: Optional[float] = None
     stack_mask_start_stop: Optional[np.ndarray] = None
 
-    @root_validator(pre=True)
-    def warning_defaults(cls, values):
-        fields_not_set = [f for f in cls.__fields__ if f not in values]
+    @model_validator(mode="before")
+    def warning_defaults(cls, data):
+        fields_not_set = [f for f in cls.model_fields if f not in data]
         if fields_not_set:
             logging.debug(
                 "WARNING: the following params were not set, now taking defaults: {}".format(
                     ",".join(fields_not_set)
                 )
             )
-        return values
+        return data
 
     class Config:
         arbitrary_types_allowed = True
 
 
 class ModelSettings(BaseModel):
     # flag to disable the computation of first order term in the SAMOSA model
```

### Comparing `pysamosa-0.4.0/pysamosa/data_access.py` & `pysamosa-0.5.8/pysamosa/data_access.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/dist2coast.py` & `pysamosa-0.5.8/pysamosa/dist2coast.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/l1b_simulator.py` & `pysamosa-0.5.8/pysamosa/l1b_simulator.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/leading_edge_detector.py` & `pysamosa-0.5.8/pysamosa/leading_edge_detector.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/luts_samosa.pickle` & `pysamosa-0.5.8/pysamosa/luts_samosa.pickle`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/main_coastalffsar.py` & `pysamosa-0.5.8/pysamosa/main_coastalffsar.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/main_coral_paper.py` & `pysamosa-0.5.8/pysamosa/main_coral_paper.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/main_cs.py` & `pysamosa-0.5.8/pysamosa/main_cs.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/main_s3.py` & `pysamosa-0.5.8/pysamosa/main_s3.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/main_s6.py` & `pysamosa-0.5.8/pysamosa/main_s6.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/main_s6jtex.py` & `pysamosa-0.5.8/pysamosa/main_s6jtex.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/main_s6jtex_raw_vs_rmc.py` & `pysamosa-0.5.8/pysamosa/main_s6jtex_raw_vs_rmc.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/model.py` & `pysamosa-0.5.8/pysamosa/model.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/model_helpers.pyx` & `pysamosa-0.5.8/pysamosa/model_helpers.pyx`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/montecarlo_simulator.py` & `pysamosa-0.5.8/pysamosa/montecarlo_simulator.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/qual_flag_estimator.py` & `pysamosa-0.5.8/pysamosa/qual_flag_estimator.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/retracker.py` & `pysamosa-0.5.8/pysamosa/retracker.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/retracker_helpers.py` & `pysamosa-0.5.8/pysamosa/retracker_helpers.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/retracker_processor.py` & `pysamosa-0.5.8/pysamosa/retracker_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -529,22 +529,20 @@
             self.output_l2 = ds_reduced
 
             logging.info(
                 f"processed L2 dataset reduced by factor {self.rp_sets.reduce_l2_factor}. "
             )
 
     def write_settings_log_file(self):
-        json_params = {"indent": 4, "separators": (",", ": ")}
-
         all_sets = ExportSettings(
             rp_sets=self.rp_sets,
             retrack_sets=self.retrack_sets,
             fitting_sets=self.fitting_sets,
             sensor_sets=self.sensor_sets,
         )
 
         dest_filepath_json = self.rp_sets.nc_dest_dir / "settings.json"
         os.umask(0)
         dest_filepath_json.parent.mkdir(parents=True, exist_ok=True)
 
         with open(dest_filepath_json, "w") as f:
-            f.write(all_sets.json(**json_params))
+            f.write(all_sets.model_dump_json(indent=4))
```

### Comparing `pysamosa-0.4.0/pysamosa/rip.py` & `pysamosa-0.5.8/pysamosa/rip.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/settings_manager.py` & `pysamosa-0.5.8/pysamosa/settings_manager.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/simple_logger.py` & `pysamosa-0.5.8/pysamosa/simple_logger.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa/utils.py` & `pysamosa-0.5.8/pysamosa/utils.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/pysamosa.egg-info/PKG-INFO` & `pysamosa-0.5.8/pysamosa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysamosa
-Version: 0.4.0
+Version: 0.5.8
 Summary: PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation.
 Home-page: https://github.com/floschl/pysamosa
 Author: Florian Schlembach
 Author-email: florian.schlembach@tum.de
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Keywords: satellite altimetry retracking samosa+ samosa coastal open ocean sentinel esasar altimetry ff-sar fully focused
 Classifier: Development Status :: 4 - Beta
@@ -18,18 +18,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PySAMOSA
 
-[![Build Status](https://app.travis-ci.com/floschl/pysamosa.svg?branch=main)](https://app.travis-ci.com/floschl/pysamosa)
+![CI](https://github.com/floschl/pysamosa/actions/workflows/ci.yml/badge.svg)
+![Release](https://github.com/floschl/pysamosa/actions/workflows/release.yml/badge.svg)
 ![PyPI](https://img.shields.io/pypi/v/pysamosa)
 [![DOI](https://zenodo.org/badge/646028227.svg)](https://zenodo.org/badge/latestdoi/646028227)
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 
 ![]() <div align="center"><img src="https://github.com/floschl/pysamosa/blob/main/resources/logo_name.png?raw=true"
 width="500"></div>
 
 PySAMOSA is a software framework for processing open ocean and coastal waveforms from SAR satellite altimetry to
 measure sea surface heights, wave heights, and wind speed for the oceans and inland water bodies. Satellite altimetry is a space-borne remote sensing technique used for Earth observation. More details on satellite altimetry can be found in this [PDF](https://www.altimetry.info/file/Radar_Altimetry_Tutorial.pdf).
 
@@ -129,25 +130,14 @@
 
     $ git clone {repo_url}
 
 Enter cloned directory
 
     $ cd pysamosa
 
-Create your isolated Python environment, e.g. anything from Python 3.8
-either via conda
-
-    $ conda create -n pysamosa python=3.8 pip
-
-or via pyenv/pipenv/venv.
-
-Activate pysamosa conda environment
-
-    $ conda activate pysamosa
-
 Install dependencies into your conda env/virtualenv
 
     $ pip install -r requirements.txt
 
 Compile the .pyx files (e.g. model_helpers.pyx) by running cython to build the extensions
 For Windows users: An installed C/C++ compiler may be required for installation, e.g. MSCV, which comes with
 the free [Visual Studio Community](https://visualstudio.microsoft.com/vs/community/)
```

### Comparing `pysamosa-0.4.0/pysamosa.egg-info/SOURCES.txt` & `pysamosa-0.5.8/pysamosa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/scripts/cs_l2_conversion.py` & `pysamosa-0.5.8/scripts/cs_l2_conversion.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/scripts/luts/AUX_RLUT_S6A_002.nc` & `pysamosa-0.5.8/scripts/luts/AUX_RLUT_S6A_002.nc`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/scripts/luts/AUX_RLUT_S6A_003.nc` & `pysamosa-0.5.8/scripts/luts/AUX_RLUT_S6A_003.nc`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/scripts/luts/F0.txt` & `pysamosa-0.5.8/scripts/luts/F0.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/scripts/luts/F1.txt` & `pysamosa-0.5.8/scripts/luts/F1.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/scripts/luts/LUT_Alpha_P_CS-2.txt` & `pysamosa-0.5.8/scripts/luts/LUT_Alpha_P_CS-2.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC` & `pysamosa-0.5.8/scripts/luts/S6A_TEST_AUX_FLUT___00000000T000000_99999999T999999_0001.NC`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt` & `pysamosa-0.5.8/scripts/luts/alphap_table_SEN3_09_Nov_2017.txt`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/scripts/luts/convert_luts.py` & `pysamosa-0.5.8/scripts/luts/convert_luts.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/scripts/thesis_plots.py` & `pysamosa-0.5.8/scripts/thesis_plots.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/scripts/track_browser.py` & `pysamosa-0.5.8/scripts/track_browser.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/scripts/track_browser_footprint.py` & `pysamosa-0.5.8/scripts/track_browser_footprint.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/setup.py` & `pysamosa-0.5.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,11 +65,11 @@
     "sar altimetry ff-sar fully focused",
     name="pysamosa",
     packages=find_packages(include=["pysamosa", "pysamosa.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     ext_modules=extensions,
     url="https://github.com/floschl/pysamosa",
-    version="0.4.0",
+    version="0.5.8",
     zip_safe=False,
     setup_requires=[],
 )
```

### Comparing `pysamosa-0.4.0/tests/helpers.py` & `pysamosa-0.5.8/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/tests/settings_dumper.py` & `pysamosa-0.5.8/tests/settings_dumper.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/tests/test_common_types.py` & `pysamosa-0.5.8/tests/test_common_types.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/tests/test_dist2coast.py` & `pysamosa-0.5.8/tests/test_dist2coast.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/tests/test_dynamic_fg_epoch.py` & `pysamosa-0.5.8/tests/test_dynamic_fg_epoch.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/tests/test_l1b_sim_retracker.py` & `pysamosa-0.5.8/tests/test_l1b_sim_retracker.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/tests/test_l1b_simulator.py` & `pysamosa-0.5.8/tests/test_l1b_simulator.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/tests/test_leading_edge_detector.py` & `pysamosa-0.5.8/tests/test_leading_edge_detector.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/tests/test_model.py` & `pysamosa-0.5.8/tests/test_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from pysamosa.retracker import oversample_wf
 
 
 def test_setting_model_parameter_obj():
     mp = ModelParameter(ascending=True)
     print(mp)
     assert mp
+    assert mp.alt_m == 815000
 
 
 def test_waveform_single_look():
     models_sets = ModelSettings.get_default_sets(st=SensorType.S3)
     sm = SamosaModel(
         sensor_sets=SensorSettings(),
         wf_sets=WaveformSettings(),
```

### Comparing `pysamosa-0.4.0/tests/test_montecarlo_sim.py` & `pysamosa-0.5.8/tests/test_montecarlo_sim.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/tests/test_retrack_multi.py` & `pysamosa-0.5.8/tests/test_retrack_multi.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/tests/test_retrack_single.py` & `pysamosa-0.5.8/tests/test_retrack_single.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/tests/test_samplusplus.py` & `pysamosa-0.5.8/tests/test_samplusplus.py`

 * *Files identical despite different names*

### Comparing `pysamosa-0.4.0/tests/test_utils.py` & `pysamosa-0.5.8/tests/test_utils.py`

 * *Files identical despite different names*

