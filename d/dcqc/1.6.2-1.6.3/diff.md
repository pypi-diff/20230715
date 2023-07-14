# Comparing `tmp/dcqc-1.6.2.tar.gz` & `tmp/dcqc-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcqc-1.6.2.tar", last modified: Mon Jun 26 15:42:17 2023, max compression
+gzip compressed data, was "dcqc-1.6.3.tar", last modified: Fri Jul 14 21:35:58 2023, max compression
```

## Comparing `dcqc-1.6.2.tar` & `dcqc-1.6.3.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.984117 dcqc-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-26 15:41:28.000000 dcqc-1.6.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.972117 dcqc-1.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.972117 dcqc-1.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-26 15:41:28.000000 dcqc-1.6.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-26 15:41:28.000000 dcqc-1.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 15:41:28.000000 dcqc-1.6.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-26 15:41:28.000000 dcqc-1.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-26 15:41:28.000000 dcqc-1.6.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-26 15:41:28.000000 dcqc-1.6.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 15:41:28.000000 dcqc-1.6.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-06-26 15:41:28.000000 dcqc-1.6.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 15:41:28.000000 dcqc-1.6.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-26 15:42:17.984117 dcqc-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-26 15:41:28.000000 dcqc-1.6.2/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   102584 2023-06-26 15:41:28.000000 dcqc-1.6.2/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-26 15:41:28.000000 dcqc-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.976117 dcqc-1.6.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.976117 dcqc-1.6.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-26 15:41:28.000000 dcqc-1.6.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-26 15:41:28.000000 dcqc-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-26 15:42:17.984117 dcqc-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 15:41:28.000000 dcqc-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.972117 dcqc-1.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.976117 dcqc-1.6.2/src/dcqc/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.976117 dcqc-1.6.2/src/dcqc/suites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/suites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/suites/suite_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/suites/suites.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.980117 dcqc-1.6.2/src/dcqc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/bioformats_info_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/file_extension_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/grep_date_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/json_load_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/jsonld_load_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/libtiff_info_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/md5_checksum_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/ome_xml_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/paired_fastq_parity_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/tests/tiff_tag_306_date_time_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/updaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/dcqc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.976117 dcqc-1.6.2/src/dcqc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-26 15:42:17.000000 dcqc-1.6.2/src/dcqc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-26 15:42:17.000000 dcqc-1.6.2/src/dcqc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:42:17.000000 dcqc-1.6.2/src/dcqc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 15:42:17.000000 dcqc-1.6.2/src/dcqc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:42:17.000000 dcqc-1.6.2/src/dcqc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-26 15:42:17.000000 dcqc-1.6.2/src/dcqc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 15:42:17.000000 dcqc-1.6.2/src/dcqc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.980117 dcqc-1.6.2/src/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-26 15:41:28.000000 dcqc-1.6.2/src/docker/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.980117 dcqc-1.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.984117 dcqc-1.6.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    76770 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/circuit.tif
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/empty_input.csv
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/example.bam
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/example.fastq
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/example.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/example.jsonld
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/example.tsv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/fastq1.fastq
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/fastq2.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/file.json
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/files.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)     2085 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/input.csv
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/small.csv
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/suite.json
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/suites.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.984117 dcqc-1.6.2/tests/data/suites_files/
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/suites_files/suites_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/suites_files/suites_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/suites_files/suites_3.json
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/target.json
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/test.computed.json
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/test.external.json
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/test.internal.json
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/test_contains_word_date.txt
--rw-r--r--   0 runner    (1001) docker     (123)   262517 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/test_image_dirty_datetime.tif
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/test_input.csv
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/test_output.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/tests.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:42:17.984117 dcqc-1.6.2/tests/data/tiffinfo/
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/tiffinfo/exit_code.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/tiffinfo/std_err.txt
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/data/tiffinfo/std_out.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/test_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/test_suites.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/test_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/test_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-26 15:41:28.000000 dcqc-1.6.2/tests/test_updaters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-26 15:41:28.000000 dcqc-1.6.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:35:58.738675 dcqc-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-14 21:35:01.000000 dcqc-1.6.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:35:58.710675 dcqc-1.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:35:58.718675 dcqc-1.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-07-14 21:35:01.000000 dcqc-1.6.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-14 21:35:01.000000 dcqc-1.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 21:35:01.000000 dcqc-1.6.3/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-14 21:35:01.000000 dcqc-1.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-14 21:35:01.000000 dcqc-1.6.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-14 21:35:01.000000 dcqc-1.6.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-14 21:35:01.000000 dcqc-1.6.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13433 2023-07-14 21:35:01.000000 dcqc-1.6.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 21:35:01.000000 dcqc-1.6.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-14 21:35:58.738675 dcqc-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-14 21:35:01.000000 dcqc-1.6.3/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   102584 2023-07-14 21:35:01.000000 dcqc-1.6.3/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-14 21:35:01.000000 dcqc-1.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:35:58.722675 dcqc-1.6.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-14 21:35:01.000000 dcqc-1.6.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:35:58.722675 dcqc-1.6.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 21:35:01.000000 dcqc-1.6.3/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-14 21:35:01.000000 dcqc-1.6.3/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-14 21:35:01.000000 dcqc-1.6.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-07-14 21:35:01.000000 dcqc-1.6.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-14 21:35:01.000000 dcqc-1.6.3/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-14 21:35:01.000000 dcqc-1.6.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 21:35:01.000000 dcqc-1.6.3/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 21:35:01.000000 dcqc-1.6.3/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-14 21:35:01.000000 dcqc-1.6.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-14 21:35:01.000000 dcqc-1.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-14 21:35:58.738675 dcqc-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-14 21:35:01.000000 dcqc-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:35:58.714675 dcqc-1.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:35:58.726675 dcqc-1.6.3/src/dcqc/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:35:58.726675 dcqc-1.6.3/src/dcqc/suites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/suites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/suites/suite_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/suites/suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:35:58.730675 dcqc-1.6.3/src/dcqc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/tests/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/tests/bioformats_info_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/tests/file_extension_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/tests/grep_date_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/tests/json_load_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/tests/jsonld_load_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/tests/libtiff_info_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/tests/md5_checksum_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/tests/ome_xml_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/tests/paired_fastq_parity_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/tests/tiff_tag_306_date_time_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/updaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/dcqc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:35:58.726675 dcqc-1.6.3/src/dcqc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-14 21:35:58.000000 dcqc-1.6.3/src/dcqc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-07-14 21:35:58.000000 dcqc-1.6.3/src/dcqc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 21:35:58.000000 dcqc-1.6.3/src/dcqc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-14 21:35:58.000000 dcqc-1.6.3/src/dcqc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 21:35:58.000000 dcqc-1.6.3/src/dcqc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-14 21:35:58.000000 dcqc-1.6.3/src/dcqc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 21:35:58.000000 dcqc-1.6.3/src/dcqc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:35:58.730675 dcqc-1.6.3/src/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-14 21:35:01.000000 dcqc-1.6.3/src/docker/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:35:58.734675 dcqc-1.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:35:58.738675 dcqc-1.6.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    76770 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/circuit.tif
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/empty_input.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/example.bam
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/example.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/example.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/example.jsonld
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/example.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/fastq1.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/fastq2.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/file.json
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/files.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2085 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/input.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/small.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/suite.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/suites.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:35:58.738675 dcqc-1.6.3/tests/data/suites_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/suites_files/suites_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/suites_files/suites_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/suites_files/suites_3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/target.json
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/test.computed.json
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/test.external.json
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/test.internal.json
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/test_contains_word_date.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   262517 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/test_image_dirty_datetime.tif
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/test_input.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/test_output.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/tests.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:35:58.738675 dcqc-1.6.3/tests/data/tiffinfo/
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/tiffinfo/exit_code.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/tiffinfo/std_err.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/data/tiffinfo/std_out.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/test_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/test_suites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/test_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/test_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-14 21:35:01.000000 dcqc-1.6.3/tests/test_updaters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-14 21:35:01.000000 dcqc-1.6.3/tox.ini
```

### Comparing `dcqc-1.6.2/.coveragerc` & `dcqc-1.6.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/.github/workflows/ci.yml` & `dcqc-1.6.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/.gitignore` & `dcqc-1.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/.pre-commit-config.yaml` & `dcqc-1.6.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/CONTRIBUTING.md` & `dcqc-1.6.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/LICENSE.txt` & `dcqc-1.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/PKG-INFO` & `dcqc-1.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcqc
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python package for performing quality control (QC) for data coordination (DC)
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Bruno Grande
 Author-email: bruno.grande@sagebase.org
 License: Apache-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `dcqc-1.6.2/Pipfile.lock` & `dcqc-1.6.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/README.md` & `dcqc-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/docs/Makefile` & `dcqc-1.6.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/docs/conf.py` & `dcqc-1.6.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/docs/index.md` & `dcqc-1.6.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/pyproject.toml` & `dcqc-1.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/setup.cfg` & `dcqc-1.6.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/setup.py` & `dcqc-1.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/__init__.py` & `dcqc-1.6.3/src/dcqc/__init__.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/file.py` & `dcqc-1.6.3/src/dcqc/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
 # TODO: These file types could be moved to an external file
 # Instantiated file types are automatically tracked by the FileType class
 FileType("*", (), "format_1915")  # To represent all file types
 FileType("TXT", (".txt",), "format_1964")
 FileType("JSON", (".json",), "format_3464")
 FileType("JSON-LD", (".jsonld",), "format_3749")
-FileType("TIFF", (".tif", ".tiff"), "format_3591")
+FileType("TIFF", (".tif", ".tiff", ".svs", ".scn"), "format_3591")
 FileType("OME-TIFF", (".ome.tif", ".ome.tiff"), "format_3727")
 FileType("TSV", (".tsv"), "format_3475")
 FileType("BAM", (".bam"), "format_2572")
 FileType("FASTQ", (".fastq", ".fastq.gz", ".fq", ".fq.gz"), "format_1930")
 
 
 # TODO: Leverage post-init function in dataclasses
```

### Comparing `dcqc-1.6.2/src/dcqc/main.py` & `dcqc-1.6.3/src/dcqc/main.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/mixins.py` & `dcqc-1.6.3/src/dcqc/mixins.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/parsers.py` & `dcqc-1.6.3/src/dcqc/parsers.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/reports.py` & `dcqc-1.6.3/src/dcqc/reports.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/suites/suite_abc.py` & `dcqc-1.6.3/src/dcqc/suites/suite_abc.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/suites/suites.py` & `dcqc-1.6.3/src/dcqc/suites/suites.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/target.py` & `dcqc-1.6.3/src/dcqc/target.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/tests/__init__.py` & `dcqc-1.6.3/src/dcqc/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/tests/base_test.py` & `dcqc-1.6.3/src/dcqc/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/tests/bioformats_info_test.py` & `dcqc-1.6.3/src/dcqc/tests/bioformats_info_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/tests/file_extension_test.py` & `dcqc-1.6.3/src/dcqc/tests/file_extension_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/tests/grep_date_test.py` & `dcqc-1.6.3/src/dcqc/tests/grep_date_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/tests/json_load_test.py` & `dcqc-1.6.3/src/dcqc/tests/json_load_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/tests/jsonld_load_test.py` & `dcqc-1.6.3/src/dcqc/tests/jsonld_load_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/tests/libtiff_info_test.py` & `dcqc-1.6.3/src/dcqc/tests/libtiff_info_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/tests/md5_checksum_test.py` & `dcqc-1.6.3/src/dcqc/tests/md5_checksum_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/tests/ome_xml_schema_test.py` & `dcqc-1.6.3/src/dcqc/tests/ome_xml_schema_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/tests/paired_fastq_parity_test.py` & `dcqc-1.6.3/src/dcqc/tests/paired_fastq_parity_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/tests/tiff_tag_306_date_time_test.py` & `dcqc-1.6.3/src/dcqc/tests/tiff_tag_306_date_time_test.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/updaters.py` & `dcqc-1.6.3/src/dcqc/updaters.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc/utils.py` & `dcqc-1.6.3/src/dcqc/utils.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/src/dcqc.egg-info/PKG-INFO` & `dcqc-1.6.3/src/dcqc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcqc
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python package for performing quality control (QC) for data coordination (DC)
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Bruno Grande
 Author-email: bruno.grande@sagebase.org
 License: Apache-2.0
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `dcqc-1.6.2/src/dcqc.egg-info/SOURCES.txt` & `dcqc-1.6.3/src/dcqc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/conftest.py` & `dcqc-1.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/data/circuit.tif` & `dcqc-1.6.3/tests/data/circuit.tif`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/data/example.jsonld` & `dcqc-1.6.3/tests/data/example.jsonld`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/data/files.csv` & `dcqc-1.6.3/tests/data/files.csv`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/data/generate.py` & `dcqc-1.6.3/tests/data/generate.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/data/suite.json` & `dcqc-1.6.3/tests/data/suite.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/data/suites.json` & `dcqc-1.6.3/tests/data/suites.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/data/suites_files/suites_1.json` & `dcqc-1.6.3/tests/data/suites_files/suites_1.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/data/suites_files/suites_2.json` & `dcqc-1.6.3/tests/data/suites_files/suites_2.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/data/suites_files/suites_3.json` & `dcqc-1.6.3/tests/data/suites_files/suites_3.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/data/test_image_dirty_datetime.tif` & `dcqc-1.6.3/tests/data/test_image_dirty_datetime.tif`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/data/tests.json` & `dcqc-1.6.3/tests/data/tests.json`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/test_acceptance.py` & `dcqc-1.6.3/tests/test_acceptance.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/test_file.py` & `dcqc-1.6.3/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/test_main.py` & `dcqc-1.6.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/test_parsers.py` & `dcqc-1.6.3/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/test_reports.py` & `dcqc-1.6.3/tests/test_reports.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/test_suites.py` & `dcqc-1.6.3/tests/test_suites.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/test_target.py` & `dcqc-1.6.3/tests/test_target.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/test_tests.py` & `dcqc-1.6.3/tests/test_tests.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tests/test_updaters.py` & `dcqc-1.6.3/tests/test_updaters.py`

 * *Files identical despite different names*

### Comparing `dcqc-1.6.2/tox.ini` & `dcqc-1.6.3/tox.ini`

 * *Files identical despite different names*

