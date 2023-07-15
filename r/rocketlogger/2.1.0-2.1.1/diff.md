# Comparing `tmp/rocketlogger-2.1.0.tar.gz` & `tmp/rocketlogger-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocketlogger-2.1.0.tar", last modified: Sun Feb 19 16:43:03 2023, max compression
+gzip compressed data, was "rocketlogger-2.1.1.tar", last modified: Sat Jul 15 10:11:08 2023, max compression
```

## Comparing `rocketlogger-2.1.0.tar` & `rocketlogger-2.1.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-02-19 16:43:03.146165 rocketlogger-2.1.0/
--rw-r--r--   0 lukas     (1000) lukas     (1000)      295 2021-08-07 16:51:48.000000 rocketlogger-2.1.0/.gitignore
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1583 2023-02-19 16:35:04.000000 rocketlogger-2.1.0/LICENSE
--rw-r--r--   0 lukas     (1000) lukas     (1000)      268 2022-03-27 19:27:07.000000 rocketlogger-2.1.0/MANIFEST.in
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3494 2023-02-19 16:43:03.146165 rocketlogger-2.1.0/PKG-INFO
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2099 2023-02-19 16:35:04.000000 rocketlogger-2.1.0/README.md
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     5107 2022-03-27 19:27:07.000000 rocketlogger-2.1.0/bug57_recover.py
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     3383 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/convert_calibration.py
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     2963 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/create_calibration.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-02-19 16:43:03.139499 rocketlogger-2.1.0/data/
--rw-r--r--   0 lukas     (1000) lukas     (1000)        6 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/.gitignore
--rw-r--r--   0 lukas     (1000) lukas     (1000)   180516 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_analog_only.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)   586468 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_calibration_i1l.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)   554340 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_calibration_i2l.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)   562372 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_calibration_ih.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  1058300 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_calibration_v.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)      104 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_calibration_v1.dat
--rw-r--r--   0 lukas     (1000) lukas     (1000)      124 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_calibration_v2.dat
--rw-r--r--   0 lukas     (1000) lukas     (1000)   180684 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_full.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)     4119 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_header_unaligned.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)   701348 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_high_current.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)      300 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_min_block_size.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2022-03-27 19:27:07.000000 rocketlogger-2.1.0/data/test_non_split.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2022-03-27 19:27:07.000000 rocketlogger-2.1.0/data/test_non_split_p1.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)     4120 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_single_block.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_split.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_split_p1.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_split_p2.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_split_truncated.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  4608584 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_split_truncated_p1.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  1621964 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_steps.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)    20260 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_truncated.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)  4196685 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_unsupported.rld
--rw-r--r--   0 lukas     (1000) lukas     (1000)    20264 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/data/test_v3_only.rld
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-02-19 16:43:03.142832 rocketlogger-2.1.0/docs/
--rw-r--r--   0 lukas     (1000) lukas     (1000)        7 2021-08-07 16:51:49.000000 rocketlogger-2.1.0/docs/.gitignore
--rw-r--r--   0 lukas     (1000) lukas     (1000)      634 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/docs/Makefile
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2653 2022-03-27 19:27:07.000000 rocketlogger-2.1.0/docs/calibration.rst
--rw-r--r--   0 lukas     (1000) lukas     (1000)     2206 2023-02-19 16:35:04.000000 rocketlogger-2.1.0/docs/conf.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1463 2022-03-27 19:27:07.000000 rocketlogger-2.1.0/docs/data.rst
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1677 2022-03-27 19:27:07.000000 rocketlogger-2.1.0/docs/index.rst
--rw-r--r--   0 lukas     (1000) lukas     (1000)      795 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/docs/make.bat
--rw-r--r--   0 lukas     (1000) lukas     (1000)      325 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/docs/rocketlogger.calibration.rst
--rw-r--r--   0 lukas     (1000) lukas     (1000)      218 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/docs/rocketlogger.data.rst
--rw-r--r--   0 lukas     (1000) lukas     (1000)      254 2022-03-27 19:27:07.000000 rocketlogger-2.1.0/docs/rocketlogger.rst
--rw-r--r--   0 lukas     (1000) lukas     (1000)      799 2022-03-27 19:27:07.000000 rocketlogger-2.1.0/docs/tests.rst
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     2249 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/process_data.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)      105 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/pyproject.toml
--rw-r--r--   0 lukas     (1000) lukas     (1000)       59 2023-02-19 16:35:04.000000 rocketlogger-2.1.0/requirements.txt
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-02-19 16:43:03.142832 rocketlogger-2.1.0/rocketlogger/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1559 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/rocketlogger/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    30148 2023-02-19 16:35:04.000000 rocketlogger-2.1.0/rocketlogger/calibration.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    53158 2023-02-19 16:35:04.000000 rocketlogger-2.1.0/rocketlogger/data.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-02-19 16:43:03.142832 rocketlogger-2.1.0/rocketlogger.egg-info/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3494 2023-02-19 16:43:03.000000 rocketlogger-2.1.0/rocketlogger.egg-info/PKG-INFO
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1347 2023-02-19 16:43:03.000000 rocketlogger-2.1.0/rocketlogger.egg-info/SOURCES.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)        1 2023-02-19 16:43:03.000000 rocketlogger-2.1.0/rocketlogger.egg-info/dependency_links.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)      107 2023-02-19 16:43:03.000000 rocketlogger-2.1.0/rocketlogger.egg-info/requires.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)       13 2023-02-19 16:43:03.000000 rocketlogger-2.1.0/rocketlogger.egg-info/top_level.txt
--rw-r--r--   0 lukas     (1000) lukas     (1000)       38 2023-02-19 16:43:03.146165 rocketlogger-2.1.0/setup.cfg
--rw-r--r--   0 lukas     (1000) lukas     (1000)     3403 2023-02-19 16:35:04.000000 rocketlogger-2.1.0/setup.py
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     1846 2023-02-19 16:35:04.000000 rocketlogger-2.1.0/test_coverage.sh
--rwxr-xr-x   0 lukas     (1000) lukas     (1000)     4428 2021-10-30 16:36:36.000000 rocketlogger-2.1.0/test_performance.py
-drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-02-19 16:43:03.142832 rocketlogger-2.1.0/tests/
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1758 2022-03-27 19:27:07.000000 rocketlogger-2.1.0/tests/__init__.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    18293 2023-02-19 16:35:04.000000 rocketlogger-2.1.0/tests/test_calibration.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)    56921 2022-03-27 19:27:07.000000 rocketlogger-2.1.0/tests/test_data.py
--rw-r--r--   0 lukas     (1000) lukas     (1000)     1622 2023-02-19 16:35:04.000000 rocketlogger-2.1.0/tox.ini
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-07-15 10:11:08.909980 rocketlogger-2.1.1/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      295 2021-08-07 16:51:48.000000 rocketlogger-2.1.1/.gitignore
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1583 2023-02-21 22:31:56.000000 rocketlogger-2.1.1/LICENSE
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      268 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/MANIFEST.in
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3494 2023-07-15 10:11:08.909980 rocketlogger-2.1.1/PKG-INFO
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2099 2023-02-21 22:31:56.000000 rocketlogger-2.1.1/README.md
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     5107 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/bug57_recover.py
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     3383 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/convert_calibration.py
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     2963 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/create_calibration.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-07-15 10:11:08.903313 rocketlogger-2.1.1/data/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        6 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/.gitignore
+-rw-r--r--   0 lukas     (1000) lukas     (1000)   180516 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_analog_only.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)   586468 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_calibration_i1l.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)   554340 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_calibration_i2l.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)   562372 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_calibration_ih.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  1058300 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_calibration_v.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      104 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_calibration_v1.dat
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      124 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_calibration_v2.dat
+-rw-r--r--   0 lukas     (1000) lukas     (1000)   180684 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_full.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     4119 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_header_unaligned.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)   701348 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_high_current.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      300 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_min_block_size.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/data/test_non_split.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/data/test_non_split_p1.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     4120 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_single_block.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_split.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_split_p1.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_split_p2.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  4608588 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_split_truncated.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  4608584 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_split_truncated_p1.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  1621964 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_steps.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    20260 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_truncated.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)  4196685 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_unsupported.rld
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    20264 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/data/test_v3_only.rld
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-07-15 10:11:08.909980 rocketlogger-2.1.1/docs/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        7 2021-08-07 16:51:49.000000 rocketlogger-2.1.1/docs/.gitignore
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      634 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/docs/Makefile
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2653 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/docs/calibration.rst
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     2206 2023-07-15 09:43:40.000000 rocketlogger-2.1.1/docs/conf.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1463 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/docs/data.rst
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1677 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/docs/index.rst
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      795 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/docs/make.bat
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      325 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/docs/rocketlogger.calibration.rst
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      218 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/docs/rocketlogger.data.rst
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      254 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/docs/rocketlogger.rst
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      799 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/docs/tests.rst
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     2249 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/process_data.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      105 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/pyproject.toml
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       59 2023-07-12 21:05:07.000000 rocketlogger-2.1.1/requirements.txt
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-07-15 10:11:08.909980 rocketlogger-2.1.1/rocketlogger/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1559 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/rocketlogger/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    30148 2023-02-21 22:31:56.000000 rocketlogger-2.1.1/rocketlogger/calibration.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    53158 2023-02-19 16:35:04.000000 rocketlogger-2.1.1/rocketlogger/data.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-07-15 10:11:08.909980 rocketlogger-2.1.1/rocketlogger.egg-info/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3494 2023-07-15 10:11:08.000000 rocketlogger-2.1.1/rocketlogger.egg-info/PKG-INFO
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1347 2023-07-15 10:11:08.000000 rocketlogger-2.1.1/rocketlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)        1 2023-07-15 10:11:08.000000 rocketlogger-2.1.1/rocketlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)      107 2023-07-15 10:11:08.000000 rocketlogger-2.1.1/rocketlogger.egg-info/requires.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       13 2023-07-15 10:11:08.000000 rocketlogger-2.1.1/rocketlogger.egg-info/top_level.txt
+-rw-r--r--   0 lukas     (1000) lukas     (1000)       38 2023-07-15 10:11:08.909980 rocketlogger-2.1.1/setup.cfg
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     3403 2023-07-15 09:43:40.000000 rocketlogger-2.1.1/setup.py
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     1846 2023-02-21 22:31:56.000000 rocketlogger-2.1.1/test_coverage.sh
+-rwxr-xr-x   0 lukas     (1000) lukas     (1000)     4428 2021-10-30 16:36:36.000000 rocketlogger-2.1.1/test_performance.py
+drwxr-xr-x   0 lukas     (1000) lukas     (1000)        0 2023-07-15 10:11:08.909980 rocketlogger-2.1.1/tests/
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1758 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/tests/__init__.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    18293 2023-02-21 22:31:56.000000 rocketlogger-2.1.1/tests/test_calibration.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)    56921 2022-03-27 19:27:07.000000 rocketlogger-2.1.1/tests/test_data.py
+-rw-r--r--   0 lukas     (1000) lukas     (1000)     1622 2023-02-21 22:31:56.000000 rocketlogger-2.1.1/tox.ini
```

### Comparing `rocketlogger-2.1.0/LICENSE` & `rocketlogger-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/PKG-INFO` & `rocketlogger-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketlogger
-Version: 2.1.0
+Version: 2.1.1
 Summary: RocketLogger Python Support
 Home-page: https://github.com/ETHZ-TEC/RocketLogger#readme
 Author: ETH Zurich, Computer Engineering Group
 License: BSD 3-Clause
 Project-URL: Documentation, https://github.com/ETHZ-TEC/RocketLogger/wiki/python
 Project-URL: Source, https://github.com/ETHZ-TEC/RocketLogger
 Project-URL: Tracker, https://github.com/ETHZ-TEC/RocketLogger/issues
```

### Comparing `rocketlogger-2.1.0/README.md` & `rocketlogger-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/bug57_recover.py` & `rocketlogger-2.1.1/bug57_recover.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/convert_calibration.py` & `rocketlogger-2.1.1/convert_calibration.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/create_calibration.py` & `rocketlogger-2.1.1/create_calibration.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_analog_only.rld` & `rocketlogger-2.1.1/data/test_analog_only.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_calibration_i1l.rld` & `rocketlogger-2.1.1/data/test_calibration_i1l.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_calibration_i2l.rld` & `rocketlogger-2.1.1/data/test_calibration_i2l.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_calibration_ih.rld` & `rocketlogger-2.1.1/data/test_calibration_ih.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_calibration_v.rld` & `rocketlogger-2.1.1/data/test_calibration_v.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_full.rld` & `rocketlogger-2.1.1/data/test_full.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_header_unaligned.rld` & `rocketlogger-2.1.1/data/test_header_unaligned.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_high_current.rld` & `rocketlogger-2.1.1/data/test_high_current.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_non_split.rld` & `rocketlogger-2.1.1/data/test_non_split.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_non_split_p1.rld` & `rocketlogger-2.1.1/data/test_non_split_p1.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_single_block.rld` & `rocketlogger-2.1.1/data/test_single_block.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_split.rld` & `rocketlogger-2.1.1/data/test_split.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_split_p1.rld` & `rocketlogger-2.1.1/data/test_split_p1.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_split_p2.rld` & `rocketlogger-2.1.1/data/test_split_p2.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_split_truncated.rld` & `rocketlogger-2.1.1/data/test_split_truncated.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_split_truncated_p1.rld` & `rocketlogger-2.1.1/data/test_split_truncated_p1.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_steps.rld` & `rocketlogger-2.1.1/data/test_steps.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_truncated.rld` & `rocketlogger-2.1.1/data/test_truncated.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_unsupported.rld` & `rocketlogger-2.1.1/data/test_unsupported.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/data/test_v3_only.rld` & `rocketlogger-2.1.1/data/test_v3_only.rld`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/docs/Makefile` & `rocketlogger-2.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/docs/calibration.rst` & `rocketlogger-2.1.1/docs/calibration.rst`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/docs/conf.py` & `rocketlogger-2.1.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'RocketLogger Python Support Library'
 copyright = '2021, ETH Zurich, Computer Engineering Group'
 author = 'ETH Zurich, Computer Engineering Group'
 
 # The full version, including alpha/beta/rc tags
-release = '2.1.0'
+release = '2.1.1'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `rocketlogger-2.1.0/docs/data.rst` & `rocketlogger-2.1.1/docs/data.rst`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/docs/index.rst` & `rocketlogger-2.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/docs/make.bat` & `rocketlogger-2.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/docs/tests.rst` & `rocketlogger-2.1.1/docs/tests.rst`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/process_data.py` & `rocketlogger-2.1.1/process_data.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/rocketlogger/__init__.py` & `rocketlogger-2.1.1/rocketlogger/__init__.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/rocketlogger/calibration.py` & `rocketlogger-2.1.1/rocketlogger/calibration.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/rocketlogger/data.py` & `rocketlogger-2.1.1/rocketlogger/data.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/rocketlogger.egg-info/PKG-INFO` & `rocketlogger-2.1.1/rocketlogger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketlogger
-Version: 2.1.0
+Version: 2.1.1
 Summary: RocketLogger Python Support
 Home-page: https://github.com/ETHZ-TEC/RocketLogger#readme
 Author: ETH Zurich, Computer Engineering Group
 License: BSD 3-Clause
 Project-URL: Documentation, https://github.com/ETHZ-TEC/RocketLogger/wiki/python
 Project-URL: Source, https://github.com/ETHZ-TEC/RocketLogger
 Project-URL: Tracker, https://github.com/ETHZ-TEC/RocketLogger/issues
```

### Comparing `rocketlogger-2.1.0/rocketlogger.egg-info/SOURCES.txt` & `rocketlogger-2.1.1/rocketlogger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/setup.py` & `rocketlogger-2.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="rocketlogger",
-    version="2.1.0",
+    version="2.1.1",
     author="ETH Zurich, Computer Engineering Group",
     description="RocketLogger Python Support",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="BSD 3-Clause",
     url="https://github.com/ETHZ-TEC/RocketLogger#readme",
     classifiers=[
```

### Comparing `rocketlogger-2.1.0/test_coverage.sh` & `rocketlogger-2.1.1/test_coverage.sh`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/test_performance.py` & `rocketlogger-2.1.1/test_performance.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/tests/__init__.py` & `rocketlogger-2.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/tests/test_calibration.py` & `rocketlogger-2.1.1/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/tests/test_data.py` & `rocketlogger-2.1.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `rocketlogger-2.1.0/tox.ini` & `rocketlogger-2.1.1/tox.ini`

 * *Files identical despite different names*

