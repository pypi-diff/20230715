# Comparing `tmp/pz-rail-0.99.1.tar.gz` & `tmp/pz-rail-0.99.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-0.99.1.tar", last modified: Fri Jun 16 04:45:31 2023, max compression
+gzip compressed data, was "pz-rail-0.99.1.1.tar", last modified: Sat Jul 15 00:33:16 2023, max compression
```

## Comparing `pz-rail-0.99.1.tar` & `pz-rail-0.99.1.1.tar`

### file list

```diff
@@ -1,100 +1,104 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.748254 pz-rail-0.99.1/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.732254 pz-rail-0.99.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.736254 pz-rail-0.99.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.github/workflows/build_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-16 04:45:19.000000 pz-rail-0.99.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-16 04:45:19.000000 pz-rail-0.99.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-16 04:45:31.748254 pz-rail-0.99.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-16 04:45:19.000000 pz-rail-0.99.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-16 04:45:19.000000 pz-rail-0.99.1/conda-reqs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.736254 pz-rail-0.99.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.728254 pz-rail-0.99.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.736254 pz-rail-0.99.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/_static/css/notebooks.css
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/demos.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/nbconvert-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.736254 pz-rail-0.99.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/source/citing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/source/futureplans.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/source/immediateplans.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-06-16 04:45:19.000000 pz-rail-0.99.1/docs/source/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-16 04:45:19.000000 pz-rail-0.99.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.736254 pz-rail-0.99.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.740254 pz-rail-0.99.1/examples/core_examples/
--rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/FileIO_DataStore.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/Pipe_Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/Run_Pipe.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/hyperbolic_magnitude_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/iterator_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/pipe_example.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/core_examples/pipe_example_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.740254 pz-rail-0.99.1/examples/creation_examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/creation_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/creation_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/creation_examples/degradation-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/creation_examples/dsps_sed_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/creation_examples/example_GridSelection_for_HSC.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/creation_examples/example_ObsConditions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/creation_examples/photometric_realization_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    24628 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/creation_examples/posterior-demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.744254 pz-rail-0.99.1/examples/estimation_examples/
--rw-r--r--   0 runner    (1001) docker     (123)    19368 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/estimation_examples/NZDir.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    24800 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/estimation_examples/RAIL_estimation_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/estimation_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    28480 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/estimation_examples/SimpleSOM_demo.ipynb.fixme
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/estimation_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/estimation_examples/nzdir_as_pipeline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    30673 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/estimation_examples/somocluSOM_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    37053 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/estimation_examples/somocluSOMcluster_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20698 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/estimation_examples/test_sampled_summarizers.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.744254 pz-rail-0.99.1/examples/evaluation_examples/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/evaluation_examples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/evaluation_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/evaluation_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/evaluation_examples/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19193 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/evaluation_examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.748254 pz-rail-0.99.1/examples/goldenspike_examples/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/goldenspike_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/goldenspike_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/goldenspike_examples/cleanup_pipeline.sh
--rw-r--r--   0 runner    (1001) docker     (123)    25570 2023-06-16 04:45:19.000000 pz-rail-0.99.1/examples/goldenspike_examples/goldenspike.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-16 04:45:19.000000 pz-rail-0.99.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-16 04:45:19.000000 pz-rail-0.99.1/rail_packages.yml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-16 04:45:19.000000 pz-rail-0.99.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 04:45:31.748254 pz-rail-0.99.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-16 04:45:19.000000 pz-rail-0.99.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.728254 pz-rail-0.99.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.748254 pz-rail-0.99.1/src/pz_rail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-16 04:45:31.000000 pz-rail-0.99.1/src/pz_rail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-16 04:45:31.000000 pz-rail-0.99.1/src/pz_rail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 04:45:31.000000 pz-rail-0.99.1/src/pz_rail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-16 04:45:31.000000 pz-rail-0.99.1/src/pz_rail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 04:45:31.000000 pz-rail-0.99.1/src/pz_rail.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.728254 pz-rail-0.99.1/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.748254 pz-rail-0.99.1/src/rail/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 04:45:19.000000 pz-rail-0.99.1/src/rail/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-16 04:45:31.000000 pz-rail-0.99.1/src/rail/hub/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.728254 pz-rail-0.99.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:45:31.748254 pz-rail-0.99.1/tests/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-16 04:45:19.000000 pz-rail-0.99.1/tests/hub/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.578542 pz-rail-0.99.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.546542 pz-rail-0.99.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.550542 pz-rail-0.99.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/.github/workflows/build_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-15 00:33:16.578542 pz-rail-0.99.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/conda-reqs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.554542 pz-rail-0.99.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.534542 pz-rail-0.99.1.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.554542 pz-rail-0.99.1.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/docs/_static/css/notebooks.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/docs/demos.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/docs/nbconvert-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.558542 pz-rail-0.99.1.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/docs/source/citing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/docs/source/fix_an_issue.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/docs/source/new_algorithm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/docs/source/new_rail_stage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/docs/source/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/docs/source/sharing_pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.558542 pz-rail-0.99.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.562542 pz-rail-0.99.1.1/examples/core_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    14993 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/core_examples/FileIO_DataStore.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/core_examples/Pipe_Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/core_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/core_examples/Run_Pipe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/core_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/core_examples/hyperbolic_magnitude_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/core_examples/iterator_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/core_examples/pipe_example.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/core_examples/pipe_example_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.566542 pz-rail-0.99.1.1/examples/creation_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/creation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/creation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/creation_examples/degradation-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/creation_examples/dsps_sed_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/creation_examples/example_GridSelection_for_HSC.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/creation_examples/example_ObsConditions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/creation_examples/photometric_realization_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    24628 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/creation_examples/posterior-demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.570542 pz-rail-0.99.1.1/examples/estimation_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/estimation_examples/NZDir.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    25214 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/estimation_examples/RAIL_estimation_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/estimation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    28442 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/estimation_examples/SimpleSOM_demo.ipynb.fixme
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/estimation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/estimation_examples/nzdir_as_pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    30650 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/estimation_examples/somocluSOM_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    37010 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/estimation_examples/somocluSOMcluster_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20904 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/estimation_examples/test_sampled_summarizers.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.574542 pz-rail-0.99.1.1/examples/evaluation_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/evaluation_examples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/evaluation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/evaluation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    19247 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/evaluation_examples/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19193 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/evaluation_examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.574542 pz-rail-0.99.1.1/examples/goldenspike_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/goldenspike_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/goldenspike_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/goldenspike_examples/cleanup_pipeline.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/goldenspike_examples/goldenspike.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/goldenspike_examples/goldenspike.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/examples/goldenspike_examples/goldenspike_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/rail_packages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 00:33:16.578542 pz-rail-0.99.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.542542 pz-rail-0.99.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.578542 pz-rail-0.99.1.1/src/pz_rail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-15 00:33:16.000000 pz-rail-0.99.1.1/src/pz_rail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-15 00:33:16.000000 pz-rail-0.99.1.1/src/pz_rail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 00:33:16.000000 pz-rail-0.99.1.1/src/pz_rail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-15 00:33:16.000000 pz-rail-0.99.1.1/src/pz_rail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-15 00:33:16.000000 pz-rail-0.99.1.1/src/pz_rail.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.542542 pz-rail-0.99.1.1/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.578542 pz-rail-0.99.1.1/src/rail/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/src/rail/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-15 00:33:16.000000 pz-rail-0.99.1.1/src/rail/hub/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.542542 pz-rail-0.99.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:33:16.578542 pz-rail-0.99.1.1/tests/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-15 00:32:59.000000 pz-rail-0.99.1.1/tests/hub/test_import.py
```

### Comparing `pz-rail-0.99.1/.github/pull_request_template.md` & `pz-rail-0.99.1.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/.github/workflows/build_documentation.yml` & `pz-rail-0.99.1.1/.github/workflows/build_documentation.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/.github/workflows/linting.yml` & `pz-rail-0.99.1.1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/.github/workflows/publish-to-pypi.yml` & `pz-rail-0.99.1.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/.github/workflows/smoke-test.yml` & `pz-rail-0.99.1.1/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/.github/workflows/testing-and-coverage.yml` & `pz-rail-0.99.1.1/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/.gitignore` & `pz-rail-0.99.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/.pre-commit-config.yaml` & `pz-rail-0.99.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/.readthedocs.yaml` & `pz-rail-0.99.1.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/LICENSE` & `pz-rail-0.99.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/docs/Makefile` & `pz-rail-0.99.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/docs/_static/css/notebooks.css` & `pz-rail-0.99.1.1/docs/_static/css/notebooks.css`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/docs/conf.py` & `pz-rail-0.99.1.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,16 @@
     'sphinx.ext.coverage',
     'sphinx.ext.ifconfig',
     'sphinx.ext.mathjax',
     'nbsphinx',
     'sphinx.ext.viewcode',
     'sphinx.ext.autosummary',
     'sphinx.ext.githubpages',
-    'sphinx.ext.napoleon']
+    'sphinx.ext.napoleon',
+    'sphinx.ext.autosectionlabel']
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
```

### Comparing `pz-rail-0.99.1/docs/demos.rst` & `pz-rail-0.99.1.1/docs/demos.rst`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/docs/index.rst` & `pz-rail-0.99.1.1/docs/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -15,24 +15,26 @@
 
 .. toctree::
    :maxdepth: 1
    :caption: Getting Started
 
    source/overview
    source/installation
-   source/contributing
    source/citing
 
 .. toctree::
    :maxdepth: 1
-   :caption: RAIL Plans
+   :caption: Contributing
+
+   source/contributing
+   source/fix_an_issue
+   source/new_rail_stage
+   source/new_algorithm
+   source/sharing_pipeline
 
-   source/immediateplans
-   source/futureplans
-   
 .. toctree::
    :maxdepth: 1
    :caption: Usage Demos
 
    demos
 
 .. toctree::
```

### Comparing `pz-rail-0.99.1/docs/source/citing.rst` & `pz-rail-0.99.1.1/docs/source/citing.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,41 @@
 ***********
 Citing RAIL
 ***********
 
-This code, while public on GitHub, has not yet been released by
-DESC and is still under active development.  Our release of v1.0 will
-be accompanied by a journal paper describing the development and
-validation of `RAIL`.
-
-If you make use of the ideas or software here, please cite this
-repository ``https://github.com/LSSTDESC/RAIL``. You are welcome to
-re-use the code, which is open source and available under terms
-consistent with our `LICENSE
-<https://github.com/LSSTDESC/RAIL/blob/master/LICENSE>`_ (`BSD 3-Clause
-<https://opensource.org/licenses/BSD-3-Clause>`_).
-
-External contributors and DESC members wishing to use RAIL for non-DESC projects
-should consult with the Photometric Redshifts (PZ) Working Group conveners,
-ideally before the work has started, but definitely before any publication or
-posting of the work to the arXiv.
-
-***********************************
-Citing individual codes within RAIL
-***********************************
-
-Several of the codes included in RAIL are pre-existing codes written by external developers,
-if these codes are used in an analysis they should be cited individually in addition to the
-citation to RAIL.
+RAIL is open source and may be used according to the terms of its `LICENSE <https://github.com/LSSTDESC/RAIL/blob/main/LICENSE>`_ `(BSD 3-Clause) <https://opensource.org/licenses/BSD-3-Clause>`_.
+If you make use of the ideas or software here in any publication, you must cite this repository <https://github.com/LSSTDESC/RAIL> as "LSST-DESC PZ WG (in prep)" with the `Zenodo DOI <https://doi.org/10.5281/zenodo.7017551>`_.
+Please consider also inviting the developers as co-authors on publications resulting from your use of RAIL by `making an issue <https://github.com/LSSTDESC/RAIL/issues/new/choose>`_.
 
-Code references:
+The following list provides the necessary references for external codes accessible through the RAIL ecosystem, which must be cited as follows if those methods are used in a publication:
+
+| Astropy: 
 
 | Bayesian Photometric Redshifts (BPZ/BPZ_lite):
 | `Benitez (2000) <https://ui.adsabs.harvard.edu/abs/2000ApJ...536..571B/abstract>`_
 | `Coe et al (2006) <https://ui.adsabs.harvard.edu/abs/2006AJ....132..926C/abstract>`_
 
 | Delight:
 | `Leistedt & Hogg (2017) <https://ui.adsabs.harvard.edu/abs/2017ApJ...838....5L/abstract>`_
 
+| DSPS:
+
 | FlexZBoost:
-| `Izbicki & Lee (2017)
-<https://projecteuclid.org/journals/electronic-journal-of-statistics/volume-11/issue-2/Converting-high-dimensional-regression-to-high-dimensional-conditional-density-estimation/10.1214/17-EJS1302.full>`_
+| `Izbicki & Lee (2017) <https://projecteuclid.org/journals/electronic-journal-of-statistics/volume-11/issue-2/Converting-high-dimensional-regression-to-high-dimensional-conditional-density-estimation/10.1214/17-EJS1302.full>`_
 | `Dalmasso et al (2020) <https://ui.adsabs.harvard.edu/abs/2020A%26C....3000362D/abstract>`_
 
-| PZFlowPDF:
-| J. F. Crenshaw (in prep)
+| FSPS:
+
+| GPz: 
+
+| PZFlowEstimator:
+| J. F. Crenshaw et al (in prep)
 | `Zenodo link <https://zenodo.org/record/6369625#.Ylcpjy-cYW8>`_
 
+| Scikit-learn:
+
+| SOM(oclu):
+
 | trainZ:
 | `Schmidt, Malz et al (2020) <https://ui.adsabs.harvard.edu/abs/2020MNRAS.499.1587S/abstract>`_
+
+| VarInfStackSummarizer:
```

### Comparing `pz-rail-0.99.1/docs/source/installation.rst` & `pz-rail-0.99.1.1/docs/source/installation.rst`

 * *Files 11% similar despite different names*

```diff
@@ -183,23 +183,23 @@
 
 For Delight you should be able to just do:
 
 .. code-block:: bash
 
     pip install pz-rail-delight
 
-However, the particular estimator `Delight` is built with `Cython` and uses `openmp`.  Mac has dropped native support for `openmp`, which will likely cause problems when trying to run the `delightPZ` estimation code in RAIL.  See the notes below for instructions on installing Delight if you wish to use this particular estimator.
+However, the particular estimator `Delight` is built with `Cython` and uses `openmp`.  Mac has dropped native support for `openmp`, which will likely cause problems when trying to run the `DelightEstimator` estimation code in RAIL.  See the notes below for instructions on installing Delight if you wish to use this particular estimator.
 
-If you are installing RAIL on a Mac, as noted above the `delightPZ` estimator requires that your machine's `gcc` be set up to work with `openmp`. If you are installing on a Mac and do not plan on using `delightPZ`, then you can simply install RAIL with `pip install .[base]` rather than `pip install .[all]`, which will skip the Delight package.  If you are on a Mac and *do* expect to run `delightPZ`, then follow the instructions `here <https://github.com/LSSTDESC/Delight/blob/master/Mac_installation.md>`_ to install Delight before running `pip install .[all]`.
+If you are installing RAIL on a Mac, as noted above the `DelightEstimator` estimator requires that your machine's `gcc` be set up to work with `openmp`. If you are installing on a Mac and do not plan on using `DelightEstimator`, then you can simply install RAIL with `pip install .[base]` rather than `pip install .[all]`, which will skip the Delight package.  If you are on a Mac and *do* expect to run `DelightEstimator`, then follow the instructions `here <https://github.com/LSSTDESC/Delight/blob/master/Mac_installation.md>`_ to install Delight before running `pip install .[all]`.
 
     
-Installing FZBoost
+Installing FlexZBoost
 ------------------
 
-For FZBoost, you should be able to just do
+For FlexZBoost, you should be able to just do
 
 .. code-block:: bash
 
     pip install pz-rail-flexzboost
 
 But if you run into problems you might need to:
 
@@ -218,38 +218,22 @@
 
 But if you run into problems you might need to:
 
 - cd to a directory where you wish to clone the DESC_BPZ package and run `git clone https://github.com/LSSTDESC/DESC_BPZ.git`
 - cd to the DESC_BPZ directory and run `python setup.py install` (add `--user` if you are on a shared system such as NERSC)
 - try `pip install pz-rail-bpz` again.
 
-If you've installed rail and bpz to different directories (most commonly, you've installed rail from 
-source and bpz from PyPI), you may run into an issue where rail cannot locate a file installed by bpz 
-(usually encountered when running the estimation step in Goldenspike). 
-
-To fix this, find your test_bpz.columns file in your bpz directory (`or grab a new one here on 
-GitHub <https://github.com/LSSTDESC/rail_bpz/blob/main/src/rail/examples/estimation/configs/test_bpz.columns>`_) 
-and copy it into your rail directory to `/RAIL/src/rail/examples/estimation/configs/test_bpz.columns`.
-
-Alternatively, if you don't want to move files, you should be able to replace the configured paths with 
-your actual `test_bpz.columns` path:
-
-* inform stage: `bpz_lite.py L89 <https://github.com/LSSTDESC/rail_bpz/blob/65870ffd93ba35356a1af44104a0a78530085789/src/rail/estimation/algos/bpz_lite.py#L89>`_
-
-* estimation: `bpz_lite.py L259 <https://github.com/LSSTDESC/rail_bpz/blob/65870ffd93ba35356a1af44104a0a78530085789/src/rail/estimation/algos/bpz_lite.py#L259>`_
-
-
 
 Using GPU-optimization for pzflow
 ---------------------------------
 
 Note that the Creation Module depends on pzflow, which has an optional GPU-compatible installation.
 For instructions, see the `pzflow Github repo <https://github.com/jfcrenshaw/pzflow/>`_.
 
-On some systems that are slightly out of date, e.g. an older version of python's `setuptools`, there can be some problems installing packages hosted on GitHub rather than PyPi.  We recommend that you update your system; however, some users have still reported problems with installation of subpackages necessary for `FZBoost` and `bpz_lite`.  If this occurs, try the following procedure:
+On some systems that are slightly out of date, e.g. an older version of python's `setuptools`, there can be some problems installing packages hosted on GitHub rather than PyPi.  We recommend that you update your system; however, some users have still reported problems with installation of subpackages necessary for `flexzboost` and `bpz_lite`.  If this occurs, try the following procedure:
 
 Once you have installed RAIL, you can import the package (via `import rail`) in any of your scripts and notebooks.
 For examples demonstrating how to use the different pieces, see the notebooks in the `examples/` directory.
 
 
 Adding your kernel to jupyter
 =============================
```

### Comparing `pz-rail-0.99.1/docs/source/overview.rst` & `pz-rail-0.99.1.1/docs/source/overview.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 ********
 Overview
 ********
 
-RAIL (Redshift Assessment Infrastructure Layers) is LSST-DESC software for the computation and assessment of redshifts derived from Rubin data.
-RAIL addresses the challenge of enabling stress-testing of multiple photo-z codes in the presence of realistically complex systematic imperfections in the input photometry and prior information (such as template libraries and training sets), everything from the handling of diverse output storage formats to the propagation of assumptions inherent to individual codes to the architecture of the machines on which the code is run.
-RAIL seeks to minimize such impacts by unifying much of the infrastructure in a single modular code base that can be used by photo-z developers and consumers alike.  
-Beyond the comparison of different photo-z approaches, RAIL will be employed to generate photo-z catalogs used by DESC members in their science analyses. 
+RAIL enables stress-testing of multiple approaches to photo-z estimation at-scale for LSST in the presence of realistically complex systematic imperfections in the input photometry and prior information (such as template libraries and training sets) under science-agnostic and science-specific metrics, with the expectation that once a pipeline is validated through controlled experimentation, the exact same estimation procedure could be applied to real data without loss of validity.
+To support such an ambitious goal, it has a highly modular structure encompassing three aspects of this kind of experiment and is built upon a number of key types of objects, however, the result is that RAIL is unavoidably complicated.
+This overview seeks to present the organizational philosophy, basic structures, and core dependencies in order to motivate an exposition to the RAIL ecosystem.
 
-There are three aspects to the RAIL approach to photo-zs: the creation of self-consistently forward-modeled, realistically complex mock data for testing purposes, the estimation of individual galaxy and galaxy sample redshift uncertainties, and the evaluation of the results of the estimators by generic and science-specific metrics.
-RAIL includes a subpackage for each, providing a flexible framework for handling different approaches and at least one baseline implementation of a method under that umbrella as an example for the broader community to integrate their own codes into RAIL.
+
+Organization
+************
+
+An end-to-end experiment entails the creation of self-consistently forward-modeled, realistically complex mock data for testing purposes, the estimation of individual galaxy and/or galaxy sample redshift uncertainties, and the evaluation of the resulting photo-z data products by informative metrics.
+RAIL includes subpackages for each, providing a flexible framework for accessing implementations of approaches under each umbrella.
 The purpose of each piece of infrastructure is outlined below.
-For a working example illustrating all four components of RAIL, see the `examples/goldenspike/goldenspike.ipynb <https://github.com/LSSTDESC/RAIL/blob/main/examples/goldenspike/goldenspike.ipynb>`_ jupyter notebook.
+For a working example illustrating all three components of RAIL, see the `examples/goldenspike/goldenspike.ipynb <https://github.com/LSSTDESC/RAIL/blob/main/examples/goldenspike/goldenspike.ipynb>`_ Jupyter notebook.
 
 
-A brief note on core DESC software dependencies
-===============================================
+Core DESC software dependencies
+===============================
 
 The `qp` Ensemble format is the expected default storage format for redshift information within DESC, and all redshift PDFs, for both individual galaxies and galaxy samples (such as tomographic bin members or galaxy cluster members), will be stored as `qp` Ensemble objects to be directly accessible to LSST-DESC pipelines, such as `TXPipe <https://github.com/LSSTDESC/TXPipe/>`_.
 The use of a unified `qp` Ensemble as the output format enables a consistent evaluation of redshift uncertainties.  See `the qp repository <https://github.com/LSSTDESC/qp>`_ for more details, though in brief, `qp` enables transformation between different PDF parameterizations, computation of many useful metrics, and easy fileIO.
 
+
+
 `creation`
 ==========
 
 The creation subpackage has two main components enabling forward-modeling of realistically complex mock data.
 The creation modules provide a joint probability space of redshift and photometry, and the degradation modules introduce systematic imperfections into galaxy catalogs, which can be used to stress-test photo-z estimators. 
 
 **Creation modules**: 
@@ -63,16 +68,16 @@
 The estimation subpackage enables the automatic execution of arbitrary redshift estimation codes in a common computing environment.  
 Each photo-z method usually has both an `inform` method that trains a model based on a dataset with known redshifts or ingests template information, and an `estimate` method that executes the particular estimation method.  
 There are two types of quantities that RAIL can estimate: redshift PDFs for individual objects and overall PDFs for ensembles of objects, one obvious use case being tomographic redshift bins commonly used in cosmological analyses.  
 Methods that estimate per-galaxy PDFs directly from photometry are referred to as Estimators, while those that produce a summary PDF and associated uncertainty of an ensemble of galaxies are referred to as Summarizers.
 Individual estimation and summarization codes are "wrapped" as RAIL stages so that they can be run in a controlled way.  
 
 **base design**: 
-Estimators for several popular codes `BPZ_lite` (a slimmed down version of the popular template-based BPZ code), `FlexZBoost`, and delight `Delight` are included in rail/estimation, as are an estimator `PZFlowPDF` that uses the same normalizing flow employed in the creation module, and `KNearNeighPDF` for a simple color-based nearest neighbor estimator.  
-The pathological `trainZ` estimator is also implemented.  
+Estimators for several popular codes `BPZliteEstimator` (a slimmed down version of the popular template-based BPZ code), `FlexZBoostEstimator`, and `DelightEstimator` are included in rail/estimation, as are an estimator `PZFlowEstimator` that uses the same normalizing flow employed in the creation module, and `KNearNeighEstimator` for a simple color-based nearest neighbor estimator.  
+The pathological `TrainZEstimator` estimator is also implemented.  
 Several very basic summarizers such as a histogram of point source estimates, the naive "stacking"/summing of PDFs, and a variational inference-based summarizer are also included in RAIL.
 
 **Usage**: 
 In the `example` directory, you can execute the estimation/RAIL_estimation_demo.ipynb notebook.  
 Estimation codes can also be run as ceci modules with variables stored in a yaml file.
 
 **Immediate next steps**: 
@@ -91,7 +96,8 @@
 **Usage**: 
 In the `example` directory, you can execute the evaluation/demo.ipynb jupyter notebook.
 
 **Future extensions**: 
 We aim to greatly expand the library of available metrics and welcome input from the community in doing so.  
 An immediate extension would propagate estimated redshift posteriors to science-motivated metrics, and/or metrics related to computational requirements of the estimators. 
 Within DESC, development of sophisticated metrics propagating photo-z uncertainties through cosmological probe analysis pipelines is now underway as part of Dark Energy Redshift Assessment Infrastructure Layers (DERAIL).
+
```

### Comparing `pz-rail-0.99.1/examples/core_examples/FileIO_DataStore.ipynb` & `pz-rail-0.99.1.1/examples/core_examples/FileIO_DataStore.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990625%*

 * *Differences: {"'cells'": '{22: {\'source\': {insert: [(2, "Now that we have our data in place, we can use it in '*

 * *            "a RAIL stage.  As an example, we'll estimate photo-z's for our data.  Let's train the "*

 * *            "`KNearNeighEstimator` algorithm with our train_data, and then estimate photo-z's for "*

 * *            'the test_data.  We need to make the RAIL stages for each of these steps, first we '*

 * *            'need to train/inform our nearest neighbor algorithm with the train_data:")], delete: '*

 * *            " […]*

```diff
@@ -217,33 +217,33 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Using the data in a pipeline stage: photo-z estimation example\n",
                 "\n",
-                "Now that we have our data in place, we can use it in a RAIL stage.  As an example, we'll estimate photo-z's for our data.  Let's train the `KNearNeighPDF` algorithm with our train_data, and then estimate photo-z's for the test_data.  We need to make the RAIL stages for each of these steps, first we need to train/inform our nearest neighbor algorithm with the train_data:"
+                "Now that we have our data in place, we can use it in a RAIL stage.  As an example, we'll estimate photo-z's for our data.  Let's train the `KNearNeighEstimator` algorithm with our train_data, and then estimate photo-z's for the test_data.  We need to make the RAIL stages for each of these steps, first we need to train/inform our nearest neighbor algorithm with the train_data:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.estimation.algos.knnpz import Inform_KNearNeighPDF, KNearNeighPDF"
+                "from rail.estimation.algos.k_nearneigh import KNearNeighInformer, KNearNeighEstimator"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "inform_knn = Inform_KNearNeighPDF.make_stage(name='inform_knn', input='train_data', \n",
+                "inform_knn = KNearNeighInformer.make_stage(name='inform_knn', input='train_data', \n",
                 "                                            nondetect_val=99.0, model='knnpz.pkl',\n",
                 "                                            hdf5_groupname='')\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -264,15 +264,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "estimate_knn = KNearNeighPDF.make_stage(name='estimate_knn', hdf5_groupname='photometry', nondetect_val=99.0,\n",
+                "estimate_knn = KNearNeighEstimator.make_stage(name='estimate_knn', hdf5_groupname='photometry', nondetect_val=99.0,\n",
                 "                                        model='knnpz.pkl', output=\"KNNPZ_estimates.hdf5\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `pz-rail-0.99.1/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb` & `pz-rail-0.99.1.1/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/examples/core_examples/Pipe_Example.ipynb` & `pz-rail-0.99.1.1/examples/core_examples/Pipe_Example.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/examples/core_examples/README.md` & `pz-rail-0.99.1.1/examples/core_examples/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/examples/core_examples/Run_Pipe.ipynb` & `pz-rail-0.99.1.1/examples/core_examples/Run_Pipe.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/examples/core_examples/hyperbolic_magnitude_test.ipynb` & `pz-rail-0.99.1.1/examples/core_examples/hyperbolic_magnitude_test.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/examples/core_examples/iterator_test.ipynb` & `pz-rail-0.99.1.1/examples/core_examples/iterator_test.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/examples/core_examples/pipe_example.yml` & `pz-rail-0.99.1.1/examples/core_examples/pipe_example.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/examples/core_examples/pipe_example_config.yml` & `pz-rail-0.99.1.1/examples/core_examples/pipe_example_config.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/examples/creation_examples/README.md` & `pz-rail-0.99.1.1/examples/creation_examples/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/examples/creation_examples/degradation-demo.ipynb` & `pz-rail-0.99.1.1/examples/creation_examples/degradation-demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/examples/creation_examples/dsps_sed_demo.ipynb` & `pz-rail-0.99.1.1/examples/creation_examples/dsps_sed_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/examples/creation_examples/example_GridSelection_for_HSC.ipynb` & `pz-rail-0.99.1.1/examples/creation_examples/example_GridSelection_for_HSC.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/examples/creation_examples/example_ObsConditions.ipynb` & `pz-rail-0.99.1.1/examples/creation_examples/example_ObsConditions.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb` & `pz-rail-0.99.1.1/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/examples/creation_examples/photometric_realization_demo.ipynb` & `pz-rail-0.99.1.1/examples/creation_examples/photometric_realization_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/examples/creation_examples/posterior-demo.ipynb` & `pz-rail-0.99.1.1/examples/creation_examples/posterior-demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/examples/estimation_examples/NZDir.ipynb` & `pz-rail-0.99.1.1/examples/estimation_examples/NZDir.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99903400997151%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(0, 'from rail.estimation.algos.nz_dir import "*

 * *            "NZDirSummarizer, NZDirInformer\\n')], delete: [0]}}, 13: {'source': ['Now, let\\'s "*

 * *            'set up or estimator, first creating a stage for the informer.  We define any input '*

 * *            'variables in a dictionary and then use that with `make_stage` to create an instance '*

 * *            "of our NZDirSummarizer.  We\\'ll create a histogram of 25 bins, using 5 nearest "*

 * *            'neighbors to define our […]*

```diff
@@ -33,15 +33,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8ac92a6d-24d9-4413-8914-f99fe4f6d91d",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.estimation.algos.NZDir import NZDir, Inform_NZDir\n",
+                "from rail.estimation.algos.nz_dir import NZDirSummarizer, NZDirInformer\n",
                 "from rail.core.data import TableHandle\n",
                 "from rail.core.stage import RailStage"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "dc589b4b-abb4-4e3b-9665-cc395f028bef",
@@ -157,25 +157,25 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f65d4835-2ff6-4206-b017-cdf1d7cad828",
             "metadata": {},
             "source": [
-                "Now, let's set up or estimator, first creating a stage for the informer.  We define any input variables in a dictionary and then use that with `make_stage` to create an instance of our NZDir summarizer.  We'll create a histogram of 25 bins, using 5 nearest neighbors to define our specz neighborhood, and above we defined our bin column as \"bin\":"
+                "Now, let's set up or estimator, first creating a stage for the informer.  We define any input variables in a dictionary and then use that with `make_stage` to create an instance of our NZDirSummarizer.  We'll create a histogram of 25 bins, using 5 nearest neighbors to define our specz neighborhood, and above we defined our bin column as \"bin\":"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "59be250d-9ff7-43e5-9d8a-e31279c1eb61",
             "metadata": {},
             "outputs": [],
             "source": [
-                "train_nzdir = Inform_NZDir.make_stage(name='train_nzdir', n_neigh=5,\n",
+                "train_nzdir = NZDirInformer.make_stage(name='train_nzdir', n_neigh=5,\n",
                 "                                      szweightcol='weight', model=\"NZDir_model.pkl\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "9b1f5c76-b3fb-4ddc-a78e-afdd04a28e55",
@@ -221,15 +221,15 @@
             "outputs": [],
             "source": [
                 "%%time\n",
                 "bin_ens = {}\n",
                 "binnames = ['low', 'mid', 'hi']\n",
                 "bin_datasets = [low_bin, mid_bin, hi_bin]\n",
                 "for bin, indata in zip(binnames, bin_datasets):\n",
-                "    nzsumm = NZDir.make_stage(name=f'nzsumm_{bin}', **summdict)\n",
+                "    nzsumm = NZDirSummarizer.make_stage(name=f'nzsumm_{bin}', **summdict)\n",
                 "    bin_ens[f'{bin}'] = nzsumm.estimate(indata)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "bc38e44b-1a7e-4368-b70f-76c9f2882c3b",
             "metadata": {},
@@ -377,15 +377,15 @@
             "execution_count": null,
             "id": "7dfe5a6b-dfd1-4df9-a4f9-f28e9d39d41c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "xinformdict = dict(n_neigh=5, bincol=\"bin\", szweightcol='weight',\n",
                 "                   model=\"NZDir_model_incompl.pkl\", hdf5_groupname='')\n",
-                "newsumm_inform = Inform_NZDir.make_stage(name='newsumm_inform', **xinformdict)"
+                "newsumm_inform = NZDirInformer.make_stage(name='newsumm_inform', **xinformdict)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7f00b7dc-af25-4dec-8ea6-8e96f0885e26",
             "metadata": {},
@@ -412,15 +412,15 @@
                 "%%time\n",
                 "xestimatedict = dict(leafsize=20, zmin=zmin, zmax=zmax, nzbins=xmanybins, hdf5_groupname='', nsamples=20,\n",
                 "                     phot_weightcol='weight', model=newsumm_inform.get_handle('model'))\n",
                 "new_ens = {}\n",
                 "binnames = ['low', 'mid', 'hi']\n",
                 "bin_datasets = [low_bin, mid_bin, hi_bin]\n",
                 "for bin, indata in zip(binnames, bin_datasets):\n",
-                "    nzsumm = NZDir.make_stage(name=f'nzsumm_{bin}', **xestimatedict)\n",
+                "    nzsumm = NZDirSummarizer.make_stage(name=f'nzsumm_{bin}', **xestimatedict)\n",
                 "    new_ens[f'{bin}'] = nzsumm.estimate(indata)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7e9d255d-f634-47ae-9eca-02e3b134d56f",
```

### Comparing `pz-rail-0.99.1/examples/estimation_examples/RAIL_estimation_demo.ipynb` & `pz-rail-0.99.1.1/examples/estimation_examples/RAIL_estimation_demo.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976253105590063%*

 * *Differences: {"'cells'": "{7: {'source': {insert: [(2, '`Randompz` is a very simple class that does not "*

 * *            'actually predict a meaningful photo-z, instead it produces a randomly drawn Gaussian '*

 * *            "for each galaxy.<br>\\n'), (5, '`FlexZBoost` is a fully functional photo-z algorithm, "*

 * *            'implementing the FlexZBoost conditional density estimate method that was used in the '*

 * *            'PhotoZDC1 paper.  FlexZBoost has been moved to its own GitHub repo, and is available '*

 * *            'in th […]*

```diff
@@ -85,36 +85,36 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "You should see a list of the available photo-z algorithms, as printed out above.  These are the names of the specific subclasses that invoke a particular method, and they are stored in the `rail.estimation.algos` subdirectory of RAIL.<br>\n",
                 "\n",
-                "`randomPZ` is a very simple class that does not actually predict a meaningful photo-z, instead it produces a randomly drawn Gaussian for each galaxy.<br>\n",
+                "`Randompz` is a very simple class that does not actually predict a meaningful photo-z, instead it produces a randomly drawn Gaussian for each galaxy.<br>\n",
                 "`trainZ` is our \"pathological\" estimator, it makes a PDF from a histogram of the training data and assigns that PDF to every galaxy.<br>\n",
                 "`simpleNN` uses `sklearn`'s neural network to predict a point redshift from the training data, then assigns a sigma width based on the redshift, another toy model example<br>\n",
-                "`FZBoost` is a fully functional photo-z algorithm, implementing the FlexZBoost conditional density estimate method that was used in the PhotoZDC1 paper.  FlexZBoost has been moved to its own GitHub repo, and is available in the [rail_flexzboost](https://github.com/LSSTDESC/rail_flexzboost/) repo.<br>\n",
+                "`FlexZBoost` is a fully functional photo-z algorithm, implementing the FlexZBoost conditional density estimate method that was used in the PhotoZDC1 paper.  FlexZBoost has been moved to its own GitHub repo, and is available in the [rail_flexzboost](https://github.com/LSSTDESC/rail_flexzboost/) repo.<br>\n",
                 "`BPZ_lite` is a template-based code that outputs the posterior estimated given a specific template set and Bayesian prior. See Benitez (2000) for more details.<br>\n",
-                "`delightPZ` is a hybrid gaussian process/template-based code, see the [Delight](https://github.com/LSSTDESC/Delight) repo for more details.<br>\n",
-                "`KNearNeighPDF` is a simple implementation of a weighted k-nearest neighbor photo-z code, it stores each PDF as a weighted sum of Gaussians based on the distance from neighbors in color space.<br>\n",
-                "`PZFlowPDF` uses the same normalizing flow code [pzflow](https://github.com/jfcrenshaw/pzflow) used in the `creation` module to predict redshift PDFs.<br>\n",
+                "`delight_hybrid` is a hybrid gaussian process/template-based code, see the [Delight](https://github.com/LSSTDESC/Delight) repo for more details.<br>\n",
+                "`KNearNeighEstimator` is a simple implementation of a weighted k-nearest neighbor photo-z code, it stores each PDF as a weighted sum of Gaussians based on the distance from neighbors in color space.<br>\n",
+                "`PZFlowEstimator` uses the same normalizing flow code [pzflow](https://github.com/jfcrenshaw/pzflow) used in the `creation` module to predict redshift PDFs.<br>\n",
                 "\n",
-                "Each code should have two specific classes associated with it: one to train/inform using a set of training data, and a second to actually estimate the photo-z PDFs.  The naming pattern is `[name of code]` for the estimating class, and `Inform_[name of code]` for the training class, for example `FZBoost` and  `Inform_FZBoost`.  \n",
+                "Each code should have two specific classes associated with it: one to train/inform using a set of training data, and a second to actually estimate the photo-z PDFs.  These should be imported from the `src/rail/estimation/algos/[name_of_code].py` module (not exactly the package name to avoid namespace collisions). The naming pattern is `[NameOfCode]Estimator` for the estimating class, and `[NameOfCode]Informer` for the training/ingesting class, for example `FlexZBoostEstimator` and  `FlexZBoostInformer`.  \n",
                 "\n",
                 "The ceci code base will have us using a pattern where we will first run a `make_stage` method for the class in order to set up the ceci infrastructure.  Each `Inform_[name]` class will have a function called `inform` that actually performs the training.  Similarly, every `[photoz name]` class will have an `estimate` function to compute the PDFs.  We will show examples of this below.\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## The code-specific parameters\n",
                 "Each photo-z code will have code-specific parameters necessary to initialize the code.  These values can be input on the command line, or passed in via a dictionary.<br>\n",
                 "\n",
-                "Let's start with a very simple demonstration using `KNearNeighPDF`.  `KNearNeighPDF` is just `sklearn`'s nearest neighbor method run on the training data and set up within the RAIL interface.  It calculates a normalized weight for the K nearest neighbors based on their distance, and makes a PDF as a sum of K Gaussians, each at the redshift of the training galaxy with amplitude based on the distance weight, and a Gaussian width set by the user.  This is a toy model estimator, but it actually performs very well for representative data sets. There are configuration parameters for the names of columns, random seeds, etc... in KNearNeighPDF, but they are assigned sensible defaults, see the [KNearNeigh code](https://github.com/LSSTDESC/RAIL/blob/eac-dev/rail/estimation/algos/knnpz.py) for more details, but here is a minimal set to run:"
+                "Let's start with a very simple demonstration using `KNearNeighEstimator`.  `KNearNeighEstimator` is just `sklearn`'s nearest neighbor method run on the training data and set up within the RAIL interface.  It calculates a normalized weight for the K nearest neighbors based on their distance, and makes a PDF as a sum of K Gaussians, each at the redshift of the training galaxy with amplitude based on the distance weight, and a Gaussian width set by the user.  This is a toy model estimator, but it actually performs very well for representative data sets. There are configuration parameters for the names of columns, random seeds, etc... in KNearNeighEstimator, but they are assigned sensible defaults, see the [KNearNeigh code](https://github.com/LSSTDESC/RAIL/blob/eac-dev/rail/estimation/algos/k_nearneigh.py) for more details, but here is a minimal set to run:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -142,16 +142,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.estimation.algos.knnpz import Inform_KNearNeighPDF, KNearNeighPDF\n",
-                "pz_train = Inform_KNearNeighPDF.make_stage(name='inform_KNN', model='demo_knn.pkl', **knn_dict)"
+                "from rail.estimation.algos.k_nearneigh import KNearNeighInformer, KNearNeighEstimator\n",
+                "pz_train = KNearNeighInformer.make_stage(name='inform_KNN', model='demo_knn.pkl', **knn_dict)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now, let's load our training data, which is stored in hdf5 format.  We'll load it into the Data Store so that the ceci stages are able to access it."
@@ -172,15 +172,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We need to train the KDTree, which is done with the `inform` function present in every RAIL/estimation code. The parameter `model` is the name that the trained model object will be saved in pickle format, in this case `demo_knn.pkl`.  In the future, rather than re-run a potentially time consuming training set, we can simply load this pickle file before we run the estimate stage.<br>\n",
                 "\n",
-                "KNearNeighPDF.inform finds the best sigma and NNeigh and stores those along with the KDTree in the model."
+                "KNearNeighEstimator.inform finds the best sigma and NNeigh and stores those along with the KDTree in the model."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -198,15 +198,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pz = KNearNeighPDF.make_stage(name='KNN', hdf5_groupname='photometry',\n",
+                "pz = KNearNeighEstimator.make_stage(name='KNN', hdf5_groupname='photometry',\n",
                 "                              model=pz_train.get_handle('model'))\n",
                 "results = pz.estimate(test_data)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -303,25 +303,25 @@
                 "# FZBoost"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "That illustrates the basics, now let's try the `FZBoost` estimator.  FlexZBoost has been moved out of the \"main\" RAIL repo, and is available in the [rail_flexzboost](https://github.com/LSSTDESC/rail_flexzboost/) repo.  You can install by cloning that repo and installing directly, or you can install it via PyPI by simply running the command <br> \n",
+                "That illustrates the basics, now let's try the `FlexZBoostEstimator` estimator.  FlexZBoost has been moved out of the \"base\" RAIL repo, and is available in the [rail_flexzboost](https://github.com/LSSTDESC/rail_flexzboost/) repo.  You can install by cloning that repo and installing directly, or you can install it via PyPI by simply running the command <br> \n",
                 "`pip install pz-rail-flexzboost` <br>\n",
                 "on the command line.  Once installed, it will function the same as any of the other estimators included in the main RAIL repo.\n",
                 "\n",
-                "`FZBoost` finds a conditional density estimate for each PDF via a set of weights for basis functions.  This can save space relative to a gridded parameterization, but it also sometimes leads to residual \"bumps\" in the PDF from the underlying parameterization.  For this reason, `FZBoost` has a post-processing stage where it \"trims\" (i.e. sets to zero) any \"bumps\" below a certain threshold.<br>\n",
+                "`FlexZBoostEstimator` finds a conditional density estimate for each PDF via a set of weights for basis functions.  This can save space relative to a gridded parameterization, but it also sometimes leads to residual \"bumps\" in the PDF from the underlying parameterization.  For this reason, `FlexZBoostEstimator` has a post-processing stage where it \"trims\" (i.e. sets to zero) any \"bumps\" below a certain threshold.<br>\n",
                 "\n",
-                "One of the dominant features seen in our PhotoZDC1 analysis of multiple photo-z codes (Schmidt, Malz et al. 2020) was that photo-z estimates were often, in general, overconfident or underconfident in their overall uncertainty in PDFs.  To remedy this, `FZBoost` has an additional post-processing step where it estimates a \"sharpening\" parameter that modulates the width of the PDFs.<br>\n",
+                "One of the dominant features seen in our PhotoZDC1 analysis of multiple photo-z codes (Schmidt, Malz et al. 2020) was that photo-z estimates were often, in general, overconfident or underconfident in their overall uncertainty in PDFs.  To remedy this, `FlexZBoostEstimator` has an additional post-processing step where it estimates a \"sharpening\" parameter that modulates the width of the PDFs.<br>\n",
                 "\n",
                 "A portion of the training data is held in reserve to find best-fit values for both `bump_thresh` and `sharpening`, which we find by simply calculating the CDE loss for a grid of `bump_thresh` and `sharpening` values.<br>\n",
                 "\n",
-                "We'll start with a dictionary of setup parameters for FZBoost, just as we had for simpleNN.  Some of the parameters are the same as in `simpleNN` above, `zmin`, `zmax`, `nzbins`.  However, FZBoost performs a more in depth training than simpleNN, and as such has more input parameters to control behavior.  These parameters are:<br>\n",
+                "We'll start with a dictionary of setup parameters for FlexZBoostEstimator, just as we had for the scikit-learn neural network.  Some of the parameters are the same as in `skl_neurnet` above, `zmin`, `zmax`, `nzbins`.  However, FlexZBoostEstimator performs a more in depth training than simpleNN, and as such has more input parameters to control behavior.  These parameters are:<br>\n",
                 "`basis_system`: which basis system to use in the density estimate. The default is `cosine` but `fourier` is also an option<br>\n",
                 "`max_basis`: the maximum number of basis functions parameters to use for PDFs<br>\n",
                 "`regression_params`: a dictionary of options fed to `xgboost` that control the maximum depth and the `objective` function.  An update in `xgboost` means that `objective` should now be set to `reg:squarederror` for proper functioning.<br>\n",
                 "`trainfrac`: The fraction of the training data to use for training the density estimate.  The remaining galaxies will be used for validation of `bump_thresh` and `sharpening`.<br>\n",
                 "`bumpmin`: the minimum value to test in the `bump_thresh` grid<br>\n",
                 "`bumpmax`: the maximum value to test in the `bump_thresh` grid<br>\n",
                 "`nbump`: how many points to test in the `bump_thresh` grid<br>\n",
@@ -345,24 +345,24 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.estimation.algos.flexzboost import Inform_FZBoost, FZBoost\n",
-                "inform_pzflex = Inform_FZBoost.make_stage(name='inform_fzboost', model=fz_modelfile, **fz_dict)"
+                "from rail.estimation.algos.flexzboost import FlexZBoostInformer, FlexZBoostEstimator\n",
+                "inform_pzflex = FlexZBoostInformer.make_stage(name='inform_fzboost', model=fz_modelfile, **fz_dict)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We can now use this data to train our model using `FZBoost`'s inform() method.  `FZBoost` uses xgboost to determine a conditional density estimate model, and also fits a `bump_thresh` parameter that erases small peaks that are an artifact of the `cosine` parameterization.  It then finds a best fit `sharpen` parameter that modulates the peaks with a power law.<br>\n",
-                "We have `save_train` set to `True` in our `inform_options`, so this will save a pickled version of the best fit model to the file specified in `inform_options['modelfile']`, which is set above to `demo_FZB_model.pkl`.  We can use the same training data that we used for `simpleNN`.  `FZBoost` is a bit more sophisticated than `simpleNN`, so it will take a bit longer to train (note: it should take about 10-15 minutes on cori for the 10,000 galaxies in our demo sample):"
+                "We can now use this data to train our model using the `FlexZBoostInformer`.  `FlexZBoost` uses xgboost to determine a conditional density estimate model, and also fits a `bump_thresh` parameter that erases small peaks that are an artifact of the `cosine` parameterization.  It then finds a best fit `sharpen` parameter that modulates the peaks with a power law.<br>\n",
+                "We have `save_train` set to `True` in our `inform_options`, so this will save a pickled version of the best fit model to the file specified in `inform_options['modelfile']`, which is set above to `demo_FZB_model.pkl`.  We can use the same training data that we used for `skl_neurnet`.  `FlexZBoost` is a bit more sophisticated than `skl_neurnet`, so it will take a bit longer to train (note: it should take about 10-15 minutes on cori for the 10,000 galaxies in our demo sample):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -392,27 +392,27 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "%%time\n",
-                "pzflex = FZBoost.make_stage(name='fzboost', hdf5_groupname='photometry',\n",
+                "pzflex = FlexZBoostEstimator.make_stage(name='fzboost', hdf5_groupname='photometry',\n",
                 "                            model=inform_pzflex.get_handle('model'))\n",
                 "\n",
                 "# For this notebook, we will use the default value of qp_representation as shown\n",
                 "# above due to the additional computation time that would be required in the\n",
                 "# later steps when working with the flexzboost representation.\n",
                 "# Below are two examples showing the explicit use of the qp_representation argument.\n",
                 "\"\"\"\n",
-                "pzflex = FZBoost.make_stage(name='fzboost', hdf5_groupname='photometry',\n",
+                "pzflex = FlexZBoostEstimator.make_stage(name='fzboost', hdf5_groupname='photometry',\n",
                 "                            model=inform_pzflex.get_handle('model'),\n",
                 "                            qp_representation='interp')\n",
                 "\n",
-                "pzflex = FZBoost.make_stage(name='fzboost', hdf5_groupname='photometry',\n",
+                "pzflex = FlexZBoostEstimator.make_stage(name='fzboost', hdf5_groupname='photometry',\n",
                 "                            model=inform_pzflex.get_handle('model'),\n",
                 "                            qp_representation='flexzboost')\n",
                 "\"\"\""
             ]
         },
         {
             "cell_type": "markdown",
@@ -505,22 +505,22 @@
             "outputs": [],
             "source": [
                 "plt.figure(figsize=(10,10))\n",
                 "plt.scatter(test_data()['photometry']['redshift'],fz_modes,s=1,c='k')\n",
                 "plt.plot([0,3],[0,3],'r--')\n",
                 "plt.xlabel(\"true redshift\")\n",
                 "plt.ylabel(\"photoz mode\")\n",
-                "plt.title(\"median point estimate for FZBoost\");"
+                "plt.title(\"median point estimate for FlexZBoost\");"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The results look very good! FZBoost is a mature algorithm, and with representative training data we see a very tight correlation with true redshift and few outliers.<br>"
+                "The results look very good! FlexZBoost is a mature algorithm, and with representative training data we see a very tight correlation with true redshift and few outliers.<br>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `pz-rail-0.99.1/examples/estimation_examples/README.md` & `pz-rail-0.99.1.1/examples/estimation_examples/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 This directory contains example notebooks explaining how to use the RAIL Estimation Module.
 
 - [nzdir_as_pipeline](https://lsstdescrail.readthedocs.io/en/latest/source/estimation-notebooks.html#the-nzdir-estimator) provides a quick demo of the NZDir estimator.
 
 - **RAIL_estimation_demo.ipynb** explains to inform a model used for photo-z estimation, and then how to use that model to estimate p(z).
 
-- **SimpleSOM_demo.ipynb**, **somocluSOM_demo.ipynb**, and **somocluSOMcluster_demo.ipynb** demonstrate of the use of the `SimpleSOMSummarizer` summarization module.
+- **SimpleSOM_demo.ipynb**, **somocluSOM_demo.ipynb**, and **somocluSOMcluster_demo.ipynb** demonstrate of the use of the `MiniSOMSummarizer` summarization module.
 
-- [test_sampled_summarizers.ipynb](https://lsstdescrail.readthedocs.io/en/latest/source/estimation-notebooks.html#testing-sampled-summarizers) outlines quick and dirty bootstrap versions of the `NaiveStack`, `PointEstimateHist`, and `VarInference` sumarizers, as well as `NZDir`.
+- [test_sampled_summarizers.ipynb](https://lsstdescrail.readthedocs.io/en/latest/source/estimation-notebooks.html#testing-sampled-summarizers) outlines quick and dirty bootstrap versions of the `NaiveStackSummarizer`, `PointEstHistSummarizer`, and `VarInference` sumarizers, as well as `NZDirSummarizer`.
```

### Comparing `pz-rail-0.99.1/examples/estimation_examples/SimpleSOM_demo.ipynb.fixme` & `pz-rail-0.99.1.1/examples/estimation_examples/SimpleSOM_demo.ipynb.fixme`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989583333333333%*

 * *Differences: {"'cells'": "{0: {'source': ['# MiniSOMSummarizer demo']}, 1: {'source': {insert: [(3, 'This "*

 * *            'notebook shows a quick demonstration of the use of the `MiniSOMSummarizer` '*

 * *            'summarization module.  Algorithmically, this module is not very different from the '*

 * *            'NZDir estimator/summarizer.  NZDir operates by finding neighboring photometric points '*

 * *            'around spectroscopic objects.  MiniSOMSummarizer takes a large training set of data '*

 * *            'in the `Inform_S […]*

```diff
@@ -1,26 +1,26 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "08afaafe",
             "metadata": {},
             "source": [
-                "# SimpleSOMSummarizer demo"
+                "# MiniSOMSummarizer demo"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a7f57f69",
             "metadata": {},
             "source": [
                 "Author: Sam Schmidt <br>\n",
                 "Last successfully run: April 26, 2023<br>\n",
                 "\n",
-                "This notebook shows a quick demonstration of the use of the `SimpleSOMSummarizer` summarization module.  Algorithmically, this module is not very different from the NZDir estimator/summarizer.  NZDir operates by finding neighboring photometric points around spectroscopic objects.  SimpleSOMSummarizer takes a large training set of data in the `Inform_SimpleSOMSUmmarizer` stage and trains a self-organized map (SOM) (using code from the `minisom` package available at: https://github.com/JustGlowing/minisom).  Once the SOM is set up, the \"winning\"/best-fit cells are determined for both the photometric/unknown data and a set of spectroscopic data with known redshifts.  For each SOM cell, the algorithm constructs a histogram using the spectroscopic members mapped to that cell, and weights these by the number of photometric galaxies in that cell.  Both the photometric and spectroscopic datasets can also employ an optional weight per-galaxy. <br>\n",
+                "This notebook shows a quick demonstration of the use of the `MiniSOMSummarizer` summarization module.  Algorithmically, this module is not very different from the NZDir estimator/summarizer.  NZDir operates by finding neighboring photometric points around spectroscopic objects.  MiniSOMSummarizer takes a large training set of data in the `Inform_SimpleSOMSUmmarizer` stage and trains a self-organized map (SOM) (using code from the `minisom` package available at: https://github.com/JustGlowing/minisom).  Once the SOM is set up, the \"winning\"/best-fit cells are determined for both the photometric/unknown data and a set of spectroscopic data with known redshifts.  For each SOM cell, the algorithm constructs a histogram using the spectroscopic members mapped to that cell, and weights these by the number of photometric galaxies in that cell.  Both the photometric and spectroscopic datasets can also employ an optional weight per-galaxy. <br>\n",
                 "\n",
                 "The summarizer also identifies SOM cells that contain photometric data but do not contain and galaxies with a measured spec-z, and thus do not have an obvious redshift estimate.  It writes out the (raveled) SOM cell indices that contain \"uncovered\"/uncalibratable data to the file specified by the `uncovered_cell_file` option as a list of integers.  The cellIDs and galaxy/objIDs for all photometric galaxies will be written out to the file specified by the `cellid_output` parameter.  Any galaxies in these cells should really be removed, and thus some iteration may be necessary in defining bin membership by looking at the properties of objects in these uncovered cells before a final N(z) is estimated, as otherwise a bias may be present.<br>\n",
                 "\n",
                 "The shape and number of cells used in constructing the SOM affects performance, as do several tuning parameters.  This paper, http://www.giscience2010.org/pdfs/paper_230.pdf gives a rough guideline that the number of cells should be of the order ~ 5 x sqrt (number of data rows x number of column rows), though this is a rough guide.  Some studies have found a 2D SOM that is more elongated in one direction to be preferential, while others claim that a square layout is optimal, the user can set the number of cells in each SOM dimension via the `n_dim` and `m_dim` parameters.  For more discussion on SOMs see the Appendices of this KiDS paper:  http://arxiv.org/abs/1909.09632.\n",
                 "\n",
                 "As with the other RAIL summarizers, we bootstrap the spectroscopic sample and return N bootstraps in an ensemble, along with a single fiducial N(z) estimate.<br>\n",
                 "\n",
@@ -86,15 +86,15 @@
             "id": "f9259d6d",
             "metadata": {},
             "outputs": [],
             "source": [
                 "training_file = \"./healpix_10326_bright_data.hdf5\"\n",
                 "\n",
                 "if not os.path.exists(training_file):\n",
-                "  os.system('curl -O https://portal.nersc.gov/cfs/lsst/schmidt9/healpix_10326_bright_data.hdf5')"
+                "  os.system('curl -O https://portal.nersc.gov/cfs/lsst/PZ/healpix_10326_bright_data.hdf5')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "4bc6e218",
             "metadata": {},
@@ -116,15 +116,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8aeca17a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.estimation.algos.simpleSOM import Inform_SimpleSOMSummarizer"
+                "from rail.estimation.algos.minisom_som import MiniSOMInformer"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d26f1b0b",
             "metadata": {},
             "source": [
@@ -156,15 +156,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "db96d9e7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "inform_som = Inform_SimpleSOMSummarizer.make_stage(name='inform_som', **inform_dict)"
+                "inform_som = MiniSOMInformer.make_stage(name='inform_som', **inform_dict)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8dc8d42d",
             "metadata": {},
             "source": [
@@ -387,15 +387,15 @@
         },
         {
             "cell_type": "markdown",
             "id": "6a47fe3f",
             "metadata": {},
             "source": [
                 "Note that we have removed the 'photometry' group, we will specify the `phot_groupname` as \"\" in the parameters below.<br>\n",
-                "As before, let us specify our initialization params for the SimpleSOMSummarizer stage, including:<br>\n",
+                "As before, let us specify our initialization params for the MiniSOMSummarizer stage, including:<br>\n",
                 "`model`: name of the pickled model that we created, in this case \"output_SOM_model.pkl\"<br>\n",
                 "`hdf5_groupname` (str): hdf5 group for our photometric data (in our case \"\")<br>\n",
                 "`objid_name` (str): string specifying the name of the ID column, if present photom data, will be written out to cellid_output file<br>\n",
                 "`spec_groupname` (str): hdf5 group for the spectroscopic data<br>\n",
                 "`nzbins` (int): number of bins to use in our histogram ensemble<br>\n",
                 "`nsamples` (int): number of bootstrap samples to generate<br>\n",
                 "`output` (str): name of the output qp file with N samples<br>\n",
@@ -429,16 +429,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "64993ca8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.estimation.algos.simpleSOM import SimpleSOMSummarizer\n",
-                "som_summarizer = SimpleSOMSummarizer.make_stage(name='SOM_summarizer', **summ_dict)"
+                "from rail.estimation.algos.minisom_som import MiniSOMSummarizer\n",
+                "som_summarizer = MiniSOMSummarizer.make_stage(name='SOM_summarizer', **summ_dict)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d05dd94f",
             "metadata": {},
@@ -498,15 +498,15 @@
             "source": [
                 "bright_dict = dict(model=\"output_SOM_model.pkl\", hdf5_groupname='photometry',\n",
                 "                   spec_groupname='photometry', nzbins=101, nsamples=25,\n",
                 "                   output='BRIGHT_SOM_ensemble.hdf5', single_NZ='BRIGHT_fiducial_SOM_NZ.hdf5',\n",
                 "                   uncovered_cell_file=\"BRIGHT_uncovered_cells.hdf5\",\n",
                 "                   objid_name='id',\n",
                 "                   cellid_output='BRIGHT_output_cellIDs.hdf5')\n",
-                "bright_summarizer = SimpleSOMSummarizer.make_stage(name='bright_summarizer', **bright_dict)"
+                "bright_summarizer = MiniSOMSummarizer.make_stage(name='bright_summarizer', **bright_dict)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "4b2911b7",
             "metadata": {},
```

### Comparing `pz-rail-0.99.1/examples/estimation_examples/nzdir_as_pipeline.ipynb` & `pz-rail-0.99.1.1/examples/estimation_examples/nzdir_as_pipeline.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995089786756453%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(7, 'from rail.estimation.algos.nz_dir import NZDirInformer, "*

 * *            "NZDirSummarizer\\n')], delete: [7]}}, 4: {'source': {insert: [(0, 'inf_nz = "*

 * *            'NZDirInformer.make_stage(n_neigh=8, hdf5_groupname="photometry", '*

 * *            'model="nzdir_model.pkl")\\n\'), (2, \'nzd = NZDirSummarizer.make_stage(leafsize=20, '*

 * *            'zmin=0.0, zmax=3.0, nzbins=31, model="NZDir_model.pkl", '*

 * *            "hdf5_groupname=\\'photometry\\',\\n')], delete: [2, 0]}}} […]*

```diff
@@ -19,15 +19,15 @@
                 "import os\n",
                 "import rail\n",
                 "import qp\n",
                 "import numpy as np\n",
                 "import pandas as pd\n",
                 "import matplotlib.pyplot as plt\n",
                 "%matplotlib inline\n",
-                "from rail.estimation.algos.NZDir import Inform_NZDir, NZDir\n",
+                "from rail.estimation.algos.nz_dir import NZDirInformer, NZDirSummarizer\n",
                 "from rail.core.data import TableHandle, QPHandle\n",
                 "from rail.core.stage import RailStage"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -57,17 +57,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ba6247dc",
             "metadata": {},
             "outputs": [],
             "source": [
-                "inf_nz = Inform_NZDir.make_stage(n_neigh=8, hdf5_groupname=\"photometry\", model=\"nzdir_model.pkl\")\n",
+                "inf_nz = NZDirInformer.make_stage(n_neigh=8, hdf5_groupname=\"photometry\", model=\"nzdir_model.pkl\")\n",
                 "inf_nz.inform(training_data)\n",
-                "nzd = NZDir.make_stage(leafsize=20, zmin=0.0, zmax=3.0, nzbins=31, model=\"NZDir_model.pkl\", hdf5_groupname='photometry',\n",
+                "nzd = NZDirSummarizer.make_stage(leafsize=20, zmin=0.0, zmax=3.0, nzbins=31, model=\"NZDir_model.pkl\", hdf5_groupname='photometry',\n",
                 "                       output='NZDir_samples.hdf5', single_NZ='NZDir_NZ.hdf5')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "14a87af8",
```

### Comparing `pz-rail-0.99.1/examples/estimation_examples/somocluSOM_demo.ipynb` & `pz-rail-0.99.1.1/examples/estimation_examples/somocluSOM_demo.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975983118657299%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, 'Last successfully run: June 16, 2023<br>\\n')], delete: "*

 * *            '[1]}}, 6: {\'source\': {insert: [(3, "  os.system(\'curl -O '*

 * *            'https://portal.nersc.gov/cfs/lsst/PZ/healpix_10326_bright_data.hdf5\')")], delete: '*

 * *            "[3]}}, 9: {'source': ['from rail.estimation.algos.somoclu_som import *']}, 12: "*

 * *            '{\'source\': ["inform_som = SOMocluInformer.make_stage(name=\'inform_som\', '*

 * *            '**inform_dict)"]}, 20: {\'source\': [\'W […]*

```diff
@@ -10,15 +10,15 @@
         },
         {
             "cell_type": "markdown",
             "id": "f40c36ff",
             "metadata": {},
             "source": [
                 "Author: Ziang Yan, Sam Schmidt <br>\n",
-                "Last successfully run: April 26, 2023<br>\n",
+                "Last successfully run: June 16, 2023<br>\n",
                 "\n",
                 "This notebook shows a quick demonstration of the use of the `SOMocluSummarizer` summarization module.  Algorithmically, this module is not very different from the NZDir estimator/summarizer.  NZDir operates by finding neighboring photometric points around spectroscopic objects.  SOMocluSummarizer takes a large training set of data in the `Inform_SOMocluUmmarizer` stage and trains a self-organized map (SOM) (using code from the `somoclu` package available at: https://github.com/peterwittek/somoclu/).  Once the SOM is set up, the \"best match unit\" are determined for both the photometric/unknown data and a set of spectroscopic data with known redshifts.  For each SOM cell, the algorithm constructs a histogram using the spectroscopic members mapped to that cell, and weights these by the number of photometric galaxies in that cell.  Both the photometric and spectroscopic datasets can also employ an optional weight per-galaxy. <br>\n",
                 "\n",
                 "The summarizer also identifies SOM cells that contain photometric data but do not contain and galaxies with a measured spec-z, and thus do not have an obvious redshift estimate.  It writes out the (raveled) SOM cell indices that contain \"uncovered\"/uncalibratable data to the file specified by the `uncovered_cell_file` option as a list of integers.  The cellIDs and galaxy/objIDs for all photometric galaxies will be written out to the file specified by the `cellid_output` parameter.  Any galaxies in these cells should really be removed, and thus some iteration may be necessary in defining bin membership by looking at the properties of objects in these uncovered cells before a final N(z) is estimated, as otherwise a bias may be present.<br>\n",
                 "\n",
                 "The shape and number of cells used in constructing the SOM affects performance, as do several tuning parameters.  This paper, http://www.giscience2010.org/pdfs/paper_230.pdf gives a rough guideline that the number of cells should be of the order ~ 5 x sqrt (number of data rows x number of column rows), though this is a rough guide.  Some studies have found a 2D SOM that is more elongated in one direction to be preferential, while others claim that a square layout is optimal, the user can set the number of cells in each SOM dimension via the `n_rows` and `n_cols` parameters.  For more discussion on SOMs see the Appendices of this KiDS paper:  http://arxiv.org/abs/1909.09632.\n",
                 "\n",
@@ -85,15 +85,15 @@
             "id": "f9429565",
             "metadata": {},
             "outputs": [],
             "source": [
                 "training_file = \"./healpix_10326_bright_data.hdf5\"\n",
                 "\n",
                 "if not os.path.exists(training_file):\n",
-                "  os.system('curl -O https://portal.nersc.gov/cfs/lsst/schmidt9/healpix_10326_bright_data.hdf5')"
+                "  os.system('curl -O https://portal.nersc.gov/cfs/lsst/PZ/healpix_10326_bright_data.hdf5')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "90e006d2",
             "metadata": {},
@@ -114,15 +114,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a27535d9",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.estimation.algos.somocluSOM import *"
+                "from rail.estimation.algos.somoclu_som import *"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4463c9b7",
             "metadata": {},
             "source": [
@@ -156,15 +156,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "1a5e5eb2",
             "metadata": {},
             "outputs": [],
             "source": [
-                "inform_som = Inform_somocluSOMSummarizer.make_stage(name='inform_som', **inform_dict)"
+                "inform_som = SOMocluInformer.make_stage(name='inform_som', **inform_dict)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "08c7b9a3",
             "metadata": {},
             "source": [
@@ -241,15 +241,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a7c85072",
             "metadata": {},
             "source": [
-                "We can calculate the best SOM cell using the get_bmus() function defined in somocluSOM.py, which will return the 2D SOM coordinates for each galaxy, and then use these for our visualizations (this step might take a while):"
+                "We can calculate the best SOM cell using the get_bmus() function defined in somoclu_som.py, which will return the 2D SOM coordinates for each galaxy, and then use these for our visualizations (this step might take a while):"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "af1719a6",
             "metadata": {},
@@ -416,15 +416,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "defa2827",
             "metadata": {},
             "outputs": [],
             "source": [
-                "som_summarizer = somocluSOMSummarizer.make_stage(name='SOMoclu_summarizer', **summ_dict)"
+                "som_summarizer = SOMocluSummarizer.make_stage(name='SOMoclu_summarizer', **summ_dict)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6b80aab2",
             "metadata": {},
@@ -506,15 +506,15 @@
             "source": [
                 "bright_dict = dict(model=\"output_SOMoclu_model.pkl\", hdf5_groupname='photometry',\n",
                 "                   spec_groupname='photometry', nzbins=101, nsamples=25,\n",
                 "                   output='BRIGHT_SOMoclu_ensemble.hdf5', single_NZ='BRIGHT_fiducial_SOMoclu_NZ.hdf5',\n",
                 "                   uncovered_cell_file=\"BRIGHT_uncovered_cells.hdf5\",\n",
                 "                   objid_name='id',\n",
                 "                   cellid_output='BRIGHT_output_cellIDs.hdf5')\n",
-                "bright_summarizer = somocluSOMSummarizer.make_stage(name='bright_summarizer', **bright_dict)"
+                "bright_summarizer = SOMocluSummarizer.make_stage(name='bright_summarizer', **bright_dict)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ee4adc22",
             "metadata": {},
@@ -766,15 +766,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.10.11"
         },
         "widgets": {
             "application/vnd.jupyter.widget-state+json": {
                 "state": {},
                 "version_major": 2,
                 "version_minor": 0
             }
```

### Comparing `pz-rail-0.99.1/examples/estimation_examples/somocluSOMcluster_demo.ipynb` & `pz-rail-0.99.1.1/examples/estimation_examples/somocluSOMcluster_demo.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978688291555938%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, 'Last successfully run: June 16, 2023<br>\\n')], delete: "*

 * *            "[1]}}, 2: {'source': {insert: [(11, 'from rail.estimation.algos.somoclu_som import "*

 * *            "SOMocluInformer, SOMocluSummarizer\\n'), (12, 'from rail.estimation.algos.somoclu_som "*

 * *            'import get_bmus, plot_som\')], delete: [12, 11]}}, 6: {\'source\': {insert: [(3, "  '*

 * *            "os.system('curl -O "*

 * *            'https://portal.nersc.gov/cfs/lsst/PZ/healpix_10326_bright_data.hdf […]*

```diff
@@ -10,15 +10,15 @@
         },
         {
             "cell_type": "markdown",
             "id": "17cd4514",
             "metadata": {},
             "source": [
                 "Author: Ziang Yan, Sam Schmidt <br>\n",
-                "Last successfully run: April 26, 2023<br>\n",
+                "Last successfully run: June 16, 2023<br>\n",
                 "\n",
                 "This notebook shows a quick demonstration of the use of the `SOMocluSummarizer` summarization module.  Algorithmically, this module is not very different from the NZDir estimator/summarizer.  NZDir operates by finding neighboring photometric points around spectroscopic objects.  SOMocluSummarizer takes a large training set of data in the `Inform_SOMocluUmmarizer` stage and trains a self-organized map (SOM) (using code from the `somoclu` package available at: https://github.com/peterwittek/somoclu/).  Once the SOM is set up, the \"best match unit\" are determined for both the photometric/unknown data and a set of spectroscopic data with known redshifts.  For each SOM cell, the algorithm constructs a histogram using the spectroscopic members mapped to that cell, and weights these by the number of photometric galaxies in that cell.  Both the photometric and spectroscopic datasets can also employ an optional weight per-galaxy. <br>\n",
                 "\n",
                 "The summarizer also identifies SOM cells that contain photometric data but do not contain and galaxies with a measured spec-z, and thus do not have an obvious redshift estimate.  It writes out the (raveled) SOM cell indices that contain \"uncovered\"/uncalibratable data to the file specified by the `uncovered_cell_file` option as a list of integers.  The cellIDs and galaxy/objIDs for all photometric galaxies will be written out to the file specified by the `cellid_output` parameter.  Any galaxies in these cells should really be removed, and thus some iteration may be necessary in defining bin membership by looking at the properties of objects in these uncovered cells before a final N(z) is estimated, as otherwise a bias may be present.<br>\n",
                 "\n",
                 "The shape and number of cells used in constructing the SOM affects performance, as do several tuning parameters.  This paper, http://www.giscience2010.org/pdfs/paper_230.pdf gives a rough guideline that the number of cells should be of the order ~ 5 x sqrt (number of data rows x number of column rows), though this is a rough guide.  Some studies have found a 2D SOM that is more elongated in one direction to be preferential, while others claim that a square layout is optimal, the user can set the number of cells in each SOM dimension via the `n_rows` and `n_cols` parameters.  For more discussion on SOMs see the Appendices of this KiDS paper:  http://arxiv.org/abs/1909.09632.\n",
                 "\n",
@@ -43,16 +43,16 @@
                 "import rail\n",
                 "import os\n",
                 "import qp\n",
                 "import tables_io\n",
                 "from rail.core.data import TableHandle\n",
                 "from rail.core.stage import RailStage\n",
                 "from rail.core.utils import RAILDIR\n",
-                "from rail.estimation.algos.somocluSOM import Inform_somocluSOMSummarizer, somocluSOMSummarizer\n",
-                "from rail.estimation.algos.somocluSOM import get_bmus, plot_som"
+                "from rail.estimation.algos.somoclu_som import SOMocluInformer, SOMocluSummarizer\n",
+                "from rail.estimation.algos.somoclu_som import get_bmus, plot_som"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "31350a6b",
             "metadata": {},
             "source": [
@@ -88,15 +88,15 @@
             "id": "2919bc24",
             "metadata": {},
             "outputs": [],
             "source": [
                 "training_file = \"./healpix_10326_bright_data.hdf5\"\n",
                 "\n",
                 "if not os.path.exists(training_file):\n",
-                "  os.system('curl -O https://portal.nersc.gov/cfs/lsst/schmidt9/healpix_10326_bright_data.hdf5')"
+                "  os.system('curl -O https://portal.nersc.gov/cfs/lsst/PZ/healpix_10326_bright_data.hdf5')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "bf29fc00",
             "metadata": {},
@@ -149,15 +149,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "62103ddf",
             "metadata": {},
             "outputs": [],
             "source": [
-                "inform_som = Inform_somocluSOMSummarizer.make_stage(name='inform_som', **inform_dict)"
+                "inform_som = SOMocluInformer.make_stage(name='inform_som', **inform_dict)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "706c5483",
             "metadata": {},
             "source": [
@@ -224,15 +224,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "79a1512b",
             "metadata": {},
             "source": [
-                "We can calculate the best SOM cell using the get_bmus() function defined in somocluSOM.py, which will return the 2D SOM coordinates for each galaxy. Then we group the SOM cells into 100 hierarchical clusters and calculate the occupation and mean redshift in each cluster. "
+                "We can calculate the best SOM cell using the get_bmus() function defined in somoclu_som.py, which will return the 2D SOM coordinates for each galaxy. Then we group the SOM cells into 100 hierarchical clusters and calculate the occupation and mean redshift in each cluster. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c6c3f518",
             "metadata": {},
@@ -441,15 +441,15 @@
             "source": [
                 "summ_dict = dict(model=\"output_SOMoclu_model.pkl\", hdf5_groupname='photometry',\n",
                 "                 spec_groupname='photometry', nzbins=101, nsamples=25,\n",
                 "                 output='SOM_ensemble.hdf5', single_NZ='fiducial_SOMoclu_NZ.hdf5',\n",
                 "                 uncovered_cell_file='all_uncovered_cells.hdf5',\n",
                 "                 objid_name='id',\n",
                 "                 cellid_output='output_cellIDs.hdf5')\n",
-                "som_summarizer = somocluSOMSummarizer.make_stage(name='SOMoclu_summarizer', **summ_dict)    \n",
+                "som_summarizer = SOMocluSummarizer.make_stage(name='SOMoclu_summarizer', **summ_dict)    \n",
                 "som_summarizer.summarize(test_data, spec_data)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "86f9f03d",
@@ -510,15 +510,15 @@
                 "    summ_dict = dict(model=\"output_SOMoclu_model.pkl\", hdf5_groupname='photometry',\n",
                 "                 spec_groupname='photometry', nzbins=101, nsamples=25,\n",
                 "                 output='SOM_ensemble.hdf5', single_NZ='fiducial_SOMoclu_NZ.hdf5',\n",
                 "                 n_clusters=n_clusters,\n",
                 "                 uncovered_cell_file='all_uncovered_cells.hdf5',\n",
                 "                 objid_name='id',\n",
                 "                 cellid_output='output_cellIDs.hdf5')\n",
-                "    som_summarizer = somocluSOMSummarizer.make_stage(name='SOMoclu_summarizer', **summ_dict)    \n",
+                "    som_summarizer = SOMocluSummarizer.make_stage(name='SOMoclu_summarizer', **summ_dict)    \n",
                 "    som_summarizer.summarize(test_data, spec_data)\n",
                 "    \n",
                 "    full_ens = qp.read(\"SOM_ensemble.hdf5\")\n",
                 "    full_means = full_ens.mean().flatten()\n",
                 "    full_stds = full_ens.std().flatten()\n",
                 "    \n",
                 "    # mean and width of bootstraps\n",
@@ -582,15 +582,15 @@
                 "                 spec_groupname='photometry', nzbins=101, nsamples=25,\n",
                 "                 output='SOM_ensemble.hdf5', single_NZ='fiducial_SOMoclu_NZ.hdf5',\n",
                 "                 n_clusters=1000,\n",
                 "                 uncovered_cell_file='all_uncovered_cells.hdf5',\n",
                 "                 objid_name='id',\n",
                 "                 cellid_output='output_cellIDs.hdf5')\n",
                 "\n",
-                "som_summarizer = somocluSOMSummarizer.make_stage(name='SOMoclu_summarizer', **summ_dict)\n",
+                "som_summarizer = SOMocluSummarizer.make_stage(name='SOMoclu_summarizer', **summ_dict)\n",
                 "som_summarizer.summarize(test_data, spec_data)\n",
                 "\n",
                 "test_nz_hist, zbin = get_cont_hist(test_data.data['photometry']['redshift'], np.linspace(0,3,101))\n",
                 "som_nz_hist = np.squeeze(fid_ens.pdf(zbin))"
             ]
         },
         {
@@ -626,15 +626,15 @@
                 "bright_dict = dict(model=\"output_SOMoclu_model.pkl\", hdf5_groupname='photometry',\n",
                 "                   spec_groupname='photometry', nzbins=101, nsamples=25,\n",
                 "                   output='BRIGHT_SOMoclu_ensemble.hdf5', single_NZ='BRIGHT_fiducial_SOMoclu_NZ.hdf5',\n",
                 "                   uncovered_cell_file=\"BRIGHT_uncovered_cells.hdf5\",\n",
                 "                   n_clusters=1000,\n",
                 "                   objid_name='id',\n",
                 "                   cellid_output='BRIGHT_output_cellIDs.hdf5')\n",
-                "bright_summarizer = somocluSOMSummarizer.make_stage(name='bright_summarizer', **bright_dict)"
+                "bright_summarizer = SOMocluSummarizer.make_stage(name='bright_summarizer', **bright_dict)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "dd2675f1",
             "metadata": {},
@@ -886,15 +886,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.10.11"
         },
         "widgets": {
             "application/vnd.jupyter.widget-state+json": {
                 "state": {},
                 "version_major": 2,
                 "version_minor": 0
             }
```

### Comparing `pz-rail-0.99.1/examples/estimation_examples/test_sampled_summarizers.ipynb` & `pz-rail-0.99.1.1/examples/estimation_examples/test_sampled_summarizers.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973692316308244%*

 * *Differences: {"'cells'": "{3: {'source': ['from rail.estimation.algos.k_nearneigh import KNearNeighInformer, "*

 * *            "KNearNeighEstimator']}, 4: {'source': {insert: [(0, 'from "*

 * *            "rail.estimation.algos.var_inf import VarInfStackSummarizer\\n'), (1, 'from "*

 * *            "rail.estimation.algos.naive_stack import NaiveStackSummarizer\\n'), (2, 'from "*

 * *            "rail.estimation.algos.point_est_hist import PointEstHistSummarizer\\n'), (3, 'from "*

 * *            "rail.estimation.algos.nz_dir import NZDirInform […]*

```diff
@@ -37,28 +37,28 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "982ac396-9707-4cd2-bcf5-56c526c91691",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.estimation.algos.knnpz import Inform_KNearNeighPDF, KNearNeighPDF"
+                "from rail.estimation.algos.k_nearneigh import KNearNeighInformer, KNearNeighEstimator"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "b00c147b-5cef-4d78-932e-7ae7df6dbf24",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.estimation.algos.varInference import VarInferenceStack\n",
-                "from rail.estimation.algos.naiveStack import NaiveStack\n",
-                "from rail.estimation.algos.pointEstimateHist import PointEstimateHist\n",
-                "from rail.estimation.algos.NZDir import Inform_NZDir, NZDir\n",
+                "from rail.estimation.algos.var_inf import VarInfStackSummarizer\n",
+                "from rail.estimation.algos.naive_stack import NaiveStackSummarizer\n",
+                "from rail.estimation.algos.point_est_hist import PointEstHistSummarizer\n",
+                "from rail.estimation.algos.nz_dir import NZDirInformer, NZDirSummarizer\n",
                 "from rail.core.data import TableHandle, QPHandle\n",
                 "from rail.core.stage import RailStage"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -81,15 +81,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ddccd67d-7321-4e8b-b4c0-e5d7e6aacc52",
             "metadata": {},
             "source": [
-                "To create some N(z) distributions, we'll want some PDFs to work with first, for a quick demo let's just run some photo-z's using the KNearNeighPDF estimator using the 10,000 training galaxies to generate ~20,000 PDFs using data from healpix 9816 of cosmoDC2_v1.1.4 that are included in the RAIL repo:"
+                "To create some N(z) distributions, we'll want some PDFs to work with first, for a quick demo let's just run some photo-z's using the KNearNeighEstimator estimator using the 10,000 training galaxies to generate ~20,000 PDFs using data from healpix 9816 of cosmoDC2_v1.1.4 that are included in the RAIL repo:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ead0f0f0-a38a-42ec-b4f6-696127439140",
             "metadata": {},
@@ -103,15 +103,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "dc9ef13c-0ab5-4b5e-ae67-d138854be4c7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pz_train = Inform_KNearNeighPDF.make_stage(name='inform_KNN', model='demo_knn.pkl', **knn_dict)"
+                "pz_train = KNearNeighInformer.make_stage(name='inform_KNN', model='demo_knn.pkl', **knn_dict)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "0ecdeb24-b5d9-4985-8968-a87158a53757",
             "metadata": {},
@@ -139,27 +139,27 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a663b2c6-2163-4efb-ae32-413f0e40790b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pz = KNearNeighPDF.make_stage(name='KNN', hdf5_groupname='photometry',\n",
+                "pz = KNearNeighEstimator.make_stage(name='KNN', hdf5_groupname='photometry',\n",
                 "                              model=pz_train.get_handle('model'))\n",
                 "qp_data = pz.estimate(test_data)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "5c63e8af-fd52-4ada-8d20-3e0e7f47b0f7",
             "metadata": {},
             "source": [
-                "So, `qp_data` now contains the 20,000 PDFs from KNearNeighPDF, we can feed this in to three summarizers to generate an overall N(z) distribution.  We won't bother with any tomographic selections for this demo, just the overall N(z).  It is stored as `qp_data`, but has also been saved to disk as `output_KNN.fits` as an astropy table.  If you want to read in this data to grab the qp Ensemble at a later stage, you can do this via qp with a `ens = qp.read(\"output_KNN.fits\")`\n",
+                "So, `qp_data` now contains the 20,000 PDFs from KNearNeighEstimator, we can feed this in to three summarizers to generate an overall N(z) distribution.  We won't bother with any tomographic selections for this demo, just the overall N(z).  It is stored as `qp_data`, but has also been saved to disk as `output_KNN.fits` as an astropy table.  If you want to read in this data to grab the qp Ensemble at a later stage, you can do this via qp with a `ens = qp.read(\"output_KNN.fits\")`\n",
                 "\n",
-                "I coded up **quick and dirty** bootstrap versions of the `NaiveStack`, `PointEstimateHist`, and `VarInference` sumarizers.  These are not optimized, not parallel (issue created for future update), but they do produce N different bootstrap realizations of the overall N(z) which are returned as a qp Ensemble (Note: the previous versions of these degraders returned only the single overall N(z) rather than samples)."
+                "I coded up **quick and dirty** bootstrap versions of the `NaiveStackSummarizer`, `PointEstHistSummarizer`, and `VarInference` sumarizers.  These are not optimized, not parallel (issue created for future update), but they do produce N different bootstrap realizations of the overall N(z) which are returned as a qp Ensemble (Note: the previous versions of these degraders returned only the single overall N(z) rather than samples)."
             ]
         },
         {
             "cell_type": "markdown",
             "id": "3f351b58-29b0-4831-b5ac-6ab0969c4d3d",
             "metadata": {},
             "source": [
@@ -171,15 +171,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "62bc3867-d992-428f-abb5-8f019fb18ace",
             "metadata": {},
             "outputs": [],
             "source": [
-                "stacker = NaiveStack.make_stage(zmin=0.0, zmax=3.0, nzbins=41, nsamples=20, output=\"Naive_samples.hdf5\", single_NZ=\"NaiveStack_NZ.hdf5\")"
+                "stacker = NaiveStackSummarizer.make_stage(zmin=0.0, zmax=3.0, nzbins=41, nsamples=20, output=\"Naive_samples.hdf5\", single_NZ=\"NaiveStack_NZ.hdf5\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e73b373d-54be-4ea3-9e1c-1f6384d2caf7",
             "metadata": {},
@@ -242,26 +242,26 @@
         },
         {
             "cell_type": "markdown",
             "id": "540e66b7-28f0-483d-a627-00a88fec063c",
             "metadata": {},
             "source": [
                 "# Point Estimate Hist\n",
-                "PointEstimateHist takes the point estimate mode of each PDF and then histograms these, we'll again generate 41 bootstrap samples of this and plot a few of the resultant histograms.\n",
+                "PointEstHistSummarizer takes the point estimate mode of each PDF and then histograms these, we'll again generate 41 bootstrap samples of this and plot a few of the resultant histograms.\n",
                 "Note: For some reason the plotting on the histogram distribution in qp is a little wonky, it appears alpha is broken, so this plot is not the best:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6f3b1cd9-61d8-42ce-882b-db8ab17f4512",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pointy = PointEstimateHist.make_stage(zmin=0.0, zmax=3.0, nzbins=41, nsamples=20, single_NZ=\"point_NZ.hdf5\", output=\"point_samples.hdf5\")"
+                "pointy = PointEstHistSummarizer.make_stage(zmin=0.0, zmax=3.0, nzbins=41, nsamples=20, single_NZ=\"point_NZ.hdf5\", output=\"point_samples.hdf5\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "164752a4-e015-40b3-9261-396c58b005aa",
             "metadata": {},
@@ -305,27 +305,27 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a390c5cb-9899-4e56-a872-04d1927a0dc7",
             "metadata": {},
             "source": [
-                "# varInference\n",
+                "# VarInfStackSummarizer\n",
                 "\n",
-                "VarInference implements Markus' variational inference scheme and returns qp.interp gridded distribution. varInference tends to get a little wonky if you use too many bins, so we'll only use 25 bins. Again let's generate 20 samples and plot a few:"
+                "VarInfStackSummarizer implements Markus' variational inference scheme and returns qp.interp gridded distribution. VarInfStackSummarizer tends to get a little wonky if you use too many bins, so we'll only use 25 bins. Again let's generate 20 samples and plot a few:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e76d50d0-fc3f-4adb-a63c-f45dba5bb550",
             "metadata": {},
             "outputs": [],
             "source": [
-                "runner=VarInferenceStack.make_stage(name='test_varinf', zmin=0.0,zmax=3.0,nzbins=25, niter=10, nsamples=20,\n",
+                "runner=VarInfStackSummarizer.make_stage(name='test_varinf', zmin=0.0,zmax=3.0,nzbins=25, niter=10, nsamples=20,\n",
                 "                                    output=\"sampletest.hdf5\", single_NZ=\"varinf_NZ.hdf5\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "326e2d0d-b615-4984-b01a-0dc946e3aa64",
@@ -368,28 +368,28 @@
         },
         {
             "cell_type": "markdown",
             "id": "42416fa7-0cce-4fed-965f-616eb916a78e",
             "metadata": {},
             "source": [
                 "# NZDir\n",
-                "NZDir is a different type of summarizer, taking a weighted set of neighbors to a set of training spectroscopic objects to reconstruct the redshift distribution of the photometric sample.  I implemented a bootstrap of the **spectroscopic data** rather than the photometric data, both because it was much easier computationally, and I think that the spectroscopic variance is more important to take account of than simple bootstrap of the large photometric sample.\n",
-                "We must first run the `inform_NZDir` stage to train up the K nearest neigh tree used by NZDir, then we will run `NZDir` to actually construct the N(z) estimate.  \n",
+                "NZDirSummarizer is a different type of summarizer, taking a weighted set of neighbors to a set of training spectroscopic objects to reconstruct the redshift distribution of the photometric sample.  I implemented a bootstrap of the **spectroscopic data** rather than the photometric data, both because it was much easier computationally, and I think that the spectroscopic variance is more important to take account of than simple bootstrap of the large photometric sample.\n",
+                "We must first run the `inform_NZDir` stage to train up the K nearest neigh tree used by NZDirSummarizer, then we will run `NZDirSummarizer` to actually construct the N(z) estimate.  \n",
                 "\n",
-                "Like PointEstimateHist NZDir returns a qp.hist ensemble of samples"
+                "Like PointEstHistSummarizer NZDirSummarizer returns a qp.hist ensemble of samples"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "997b287c-07ba-48a4-9be9-d4e2ad5212ca",
             "metadata": {},
             "outputs": [],
             "source": [
-                "inf_nz = Inform_NZDir.make_stage(n_neigh=8, hdf5_groupname=\"photometry\", model=\"nzdir_model.pkl\")"
+                "inf_nz = NZDirInformer.make_stage(n_neigh=8, hdf5_groupname=\"photometry\", model=\"nzdir_model.pkl\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d23200cf-041c-4ab2-af06-d0b942442cad",
             "metadata": {},
@@ -401,15 +401,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "fd515f9f-4efa-416a-b6d0-96d088c9150b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "nzd = NZDir.make_stage(leafsize=20, zmin=0.0, zmax=3.0, nzbins=31, model=\"NZDir_model.pkl\", hdf5_groupname='photometry',\n",
+                "nzd = NZDirSummarizer.make_stage(leafsize=20, zmin=0.0, zmax=3.0, nzbins=31, model=\"NZDir_model.pkl\", hdf5_groupname='photometry',\n",
                 "                       output='NZDir_samples.hdf5', single_NZ='NZDir_NZ.hdf5')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f149c641-7644-4b72-a266-f674b9488a83",
@@ -455,15 +455,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a870aa08-7de2-49c1-bd9a-cfda3eb17631",
             "metadata": {},
             "source": [
-                "As we also wrote out the single estimate of N(z) we can read that data from the second file written (specified by the `single_NZ` argument given in NZDir.make_stage above, in this case \"NZDir_NZ.hdf5\")"
+                "As we also wrote out the single estimate of N(z) we can read that data from the second file written (specified by the `single_NZ` argument given in NZDirSummarizer.make_stage above, in this case \"NZDir_NZ.hdf5\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7d5a8570-ba5d-4a2e-828a-3d640e9133b9",
             "metadata": {},
@@ -485,15 +485,15 @@
         {
             "cell_type": "markdown",
             "id": "bfa7ee13-1f2e-4549-8bca-a5e3e78b61cd",
             "metadata": {},
             "source": [
                 "# Results\n",
                 "\n",
-                "All three results files are qp distributions, NaiveStack and varInference return qp.interp distributions while pointEstimateHist returns a qp.histogram distribution.  Even with the different distributions you can use qp functionality to do things like determine the means, modes, etc... of the distributions.  You could then use the std dev of any of these to estimate a 1 sigma \"shift\", etc..."
+                "All three results files are qp distributions, NaiveStackSummarizer and VarInfStackSummarizer return qp.interp distributions while PointEstHistSummarizer returns a qp.histogram distribution.  Even with the different distributions you can use qp functionality to do things like determine the means, modes, etc... of the distributions.  You could then use the std dev of any of these to estimate a 1 sigma \"shift\", etc..."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "cd55a38f-fc53-48b5-b829-4a1db5020f87",
             "metadata": {},
```

### Comparing `pz-rail-0.99.1/examples/evaluation_examples/demo.ipynb` & `pz-rail-0.99.1.1/examples/evaluation_examples/demo.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991035353535354%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'last run successfully: June 16, 2023 (with qp-prob >= "*

 * *            '0.8.2)\\n\')], delete: [4]}}, 4: {\'source\': {insert: [(4, "To compute the photo-z '*

 * *            'metrics of a given test sample, it is necessary to read the output of a photo-z code '*

 * *            "containing galaxies' photo-z PDFs. Let's use the toy data available in `tests/data/` "*

 * *            '(**test_dc2_training_9816.hdf5** and **test_dc2_validation_9816.hdf5**) to generate a '*

 * *            " […]*

```diff
@@ -4,15 +4,15 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Demo: RAIL Evaluation \n",
                 "\n",
                 "Author: Sam Schmidt, Alex Malz, Julia Gschwend, others...\n",
                 "\n",
-                "last run successfully: April 28, 2023 (with qp-prob >= 0.8.2)\n",
+                "last run successfully: June 16, 2023 (with qp-prob >= 0.8.2)\n",
                 "\n",
                 "The purpose of this notebook is to demonstrate the application of the metrics scripts to be used on the photo-z PDF catalogs produced by the PZ working group. The first implementation of the _evaluation_ module is based on the refactoring of the code used in [Schmidt et al. 2020](https://arxiv.org/pdf/2001.03621.pdf), available on Github repository [PZDC1paper](https://github.com/LSSTDESC/PZDC1paper). \n",
                 "\n",
                 "To run this notebook, you must install qp and have the notebook in the same directory as `utils.py` (available in RAIL's examples directrory). You must also have installed all RAIL dependencies, particularly for the estimation codes that you want to run, as well as ceci, qp, tables_io, etc...  See the RAIL installation instructions for more info.\n",
                 "\n",
                 "### Contents\n",
                 "\n",
@@ -69,28 +69,28 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "<a class=\"anchor\" id=\"data\"></a>\n",
                 "# Data  \n",
                 "\n",
                 "\n",
-                "To compute the photo-z metrics of a given test sample, it is necessary to read the output of a photo-z code containing galaxies' photo-z PDFs. Let's use the toy data available in `tests/data/` (**test_dc2_training_9816.hdf5** and **test_dc2_validation_9816.hdf5**) to generate a small sample of photo-z PDFs using the **FZBoost** algorithm available on RAIL's _estimation_ module."
+                "To compute the photo-z metrics of a given test sample, it is necessary to read the output of a photo-z code containing galaxies' photo-z PDFs. Let's use the toy data available in `tests/data/` (**test_dc2_training_9816.hdf5** and **test_dc2_validation_9816.hdf5**) to generate a small sample of photo-z PDFs using the **FlexZBoost** algorithm available on RAIL's _estimation_ module."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "<a class=\"anchor\" id=\"fzboost\"></a>\n",
                 "### Photo-z Results\n",
-                "#### Run FZBoost\n",
+                "#### Run FlexZBoost\n",
                 "\n",
-                "If you have run the notebook `RAIL_estimation_demo.ipynb`, this will produce a file `output_fzboost.fits`, \n",
+                "If you have run the notebook `RAIL_estimation_demo.ipynb`, this will produce a file `output_fzboost.hdf5`, \n",
                 "writen at the location:<br> \n",
-                "`<your_path>/RAIL/examples/estimation_examples/output_fzboost.fits`. \n",
+                "`<your_path>/RAIL/examples/estimation_examples/output_fzboost.hdf5`. \n",
                 "\n",
                 "Otherwise we can download the file from NERSC\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -116,15 +116,15 @@
             "outputs": [],
             "source": [
                 "if not os.path.exists(pdfs_file):\n",
                 "    try:\n",
                 "        os.makedirs(os.path.dirname(pdfs_file))\n",
                 "    except FileExistsError:\n",
                 "        pass\n",
-                "    curl_com = f\"curl -o {pdfs_file} https://portal.nersc.gov/cfs/lsst/schmidt9/output_fzboost.hdf5\"\n",
+                "    curl_com = f\"curl -o {pdfs_file} https://portal.nersc.gov/cfs/lsst/PZ/output_fzboost.hdf5\"\n",
                 "    os.system(curl_com)\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -178,15 +178,15 @@
                 "# Make an evaulator stage"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Now let's set up the Evaluator stage to compute our metrics for the FZBoost data"
+                "Now let's set up the Evaluator stage to compute our metrics for the FlexZBoost results"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -355,15 +355,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "pdfs = fzdata.data.objdata()['yvals']\n",
-                "plot_pit_qq(pdfs, zgrid, ztrue, title=\"PIT-QQ - toy data\", code=\"FZBoost\",\n",
+                "plot_pit_qq(pdfs, zgrid, ztrue, title=\"PIT-QQ - toy data\", code=\"FlexZBoost\",\n",
                 "                pit_out_rate=pit_out_rate, savefig=False)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `pz-rail-0.99.1/examples/evaluation_examples/utils.py` & `pz-rail-0.99.1.1/examples/evaluation_examples/utils.py`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/examples/goldenspike_examples/cleanup.sh` & `pz-rail-0.99.1.1/examples/goldenspike_examples/cleanup.sh`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/examples/goldenspike_examples/goldenspike.ipynb` & `pz-rail-0.99.1.1/examples/goldenspike_examples/goldenspike.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971328606254632%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(10, 'from rail.estimation.algos.bpz_lite import "*

 * *            "BPZliteInformer, BPZliteEstimator\\n'), (11, 'from rail.estimation.algos.k_nearneigh "*

 * *            "import KNearNeighInformer, KNearNeighEstimator\\n'), (12, 'from "*

 * *            "rail.estimation.algos.flexzboost import FlexZBoostInformer, FlexZBoostEstimator\\n'), "*

 * *            "(14, 'from rail.estimation.algos.naive_stack import NaiveStackSummarizer\\n'), (15, "*

 * *            "'from rail.estimation.algos.poi […]*

```diff
@@ -69,20 +69,20 @@
                 "from rail.creation.degradation.spectroscopic_degraders import InvRedshiftIncompleteness, LineConfusion\n",
                 "from rail.creation.degradation.quantityCut import QuantityCut\n",
                 "from rail.creation.engines.flowEngine import FlowModeler, FlowCreator, FlowPosterior\n",
                 "from rail.core.data import TableHandle\n",
                 "from rail.core.stage import RailStage\n",
                 "from rail.core.utilStages import ColumnMapper, TableConverter\n",
                 "\n",
-                "from rail.estimation.algos.bpz_lite import Inform_BPZ_lite, BPZ_lite\n",
-                "from rail.estimation.algos.knnpz import Inform_KNearNeighPDF, KNearNeighPDF\n",
-                "from rail.estimation.algos.flexzboost import Inform_FZBoost, FZBoost\n",
+                "from rail.estimation.algos.bpz_lite import BPZliteInformer, BPZliteEstimator\n",
+                "from rail.estimation.algos.k_nearneigh import KNearNeighInformer, KNearNeighEstimator\n",
+                "from rail.estimation.algos.flexzboost import FlexZBoostInformer, FlexZBoostEstimator\n",
                 "\n",
-                "from rail.estimation.algos.naiveStack import NaiveStack\n",
-                "from rail.estimation.algos.pointEstimateHist import PointEstimateHist\n",
+                "from rail.estimation.algos.naive_stack import NaiveStackSummarizer\n",
+                "from rail.estimation.algos.point_est_hist import PointEstHistSummarizer\n",
                 "\n",
                 "from rail.evaluation.evaluator import Evaluator\n",
                 "\n"
             ]
         },
         {
             "cell_type": "markdown",
@@ -429,28 +429,28 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "accredited-circle",
             "metadata": {},
             "outputs": [],
             "source": [
-                "inform_bpz = Inform_BPZ_lite.make_stage(\n",
+                "inform_bpz = BPZliteInformer.make_stage(\n",
                 "    name=\"inform_bpz\",\n",
                 "    model=\"bpz.pkl\",\n",
                 "    hdf5_groupname=\"\",\n",
                 ")\n",
                 "\n",
-                "inform_knn = Inform_KNearNeighPDF.make_stage(\n",
+                "inform_knn = KNearNeighInformer.make_stage(\n",
                 "    name='inform_knn', \n",
                 "    nondetect_val=np.nan,\n",
                 "    model='knnpz.pkl', \n",
                 "    hdf5_groupname='',\n",
                 ")\n",
                 "\n",
-                "inform_fzboost = Inform_FZBoost.make_stage(\n",
+                "inform_fzboost = FlexZBoostInformer.make_stage(\n",
                 "    name='inform_FZBoost', \n",
                 "    model='fzboost.pkl', \n",
                 "    hdf5_groupname='',\n",
                 ")"
             ]
         },
         {
@@ -463,67 +463,47 @@
                 "inform_bpz.inform(train_data)\n",
                 "inform_knn.inform(train_data)\n",
                 "inform_fzboost.inform(train_data)"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "29d6f99e",
-            "metadata": {},
-            "source": [
-                "\n",
-                "**If you run into issues here:** \n",
-                "\n",
-                "If you've installed rail and bpz to different directories (most commonly, you've installed rail from \n",
-                "source and bpz from PyPI), you may run into an issue where rail cannot locate a file installed by bpz.\n",
-                "\n",
-                "To fix this, find your test_bpz.columns file in your bpz directory ([or grab a new one here on \n",
-                "GitHub](https://github.com/LSSTDESC/rail_bpz/blob/main/src/rail/examples/estimation/configs/test_bpz.columns>)) \n",
-                "and copy it into your rail directory to `/RAIL/src/rail/examples/estimation_examples/configs/test_bpz.columns`. \n",
-                "\n",
-                "Alternatively, if you don't want to move files, you should be able rewrite code to replace the configured paths with \n",
-                "your actual `test_bpz.columns` path (inform stage: [bpz_lite.py L89](https://github.com/LSSTDESC/rail_bpz/blob/65870ffd93ba35356a1af44104a0a78530085789/src/rail/estimation/algos/bpz_lite.py#L89) and estimation: [bpz_lite.py L259](https://github.com/LSSTDESC/rail_bpz/blob/65870ffd93ba35356a1af44104a0a78530085789/src/rail/estimation/algos/bpz_lite.py#L259>)).\n",
-                "\n"
-            ]
-        },
-        {
-            "cell_type": "markdown",
             "id": "colonial-trailer",
             "metadata": {},
             "source": [
                 "## Estimate photo-z posteriors\n",
                 "\n",
                 "More details about the estimators is available in the `rail/examples/estimation_examples/RAIL_estimation_demo.ipynb` notebook.\n",
                 "\n",
-                "`randomPZ` is a very simple class that does not actually predict a meaningful photo-z, instead it produces a randomly drawn Gaussian for each galaxy.<br>\n",
-                "`trainZ` is our \"pathological\" estimator, it makes a PDF from a histogram of the training data and assigns that PDF to every galaxy.<br>\n",
-                "`BPZ_lite` is a template-based code that outputs the posterior estimated given a specific template set and Bayesian prior. See Benitez (2000) for more details.<br>\n"
+                "`RandomGaussEstimator` is a very simple class that does not actually predict a meaningful photo-z, instead it produces a randomly drawn Gaussian for each galaxy.<br>\n",
+                "`trainZEstimator` is our \"pathological\" estimator, it makes a PDF from a histogram of the training data and assigns that PDF to every galaxy.<br>\n",
+                "`BPZliteEstimator` is a template-based code that outputs the posterior estimated given a specific template set and Bayesian prior. See Benitez (2000) for more details.<br>\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "electric-minute",
             "metadata": {},
             "outputs": [],
             "source": [
-                "estimate_bpz = BPZ_lite.make_stage(\n",
+                "estimate_bpz = BPZliteEstimator.make_stage(\n",
                 "    name='estimate_bpz', \n",
                 "    hdf5_groupname='', \n",
                 "    model=inform_bpz.get_handle('model'),\n",
                 ")\n",
                 "\n",
-                "estimate_knn = KNearNeighPDF.make_stage(\n",
+                "estimate_knn = KNearNeighEstimator.make_stage(\n",
                 "    name='estimate_knn', \n",
                 "    hdf5_groupname='', \n",
                 "    nondetect_val=np.nan, \n",
                 "    model=inform_knn.get_handle('model'),\n",
                 ")\n",
                 "\n",
-                "estimate_fzboost = FZBoost.make_stage(\n",
+                "estimate_fzboost = FlexZBoostEstimator.make_stage(\n",
                 "    name='test_FZBoost', \n",
                 "    nondetect_val=np.nan,\n",
                 "    model=inform_fzboost.get_handle('model'), \n",
                 "    hdf5_groupname='',\n",
                 "    aliases=dict(input='test_data', output='fzboost_estim'),\n",
                 ")"
             ]
@@ -633,16 +613,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "white-replacement",
             "metadata": {},
             "outputs": [],
             "source": [
-                "point_estimate_test = PointEstimateHist.make_stage(name='point_estimate_test')\n",
-                "naive_stack_test = NaiveStack.make_stage(name='naive_stack_test')"
+                "point_estimate_test = PointEstHistSummarizer.make_stage(name='point_estimate_test')\n",
+                "naive_stack_test = NaiveStackSummarizer.make_stage(name='naive_stack_test')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "korean-guess",
             "metadata": {},
```

### Comparing `pz-rail-0.99.1/pyproject.toml` & `pz-rail-0.99.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-0.99.1/src/pz_rail.egg-info/SOURCES.txt` & `pz-rail-0.99.1.1/src/pz_rail.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,20 @@
 docs/demos.rst
 docs/index.rst
 docs/nbconvert-requirements.txt
 docs/requirements.txt
 docs/_static/css/notebooks.css
 docs/source/citing.rst
 docs/source/contributing.rst
-docs/source/futureplans.rst
-docs/source/immediateplans.rst
+docs/source/fix_an_issue.rst
 docs/source/installation.rst
+docs/source/new_algorithm.rst
+docs/source/new_rail_stage.rst
 docs/source/overview.rst
+docs/source/sharing_pipeline.rst
 examples/.gitignore
 examples/core_examples/FileIO_DataStore.ipynb
 examples/core_examples/FluxtoMag_and_Deredden_example.ipynb
 examples/core_examples/Pipe_Example.ipynb
 examples/core_examples/README.md
 examples/core_examples/Run_Pipe.ipynb
 examples/core_examples/cleanup.sh
@@ -65,14 +67,16 @@
 examples/evaluation_examples/cleanup.sh
 examples/evaluation_examples/demo.ipynb
 examples/evaluation_examples/utils.py
 examples/goldenspike_examples/README.md
 examples/goldenspike_examples/cleanup.sh
 examples/goldenspike_examples/cleanup_pipeline.sh
 examples/goldenspike_examples/goldenspike.ipynb
+examples/goldenspike_examples/goldenspike.yml
+examples/goldenspike_examples/goldenspike_config.yml
 src/pz_rail.egg-info/PKG-INFO
 src/pz_rail.egg-info/SOURCES.txt
 src/pz_rail.egg-info/dependency_links.txt
 src/pz_rail.egg-info/requires.txt
 src/pz_rail.egg-info/top_level.txt
 src/rail/hub/__init__.py
 src/rail/hub/_version.py
```

