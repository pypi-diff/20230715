# Comparing `tmp/pz-rail-gpz-v1-0.1.2.tar.gz` & `tmp/pz-rail-gpz-v1-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-gpz-v1-0.1.2.tar", last modified: Tue Jun 13 20:05:05 2023, max compression
+gzip compressed data, was "pz-rail-gpz-v1-0.1.3.tar", last modified: Fri Jul 14 23:55:10 2023, max compression
```

## Comparing `pz-rail-gpz-v1-0.1.2.tar` & `pz-rail-gpz-v1-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.426433 pz-rail-gpz-v1-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2083 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)      548 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1811 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3314 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/added_examples/
--rw-r--r--   0 runner    (1001) docker     (122)     8769 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/added_examples/GPz_estimation_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/src/pz_rail_gpz_v1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-06-13 20:05:05.000000 pz-rail-gpz-v1-0.1.2/src/pz_rail_gpz_v1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-06-13 20:05:05.000000 pz-rail-gpz-v1-0.1.2/src/pz_rail_gpz_v1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 20:05:05.000000 pz-rail-gpz-v1-0.1.2/src/pz_rail_gpz_v1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-06-13 20:05:05.000000 pz-rail-gpz-v1-0.1.2/src/pz_rail_gpz_v1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-13 20:05:05.000000 pz-rail-gpz-v1-0.1.2/src/pz_rail_gpz_v1.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (122)    21483 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/src/rail/estimation/algos/GPz.py
--rw-r--r--   0 runner    (1001) docker     (122)     6791 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/src/rail/estimation/algos/gpz_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/src/rail/gpz/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/src/rail/gpz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-13 20:05:04.000000 pz-rail-gpz-v1-0.1.2/src/rail/gpz/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:05:05.430434 pz-rail-gpz-v1-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-06-13 20:04:49.000000 pz-rail-gpz-v1-0.1.2/tests/test_gpz.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 23:55:10.319327 pz-rail-gpz-v1-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 23:55:10.319327 pz-rail-gpz-v1-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 23:55:10.319327 pz-rail-gpz-v1-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2080 2023-07-14 23:54:53.000000 pz-rail-gpz-v1-0.1.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      548 2023-07-14 23:54:53.000000 pz-rail-gpz-v1-0.1.3/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1811 2023-07-14 23:54:53.000000 pz-rail-gpz-v1-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-07-14 23:54:53.000000 pz-rail-gpz-v1-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-07-14 23:55:10.319327 pz-rail-gpz-v1-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6484 2023-07-14 23:54:53.000000 pz-rail-gpz-v1-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 23:55:10.319327 pz-rail-gpz-v1-0.1.3/added_examples/
+-rw-r--r--   0 runner    (1001) docker     (122)     8778 2023-07-14 23:54:53.000000 pz-rail-gpz-v1-0.1.3/added_examples/GPz_estimation_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-07-14 23:54:53.000000 pz-rail-gpz-v1-0.1.3/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-07-14 23:54:53.000000 pz-rail-gpz-v1-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-14 23:55:10.319327 pz-rail-gpz-v1-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-14 23:54:53.000000 pz-rail-gpz-v1-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 23:55:10.319327 pz-rail-gpz-v1-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 23:55:10.319327 pz-rail-gpz-v1-0.1.3/src/pz_rail_gpz_v1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-07-14 23:55:10.000000 pz-rail-gpz-v1-0.1.3/src/pz_rail_gpz_v1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-07-14 23:55:10.000000 pz-rail-gpz-v1-0.1.3/src/pz_rail_gpz_v1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 23:55:10.000000 pz-rail-gpz-v1-0.1.3/src/pz_rail_gpz_v1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-07-14 23:55:10.000000 pz-rail-gpz-v1-0.1.3/src/pz_rail_gpz_v1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-14 23:55:10.000000 pz-rail-gpz-v1-0.1.3/src/pz_rail_gpz_v1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 23:55:10.319327 pz-rail-gpz-v1-0.1.3/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 23:55:10.319327 pz-rail-gpz-v1-0.1.3/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 23:55:10.319327 pz-rail-gpz-v1-0.1.3/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (122)    21483 2023-07-14 23:54:53.000000 pz-rail-gpz-v1-0.1.3/src/rail/estimation/algos/_gpz_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6815 2023-07-14 23:54:53.000000 pz-rail-gpz-v1-0.1.3/src/rail/estimation/algos/gpz.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 23:55:10.319327 pz-rail-gpz-v1-0.1.3/src/rail/gpz/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-07-14 23:54:53.000000 pz-rail-gpz-v1-0.1.3/src/rail/gpz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-07-14 23:55:09.000000 pz-rail-gpz-v1-0.1.3/src/rail/gpz/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 23:55:10.319327 pz-rail-gpz-v1-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1277 2023-07-14 23:54:53.000000 pz-rail-gpz-v1-0.1.3/tests/test_gpz.py
```

### Comparing `pz-rail-gpz-v1-0.1.2/.github/workflows/main.yml` & `pz-rail-gpz-v1-0.1.3/.github/workflows/main.yml`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         python -m pip install --upgrade pip
         pip install wheel numpy # For somoclu
         pip install .[dev]
         pip install flake8 pytest pytest-cov mockmpi pytest-timeout
         if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
     - name: Test with pytest
       run: |
-        python -m pytest --cov=rail.estimation.algos.gpz_v1 --cov-report=xml
+        python -m pytest --cov=rail.estimation.algos.gpz --cov-report=xml
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v1
       with:
         file: ./coverage.xml
         flags: unittests
         env_vars: OS,PYTHON
         name: codecov-umbrella
```

### Comparing `pz-rail-gpz-v1-0.1.2/.github/workflows/pypi.yaml` & `pz-rail-gpz-v1-0.1.3/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-gpz-v1-0.1.2/.gitignore` & `pz-rail-gpz-v1-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-gpz-v1-0.1.2/LICENSE` & `pz-rail-gpz-v1-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-gpz-v1-0.1.2/PKG-INFO` & `pz-rail-gpz-v1-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-gpz-v1
-Version: 0.1.2
+Version: 0.1.3
 Summary: RAIL GPz v1 (pure python) Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-gpz-v1-0.1.2/added_examples/GPz_estimation_example.ipynb` & `pz-rail-gpz-v1-0.1.3/added_examples/GPz_estimation_example.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967287841062351%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# GPzEstimator example notebook\\n'), (2, 'A quick demo "*

 * *            'of running GPz on the typical test data.  You should have installed rail_gpz_v1 (we '*

 * *            'highly recommend that you do this from within a custom conda environment so that all '*

 * *            'dependencies for package versions are met), either by cloning and installing from '*

 * *            "github, or with:\\n'), (7, 'As RAIL is a namespace package, installing rail_gpz_v1 "*

 * *            'will […]*

```diff
@@ -1,24 +1,24 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "69a40421-e7b3-4a7d-9a97-b70bf6cb8f28",
             "metadata": {},
             "source": [
-                "# GPz_v1 example notebook\n",
+                "# GPzEstimator example notebook\n",
                 "\n",
-                "A quick demo of running gpz_v1 on the typical test data.  You should have installed both RAIL and rail_gpz_v1 (we highly recommend that you do this from within a custom conda environment so that all dependencies for package versions are met), either by cloning and installing from github, or with:\n",
+                "A quick demo of running GPz on the typical test data.  You should have installed rail_gpz_v1 (we highly recommend that you do this from within a custom conda environment so that all dependencies for package versions are met), either by cloning and installing from github, or with:\n",
                 "```\n",
                 "pip install pz-rail-gpz-v1\n",
                 "```\n",
                 "\n",
-                "As RAIL is a namespace package, installing rail_gpz_v1 will make `Inform_GPz_v1` and `GPz_v1` available, and they can be imported via:<br>\n",
+                "As RAIL is a namespace package, installing rail_gpz_v1 will make `GPzInformer` and `GPzEstimator` available, and they can be imported via:<br>\n",
                 "```\n",
-                "from rail.estimation.algos.gpz_v1 import Inform_GPz_v1, GPz_v1\n",
+                "from rail.estimation.algos.gpz import GPzInformer, GPzEstimator\n",
                 "```\n",
                 "\n",
                 "Let's start with all of our necessary imports:"
             ]
         },
         {
             "cell_type": "code",
@@ -30,15 +30,15 @@
                 "import os\n",
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "import rail\n",
                 "import qp\n",
                 "from rail.core.data import TableHandle\n",
                 "from rail.core.stage import RailStage\n",
-                "from rail.estimation.algos.gpz_v1 import Inform_GPz_v1, GPz_v1"
+                "from rail.estimation.algos.gpz import GPzInformer, GPzEstimator"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "abf96656-7cdc-4d45-ba13-355e3386e94d",
             "metadata": {},
@@ -94,23 +94,23 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "dee70194-46d5-4b3a-a282-b7ca123d008a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# set up the stage to run our GPZ_training\n",
-                "pz_train = Inform_GPz_v1.make_stage(name=\"GPz_Train\", model=\"GPz_model.pkl\", **gpz_train_dict)"
+                "pz_train = GPzInformer.make_stage(name=\"GPz_Train\", model=\"GPz_model.pkl\", **gpz_train_dict)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2cceb899-0acb-448d-8a58-7a61227547a9",
             "metadata": {},
             "source": [
-                "We are now ready to run the stage to create the model.  We will use the training data from `test_dc2_training_9816.hdf5`, which contains 10,225 galaxies drawn from healpix 9816 from the cosmoDC2_v1.1.4 dataset, to train the model.  Note that we read this data in called `train_data` in the DataStore.  Note that we set `trainfrac` to 0.8, so 80% of the data will be used in the \"main\" training, but 20% will be reserved by `Inform_GPz_v1` to determine a SIGMA parameter.  We set `max_iter` to 150, so we will see 150 steps where the stage tries to maximize the likelihood. We run the stage as follows:"
+                "We are now ready to run the stage to create the model.  We will use the training data from `test_dc2_training_9816.hdf5`, which contains 10,225 galaxies drawn from healpix 9816 from the cosmoDC2_v1.1.4 dataset, to train the model.  Note that we read this data in called `train_data` in the DataStore.  Note that we set `trainfrac` to 0.8, so 80% of the data will be used in the \"main\" training, but 20% will be reserved by `GPzInformer` to determine a SIGMA parameter.  We set `max_iter` to 150, so we will see 150 steps where the stage tries to maximize the likelihood. We run the stage as follows:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "d925f67e-d3a5-49ae-9a1e-6ac043dbdd0a",
             "metadata": {},
@@ -121,27 +121,27 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c5c7a409-1919-49c6-a258-4af05fe30e00",
             "metadata": {},
             "source": [
-                "This should have taken about 30 seconds on a typical desktop computer, and you should now see a file called `GPz_model.pkl` in the directory.  This model file is used by the `GPz_v1` stage to determine our redshift PDFs for the test set of galaxies.  Let's set up that stage, again defining a dictionary of variables for the config params:"
+                "This should have taken about 30 seconds on a typical desktop computer, and you should now see a file called `GPz_model.pkl` in the directory.  This model file is used by the `GPzEstimator` stage to determine our redshift PDFs for the test set of galaxies.  Let's set up that stage, again defining a dictionary of variables for the config params:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "cc2a9632-adfd-42cc-96c7-c0bb34390b15",
             "metadata": {},
             "outputs": [],
             "source": [
                 "gpz_test_dict = dict(hdf5_groupname=\"photometry\", model=\"GPz_model.pkl\")\n",
                 "\n",
-                "gpz_run = GPz_v1.make_stage(name=\"gpz_run\", **gpz_test_dict)"
+                "gpz_run = GPzEstimator.make_stage(name=\"gpz_run\", **gpz_test_dict)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8bfe0f11-5c38-4856-b845-d5fb830e707a",
             "metadata": {},
             "source": [
@@ -193,15 +193,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "093dd6f9-f935-4aa5-9898-1c52b3bef6d1",
             "metadata": {},
             "source": [
-                "GPz_v1 parameterizes each PDF as a single Gaussian, here we see a few examples of Gaussians of different widths.  Now let's grab the mode of each PDF (stored as ancil data in the ensemble) and compare to the true redshifts from the test_data file:"
+                "GPzEstimator parameterizes each PDF as a single Gaussian, here we see a few examples of Gaussians of different widths.  Now let's grab the mode of each PDF (stored as ancil data in the ensemble) and compare to the true redshifts from the test_data file:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e33ac16a-1c2b-4be8-a947-362bcc039431",
             "metadata": {},
```

### Comparing `pz-rail-gpz-v1-0.1.2/pyproject.toml` & `pz-rail-gpz-v1-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-gpz-v1-0.1.2/src/pz_rail_gpz_v1.egg-info/PKG-INFO` & `pz-rail-gpz-v1-0.1.3/src/pz_rail_gpz_v1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-gpz-v1
-Version: 0.1.2
+Version: 0.1.3
 Summary: RAIL GPz v1 (pure python) Interface
 Author-email: The LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pz-rail-gpz-v1-0.1.2/src/rail/estimation/algos/GPz.py` & `pz-rail-gpz-v1-0.1.3/src/rail/estimation/algos/_gpz_util.py`

 * *Files identical despite different names*

### Comparing `pz-rail-gpz-v1-0.1.2/src/rail/estimation/algos/gpz_v1.py` & `pz-rail-gpz-v1-0.1.3/src/rail/estimation/algos/gpz.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 can be found at:
 https://github.com/pwhatfield/GPz_py3
 """
 import numpy as np
 from ceci.config import StageParameter as Param
 from rail.core.common_params import SHARED_PARAMS
 from rail.estimation.estimator import CatEstimator, CatInformer
-from .GPz import GP, getOmega
+from ._gpz_util import GP, getOmega
 import qp
 
 
 
 def _prepare_data(data_dict, bands, err_bands, nondet_val, maglims, logflag):
     """Put data in 2D np array expected by GPz.
     For some reason they like to take the log of the magnitude errors, so
@@ -29,26 +29,26 @@
             data[:, numbands + i] = np.log(data_dict[eband])
         else:  # pragma: no cover
             data[:, numbands + i] = data_dict[eband]
         data[:, numbands + i][mask] = 1.0
     return data
 
 
-class Inform_GPz_v1(CatInformer):
+class GPzInformer(CatInformer):
     """Inform stage for GPz_v1
     Parameters
     ----------
 
     Returns
     -------
     gpz_model: model
       model file containing the trained GPz model to be used in estimate
       stage
     """
-    name = "Inform_GPz_v1"
+    name = "GPzInformer"
     config_options = CatInformer.config_options.copy()
     config_options.update(nondetect_val=SHARED_PARAMS,
                           mag_limits=SHARED_PARAMS,
                           trainfrac=Param(float, 0.75,
                                           msg="fraction of training data used to make tree, rest used to set best sigma"),
                           seed=Param(int, 87, msg="random seed"),
                           bands=SHARED_PARAMS,
@@ -111,18 +111,18 @@
         model.train(input_array, sz, omega=omega_weights, training=train_mask,
                     validation=val_mask, maxIter=self.config.max_iter,
                     maxAttempts=self.config.max_attempt)
         self.model = model
         self.add_data('model', self.model)
 
 
-class GPz_v1(CatEstimator):
-    """GPz_v1 estimator
+class GPzEstimator(CatEstimator):
+    """ Estimate stage for GPz_v1
     """
-    name = "GPz_v1"
+    name = "GPzEstimator"
     config_options = CatEstimator.config_options.copy()
     config_options.update(zmin=SHARED_PARAMS,
                           zmax=SHARED_PARAMS,
                           nzbins=SHARED_PARAMS,
                           nondetect_val=SHARED_PARAMS,
                           mag_limits=SHARED_PARAMS,
                           bands=SHARED_PARAMS,
```

### Comparing `pz-rail-gpz-v1-0.1.2/tests/test_gpz.py` & `pz-rail-gpz-v1-0.1.3/tests/test_gpz.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import numpy as np
 import os
 from rail.core.stage import RailStage
 from rail.core.algo_utils import one_algo
 from rail.core.utils import RAILDIR
-from rail.estimation.algos.gpz_v1 import Inform_GPz_v1, GPz_v1
+from rail.estimation.algos.gpz import GPzInformer, GPzEstimator
 import scipy.special
 sci_ver_str = scipy.__version__.split(".")
 
 
 traindata = os.path.join(RAILDIR, "rail/examples_data/testdata/training_100gal.hdf5")
 validdata = os.path.join(RAILDIR, "rail/examples_data/testdata/validation_10gal.hdf5")
 DS = RailStage.data_store
 DS.__class__.allow_overwrite = True
 
 
 def test_gpz_v1():
     train_config_dict = {"hdf5_groupname": "photometry", "max_iter": 30, "max_attempt": 25,
                          "model": "gpz_default.pkl"}
     estim_config_dict = {"hdf5_groupname": "photometry", "model": "gpz_default.pkl"}
-    train_algo = Inform_GPz_v1
-    pz_algo = GPz_v1
+    train_algo = GPzInformer
+    pz_algo = GPzEstimator
     zb_expected = np.array([0.12, 0.13, 0.12, 0.14, 0.07, 0.13, 0.14, 0.13,
                             0.06, 0.12])
     results, rerun_results, _ = one_algo("GPz_v1", train_algo, pz_algo,
                                          train_config_dict, estim_config_dict)
     flatres = results.ancil["zmode"].flatten()
     assert np.isclose(flatres, zb_expected, atol=2.e-02).all()
     assert np.isclose(results.ancil["zmode"], rerun_results.ancil["zmode"]).all()
```

