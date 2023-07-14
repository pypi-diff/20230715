# Comparing `tmp/pz-rail-base-0.0.4.tar.gz` & `tmp/pz-rail-base-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-base-0.0.4.tar", last modified: Fri Jun 16 04:47:15 2023, max compression
+gzip compressed data, was "pz-rail-base-0.0.5.tar", last modified: Fri Jul 14 23:10:18 2023, max compression
```

## Comparing `pz-rail-base-0.0.4.tar` & `pz-rail-base-0.0.5.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.854332 pz-rail-base-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.822332 pz-rail-base-0.0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-16 04:47:15.854332 pz-rail-base-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/rail_packages.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 04:47:15.854332 pz-rail-base-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.818332 pz-rail-base-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/pz_rail_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-16 04:47:15.000000 pz-rail-base-0.0.4/src/pz_rail_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-06-16 04:47:15.000000 pz-rail-base-0.0.4/src/pz_rail_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 04:47:15.000000 pz-rail-base-0.0.4/src/pz_rail_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 04:47:15.000000 pz-rail-base-0.0.4/src/pz_rail_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-16 04:47:15.000000 pz-rail-base-0.0.4/src/pz_rail_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 04:47:15.000000 pz-rail-base-0.0.4/src/pz_rail_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.822332 pz-rail-base-0.0.4/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/cli/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/core/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 04:47:15.000000 pz-rail-base-0.0.4/src/rail/core/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/core/algo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/core/common_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/core/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/core/introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)    14109 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/core/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/core/utilStages.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/creation/degradation/
--rw-r--r--   0 runner    (1001) docker     (123)    30116 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/creation/degradation/lsst_error_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/creation/degradation/quantityCut.py
--rw-r--r--   0 runner    (1001) docker     (123)    22286 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/creation/degradation/spectroscopic_selections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/creation/degrader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/creation/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/estimation/algos/naiveStack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/estimation/algos/pointEstimateHist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/estimation/algos/randomPZ.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/estimation/algos/trainZ.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/estimation/algos/varInference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/estimation/estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/estimation/summarizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/evaluation/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/evaluation/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/evaluation/metrics/cdeloss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/evaluation/metrics/pointestimates.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/evaluation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/examples_data/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.818332 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/configs/flowModeler.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.826332 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.838332 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_I_success.txt
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt
--rw-r--r--   0 runner    (1001) docker     (123)  1000000 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt
--rw-r--r--   0 runner    (1001) docker     (123)   431705 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.822332 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.838332 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.838332 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/AB/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/AB/dummy.txt
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.838332 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/
--rw-r--r--   0 runner    (1001) docker     (123)    98003 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
--rw-r--r--   0 runner    (1001) docker     (123)    95326 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
--rw-r--r--   0 runner    (1001) docker     (123)    96635 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
--rw-r--r--   0 runner    (1001) docker     (123)    90216 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
--rw-r--r--   0 runner    (1001) docker     (123)   100126 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
--rw-r--r--   0 runner    (1001) docker     (123)    93013 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.838332 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/
--rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
--rwxr-xr-x   0 runner    (1001) docker     (123)    43750 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)    42830 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)    72228 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)    68560 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)    43351 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)    42789 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)   179585 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
--rwxr-xr-x   0 runner    (1001) docker     (123)   179584 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.842332 pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.842332 pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.842332 pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1158108 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl
--rw-r--r--   0 runner    (1001) docker     (123)   873947 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/goldenspike.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.854332 pz-rail-base-0.0.4/src/rail/examples_data/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    91936 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/lsst_filters.npy
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/make_rail_sample_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/output_BPZ_lite.fits
--rw-r--r--   0 runner    (1001) docker     (123)    24574 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq
--rw-r--r--   0 runner    (1001) docker     (123)   662976 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)   873930 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_training_9816.pq
--rw-r--r--   0 runner    (1001) docker     (123)  1192254 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
--rw-r--r--   0 runner    (1001) docker     (123)  1316984 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/training_100gal.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/examples_data/testdata/validation_10gal.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.854332 pz-rail-base-0.0.4/src/rail/stages/
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/src/rail/stages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.822332 pz-rail-base-0.0.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.854332 pz-rail-base-0.0.4/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/tests/cli/test_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.854332 pz-rail-base-0.0.4/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/tests/core/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/tests/core/test_degraders.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/tests/core/test_introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/tests/core/test_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.854332 pz-rail-base-0.0.4/tests/estimation/
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/tests/estimation/test_algos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/tests/estimation/test_summarizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 04:47:15.854332 pz-rail-base-0.0.4/tests/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-16 04:46:59.000000 pz-rail-base-0.0.4/tests/evaluation/test_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.166426 pz-rail-base-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.130423 pz-rail-base-0.0.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.130423 pz-rail-base-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-14 23:10:18.166426 pz-rail-base-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/rail_packages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 23:10:18.166426 pz-rail-base-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.114422 pz-rail-base-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.134424 pz-rail-base-0.0.5/src/pz_rail_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-14 23:10:18.000000 pz-rail-base-0.0.5/src/pz_rail_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-07-14 23:10:18.000000 pz-rail-base-0.0.5/src/pz_rail_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:10:18.000000 pz-rail-base-0.0.5/src/pz_rail_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 23:10:18.000000 pz-rail-base-0.0.5/src/pz_rail_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-14 23:10:18.000000 pz-rail-base-0.0.5/src/pz_rail_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 23:10:18.000000 pz-rail-base-0.0.5/src/pz_rail_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.122423 pz-rail-base-0.0.5/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.134424 pz-rail-base-0.0.5/src/rail/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/cli/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.138424 pz-rail-base-0.0.5/src/rail/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 23:10:17.000000 pz-rail-base-0.0.5/src/rail/core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/core/algo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/core/common_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16251 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/core/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14109 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/core/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/core/utilStages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.138424 pz-rail-base-0.0.5/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.138424 pz-rail-base-0.0.5/src/rail/creation/degradation/
+-rw-r--r--   0 runner    (1001) docker     (123)    30116 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/creation/degradation/lsst_error_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/creation/degradation/quantityCut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22286 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/creation/degradation/spectroscopic_selections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/creation/degrader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/creation/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.142424 pz-rail-base-0.0.5/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.142424 pz-rail-base-0.0.5/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/estimation/algos/naive_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/estimation/algos/point_est_hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/estimation/algos/random_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/estimation/algos/train_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/estimation/algos/var_inf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/estimation/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/estimation/summarizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.142424 pz-rail-base-0.0.5/src/rail/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/evaluation/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.142424 pz-rail-base-0.0.5/src/rail/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/evaluation/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/evaluation/metrics/cdeloss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/evaluation/metrics/pointestimates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/evaluation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.142424 pz-rail-base-0.0.5/src/rail/examples_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.118423 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.142424 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/configs/flowModeler.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.146425 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.146425 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_I_success.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1000000 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   431705 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.122423 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.150425 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.150425 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/AB/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/AB/dummy.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.150425 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/
+-rw-r--r--   0 runner    (1001) docker     (123)    98003 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
+-rw-r--r--   0 runner    (1001) docker     (123)    95326 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
+-rw-r--r--   0 runner    (1001) docker     (123)    96635 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
+-rw-r--r--   0 runner    (1001) docker     (123)    90216 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
+-rw-r--r--   0 runner    (1001) docker     (123)   100126 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
+-rw-r--r--   0 runner    (1001) docker     (123)    93013 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.154425 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      125 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43750 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42830 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)    72228 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)    68560 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43351 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42789 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)   179585 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
+-rwxr-xr-x   0 runner    (1001) docker     (123)   179584 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.154425 pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.154425 pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.154425 pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1158108 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   873947 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/goldenspike.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.166426 pz-rail-base-0.0.5/src/rail/examples_data/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    91936 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/lsst_filters.npy
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/make_rail_sample_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    43200 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/output_BPZ_lite.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    24574 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq
+-rw-r--r--   0 runner    (1001) docker     (123)   662976 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)   873930 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_training_9816.pq
+-rw-r--r--   0 runner    (1001) docker     (123)  1192254 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
+-rw-r--r--   0 runner    (1001) docker     (123)  1316984 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/training_100gal.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/examples_data/testdata/validation_10gal.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.166426 pz-rail-base-0.0.5/src/rail/stages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/src/rail/stages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.126423 pz-rail-base-0.0.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.166426 pz-rail-base-0.0.5/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/tests/cli/test_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.166426 pz-rail-base-0.0.5/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/tests/core/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/tests/core/test_degraders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/tests/core/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/tests/core/test_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.166426 pz-rail-base-0.0.5/tests/estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/tests/estimation/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/tests/estimation/test_summarizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:10:18.166426 pz-rail-base-0.0.5/tests/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-14 23:10:03.000000 pz-rail-base-0.0.5/tests/evaluation/test_evaluation.py
```

### Comparing `pz-rail-base-0.0.4/.github/pull_request_template.md` & `pz-rail-base-0.0.5/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/.github/workflows/linting.yml` & `pz-rail-base-0.0.5/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/.github/workflows/publish-to-pypi.yml` & `pz-rail-base-0.0.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/.github/workflows/smoke-test.yml` & `pz-rail-base-0.0.5/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/.github/workflows/testing-and-coverage.yml` & `pz-rail-base-0.0.5/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/.gitignore` & `pz-rail-base-0.0.5/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -134,7 +134,10 @@
 .vscode/
 
 # dask
 dask-worker-space/
 
 # tmp directory
 tmp/
+
+# macOS
+.DS_Store
```

### Comparing `pz-rail-base-0.0.4/.pre-commit-config.yaml` & `pz-rail-base-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/LICENSE` & `pz-rail-base-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/pyproject.toml` & `pz-rail-base-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/pz_rail_base.egg-info/SOURCES.txt` & `pz-rail-base-0.0.5/src/pz_rail_base.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,19 +34,19 @@
 src/rail/creation/degrader.py
 src/rail/creation/engine.py
 src/rail/creation/degradation/lsst_error_model.py
 src/rail/creation/degradation/quantityCut.py
 src/rail/creation/degradation/spectroscopic_selections.py
 src/rail/estimation/estimator.py
 src/rail/estimation/summarizer.py
-src/rail/estimation/algos/naiveStack.py
-src/rail/estimation/algos/pointEstimateHist.py
-src/rail/estimation/algos/randomPZ.py
-src/rail/estimation/algos/trainZ.py
-src/rail/estimation/algos/varInference.py
+src/rail/estimation/algos/naive_stack.py
+src/rail/estimation/algos/point_est_hist.py
+src/rail/estimation/algos/random_gauss.py
+src/rail/estimation/algos/train_z.py
+src/rail/estimation/algos/var_inf.py
 src/rail/evaluation/evaluator.py
 src/rail/evaluation/utils.py
 src/rail/evaluation/metrics/base.py
 src/rail/evaluation/metrics/cdeloss.py
 src/rail/evaluation/metrics/pointestimates.py
 src/rail/examples_data/.gitignore
 src/rail/examples_data/creation_data/configs/flowModeler.yaml
```

### Comparing `pz-rail-base-0.0.4/src/rail/cli/commands.py` & `pz-rail-base-0.0.5/src/rail/cli/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,7 +50,15 @@
 @options.print_modules()
 @options.print_tree()
 @options.print_stages()
 def info(**kwargs):
     """Print information about the rail ecosystem"""
     scripts.info(**kwargs)
     return 0
+
+
+@cli.command()
+@options.verbose_download()
+def get_data(verbose, **kwargs):
+    """Downloads data from NERSC (if not already found)"""
+    scripts.get_data(verbose, **kwargs)
+    return 0
```

### Comparing `pz-rail-base-0.0.4/src/rail/cli/options.py` & `pz-rail-base-0.0.5/src/rail/cli/options.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "print_packages",
     "print_namespaces",
     "print_modules",
     "print_tree",
     "print_stages",
     "package_file",
     "inputs",
+    "verbose_download"
 ]
 
 
 class GitMode(enum.Enum):
     """Choose git clone mode"""
     ssh = 0
     https = 1
@@ -127,23 +128,25 @@
 
 print_stages = PartialOption(
     "--print-stages",
     help="Print RAIL stages",
     is_flag=True,
 )
 
-
-
-
-
 package_file = PartialOption(
     "--package-file",
     type=click.Path(),
     default=None,
     help="File with package",
 )
 
 inputs = PartialArgument(
     "inputs",
     nargs=-1
 )
 
+verbose_download = PartialOption(
+    "-v",
+    "--verbose",
+    help="Verbose output when downloading",
+    is_flag=True
+)
```

### Comparing `pz-rail-base-0.0.4/src/rail/cli/scripts.py` & `pz-rail-base-0.0.5/src/rail/cli/scripts.py`

 * *Files 9% similar despite different names*

```diff
@@ -116,9 +116,21 @@
         print("\n\n")
     if kwargs.get('print_stages') or print_all:
         print("======= Printing RAIL stages ==============")
         RailEnv.print_rail_stage_dict()
         print("\n\n")
     
 
+def get_data(verbose, **kwargs):  # pragma: no cover
 
-    
+    data_files = [
+        {
+            "local_path": "src/rail/examples_data/goldenspike_data/data/base_catalog.pq",
+            "remote_path": "https://portal.nersc.gov/cfs/lsst/PZ/base_catalog.pq"
+        }
+    ]
+
+    for data_file in data_files:
+        if verbose:
+            print(f'Check file: {data_file["local_path"]}')
+        if not os.path.exists(data_file["local_path"]):
+            os.system(f'curl -o {data_file["local_path"]} {data_file["remote_path"]} --create-dirs')
```

### Comparing `pz-rail-base-0.0.4/src/rail/core/__init__.py` & `pz-rail-base-0.0.5/src/rail/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/core/algo_utils.py` & `pz-rail-base-0.0.5/src/rail/core/algo_utils.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/core/common_params.py` & `pz-rail-base-0.0.5/src/rail/core/common_params.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/core/data.py` & `pz-rail-base-0.0.5/src/rail/core/data.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/core/introspection.py` & `pz-rail-base-0.0.5/src/rail/core/introspection.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/core/stage.py` & `pz-rail-base-0.0.5/src/rail/core/stage.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/core/utilStages.py` & `pz-rail-base-0.0.5/src/rail/core/utilStages.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/core/utils.py` & `pz-rail-base-0.0.5/src/rail/core/utils.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/creation/degradation/lsst_error_model.py` & `pz-rail-base-0.0.5/src/rail/creation/degradation/lsst_error_model.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/creation/degradation/quantityCut.py` & `pz-rail-base-0.0.5/src/rail/creation/degradation/quantityCut.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/creation/degradation/spectroscopic_selections.py` & `pz-rail-base-0.0.5/src/rail/creation/degradation/spectroscopic_selections.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/creation/degrader.py` & `pz-rail-base-0.0.5/src/rail/creation/degrader.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/creation/engine.py` & `pz-rail-base-0.0.5/src/rail/creation/engine.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/estimation/algos/naiveStack.py` & `pz-rail-base-0.0.5/src/rail/estimation/algos/naive_stack.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 import numpy as np
 from ceci.config import StageParameter as Param
 from rail.estimation.summarizer import PZSummarizer
 from rail.core.data import QPHandle
 import qp
 
 
-class NaiveStack(PZSummarizer):
+class NaiveStackSummarizer(PZSummarizer):
     """Summarizer which simply histograms a point estimate
     """
 
-    name = 'NaiveStack'
+    name = 'NaiveStackSummarizer'
     config_options = PZSummarizer.config_options.copy()
     config_options.update(zmin=Param(float, 0.0, msg="The minimum redshift of the z grid"),
                           zmax=Param(float, 3.0, msg="The maximum redshift of the z grid"),
                           nzbins=Param(int, 301, msg="The number of gridpoints in the z grid"),
                           seed=Param(int, 87, msg="random seed"),
                           nsamples=Param(int, 1000, msg="Number of sample distributions to create"))
     outputs = [('output', QPHandle),
```

### Comparing `pz-rail-base-0.0.4/src/rail/estimation/algos/pointEstimateHist.py` & `pz-rail-base-0.0.5/src/rail/estimation/algos/point_est_hist.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 import numpy as np
 from ceci.config import StageParameter as Param
 from rail.estimation.summarizer import PZSummarizer
 from rail.core.data import QPHandle
 import qp
 
 
-class PointEstimateHist(PZSummarizer):
+class PointEstHistSummarizer(PZSummarizer):
     """Summarizer which simply histograms a point estimate
     """
 
-    name = 'PointEstimateHist'
+    name = 'PointEstHistSummarizer'
     config_options = PZSummarizer.config_options.copy()
     config_options.update(zmin=Param(float, 0.0, msg="The minimum redshift of the z grid"),
                           zmax=Param(float, 3.0, msg="The maximum redshift of the z grid"),
                           nzbins=Param(int, 301, msg="The number of gridpoints in the z grid"),
                           seed=Param(int, 87, msg="random seed"),
                           point_estimate=Param(str, 'zmode', msg="Which point estimate to use"),
                           nsamples=Param(int, 1000, msg="Number of sample distributions to return"))
```

### Comparing `pz-rail-base-0.0.4/src/rail/estimation/algos/randomPZ.py` & `pz-rail-base-0.0.5/src/rail/estimation/algos/random_gauss.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from scipy.stats import norm
 from ceci.config import StageParameter as Param
 from rail.estimation.estimator import CatEstimator
 from rail.core.data import TableHandle
 import qp
 
 
-class RandomPZ(CatEstimator):
+class RandomGaussEstimator(CatEstimator):
     """Random CatEstimator
     """
 
-    name = 'RandomPZ'
+    name = 'RandomGaussEstimator'
     inputs = [('input', TableHandle)]
     config_options = CatEstimator.config_options.copy()
     config_options.update(rand_width=Param(float, 0.025, "ad hock width of PDF"),
                           rand_zmin=Param(float, 0.0, msg="The minimum redshift of the z grid"),
                           rand_zmax=Param(float, 3.0, msg="The maximum redshift of the z grid"),
                           nzbins=Param(int, 301, msg="The number of gridpoints in the z grid"),
                           seed=Param(int, 87, msg="random seed"),
```

### Comparing `pz-rail-base-0.0.4/src/rail/estimation/algos/trainZ.py` & `pz-rail-base-0.0.5/src/rail/estimation/algos/train_z.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
     """
     def __init__(self, zgrid, pdf, zmode):
         self.zgrid = zgrid
         self.pdf = pdf
         self.zmode = zmode
 
 
-class Inform_trainZ(CatInformer):
+class TrainZInformer(CatInformer):
     """Train an Estimator which returns a global PDF for all galaxies
     """
 
-    name = 'Inform_trainZ'
+    name = 'TrainZInformer'
     config_options = CatInformer.config_options.copy()
     config_options.update(zmin=SHARED_PARAMS,
                           zmax=SHARED_PARAMS,
                           nzbins=SHARED_PARAMS,
                           redshift_col=SHARED_PARAMS)
 
     def __init__(self, args, comm=None):
@@ -52,19 +52,19 @@
         norm = cdf[-1] * (zbins[2] - zbins[1])
         train_pdf = train_pdf / norm
         zgrid = midpoints
         self.model = trainZmodel(zgrid, train_pdf, zmode)
         self.add_data('model', self.model)
 
 
-class TrainZ(CatEstimator):
+class TrainZEstimator(CatEstimator):
     """CatEstimator which returns a global PDF for all galaxies
     """
 
-    name = 'TrainZ'
+    name = 'TrainZEstimator'
     config_options = CatEstimator.config_options.copy()
     config_options.update(zmin=SHARED_PARAMS,
                           zmax=SHARED_PARAMS,
                           nzbins=SHARED_PARAMS)
 
     def __init__(self, args, comm=None):
         self.zgrid = None
```

### Comparing `pz-rail-base-0.0.4/src/rail/estimation/algos/varInference.py` & `pz-rail-base-0.0.5/src/rail/estimation/algos/var_inf.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import qp
 from scipy.special import digamma
 from scipy.stats import dirichlet
 
 TEENY = 1.e-15
 
 
-class VarInferenceStack(PZSummarizer):
+class VarInfStackSummarizer(PZSummarizer):
     """Variational inference summarizer based on notebook created by Markus Rau
     The summzarizer is appropriate for the likelihoods returned by
     template-based codes, for which the NaiveSummarizer are not appropriate.
 
     Parameters
     ----------
     zmin: float
@@ -28,15 +28,15 @@
       number of bins for redshift grid
     niter: int
       number of iterations to perform in the variational inference
     nsamples: int
       number of samples used in dirichlet to determind error bar
     """
 
-    name = 'VarInferenceStack'
+    name = 'VarInfStackSummarizer'
     config_options = PZSummarizer.config_options.copy()
     config_options.update(zmin=Param(float, 0.0, msg="The minimum redshift of the z grid"),
                           zmax=Param(float, 3.0, msg="The maximum redshift of the z grid"),
                           nzbins=Param(int, 301, msg="The number of gridpoints in the z grid"),
                           seed=Param(int, 87, msg="random seed"),
                           niter=Param(int, 100, msg="The number of iterations in the variational inference"),
                           nsamples=Param(int, 500, msg="The number of samples used in dirichlet uncertainty"))
```

### Comparing `pz-rail-base-0.0.4/src/rail/estimation/estimator.py` & `pz-rail-base-0.0.5/src/rail/estimation/estimator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/estimation/summarizer.py` & `pz-rail-base-0.0.5/src/rail/estimation/summarizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         self.run()
         self.finalize()
         return self.get_handle('output')
 
 
 class SZPZSummarizer(RailStage):  #pragma: no cover
     """The base class for classes that use two sets of data: a photometry sample with
-    spec-z values, and a photometry sample with unknown redshifts, e.g. simpleSOM and
+    spec-z values, and a photometry sample with unknown redshifts, e.g. minisom_som and
     outputs a QP Ensemble with bootstrap realization of the N(z) distribution
     """
     name = 'SZPZtoNZSummarizer'
     config_options = RailStage.config_options.copy()
     config_options.update(chunk_size=10000)
     inputs = [('input', TableHandle),
               ('spec_input', TableHandle),
```

### Comparing `pz-rail-base-0.0.4/src/rail/evaluation/evaluator.py` & `pz-rail-base-0.0.5/src/rail/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/evaluation/metrics/base.py` & `pz-rail-base-0.0.5/src/rail/evaluation/metrics/base.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/evaluation/metrics/cdeloss.py` & `pz-rail-base-0.0.5/src/rail/evaluation/metrics/cdeloss.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/evaluation/metrics/pointestimates.py` & `pz-rail-base-0.0.5/src/rail/evaluation/metrics/pointestimates.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt` & `pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt` & `pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt` & `pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt` & `pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt` & `pz-rail-base-0.0.5/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res` & `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res` & `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res` & `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res` & `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res` & `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res` & `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed` & `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed` & `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed` & `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed` & `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed` & `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed` & `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed` & `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed` & `pz-rail-base-0.0.5/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml` & `pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl` & `pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq` & `pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/goldenspike_data/goldenspike.yml` & `pz-rail-base-0.0.5/src/rail/examples_data/goldenspike_data/goldenspike.yml`

 * *Files 5% similar despite different names*

```diff
@@ -38,25 +38,25 @@
   nprocess: 1
 - classname: LineConfusion
   name: line_confusion
   nprocess: 1
 - classname: QuantityCut
   name: quantity_cut
   nprocess: 1
-- classname: Inform_trainZ
+- classname: TrainZInformer
   name: inform_trainZ
   nprocess: 1
 - classname: Estimator
   name: estimate_bpz
   nprocess: 1
-- classname: TrainZ
+- classname: TrainZEstimator
   name: estimate_trainZ
   nprocess: 1
-- classname: RandomPZ
+- classname: RandomGaussEstimator
   name: estimate_randomZ
   nprocess: 1
-- classname: PointEstimateHist
+- classname: PointEstHistSummarizer
   name: point_estimate_test
   nprocess: 1
-- classname: NaiveStack
+- classname: NaiveStackSummarizer
   name: naive_stack_test
   nprocess: 1
```

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/testdata/README.md` & `pz-rail-base-0.0.5/src/rail/examples_data/testdata/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/testdata/lsst_filters.npy` & `pz-rail-base-0.0.5/src/rail/examples_data/testdata/lsst_filters.npy`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/testdata/make_rail_sample_data.ipynb` & `pz-rail-base-0.0.5/src/rail/examples_data/testdata/make_rail_sample_data.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/testdata/output_BPZ_lite.fits` & `pz-rail-base-0.0.5/src/rail/examples_data/testdata/output_BPZ_lite.fits`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq` & `pz-rail-base-0.0.5/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5` & `pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_training_9816.pq` & `pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_training_9816.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq` & `pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq` & `pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5` & `pz-rail-base-0.0.5/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/testdata/training_100gal.hdf5` & `pz-rail-base-0.0.5/src/rail/examples_data/testdata/training_100gal.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/examples_data/testdata/validation_10gal.hdf5` & `pz-rail-base-0.0.5/src/rail/examples_data/testdata/validation_10gal.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/src/rail/stages/__init__.py` & `pz-rail-base-0.0.5/src/rail/stages/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 import rail
 from rail.core import RailEnv
 
 from rail.estimation.estimator import *
 from rail.estimation.summarizer import *
-from rail.estimation.algos.naiveStack import *
-from rail.estimation.algos.randomPZ import *
-from rail.estimation.algos.pointEstimateHist import *
-from rail.estimation.algos.trainZ import *
-from rail.estimation.algos.varInference import *
+from rail.estimation.algos.naive_stack import *
+from rail.estimation.algos.random_gauss import *
+from rail.estimation.algos.point_est_hist import *
+from rail.estimation.algos.train_z import *
+from rail.estimation.algos.var_inf import *
 
 from rail.creation.degrader import *
 #from rail.creation.degradation.spectroscopic_degraders import *
 from rail.creation.degradation.spectroscopic_selections import *
 from rail.creation.degradation.quantityCut import *
 from rail.creation.degradation.lsst_error_model import *
```

### Comparing `pz-rail-base-0.0.4/tests/cli/test_scripts.py` & `pz-rail-base-0.0.5/tests/cli/test_scripts.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/tests/core/test_core.py` & `pz-rail-base-0.0.5/tests/core/test_core.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/tests/core/test_degraders.py` & `pz-rail-base-0.0.5/tests/core/test_degraders.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/tests/core/test_introspection.py` & `pz-rail-base-0.0.5/tests/core/test_introspection.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/tests/core/test_pipeline.py` & `pz-rail-base-0.0.5/tests/core/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.0.4/tests/estimation/test_algos.py` & `pz-rail-base-0.0.5/tests/estimation/test_algos.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import pytest
 import scipy.special
 
 from rail.core.algo_utils import one_algo
 from rail.core.stage import RailStage
-from rail.estimation.algos import randomPZ, trainZ
+from rail.estimation.algos import random_gauss, train_z
 
 sci_ver_str = scipy.__version__.split(".")
 
 
 DS = RailStage.data_store
 DS.__class__.allow_overwrite = True
 
@@ -21,15 +21,15 @@
         "rand_zmax": 3.0,
         "nzbins": 301,
         "hdf5_groupname": "photometry",
         "model": "None",
     }
     # zb_expected = np.array([1.359, 0.013, 0.944, 1.831, 2.982, 1.565, 0.308, 0.157, 0.986, 1.679])
     train_algo = None
-    pz_algo = randomPZ.RandomPZ
+    pz_algo = random_gauss.RandomGaussEstimator
     results, rerun_results, rerun3_results = one_algo(
         "RandomPZ", train_algo, pz_algo, train_config_dict, estim_config_dict
     )
     # assert np.isclose(results.ancil['zmode'], zb_expected).all()
     # assert np.isclose(pz_dict['zmode'], rerun_pz_dict['zmode']).all()
     # we skip this assert since the random number generator will return
     # different results the second run!
@@ -40,16 +40,16 @@
         zmin=0.0, zmax=3.0, nzbins=301, hdf5_groupname="photometry", model="model_train_z.tmp"
     )
     estim_config_dict = dict(hdf5_groupname="photometry", model="model_train_z.tmp")
 
     zb_expected = np.repeat(0.1445183, 10)
     pdf_expected = np.zeros(shape=(301,))
     pdf_expected[10:16] = [7, 23, 8, 23, 26, 13]
-    train_algo = trainZ.Inform_trainZ
-    pz_algo = trainZ.TrainZ
+    train_algo = train_z.TrainZInformer
+    pz_algo = train_z.TrainZEstimator
     results, rerun_results, rerun3_results = one_algo(
         "TrainZ", train_algo, pz_algo, train_config_dict, estim_config_dict
     )
     assert np.isclose(results.ancil["zmode"], zb_expected).all()
     assert np.isclose(results.ancil["zmode"], rerun_results.ancil["zmode"]).all()
```

### Comparing `pz-rail-base-0.0.4/tests/estimation/test_summarizers.py` & `pz-rail-base-0.0.5/tests/estimation/test_summarizers.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import pytest
 
 from rail.core.data import QPHandle
 from rail.core.stage import RailStage
 from rail.core.utils import RAILDIR
-from rail.estimation.algos import naiveStack, pointEstimateHist, varInference
+from rail.estimation.algos import naive_stack, point_est_hist, var_inf
 
 testdata = os.path.join(RAILDIR, "rail/examples_data/testdata/output_BPZ_lite.fits")
 DS = RailStage.data_store
 
 
 def one_algo(key, summarizer_class, summary_kwargs):
     """
@@ -25,21 +25,21 @@
     os.remove(summarizer.get_output(summarizer.get_aliased_tag("output"), final_name=True))
     os.remove(summarizer.get_output(summarizer.get_aliased_tag("single_NZ"), final_name=True))
     return summary_ens
 
 
 def test_naive_stack():
     summary_config_dict = {}
-    summarizer_class = naiveStack.NaiveStack
+    summarizer_class = naive_stack.NaiveStackSummarizer
     results = one_algo("NaiveStack", summarizer_class, summary_config_dict)
 
 
 def test_point_estimate_hist():
     summary_config_dict = {}
-    summarizer_class = pointEstimateHist.PointEstimateHist
+    summarizer_class = point_est_hist.PointEstHistSummarizer
     results = one_algo("PointEstimateHist", summarizer_class, summary_config_dict)
 
 
 def test_var_inference_stack():
     summary_config_dict = {}
-    summarizer_class = varInference.VarInferenceStack
+    summarizer_class = var_inf.VarInfStackSummarizer
     results = one_algo("VariationalInference", summarizer_class, summary_config_dict)
```

### Comparing `pz-rail-base-0.0.4/tests/evaluation/test_evaluation.py` & `pz-rail-base-0.0.5/tests/evaluation/test_evaluation.py`

 * *Files identical despite different names*

