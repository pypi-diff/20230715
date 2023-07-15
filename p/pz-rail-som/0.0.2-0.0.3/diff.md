# Comparing `tmp/pz-rail-som-0.0.2.tar.gz` & `tmp/pz-rail-som-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-som-0.0.2.tar", last modified: Tue Jun 13 17:08:20 2023, max compression
+gzip compressed data, was "pz-rail-som-0.0.3.tar", last modified: Fri Jul 14 23:55:36 2023, max compression
```

## Comparing `pz-rail-som-0.0.2.tar` & `pz-rail-som-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.732943 pz-rail-som-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.724943 pz-rail-som-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.728943 pz-rail-som-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-13 17:08:20.732943 pz-rail-som-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 17:08:20.732943 pz-rail-som-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.720943 pz-rail-som-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.728943 pz-rail-som-0.0.2/src/pz_rail_som.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-13 17:08:20.000000 pz-rail-som-0.0.2/src/pz_rail_som.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-13 17:08:20.000000 pz-rail-som-0.0.2/src/pz_rail_som.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:08:20.000000 pz-rail-som-0.0.2/src/pz_rail_som.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-13 17:08:20.000000 pz-rail-som-0.0.2/src/pz_rail_som.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 17:08:20.000000 pz-rail-som-0.0.2/src/pz_rail_som.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.724943 pz-rail-som-0.0.2/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.724943 pz-rail-som-0.0.2/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.728943 pz-rail-som-0.0.2/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (123)    16320 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/src/rail/estimation/algos/simpleSOM.py
--rw-r--r--   0 runner    (1001) docker     (123)    26111 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/src/rail/estimation/algos/somocluSOM.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.732943 pz-rail-som-0.0.2/src/rail/som/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/src/rail/som/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 17:08:20.000000 pz-rail-som-0.0.2/src/rail/som/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.724943 pz-rail-som-0.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:08:20.732943 pz-rail-som-0.0.2/tests/som/
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/tests/som/test_som_summarizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-13 17:08:08.000000 pz-rail-som-0.0.2/tests/som/test_somoclu_summarizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:36.506935 pz-rail-som-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:36.502935 pz-rail-som-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:36.502935 pz-rail-som-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-14 23:55:36.506935 pz-rail-som-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 23:55:36.506935 pz-rail-som-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:36.502935 pz-rail-som-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:36.506935 pz-rail-som-0.0.3/src/pz_rail_som.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-14 23:55:36.000000 pz-rail-som-0.0.3/src/pz_rail_som.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-14 23:55:36.000000 pz-rail-som-0.0.3/src/pz_rail_som.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:55:36.000000 pz-rail-som-0.0.3/src/pz_rail_som.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-14 23:55:36.000000 pz-rail-som-0.0.3/src/pz_rail_som.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 23:55:36.000000 pz-rail-som-0.0.3/src/pz_rail_som.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:36.502935 pz-rail-som-0.0.3/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:36.502935 pz-rail-som-0.0.3/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:36.506935 pz-rail-som-0.0.3/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (123)    16304 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/src/rail/estimation/algos/minisom_som.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26094 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/src/rail/estimation/algos/somoclu_som.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:36.506935 pz-rail-som-0.0.3/src/rail/som/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/src/rail/som/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 23:55:36.000000 pz-rail-som-0.0.3/src/rail/som/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:36.502935 pz-rail-som-0.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:55:36.506935 pz-rail-som-0.0.3/tests/som/
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/tests/som/test_som_summarizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-14 23:55:24.000000 pz-rail-som-0.0.3/tests/som/test_somoclu_summarizers.py
```

### Comparing `pz-rail-som-0.0.2/.github/pull_request_template.md` & `pz-rail-som-0.0.3/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.2/.github/workflows/linting.yml` & `pz-rail-som-0.0.3/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.2/.github/workflows/publish-to-pypi.yml` & `pz-rail-som-0.0.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.2/.github/workflows/smoke-test.yml` & `pz-rail-som-0.0.3/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.2/.github/workflows/testing-and-coverage.yml` & `pz-rail-som-0.0.3/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.2/.gitignore` & `pz-rail-som-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.2/.pre-commit-config.yaml` & `pz-rail-som-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.2/LICENSE` & `pz-rail-som-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.2/pyproject.toml` & `pz-rail-som-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-som-0.0.2/src/pz_rail_som.egg-info/SOURCES.txt` & `pz-rail-som-0.0.3/src/pz_rail_som.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 .copier-answers.yml
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 README.md
+environment.yml
 pyproject.toml
 setup.py
 .github/pull_request_template.md
 .github/workflows/add-issue-to-project-tracker.yml
 .github/workflows/linting.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/smoke-test.yml
 .github/workflows/testing-and-coverage.yml
 src/pz_rail_som.egg-info/PKG-INFO
 src/pz_rail_som.egg-info/SOURCES.txt
 src/pz_rail_som.egg-info/dependency_links.txt
 src/pz_rail_som.egg-info/requires.txt
 src/pz_rail_som.egg-info/top_level.txt
-src/rail/estimation/algos/simpleSOM.py
-src/rail/estimation/algos/somocluSOM.py
+src/rail/estimation/algos/minisom_som.py
+src/rail/estimation/algos/somoclu_som.py
 src/rail/som/__init__.py
 src/rail/som/_version.py
 tests/som/test_som_summarizers.py
 tests/som/test_somoclu_summarizers.py
```

### Comparing `pz-rail-som-0.0.2/src/rail/estimation/algos/simpleSOM.py` & `pz-rail-som-0.0.3/src/rail/estimation/algos/minisom_som.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     if colusage == 'columns':  # pragma: no cover
         coldata = np.array(data[column_names[0]])
         for i in range(numcols - 1):
             coldata = np.vstack((coldata, np.array(data[column_names[i + 1]])))
     return coldata.T
 
 
-class Inform_SimpleSOMSummarizer(CatInformer):
+class MiniSOMInformer(CatInformer):
     """Summarizer that uses a SOM to construct a weighted sum
     of spec-z objects in the same SOM cell as each photometric
     galaxy in order to estimate the overall N(z).  This is
     very related to the NZDir estimator, though that estimator
     actually reverses this process and looks for photometric
     neighbors around each spectroscopic galaxy, which can
     lead to problems if there are photometric galaxies with
@@ -69,15 +69,15 @@
 
     Returns
     -------
     model: pickle file
       pickle file containing the `minisom` SOM object that
     will be used by the estimation/summarization stage
     """
-    name = 'Inform_SimpleSOM'
+    name = 'MiniSOMInformer'
     config_options = CatInformer.config_options.copy()
     config_options.update(nondetect_val=SHARED_PARAMS,
                           mag_limits=SHARED_PARAMS,
                           bands=SHARED_PARAMS,
                           ref_band=SHARED_PARAMS,
                           hdf5_groupname=SHARED_PARAMS,
                           column_usage=Param(str, "magandcolors", msg="switch for how SOM uses columns, "
@@ -126,15 +126,15 @@
                          ref_column=self.config.ref_band,
                          m_dim=self.config.m_dim, n_dim=self.config.n_dim,
                          column_usage=self.config.column_usage)
         self.model = modeldict
         self.add_data('model', self.model)
 
 
-class SimpleSOMSummarizer(SZPZSummarizer):
+class MiniSOMSummarizer(SZPZSummarizer):
     """Quick implementation of a SOM-based summarizer that
     constructs and N(z) estimate via a weighted sum of the
     empirical N(z) consisting of the normalized histogram
     of spec-z values contained in the same SOM cell as
     each photometric galaxy.
     There are some general guidelines to choosing the geometry
     and number of total cells in the SOM.  This paper:
@@ -188,15 +188,15 @@
       number of bootstrap spec-z samples to generate
 
     Returns
     -------
     qp_ens: qp Ensemble
       ensemble of bootstrap realizations of the estimated N(z) for the input photometric data
     """
-    name = 'SimpleSOMSummarizer'
+    name = 'MiniSOMSummarizer'
     config_options = SZPZSummarizer.config_options.copy()
     config_options.update(zmin=SHARED_PARAMS,
                           zmax=SHARED_PARAMS,
                           nzbins=SHARED_PARAMS,
                           nondetect_val=SHARED_PARAMS,
                           mag_limits=SHARED_PARAMS,
                           hdf5_groupname=SHARED_PARAMS,
```

### Comparing `pz-rail-som-0.0.2/src/rail/estimation/algos/somocluSOM.py` & `pz-rail-som-0.0.3/src/rail/estimation/algos/somoclu_som.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
     cb = plt.colorbar(scmap, cax=cax)
     cb.ax.tick_params(labelsize=15)
     cb.set_label(cbar_name, size=15)
     ax.axis('off')
 
 
-class Inform_somocluSOMSummarizer(CatInformer):
+class SOMocluInformer(CatInformer):
     """Summarizer that uses a SOM to construct a weighted sum
     of spec-z objects in the same SOM cell as each photometric
     galaxy in order to estimate the overall N(z).  This is
     very related to the NZDir estimator, though that estimator
     actually reverses this process and looks for photometric
     neighbors around each spectroscopic galaxy, which can
     lead to problems if there are photometric galaxies with
@@ -165,15 +165,15 @@
 
     Returns
     -------
     model: pickle file
       pickle file containing the `somoclu` SOM object that
     will be used by the estimation/summarization stage
     """
-    name = 'Inform_SOMoclu'
+    name = 'SOMocluInformer'
     config_options = CatInformer.config_options.copy()
     config_options.update(nondetect_val=SHARED_PARAMS,
                           mag_limits=SHARED_PARAMS,
                           bands=SHARED_PARAMS,
                           err_bands=SHARED_PARAMS,
                           ref_band=SHARED_PARAMS,
                           redshift_col=SHARED_PARAMS,
@@ -229,15 +229,15 @@
                          ref_column=self.config.ref_band,
                          n_rows=self.config.n_rows, n_columns=self.config.n_columns,
                          column_usage=self.config.column_usage)
         self.model = modeldict
         self.add_data('model', self.model)
 
 
-class somocluSOMSummarizer(SZPZSummarizer):
+class SOMocluSummarizer(SZPZSummarizer):
     """Quick implementation of a SOM-based summarizer. It will
     group a pre-trained SOM into hierarchical clusters and assign
     a galaxy sample into SOM cells and clusters. Then it
     constructs an N(z) estimation via a weighted sum of the
     empirical N(z) consisting of the normalized histogram
     of spec-z values contained in the same SOM cluster as
     each photometric galaxy.
@@ -294,15 +294,15 @@
     n_clusters: int
       number of hierarchical clusters of the SOM cells. If not given, the SOM will not be grouped into clusters (or equivalently n_cluster=the total number of SOM cells.)
     Returns
     -------
     qp_ens: qp Ensemble
       ensemble of bootstrap realizations of the estimated N(z) for the input photometric data
     """
-    name = 'somocluSOMSummarizer'
+    name = 'SOMocluSummarizer'
     config_options = SZPZSummarizer.config_options.copy()
     config_options.update(zmin=SHARED_PARAMS,
                           zmax=SHARED_PARAMS,
                           nzbins=SHARED_PARAMS,
                           nondetect_val=SHARED_PARAMS,
                           mag_limits=SHARED_PARAMS,
                           hdf5_groupname=SHARED_PARAMS,
```

### Comparing `pz-rail-som-0.0.2/tests/som/test_som_summarizers.py` & `pz-rail-som-0.0.3/tests/som/test_som_summarizers.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import qp
 
 from rail.core.data import TableHandle
 from rail.core.stage import RailStage
 from rail.core.utils import RAILDIR
-from rail.estimation.algos import simpleSOM
+from rail.estimation.algos import minisom_som
 
 testszdata = os.path.join(RAILDIR, "rail/examples_data/testdata/training_100gal.hdf5")
 testphotdata = os.path.join(RAILDIR, "rail/examples_data/testdata/validation_10gal.hdf5")
 DS = RailStage.data_store
 DS.__class__.allow_overwrite = True
 
 
@@ -57,22 +57,22 @@
     os.remove(summarizer2.get_output(summarizer2.get_aliased_tag("output"), final_name=True))
     os.remove(f"tmpsom_{key}.pkl")
     return summary_ens
 
 
 def test_SimpleSOM():
     summary_config_dict = {"m_dim": 21, "n_dim": 21, "column_usage": "colors"}
-    inform_class = simpleSOM.Inform_SimpleSOMSummarizer
-    summarizerclass = simpleSOM.SimpleSOMSummarizer
+    inform_class = minisom_som.MiniSOMInformer
+    summarizerclass = minisom_som.MiniSOMSummarizer
     _ = one_algo("SimpleSOM", inform_class, summarizerclass, summary_config_dict)
 
 
 def test_SimpeSOM_with_mag_and_colors():
     summary_config_dict = {
         "m_dim": 21,
         "n_dim": 21,
         "column_usage": "magandcolors",
         "objid_name": "id",
     }
-    inform_class = simpleSOM.Inform_SimpleSOMSummarizer
-    summarizerclass = simpleSOM.SimpleSOMSummarizer
+    inform_class = minisom_som.MiniSOMInformer
+    summarizerclass = minisom_som.MiniSOMSummarizer
     _ = one_algo("SimpleSOM_wmag", inform_class, summarizerclass, summary_config_dict)
```

### Comparing `pz-rail-som-0.0.2/tests/som/test_somoclu_summarizers.py` & `pz-rail-som-0.0.3/tests/som/test_somoclu_summarizers.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import qp
 
 from rail.core.data import TableHandle
 from rail.core.stage import RailStage
 from rail.core.utils import RAILDIR
-from rail.estimation.algos import somocluSOM
+from rail.estimation.algos import somoclu_som
 
 testszdata = os.path.join(RAILDIR, "rail/examples_data/testdata/training_100gal.hdf5")
 testphotdata = os.path.join(RAILDIR, "rail/examples_data/testdata/validation_10gal.hdf5")
 DS = RailStage.data_store
 DS.__class__.allow_overwrite = True
 
 
@@ -57,22 +57,22 @@
     os.remove(summarizer2.get_output(summarizer2.get_aliased_tag("output"), final_name=True))
     os.remove(f"tmpsomoclu_" + key + ".pkl")
     return summary_ens
 
 
 def test_SomocluSOM():
     summary_config_dict = {"n_rows": 21, "n_columns": 21, "column_usage": "colors"}
-    inform_class = somocluSOM.Inform_somocluSOMSummarizer
-    summarizerclass = somocluSOM.somocluSOMSummarizer
+    inform_class = somoclu_som.SOMocluInformer
+    summarizerclass = somoclu_som.SOMocluSummarizer
     _ = one_algo("SOMomoclu", inform_class, summarizerclass, summary_config_dict)
 
 
 def test_SomocluSOM_with_mag_and_colors():
     summary_config_dict = {
         "n_rows": 21,
         "n_columns": 21,
         "column_usage": "magandcolors",
         "objid_name": "id",
     }
-    inform_class = somocluSOM.Inform_somocluSOMSummarizer
-    summarizerclass = somocluSOM.somocluSOMSummarizer
+    inform_class = somoclu_som.SOMocluInformer
+    summarizerclass = somoclu_som.SOMocluSummarizer
     _ = one_algo("SOMoclu_wmag", inform_class, summarizerclass, summary_config_dict)
```

