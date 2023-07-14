# Comparing `tmp/pz-rail-bpz-0.1.0.tar.gz` & `tmp/pz-rail-bpz-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-bpz-0.1.0.tar", last modified: Tue Jun 13 20:03:20 2023, max compression
+gzip compressed data, was "pz-rail-bpz-0.1.1.tar", last modified: Fri Jul 14 23:55:11 2023, max compression
```

## Comparing `pz-rail-bpz-0.1.0.tar` & `pz-rail-bpz-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.530973 pz-rail-bpz-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)      123 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.518972 pz-rail-bpz-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.522972 pz-rail-bpz-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)      548 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-06-13 20:03:20.530973 pz-rail-bpz-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1604 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.526972 pz-rail-bpz-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (122)    33291 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/examples/BPZ_lite_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)    22127 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/examples/BPZ_lite_with_custom_SEDs.ipynb
--rw-r--r--   0 runner    (1001) docker     (122)   460800 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/examples/nonphysical_dc2_templates.tar
--rw-r--r--   0 runner    (1001) docker     (122)    83848 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/examples/test_dc2_train_customtemp_broadttypes.hdf5
--rw-r--r--   0 runner    (1001) docker     (122)    83848 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/examples/test_dc2_training_9816_broadtypes.hdf5
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 20:03:20.530973 pz-rail-bpz-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.518972 pz-rail-bpz-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.526972 pz-rail-bpz-0.1.0/src/pz_rail_bpz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-06-13 20:03:20.000000 pz-rail-bpz-0.1.0/src/pz_rail_bpz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-06-13 20:03:20.000000 pz-rail-bpz-0.1.0/src/pz_rail_bpz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 20:03:20.000000 pz-rail-bpz-0.1.0/src/pz_rail_bpz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-06-13 20:03:20.000000 pz-rail-bpz-0.1.0/src/pz_rail_bpz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-13 20:03:20.000000 pz-rail-bpz-0.1.0/src/pz_rail_bpz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.518972 pz-rail-bpz-0.1.0/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.526972 pz-rail-bpz-0.1.0/src/rail/bpz/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/src/rail/bpz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-13 20:03:19.000000 pz-rail-bpz-0.1.0/src/rail/bpz/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)      147 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/src/rail/bpz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.518972 pz-rail-bpz-0.1.0/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.530973 pz-rail-bpz-0.1.0/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (122)    26630 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/src/rail/estimation/algos/bpz_lite.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.522972 pz-rail-bpz-0.1.0/src/rail/examples_data/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.522972 pz-rail-bpz-0.1.0/src/rail/examples_data/estimation_data/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.530973 pz-rail-bpz-0.1.0/src/rail/examples_data/estimation_data/configs/
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/src/rail/examples_data/estimation_data/configs/test_bpz.columns
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 20:03:20.530973 pz-rail-bpz-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     6092 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/tests/test_algos.py
--rw-r--r--   0 runner    (1001) docker     (122)    10624 2023-06-13 20:03:02.000000 pz-rail-bpz-0.1.0/tests/validation_10gal.pq
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:11.894701 pz-rail-bpz-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:11.890701 pz-rail-bpz-0.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:11.890701 pz-rail-bpz-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/.prepare_project.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-14 23:55:11.894701 pz-rail-bpz-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:11.894701 pz-rail-bpz-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    33371 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/examples/BPZ_lite_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22159 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/examples/BPZ_lite_with_custom_SEDs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   460800 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/examples/nonphysical_dc2_templates.tar
+-rw-r--r--   0 runner    (1001) docker     (123)    83848 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/examples/test_dc2_train_customtemp_broadttypes.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)    83848 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/examples/test_dc2_training_9816_broadtypes.hdf5
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 23:55:11.894701 pz-rail-bpz-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:11.886701 pz-rail-bpz-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:11.894701 pz-rail-bpz-0.1.1/src/pz_rail_bpz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-14 23:55:11.000000 pz-rail-bpz-0.1.1/src/pz_rail_bpz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-14 23:55:11.000000 pz-rail-bpz-0.1.1/src/pz_rail_bpz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:55:11.000000 pz-rail-bpz-0.1.1/src/pz_rail_bpz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 23:55:11.000000 pz-rail-bpz-0.1.1/src/pz_rail_bpz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 23:55:11.000000 pz-rail-bpz-0.1.1/src/pz_rail_bpz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:11.886701 pz-rail-bpz-0.1.1/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:11.894701 pz-rail-bpz-0.1.1/src/rail/bpz/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/src/rail/bpz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 23:55:11.000000 pz-rail-bpz-0.1.1/src/rail/bpz/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/src/rail/bpz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:11.886701 pz-rail-bpz-0.1.1/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:11.894701 pz-rail-bpz-0.1.1/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)    26654 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/src/rail/estimation/algos/bpz_lite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:11.886701 pz-rail-bpz-0.1.1/src/rail/examples_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:11.886701 pz-rail-bpz-0.1.1/src/rail/examples_data/estimation_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:11.894701 pz-rail-bpz-0.1.1/src/rail/examples_data/estimation_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/src/rail/examples_data/estimation_data/configs/test_bpz.columns
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:11.894701 pz-rail-bpz-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/tests/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-14 23:54:56.000000 pz-rail-bpz-0.1.1/tests/validation_10gal.pq
```

### Comparing `pz-rail-bpz-0.1.0/.gitignore` & `pz-rail-bpz-0.1.1/.gitignore`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 *$py.class
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
-_version.py
 build/
 develop-eggs/
 dist/
 downloads/
 eggs/
 .eggs/
 lib/
@@ -23,28 +22,26 @@
 wheels/
 pip-wheel-metadata/
 share/python-wheels/
 *.egg-info/
 .installed.cfg
 *.egg
 MANIFEST
+_version.py
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
 
 # Installer logs
 pip-log.txt
 pip-delete-this-directory.txt
 
-# AB files
-*.AB
-
 # Unit test / coverage reports
 htmlcov/
 .tox/
 .nox/
 .coverage
 .coverage.*
 .cache
@@ -70,14 +67,15 @@
 .webassets-cache
 
 # Scrapy stuff:
 .scrapy
 
 # Sphinx documentation
 docs/_build/
+_readthedocs/
 
 # PyBuilder
 target/
 
 # Jupyter Notebook
 .ipynb_checkpoints
 
@@ -127,7 +125,19 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# vscode
+.vscode/
+
+# dask
+dask-worker-space/
+
+# tmp directory
+tmp/
+
+# BPZ AB Files
+*.AB
```

### Comparing `pz-rail-bpz-0.1.0/LICENSE` & `pz-rail-bpz-0.1.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 LSST Dark Energy Science Collaboration (DESC)
+Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pz-rail-bpz-0.1.0/README.md` & `pz-rail-bpz-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # rail_bpz
-RAIL interface to BPZ algorithms via the [DESC_BPZ](https://github.com/LSSTDESC/DESC_BPZ) package implementation (also available via PyPI with `pip install desc-bpz`).
+
+[![codecov](https://codecov.io/gh/LSSTDESC/rail_bpz/branch/main/graph/badge.svg)](https://codecov.io/gh/LSSTDESC/rail_bpz)
+[![PyPI](https://img.shields.io/pypi/v/bpz?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/pz-rail-bpz/)
+
+
+RAIL interface to BPZ algorithms via the [DESC_BPZ](https://github.com/LSSTDESC/DESC_BPZ) package implementation (also available via PyPI with `pip install desc-bpz`).  Anyone using BPZ via either rail_bpz or DESC_BPZ should cite both [Benitez (2000)](https://ui.adsabs.harvard.edu/abs/2000ApJ...536..571B/abstract) and [Coe et al. (2006)](https://ui.adsabs.harvard.edu/abs/2006AJ....132..926C/abstract).
 
 As the "lite" name implies, not all features of BPZ are implemented, the main product is the marginalized redshift PDF, which is output for a sample as a `qp` ensemble.  However, several other quantities are computed and stored as "ancillary" data and stored with the ensemble, these are:
 - zmode (float): the mode of the marginalized posterior redshift PDF distribution.
 - zmean (float): the mean of the marginalized posterior redshift PDF distribution.
 - tb (int): the integer index for the "best-fit" SED template **at the redshift mode, `zmode`**.  Note that the best-fit template can be different at different redshifts as the SED observed colors change with redshift, so you **can not** assume this single SED for the full marginalized PDF, it should only be used for the "point estimate" redshift `zmode`.
 - todds (float): relating to the comment above on tb, `todds` is a new quantity not included with the original BPZ implementation, it is the fraction of marginalized posterior probability assigned to `tb`.  So, high values of `todds` would mean that no other templates fit well, even at other redshifts, while a lower value of `todds` means that there are alternative fits, either at the same redshift or other redshifts.  If you are wanting to compute physical quantities based on `tb`, a lower value of `todds` would mean that such fits would be missing degenerate SED solutions, and should not be trusted.
```

### Comparing `pz-rail-bpz-0.1.0/examples/BPZ_lite_demo.ipynb` & `pz-rail-bpz-0.1.1/examples/BPZ_lite_demo.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985210401428074%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(10, 'from rail.estimation.algos.bpz_lite import "*

 * *            "BPZliteInformer, BPZliteEstimator')], delete: [10]}}, 7: {'source': {insert: [(0, '## "*

 * *            "running BPZliteEstimator with a pre-existing model\\n'), (2, 'BPZ is a "*

 * *            'template-fitting code that works by calculating the chi^2 value for observed '*

 * *            'photometry and errors compared with a grid of theoretical photometric fluxes '*

 * *            'generated from a set of template SEDs a […]*

```diff
@@ -26,15 +26,15 @@
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "import pandas as pd\n",
                 "import desc_bpz\n",
                 "from rail.core.data import TableHandle\n",
                 "from rail.core.stage import RailStage\n",
                 "from rail.core.utils import RAILDIR\n",
-                "from rail.estimation.algos.bpz_lite import Inform_BPZ_lite, BPZ_lite"
+                "from rail.estimation.algos.bpz_lite import BPZliteInformer, BPZliteEstimator"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b04c8503-74ee-4de7-b0f7-a2d8d1398db7",
             "metadata": {},
             "source": [
@@ -84,43 +84,43 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "979d5363-af4e-4478-9820-29214292bf16",
             "metadata": {},
             "source": [
-                "## running BPZ_lite with a pre-existing model\n",
+                "## running BPZliteEstimator with a pre-existing model\n",
                 "\n",
-                "BPZ is a template-fitting code that works by calculating the chi^2 value for observed photometry and errors compared with a grid of theoretical photometric fluxes generated from a set of template SEDs at each of a grid of redshift values.  These chi^2 values are converted to likelihoods.  If desired, a Bayesian prior can be applied that parameterizes the expected distribution of galaxies in terms of both probability of a \"broad\" SED type as a function of apparent magnitude, and the probability of a galaxy being at a certain redshift given broad SED type and apparent magnitude.  The product of this prior and the likelihoods is then summed over the SED types to return a marginalized posterior PDF, or p(z) for each galaxy.  If the config option `no_prior` is set to `True`, then no prior is applied, and BPZ_lite will return a likelihood for each galaxy rather than a posterior.\n",
+                "BPZ is a template-fitting code that works by calculating the chi^2 value for observed photometry and errors compared with a grid of theoretical photometric fluxes generated from a set of template SEDs at each of a grid of redshift values.  These chi^2 values are converted to likelihoods.  If desired, a Bayesian prior can be applied that parameterizes the expected distribution of galaxies in terms of both probability of a \"broad\" SED type as a function of apparent magnitude, and the probability of a galaxy being at a certain redshift given broad SED type and apparent magnitude.  The product of this prior and the likelihoods is then summed over the SED types to return a marginalized posterior PDF, or p(z) for each galaxy.  If the config option `no_prior` is set to `True`, then no prior is applied, and BPZliteEstimator will return a likelihood for each galaxy rather than a posterior.\n",
                 "\n",
                 "\n",
-                "`bpz-1.99.3`, the code written by Dan Coe and Narcisso Benitez and available at https://www.stsci.edu/~dcoe/BPZ/, uses a default set of eight SED templates: four templates from Coleman, Wu, & Weedman (CWW, one Elliptical, two Spirals Sbc and Scd, and one Irregular), two starburst (WB) templates, and two very blue star forming templates generated using Bruzual & Charlot models with very young ages of 25Myr and 5Myr.  The original BPZ paper, Benitez(2000) computed a \"default\" prior fit to data from the Hubble Deep Field North (HDFN).  A pickle file with these parameters and the default SEDs are included with RAIL, named `CWW_HDFN_prior.pkl`.  You can run BPZ_lite with these default templates and priors without doing any training, the equivalent of \"running BPZ with the defaults\" had you downloaded bpz-1.99.3 and run it.  **Note, however**, that the cosmoDC2_v1.1.4 dataset has a population of galaxy SEDs that are fairly different from the \"default\" CWWSB templates, and the prior distributions do not exactly match.  So, you will get results that do not look particularly good.  We will demonstrate that use case here, though, as it is the most simple way to run the code out of the box (and illustrates the dangers of grabbing code and running it out of the box):\n",
+                "`bpz-1.99.3`, the code written by Dan Coe and Narcisso Benitez and available at https://www.stsci.edu/~dcoe/BPZ/, uses a default set of eight SED templates: four templates from Coleman, Wu, & Weedman (CWW, one Elliptical, two Spirals Sbc and Scd, and one Irregular), two starburst (WB) templates, and two very blue star forming templates generated using Bruzual & Charlot models with very young ages of 25Myr and 5Myr.  The original BPZ paper, Benitez(2000) computed a \"default\" prior fit to data from the Hubble Deep Field North (HDFN).  A pickle file with these parameters and the default SEDs are included with RAIL, named `CWW_HDFN_prior.pkl`.  You can run BPZliteEstimator with these default templates and priors without doing any training, the equivalent of \"running BPZ with the defaults\" had you downloaded bpz-1.99.3 and run it.  **Note, however**, that the cosmoDC2_v1.1.4 dataset has a population of galaxy SEDs that are fairly different from the \"default\" CWWSB templates, and the prior distributions do not exactly match.  So, you will get results that do not look particularly good.  We will demonstrate that use case here, though, as it is the most simple way to run the code out of the box (and illustrates the dangers of grabbing code and running it out of the box):\n",
                 "\n",
                 "We need to set up a RAIL stage for the default run of BPZ, including specifying the location of the model pickle file:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a03c3e9f-7080-4334-bcf1-7993239b69db",
             "metadata": {},
             "outputs": [],
             "source": [
                 "hdfnfile = os.path.join(RAILDIR, \"rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl\")\n",
                 "default_dict = dict(hdf5_groupname=\"photometry\", output=\"bpz_results_defaultprior.hdf5\",\n",
                 "                    prior_band=\"mag_i_lsst\", no_prior=False)\n",
-                "run_default = BPZ_lite.make_stage(name=\"bpz_def_prior\", model=hdfnfile, **default_dict)"
+                "run_default = BPZliteEstimator.make_stage(name=\"bpz_def_prior\", model=hdfnfile, **default_dict)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e8bba83c-d3ed-4385-852c-639e59170c48",
             "metadata": {},
             "source": [
-                "Let's run the estimate stage, if this is the first run of ``BPZ_lite`` or ``Inform_BPZ_lite``, you may see a bunch of output lines as ``DESC_BPZ`` creates the synthetic photometry \"AB\" files for the SEDs and filters."
+                "Let's run the estimate stage, if this is the first run of ``BPZliteEstimator`` or ``BPZliteInformer``, you may see a bunch of output lines as ``DESC_BPZ`` creates the synthetic photometry \"AB\" files for the SEDs and filters."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2b5cd587-122e-41ef-9d3f-77333a54c6bc",
             "metadata": {},
@@ -175,15 +175,15 @@
         {
             "cell_type": "markdown",
             "id": "e487194d-1af0-4a1f-ac35-06490ab7a735",
             "metadata": {},
             "source": [
                 "Results do not look bad, there are some catastrophic outliers, and there appears to be some bias in the redshift estimates, but as the SED templates have slightly systematically different colors than our test data, that is just what we expect to see.\n",
                 "\n",
-                "BPZ_lite also produces a `tb` , a \"best-fit type\"; that is, the SED template with the highest posterior probability contribution at the value of the `zmode`. We can plot up a color color diagram of our test data and we should see a pattern in color space reflecting the different populations in different areas of color space.  `tb` is stored as an 1-indexed integer corresponding the the number of the SED in our template set."
+                "BPZliteEstimator also produces a `tb` , a \"best-fit type\"; that is, the SED template with the highest posterior probability contribution at the value of the `zmode`. We can plot up a color color diagram of our test data and we should see a pattern in color space reflecting the different populations in different areas of color space.  `tb` is stored as an 1-indexed integer corresponding the the number of the SED in our template set."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e9ef1cc3-2368-4426-b570-0a788f39846f",
             "metadata": {},
@@ -227,15 +227,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "6ee27ab8-2282-45ae-99bc-a8fcc5691ee1",
             "metadata": {},
             "source": [
-                "BPZ_lite also computes a quantity called `todds`, which is the fraction of posterior probability in the best-fit SED relative to the overall probability of all templates.  If the value is high, then a single SED is providing more of the probability.  If the value is low, then multiple SEDs are contributing, which means that `tb`, the best-fit-SED-type, is less meaningful.  The values of todds whould be lower where SEDs have degenerate broad-band colors, let's highlight the values of low todds and see where they lie in color space."
+                "BPZliteEstimator also computes a quantity called `todds`, which is the fraction of posterior probability in the best-fit SED relative to the overall probability of all templates.  If the value is high, then a single SED is providing more of the probability.  If the value is low, then multiple SEDs are contributing, which means that `tb`, the best-fit-SED-type, is less meaningful.  The values of todds whould be lower where SEDs have degenerate broad-band colors, let's highlight the values of low todds and see where they lie in color space."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "32143555-6e79-4dd5-a128-40afdb8c4a97",
             "metadata": {},
@@ -260,38 +260,38 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e80d59ce-ca73-4bf3-9f3d-682c4dbdcb3e",
             "metadata": {},
             "source": [
-                "# Inform_BPZ_lite: training a custom prior\n",
+                "# BPZliteInformer: training a custom prior\n",
                 "\n",
-                "If you want to go beyond the default prior, there is an `Inform_BPZ_lite` stage that allows you to use a training dataset to fit a custom parameterized prior that better matches the magnitude and type distributions of the training set.\n",
+                "If you want to go beyond the default prior, there is an `BPZliteInformer` stage that allows you to use a training dataset to fit a custom parameterized prior that better matches the magnitude and type distributions of the training set.\n",
                 "\n",
-                "`bpz-1.99.3` and our local fork, `DESC_BPZ` both parameterize the Bayesian prior using the form described in Benitez (2000), where the individual SED types are grouped into \"broad types\", e.g. 1 Elliptical makes up one type, the two spirals (Sbc and Scd) make up a second, and the five remaining \"blue\" templates (Im, SB3, SB2, ssp25Myr, and ssp5Myr) make up a third type.  This grouping is somewhat ad-hoc, but does have physical motivation, in that we have observed that Ellipticals, spirals, and irregular/starburst galaxies do show distinctly evolving observed fractions as a function of apparent/absolute magnitude and redshift.  Things get more complicated with more complex SED sets that contain variations in dust content, star formation histories, emission lines, etc...  Due to such complications, the **current** implementation of `inform_BPZ_lite` leaves the assignment of a \"broad-SED-type\" to the user, and these broad types are a necessary input to `Inform_BPZ_lite` via the `type_file` config option.  In the future, determination of broad SED type will be added as a pre-processing step to the rail_bpz package.\n",
+                "`bpz-1.99.3` and our local fork, `DESC_BPZ` both parameterize the Bayesian prior using the form described in Benitez (2000), where the individual SED types are grouped into \"broad types\", e.g. 1 Elliptical makes up one type, the two spirals (Sbc and Scd) make up a second, and the five remaining \"blue\" templates (Im, SB3, SB2, ssp25Myr, and ssp5Myr) make up a third type.  This grouping is somewhat ad-hoc, but does have physical motivation, in that we have observed that Ellipticals, spirals, and irregular/starburst galaxies do show distinctly evolving observed fractions as a function of apparent/absolute magnitude and redshift.  Things get more complicated with more complex SED sets that contain variations in dust content, star formation histories, emission lines, etc...  Due to such complications, the **current** implementation of `BPZliteInformer` leaves the assignment of a \"broad-SED-type\" to the user, and these broad types are a necessary input to `BPZliteInformer` via the `type_file` config option.  In the future, determination of broad SED type will be added as a pre-processing step to the rail_bpz package.\n",
                 "\n",
                 "The easiest way to obtain these broad SED types is to run `DESC_BPZ` with the parameter `ONLY_TYPE` set to `yes`.  When the `ONLY_TYPE` option is turned on in `DESC_BPZ`, the code returns a best-fit SED type evaluated only at the spectroscopic redshift for the object (determined as the best chi^2 amongst the N templates).  The user then needs to map these N integers down to a set of \"broad-type\" integers corresponding to however they wish to define the mapping from N SED types to M broad types.  As an example, I have done this using the CWWSB templates and the 1 Ell, 2 sp, 5 Im/SB broad type mapping for our `test_dc2_training_9816.hdf5` dataset and included that mapping file in this directory in a file named `test_dc2_training_9816_broadtypes.hdf5` for use in our demo, which consists of an array of integers named `types` with values 0 (Elliptical), 1 (Spiral), and 2 (Irregular/Starburst) corresponding to the best-fit broad SED for each of the 10,225 galaxies in our training sample.\n",
                 "\n",
-                "Now, let's set up our inform stage to calculate a new prior.  We will name the new prior `test_9816_demo_prior.pkl`, setting this as the `model` config parameter will tell `Inform_BPZ_lite` to save our trained model by that name in the current directory.\n",
+                "Now, let's set up our inform stage to calculate a new prior.  We will name the new prior `test_9816_demo_prior.pkl`, setting this as the `model` config parameter will tell `BPZliteInformer` to save our trained model by that name in the current directory.\n",
                 "\n",
                 "When we run `inform` it will display values for the parameters as the minimizer runs, including final values for the parameters.  You do not need to pay attention to these values, though if you are curious you can plot them up and compare to the distributions of the HDFN prior."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "5a283f01-f110-436c-9bf1-ec9d702782f3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "train_dict = dict(hdf5_groupname=\"photometry\", model=\"test_9816_demo_prior.pkl\",\n",
                 "                 type_file=\"test_dc2_training_9816_broadtypes.hdf5\",\n",
                 "                 nt_array=[1,2,5])\n",
-                "run_bpz_train = Inform_BPZ_lite.make_stage(name=\"bpz_new_prior\", **train_dict)"
+                "run_bpz_train = BPZliteInformer.make_stage(name=\"bpz_new_prior\", **train_dict)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "9f2e34ec-19d2-4be6-9c06-35574d5fd798",
             "metadata": {},
@@ -416,27 +416,27 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "82d0919d-5842-4297-9a03-3838c6be6a2c",
             "metadata": {},
             "source": [
-                "Now, let's re-run BPZ_lite using this new prior and see if our results are any different:"
+                "Now, let's re-run BPZliteEstimator using this new prior and see if our results are any different:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "00c43a9a-4afe-4d8b-8aeb-5cd4845bdbe0",
             "metadata": {},
             "outputs": [],
             "source": [
                 "rerun_dict = dict(hdf5_groupname=\"photometry\", output=\"bpz_results_rerun.hdf5\", prior_band='mag_i_lsst',\n",
                 "                 no_prior=False)\n",
-                "rerun = BPZ_lite.make_stage(name=\"rerun_bpz\", **rerun_dict, \n",
+                "rerun = BPZliteEstimator.make_stage(name=\"rerun_bpz\", **rerun_dict, \n",
                 "                            model=run_bpz_train.get_handle('model'))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "1fd05674-9cb6-4c0f-94dc-f3947d711f41",
```

### Comparing `pz-rail-bpz-0.1.0/examples/BPZ_lite_with_custom_SEDs.ipynb` & `pz-rail-bpz-0.1.1/examples/BPZ_lite_with_custom_SEDs.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9969671291285875%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Running BPZliteEstimator with a custom set of "*

 * *            "SEDs\\n')], delete: [0]}}, 5: {'source': {insert: [(9, 'from "*

 * *            "rail.estimation.algos.bpz_lite import BPZliteInformer, BPZliteEstimator')], delete: "*

 * *            "[9]}}, 10: {'source': {insert: [(0, '# BPZliteInformer: training a custom prior with "*

 * *            "our new SEDs\\n'), (2, 'We will run the inform stage just as we did in the main demo "*

 * *            'notebook; however, we will have […]*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "85906442-6d29-407a-8d80-4108d45af015",
             "metadata": {},
             "source": [
-                "# Running BPZ_lite with a custom set of SEDs\n",
+                "# Running BPZliteEstimator with a custom set of SEDs\n",
                 "authors: Sam Schmidt<br>\n",
                 "Last successfully run: Apr 14, 2023<br>\n",
                 "\n",
                 "This notebook will go through an example of running rail_bpz estimate and inform stages with a custom set of SEDs.\n",
                 "\n",
                 "## **NOTE: the SEDs used in this example are SPECIFIC to DESC's cosmoDC2_v1.1.4 data, they contain some non-physical features that would add systematics if run on any real data! DO NOT USE THESE TEMPLATES FOR ANY SCIENCE WITH REAL DATA!**\n",
                 "\n",
@@ -73,15 +73,15 @@
                 "import pickle\n",
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "import pandas as pd\n",
                 "import desc_bpz\n",
                 "from rail.core.data import TableHandle\n",
                 "from rail.core.stage import RailStage\n",
-                "from rail.estimation.algos.bpz_lite import Inform_BPZ_lite, BPZ_lite"
+                "from rail.estimation.algos.bpz_lite import BPZliteInformer, BPZliteEstimator"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b04c8503-74ee-4de7-b0f7-a2d8d1398db7",
             "metadata": {},
             "source": [
@@ -121,32 +121,32 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e80d59ce-ca73-4bf3-9f3d-682c4dbdcb3e",
             "metadata": {},
             "source": [
-                "# Inform_BPZ_lite: training a custom prior with our new SEDs\n",
+                "# BPZliteInformer: training a custom prior with our new SEDs\n",
                 "\n",
-                "We will run the inform stage just as we did in the main demo notebook; however, we will have to define a few extra configuration parameters in order to tell Inform_BPZ_lite to use our new SEDs.  We specify the SED set using the `spectra_file` configuration parameter, which points to an ascii file that contains the names of the SEDs, which must be sorted in the same order as the \"broad type array\" (usually done in ascending rest-frame \"blueness\", that is Elliptical red galaxies first, then increasingly blue galaxies). In this case, the tar file that we copied to the SED directory contained this file, named `baddc2templates.list`.   As before, we need a \"best fit type\" for each of the galaxies in our training set. And, as before, this has been computed separately (computing best type within rail_bpz will be added in the future).  The best fit broad types are available in a dictionary stored in the file `test_dc2_train_customtemp_broadttypes.hdf5`, which we will point to with the `type_file` config parameter.  This file should already exist in this directory.  As stated above, we have two Elliptical, three Spiral, and four Irregular/Starburst seds, so we'll set the `nt_array` configuration parameter to a list `[2, 3, 4]` to specify those numbers of the three broad types."
+                "We will run the inform stage just as we did in the main demo notebook; however, we will have to define a few extra configuration parameters in order to tell BPZliteInformer to use our new SEDs.  We specify the SED set using the `spectra_file` configuration parameter, which points to an ascii file that contains the names of the SEDs, which must be sorted in the same order as the \"broad type array\" (usually done in ascending rest-frame \"blueness\", that is Elliptical red galaxies first, then increasingly blue galaxies). In this case, the tar file that we copied to the SED directory contained this file, named `baddc2templates.list`.   As before, we need a \"best fit type\" for each of the galaxies in our training set. And, as before, this has been computed separately (computing best type within rail_bpz will be added in the future).  The best fit broad types are available in a dictionary stored in the file `test_dc2_train_customtemp_broadttypes.hdf5`, which we will point to with the `type_file` config parameter.  This file should already exist in this directory.  As stated above, we have two Elliptical, three Spiral, and four Irregular/Starburst seds, so we'll set the `nt_array` configuration parameter to a list `[2, 3, 4]` to specify those numbers of the three broad types."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "5a283f01-f110-436c-9bf1-ec9d702782f3",
             "metadata": {},
             "outputs": [],
             "source": [
                 "train_dict = dict(hdf5_groupname=\"photometry\", model=\"test_9816_customsed_demo_prior.pkl\",\n",
                 "                  spectra_file=\"baddc2templates.list\",\n",
                 "                  type_file=\"test_dc2_train_customtemp_broadttypes.hdf5\",\n",
                 "                  prior_band=\"mag_i_lsst\",\n",
                 "                  nt_array=[2,3,4])\n",
-                "run_bpz_train = Inform_BPZ_lite.make_stage(name=\"bpz_custom_sed_prior\", **train_dict)"
+                "run_bpz_train = BPZliteInformer.make_stage(name=\"bpz_custom_sed_prior\", **train_dict)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "9f2e34ec-19d2-4be6-9c06-35574d5fd798",
             "metadata": {},
@@ -269,15 +269,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "82d0919d-5842-4297-9a03-3838c6be6a2c",
             "metadata": {},
             "source": [
-                "Now, let's re-run BPZ_lite using this new prior and see if our results are any different:"
+                "Now, let's re-run BPZliteEstimator using this new prior and see if our results are any different:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "00c43a9a-4afe-4d8b-8aeb-5cd4845bdbe0",
             "metadata": {},
@@ -285,15 +285,15 @@
             "source": [
                 "custom_dict = dict(hdf5_groupname=\"photometry\",\n",
                 "                   spectra_file=\"baddc2templates.list\",\n",
                 "                   output=\"bpz_results_customprior.hdf5\", \n",
                 "                   prior_band='mag_i_lsst',\n",
                 "                   data_path=custom_data_path,\n",
                 "                   no_prior=False)\n",
-                "custom_run = BPZ_lite.make_stage(name=\"rerun_bpz\", **custom_dict, \n",
+                "custom_run = BPZliteEstimator.make_stage(name=\"rerun_bpz\", **custom_dict, \n",
                 "                                 model=run_bpz_train.get_handle('model'))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "2ae7bdd8-bd48-4dc5-886a-3461ae3b1935",
             "metadata": {},
@@ -547,13 +547,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.10.12"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz-rail-bpz-0.1.0/examples/nonphysical_dc2_templates.tar` & `pz-rail-bpz-0.1.1/examples/nonphysical_dc2_templates.tar`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.0/examples/test_dc2_train_customtemp_broadttypes.hdf5` & `pz-rail-bpz-0.1.1/examples/test_dc2_train_customtemp_broadttypes.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.0/examples/test_dc2_training_9816_broadtypes.hdf5` & `pz-rail-bpz-0.1.1/examples/test_dc2_training_9816_broadtypes.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.0/pyproject.toml` & `pz-rail-bpz-0.1.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,126 +1,77 @@
 [project]
 name = "pz-rail-bpz"
-description = "RAIL BPZ Interface"
-readme = "README.rst"
-requires-python = ">=3.8"
-license = { file = "LICENSE" }
+license = {file = "LICENSE"}
+readme = "README.md"
 authors = [
-    { name = "The LSST DESC PZ WG", email = "samuel.j.schmidt@gmail.com" }
+    { name = "LSST DESC PZ WG", email = "samuel.j.schmidt@gmail.com" }
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
+    "Operating System :: OS Independent",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.10",
-    "Natural Language :: English",
-    "Operating System :: POSIX"
 ]
 dynamic = ["version"]
+
 dependencies = [
     "desc-bpz",
     "pz-rail-base",
     "qp-prob[full]",
 ]
 
+# On a mac, install optional dependencies with `pip install '.[dev]'` (include the single quotes)
 [project.optional-dependencies]
 dev = [
-    "coverage",
-    "pylint",
     "pytest",
-    "pytest-cov",
+    "pytest-cov", # Used to report total code coverage
     "pre-commit", # Used to run checks before finalizing a git commit
-    "yamllint",
+    "pylint", # Used for static linting of files
 ]
 
 [build-system]
-requires = ["setuptools>=61", "wheel", "setuptools_scm[toml]>=6.2"]
+requires = [
+    "setuptools>=62", # Used to build and package the Python project
+    "wheel",
+    "setuptools_scm>=6.2", # Gets release version from git. Makes it available programmatically
+]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "src/rail/bpz/_version.py"
 
 [tool.setuptools.package-data]
 "rail.examples.estimation.configs" = ["*.columns"]
 
-[tool.coverage.run]
-source = ["src/rail"]
-branch = true
-
-[tool.coverage.report]
-show_missing = true
-exclude_lines = [
-    "pragma: no cover",
-    "def __repr__",
-    "if self.debug:",
-    "if settings.DEBUG",
-    "raise AssertionError",
-    "raise NotImplementedError",
-    "if 0:",
-    "if __name__ == .__main__.:",
-    "if TYPE_CHECKING:"
-]
-
-[tool.black]
-line-length = 110
-target-version = ["py310"]
-
-[tool.pydocstyle]
-convention = "numpy"
-add_select = [
-    "D212" # Multi-line docstring summary should start at the first line
-]
-add-ignore = [
-    "D105", # Missing docstring in magic method
-    "D102", # Missing docstring in public method (needed for docstring inheritance)
-    "D100", # Missing docstring in public module
-    # Below are required to allow multi-line summaries.
-    "D200", # One-line docstring should fit on one line with quotes
-    "D205", # 1 blank line required between summary line and description
-    "D400", # First line should end with a period
-    # Properties shouldn't be written in imperative mode. This will be fixed
-    # post 6.1.1, see https://github.com/PyCQA/pydocstyle/pull/546
-    "D401",
+[tools.setuptools.packages.find]
+where = ["."]
+include = ["rail"]
+namespaces = true
+
+[tool.pytest.ini_options]
+testpaths = [
+    "tests",
+]
+addopts = [
+    "--cov=rail",
+    "--cov-report=html"
 ]
 
 [tool.pylint]
 disable = [
     "abstract-method",
     "invalid-name",
     "too-many-statements",
     "missing-module-docstring",
     "missing-class-docstring",
     "missing-function-docstring",
     "too-few-public-methods",
-    "duplicate-code"
+    "duplicate-code",
+    "use-dict-literal",
+    "broad-exception-caught",
 ]
 max-line-length = 110
 max-locals = 50
 max-branches = 25
 max-public-methods = 50
-
-[tool.isort]
-profile = "black"
-line_length = 110
-
-[tool.pytest.ini_options]
-addopts = [
-    "--cov=rail.estimation.algos.bpz_lite",
-    "--cov-branch",
-    "--cov-report=html"
-]
-flake8-ignore = "E203"
-
-[tool.mypy]
-disallow_untyped_defs = true
-disallow_incomplete_defs = true
-ignore_missing_imports = true
-namespace_packages = true
-plugins = "sqlalchemy.ext.mypy.plugin"
-show_error_codes = true
-strict_equality = true
-warn_redundant_casts = true
-warn_unreachable = true
-warn_unused_ignores = true
```

### Comparing `pz-rail-bpz-0.1.0/src/rail/estimation/algos/bpz_lite.py` & `pz-rail-bpz-0.1.1/src/rail/estimation/algos/bpz_lite.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 
 
 def nzfunc(z, z0, alpha, km, m, m0):  # pragma: no cover
     zm = z0 + (km * (m - m0))
     return np.power(z, alpha) * np.exp(-1. * np.power((z / zm), alpha))
 
 
-class Inform_BPZ_lite(CatInformer):
-    """Inform stage for BPZ_lite, this stage *assumes* that you have a set of
+class BPZliteInformer(CatInformer):
+    """Inform stage for BPZliteEstimator, this stage *assumes* that you have a set of
     SED templates and that the training data has already been assigned a
     'best fit broad type' (that is, something like ellliptical, spiral,
     irregular, or starburst, similar to how the six SEDs in the CWW/SB set
     of Benitez (2000) are assigned 3 broad types).  This informer will then
     fit parameters for the evolving type fraction as a function of apparent
     magnitude in a reference band, P(T|m), as well as the redshift prior
     of finding a galaxy of the broad type at a particular redshift, p(z|m, T)
@@ -57,15 +57,15 @@
     For p(z|T,m) we have
     P(z|T,m) = f_x*z0_x^a *exp(-(z/zm_x)^a)
     where zm_x = z0_x*(km_x-m0)
     where f_x is the type fraction from p(T|m), and we fit for values of
     z0, km, and a for each type.  These parameters are then fed to the BPZ
     prior for use in the estimation stage.
     """
-    name = "Inform_BPZ_lite"
+    name = "BPZliteInformer"
     config_options = CatInformer.config_options.copy()
     config_options.update(zmin=SHARED_PARAMS,
                           zmax=SHARED_PARAMS,
                           nzbins=SHARED_PARAMS,
                           nondetect_val=SHARED_PARAMS,
                           mag_limits=SHARED_PARAMS,
                           bands=SHARED_PARAMS,
@@ -228,26 +228,26 @@
 
         self.model = dict(fo_arr=self.fo_arr, kt_arr=self.kt_arr, zo_arr=zo_arr,
                           km_arr=km_arr, a_arr=a_arr, mo=self.config.m0,
                           nt_array=self.config.nt_array)
         self.add_data("model", self.model)
 
 
-class BPZ_lite(CatEstimator):
+class BPZliteEstimator(CatEstimator):
     """CatEstimator subclass to implement basic marginalized PDF for BPZ
     In addition to the marginalized redshift PDF, we also compute several
     ancillary quantities that will be stored in the ensemble ancil data:
     zmode: mode of the PDF
     amean: mean of the PDF
     tb: integer specifying the best-fit SED *at the redshift mode*
     todds: fraction of marginalized posterior prob. of best template,
     so lower numbers mean other templates could be better fits, likely
     at other redshifts
     """
-    name = "BPZ_lite"
+    name = "BPZliteEstimator"
     config_options = CatEstimator.config_options.copy()
     config_options.update(zmin=SHARED_PARAMS,
                           zmax=SHARED_PARAMS,
                           nzbins=SHARED_PARAMS,
                           nondetect_val=SHARED_PARAMS,
                           mag_limits=SHARED_PARAMS,
                           bands=SHARED_PARAMS,
```

### Comparing `pz-rail-bpz-0.1.0/src/rail/examples_data/estimation_data/configs/test_bpz.columns` & `pz-rail-bpz-0.1.1/src/rail/examples_data/estimation_data/configs/test_bpz.columns`

 * *Files identical despite different names*

### Comparing `pz-rail-bpz-0.1.0/tests/test_algos.py` & `pz-rail-bpz-0.1.1/tests/test_algos.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                          'model': 'testmodel_bpz.pkl'}
     if len(ntarray) == 2:
         broad_types = np.random.randint(2, size=100)
     else:
         broad_types = np.zeros(100, dtype=int)
     typedict = dict(types=broad_types)
     tables_io.write(typedict, "tmp_broad_types.hdf5")
-    train_algo = bpz_lite.Inform_BPZ_lite
+    train_algo = bpz_lite.BPZliteInformer
     DS.clear()
     training_data = DS.read_file('training_data', TableHandle, traindata)
     train_stage = train_algo.make_stage(**train_config_dict)
     train_stage.inform(training_data)
     expected_keys = ['fo_arr', 'kt_arr', 'zo_arr', 'km_arr', 'a_arr', 'mo', 'nt_array']
     with open("testmodel_bpz.pkl", "rb") as f:
         tmpmodel = pickle.load(f)
@@ -69,15 +69,15 @@
                          'zp_errors': np.array([0.01, 0.01, 0.01, 0.01, 0.01, 0.01]),
                          'mag_err_min': 0.005,
                          'hdf5_groupname': 'photometry',
                          'nt_array': [8],
                          'model': 'testmodel_bpz.pkl'}
     zb_expected = np.array([0.16, 0.12, 0.14, 0.14, 0.06, 0.14, 0.12, 0.14, 0.06, 0.16])
     train_algo = None
-    pz_algo = bpz_lite.BPZ_lite
+    pz_algo = bpz_lite.BPZliteEstimator
     results, rerun_results, rerun3_results = one_algo("BPZ_lite", train_algo, pz_algo, train_config_dict, estim_config_dict)
     assert np.isclose(results.ancil['zmode'], zb_expected).all()
     assert np.isclose(results.ancil['zmode'], rerun_results.ancil['zmode']).all()
 
 @pytest.mark.parametrize(
     "inputdata, groupname",
     [
@@ -102,15 +102,15 @@
                          'hdf5_groupname': groupname,
                          'nt_array': [1, 2, 5],
                          'model': os.path.join(RAILDIR, 'rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl')}
     zb_expected = np.array([0.18, 2.88, 0.12, 0.15, 2.97, 2.78, 0.11, 0.19,
                             2.98, 2.92])
 
     validation_data = DS.read_file('validation_data', TableHandle, inputdata)
-    pz = bpz_lite.BPZ_lite.make_stage(name='bpz_hdfn', **estim_config_dict)
+    pz = bpz_lite.BPZliteEstimator.make_stage(name='bpz_hdfn', **estim_config_dict)
     results = pz.estimate(validation_data)
     assert np.isclose(results.data.ancil['zmode'], zb_expected).all()
     DS.clear()
     os.remove(pz.get_output(pz.get_aliased_tag('output'), final_name=True))
 
 
 def test_bpz_lite_wkernel_flatprior():
@@ -128,11 +128,11 @@
                          'gauss_kernel': 0.1,
                          'zp_errors': np.array([0.01, 0.01, 0.01, 0.01, 0.01, 0.01]),
                          'mag_err_min': 0.005,
                          'hdf5_groupname': 'photometry'}
     # zb_expected = np.array([0.18, 2.88, 0.12, 0.15, 2.97, 2.78, 0.11, 0.19,
     #                         2.98, 2.92])
     train_algo = None
-    pz_algo = bpz_lite.BPZ_lite
+    pz_algo = bpz_lite.BPZliteEstimator
     results, rerun_results, rerun3_results = one_algo("BPZ_lite", train_algo, pz_algo, train_config_dict, estim_config_dict)
     # assert np.isclose(results.ancil['zmode'], zb_expected).all()
     assert np.isclose(results.ancil['zmode'], rerun_results.ancil['zmode']).all()
```

### Comparing `pz-rail-bpz-0.1.0/tests/validation_10gal.pq` & `pz-rail-bpz-0.1.1/tests/validation_10gal.pq`

 * *Files identical despite different names*

