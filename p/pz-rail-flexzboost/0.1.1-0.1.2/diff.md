# Comparing `tmp/pz-rail-flexzboost-0.1.1.tar.gz` & `tmp/pz-rail-flexzboost-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-flexzboost-0.1.1.tar", last modified: Tue Jun 13 20:59:31 2023, max compression
+gzip compressed data, was "pz-rail-flexzboost-0.1.2.tar", last modified: Fri Jul 14 23:55:00 2023, max compression
```

## Comparing `pz-rail-flexzboost-0.1.1.tar` & `pz-rail-flexzboost-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.257141 pz-rail-flexzboost-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.249141 pz-rail-flexzboost-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.253141 pz-rail-flexzboost-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-13 20:59:31.257141 pz-rail-flexzboost-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.253141 pz-rail-flexzboost-0.1.1/archive/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/archive/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/archive/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/archive/x_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/archive/x_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.249141 pz-rail-flexzboost-0.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.253141 pz-rail-flexzboost-0.1.1/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/docs/notebooks/fzboost_pdf_representation_comparison.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:59:31.257141 pz-rail-flexzboost-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.253141 pz-rail-flexzboost-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.257141 pz-rail-flexzboost-0.1.1/src/pz_rail_flexzboost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-13 20:59:31.000000 pz-rail-flexzboost-0.1.1/src/pz_rail_flexzboost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-13 20:59:31.000000 pz-rail-flexzboost-0.1.1/src/pz_rail_flexzboost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:59:31.000000 pz-rail-flexzboost-0.1.1/src/pz_rail_flexzboost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 20:59:31.000000 pz-rail-flexzboost-0.1.1/src/pz_rail_flexzboost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 20:59:31.000000 pz-rail-flexzboost-0.1.1/src/pz_rail_flexzboost.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.253141 pz-rail-flexzboost-0.1.1/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.253141 pz-rail-flexzboost-0.1.1/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.257141 pz-rail-flexzboost-0.1.1/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/src/rail/estimation/algos/flexzboost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.257141 pz-rail-flexzboost-0.1.1/src/rail/flexzboost/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/src/rail/flexzboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 20:59:31.000000 pz-rail-flexzboost-0.1.1/src/rail/flexzboost/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:59:31.257141 pz-rail-flexzboost-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-06-13 20:59:15.000000 pz-rail-flexzboost-0.1.1/tests/test_algos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:00.018441 pz-rail-flexzboost-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-14 23:54:47.000000 pz-rail-flexzboost-0.1.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:00.002441 pz-rail-flexzboost-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:00.010441 pz-rail-flexzboost-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-14 23:54:47.000000 pz-rail-flexzboost-0.1.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-14 23:54:47.000000 pz-rail-flexzboost-0.1.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-14 23:54:47.000000 pz-rail-flexzboost-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-14 23:54:47.000000 pz-rail-flexzboost-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-14 23:55:00.018441 pz-rail-flexzboost-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-14 23:54:47.000000 pz-rail-flexzboost-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:00.014441 pz-rail-flexzboost-0.1.2/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-14 23:54:47.000000 pz-rail-flexzboost-0.1.2/archive/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-14 23:54:47.000000 pz-rail-flexzboost-0.1.2/archive/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-14 23:54:47.000000 pz-rail-flexzboost-0.1.2/archive/x_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-14 23:54:47.000000 pz-rail-flexzboost-0.1.2/archive/x_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:00.006441 pz-rail-flexzboost-0.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:00.014441 pz-rail-flexzboost-0.1.2/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    12086 2023-07-14 23:54:47.000000 pz-rail-flexzboost-0.1.2/docs/notebooks/fzboost_pdf_representation_comparison.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-14 23:54:47.000000 pz-rail-flexzboost-0.1.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-14 23:54:47.000000 pz-rail-flexzboost-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 23:55:00.018441 pz-rail-flexzboost-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:00.006441 pz-rail-flexzboost-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:00.014441 pz-rail-flexzboost-0.1.2/src/pz_rail_flexzboost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-14 23:54:59.000000 pz-rail-flexzboost-0.1.2/src/pz_rail_flexzboost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-14 23:55:00.000000 pz-rail-flexzboost-0.1.2/src/pz_rail_flexzboost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:54:59.000000 pz-rail-flexzboost-0.1.2/src/pz_rail_flexzboost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-14 23:54:59.000000 pz-rail-flexzboost-0.1.2/src/pz_rail_flexzboost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 23:54:59.000000 pz-rail-flexzboost-0.1.2/src/pz_rail_flexzboost.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:00.006441 pz-rail-flexzboost-0.1.2/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:00.006441 pz-rail-flexzboost-0.1.2/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:00.018441 pz-rail-flexzboost-0.1.2/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-07-14 23:54:47.000000 pz-rail-flexzboost-0.1.2/src/rail/estimation/algos/flexzboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:00.018441 pz-rail-flexzboost-0.1.2/src/rail/flexzboost/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-14 23:54:47.000000 pz-rail-flexzboost-0.1.2/src/rail/flexzboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 23:54:59.000000 pz-rail-flexzboost-0.1.2/src/rail/flexzboost/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:00.018441 pz-rail-flexzboost-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-07-14 23:54:47.000000 pz-rail-flexzboost-0.1.2/tests/test_algos.py
```

### Comparing `pz-rail-flexzboost-0.1.1/.github/workflows/main.yml` & `pz-rail-flexzboost-0.1.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.1/.github/workflows/publish-to-pypi.yml` & `pz-rail-flexzboost-0.1.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.1/.gitignore` & `pz-rail-flexzboost-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.1/LICENSE` & `pz-rail-flexzboost-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.1/archive/README.md` & `pz-rail-flexzboost-0.1.2/archive/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.1/archive/pypi.yaml` & `pz-rail-flexzboost-0.1.2/archive/pypi.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.1/docs/notebooks/fzboost_pdf_representation_comparison.ipynb` & `pz-rail-flexzboost-0.1.2/docs/notebooks/fzboost_pdf_representation_comparison.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993918918918919%*

 * *Differences: {"'cells'": "{8: {'source': ['from rail.estimation.algos.flexzboost import FlexZBoostInformer, "*

 * *            'FlexZBoostEstimator\\n\', "inform_pzflex = '*

 * *            "FlexZBoostInformer.make_stage(name='inform_fzboost', model=fz_modelfile, "*

 * *            '**fz_dict)"]}, 12: {\'source\': {insert: [(0, "pzflex_qp_flexzboost = '*

 * *            "FlexZBoostEstimator.make_stage(name='fzboost_flexzboost', "*

 * *            'hdf5_groupname=\'photometry\',\\n")], delete: [0]}}, 24: {\'source\': {insert: [(0, '*

 * *             […]*

```diff
@@ -91,16 +91,16 @@
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
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -128,15 +128,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pzflex_qp_flexzboost = FZBoost.make_stage(name='fzboost_flexzboost', hdf5_groupname='photometry',\n",
+                "pzflex_qp_flexzboost = FlexZBoostEstimator.make_stage(name='fzboost_flexzboost', hdf5_groupname='photometry',\n",
                 "                            model=inform_pzflex.get_handle('model'),\n",
                 "                            output='flexzboost.hdf5',\n",
                 "                            qp_representation='flexzboost')"
             ]
         },
         {
             "attachments": {},
@@ -254,15 +254,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "pzflex_qp_interp = FZBoost.make_stage(name='fzboost_interp', hdf5_groupname='photometry',\n",
+                "pzflex_qp_interp = FlexZBoostEstimator.make_stage(name='fzboost_interp', hdf5_groupname='photometry',\n",
                 "                            model=inform_pzflex.get_handle('model'),\n",
                 "                            output='interp.hdf5',\n",
                 "                            qp_representation='interp')"
             ]
         },
         {
             "attachments": {},
```

### Comparing `pz-rail-flexzboost-0.1.1/pyproject.toml` & `pz-rail-flexzboost-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-flexzboost-0.1.1/src/pz_rail_flexzboost.egg-info/SOURCES.txt` & `pz-rail-flexzboost-0.1.2/src/pz_rail_flexzboost.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .flake8
 .gitignore
 LICENSE
 README.md
+environment.yml
 pyproject.toml
 .github/workflows/main.yml
 .github/workflows/publish-to-pypi.yml
 archive/README.md
 archive/pypi.yaml
 archive/x_requirements.txt
 archive/x_setup.py
```

### Comparing `pz-rail-flexzboost-0.1.1/src/rail/estimation/algos/flexzboost.py` & `pz-rail-flexzboost-0.1.2/src/rail/estimation/algos/flexzboost.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,18 +37,18 @@
         color = data_dict[bands[i]] - data_dict[bands[i + 1]]
         input_data = np.vstack((input_data, color))
         colorerr = np.sqrt(data_dict[err_bands[i]]**2 + data_dict[err_bands[i + 1]]**2)
         np.vstack((input_data, colorerr))
     return input_data.T
 
 
-class Inform_FZBoost(CatInformer):
-    """ Train a FZBoost CatEstimator
+class FlexZBoostInformer(CatInformer):
+    """ Train a FlexZBoost CatInformer
     """
-    name = 'Inform_FZBoost'
+    name = 'FlexZBoostInformer'
     config_options = CatInformer.config_options.copy()
     config_options.update(zmin=SHARED_PARAMS,
                           zmax=SHARED_PARAMS,
                           nzbins=SHARED_PARAMS,
                           nondetect_val=SHARED_PARAMS,
                           mag_limits=SHARED_PARAMS,
                           bands=SHARED_PARAMS,
@@ -186,18 +186,18 @@
             print(f"Skipping retraining, only fraction {self.config.trainfrac}"
                   "of training data used when training model")
 
         self.model = model
         self.add_data('model', self.model)
 
 
-class FZBoost(CatEstimator):
-    """FZBoost-based CatEstimator
+class FlexZBoostEstimator(CatEstimator):
+    """FlexZBoost-based CatEstimator
     """
-    name = 'FZBoost'
+    name = 'FlexZBoostEstimator'
     config_options = CatEstimator.config_options.copy()
     config_options.update(nzbins=SHARED_PARAMS,
                           nondetect_val=SHARED_PARAMS,
                           mag_limits=SHARED_PARAMS,
                           bands=SHARED_PARAMS,
                           err_bands=SHARED_PARAMS,
                           ref_band=SHARED_PARAMS,
```

### Comparing `pz-rail-flexzboost-0.1.1/tests/test_algos.py` & `pz-rail-flexzboost-0.1.2/tests/test_algos.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,16 +27,16 @@
                                                'reg:squarederror'},
                          'hdf5_groupname': 'photometry',
                          'model': 'model.tmp'}
     estim_config_dict = {'hdf5_groupname': 'photometry',
                          'model': 'model.tmp'}
     # zb_expected = np.array([0.13, 0.13, 0.13, 0.12, 0.12, 0.13, 0.12, 0.13,
     #                         0.12, 0.12])
-    train_algo = flexzboost.Inform_FZBoost
-    pz_algo = flexzboost.FZBoost
+    train_algo = flexzboost.FlexZBoostInformer
+    pz_algo = flexzboost.FlexZBoostEstimator
     results, rerun_results, rerun3_results = one_algo("FZBoost", train_algo, pz_algo, train_config_dict, estim_config_dict)
     # assert np.isclose(results.ancil['zmode'], zb_expected).all()
     assert np.isclose(results.ancil['zmode'], rerun_results.ancil['zmode']).all()
 
 def test_flexzboost_with_interp():
     train_config_dict = {'zmin': 0.0, 'zmax': 3.0, 'nzbins': 301,
                          'trainfrac': 0.75, 'bumpmin': 0.02,
@@ -50,16 +50,16 @@
                          'hdf5_groupname': 'photometry',
                          'model': 'model.tmp'}
     estim_config_dict = {'hdf5_groupname': 'photometry',
                          'model': 'model.tmp',
                          'qp_representation': 'interp'}
     # zb_expected = np.array([0.13, 0.13, 0.13, 0.12, 0.12, 0.13, 0.12, 0.13,
     #                         0.12, 0.12])
-    train_algo = flexzboost.Inform_FZBoost
-    pz_algo = flexzboost.FZBoost
+    train_algo = flexzboost.FlexZBoostInformer
+    pz_algo = flexzboost.FlexZBoostEstimator
     results, rerun_results, rerun3_results = one_algo("FZBoost", train_algo, pz_algo, train_config_dict, estim_config_dict)
     # assert np.isclose(results.ancil['zmode'], zb_expected).all()
     assert np.isclose(results.ancil['zmode'], rerun_results.ancil['zmode']).all()
 
 def test_flexzboost_with_qp_flexzboost():
     train_config_dict = {'zmin': 0.0, 'zmax': 3.0, 'nzbins': 301,
                          'trainfrac': 0.75, 'bumpmin': 0.02,
@@ -73,16 +73,16 @@
                          'hdf5_groupname': 'photometry',
                          'model': 'model.tmp'}
     estim_config_dict = {'hdf5_groupname': 'photometry',
                          'model': 'model.tmp',
                          'qp_representation': 'flexzboost'}
     # zb_expected = np.array([0.13, 0.13, 0.13, 0.12, 0.12, 0.13, 0.12, 0.13,
     #                         0.12, 0.12])
-    train_algo = flexzboost.Inform_FZBoost
-    pz_algo = flexzboost.FZBoost
+    train_algo = flexzboost.FlexZBoostInformer
+    pz_algo = flexzboost.FlexZBoostEstimator
     results, rerun_results, rerun3_results = one_algo("FZBoost", train_algo, pz_algo, train_config_dict, estim_config_dict)
     # assert np.isclose(results.ancil['zmode'], zb_expected).all()
     assert np.isclose(results.ancil['zmode'], rerun_results.ancil['zmode']).all()
 
 def test_flexzboost_with_unknown_qp_representation():
     """Pass a bogus qp_representation string to the config, expect a ValueError"""
     train_config_dict = {'zmin': 0.0, 'zmax': 3.0, 'nzbins': 301,
@@ -97,40 +97,40 @@
                          'hdf5_groupname': 'photometry',
                          'model': 'model.tmp'}
     estim_config_dict = {'hdf5_groupname': 'photometry',
                          'model': 'model.tmp',
                          'qp_representation': 'bogus'}
     # zb_expected = np.array([0.13, 0.13, 0.13, 0.12, 0.12, 0.13, 0.12, 0.13,
     #                         0.12, 0.12])
-    train_algo = flexzboost.Inform_FZBoost
-    pz_algo = flexzboost.FZBoost
+    train_algo = flexzboost.FlexZBoostInformer
+    pz_algo = flexzboost.FlexZBoostEstimator
     with pytest.raises(ValueError) as excinfo:
         one_algo("FZBoost", train_algo, pz_algo, train_config_dict, estim_config_dict)
         assert "Unknown qp_representation" in str(excinfo.value)
 
 def test_catch_bad_bands():
     params = dict(bands='u,g,r,i,z,y')
     with pytest.raises(ValueError):
-        flexzboost.Inform_FZBoost.make_stage(hdf5_groupname='', **params)
+        flexzboost.FlexZBoostInformer.make_stage(hdf5_groupname='', **params)
     with pytest.raises(ValueError):
-        flexzboost.FZBoost.make_stage(hdf5_groupname='', **params)
+        flexzboost.FlexZBoostEstimator.make_stage(hdf5_groupname='', **params)
 
 
 def test_missing_groupname_keyword():
     config_dict = {'zmin': 0.0, 'zmax': 3.0, 'nzbins': 301,
                    'trainfrac': 0.75, 'bumpmin': 0.02,
                    'bumpmax': 0.35, 'nbump': 3,
                    'sharpmin': 0.7, 'sharpmax': 2.1,
                    'nsharp': 3, 'max_basis': 35,
                    'basis_system': 'cosine',
                    'regression_params': {'max_depth': 8,
                                              'objective':
                                              'reg:squarederror'}}
     with pytest.raises(ValueError):
-        _ = flexzboost.FZBoost.make_stage(**config_dict)
+        _ = flexzboost.FlexZBoostEstimator.make_stage(**config_dict)
 
 
 def test_wrong_modelfile_keyword():
     RailStage.data_store.clear()
     config_dict = {'zmin': 0.0, 'zmax': 3.0, 'nzbins': 301,
                    'trainfrac': 0.75, 'bumpmin': 0.02,
                    'bumpmax': 0.35, 'nbump': 3,
@@ -139,9 +139,9 @@
                    'basis_system': 'cosine',
                    'hdf5_groupname': 'photometry',
                    'regression_params': {'max_depth': 8,
                                              'objective':
                                              'reg:squarederror'},
                    'model': 'nonexist.pkl'}
     with pytest.raises(FileNotFoundError):
-        pz_algo = flexzboost.FZBoost.make_stage(**config_dict)
+        pz_algo = flexzboost.FlexZBoostEstimator.make_stage(**config_dict)
         assert pz_algo.model is None
```

